# Capítulo V: Product Implementation, Validation & Deployment

## 5.1. Testing Suites & General Patterns

En las siguientes secciones se presentan las pruebas realizadas y los patrones utilizados para el desarrollo del backend que estará orientado a una arquitectura de microservicios.

## 5.1.1. Backend Application Core Testing Suite

En este apartado se evidencian nuestras pruebas funcionales y no funcionales del dominio core del negocio. Estas estan divididas de la siguiente manera:

### Pruebas funcionales
Verifican que el sistema **cumpla con los requisitos funcionales**.

#### 🔹 Pruebas unitarias (Core Entities Unit Tests)
Prueban funciones o métodos individuales de forma aislada. Para ello, utilizaremos JUnit y la librería Mockito.

[![1-lc-Ursqc0ls-M3-WPNrtv-T8b-A.jpg](https://i.postimg.cc/Dz0tKGBB/1-lc-Ursqc0ls-M3-WPNrtv-T8b-A.jpg)](https://postimg.cc/PLG6WCGw)


#### 🔹 Pruebas de integración (Core Integration Tests)
Verifican la interacción entre módulos o componentes. Para ello, utilizaremos Postman.

[![postman.jpg](https://i.postimg.cc/zvxC5ydF/postman.jpg)](https://postimg.cc/rRt0Nw2D)

#### 🔹 Pruebas de aceptación (User Acceptance Tests)
Validan si el sistema cumple con las necesidades del cliente/usuario. Para ello, utilizaremos Cucumber / Gherkin.

[![cucumber.jpg](https://i.postimg.cc/3xvvffHB/cucumber.jpg)](https://postimg.cc/jDR2LX2w)


#### 🔹 Pruebas automatizadas (Automated Tests)
Permiten realizar pruebas funcionales de forma automática para acciones como llenar formularios, hacer clic en botones o verificar textos en pantalla. Esto es útil para validar que una aplicación funciona correctamente después de cada cambio, sin necesidad de realizar pruebas manuales repetitivas.

---



## 2. Pruebas no funcionales
Evalúan atributos del sistema **como rendimiento, seguridad o usabilidad**.

### 🔹 Pruebas de rendimiento (Quality Attributes Tests)
Miden tiempos de respuesta, velocidad, escalabilidad. Para ello, utilizaremos la herramientas Lighthouse.

[![lighthouse2.jpg](https://i.postimg.cc/Wzd3FtNn/lighthouse2.jpg)](https://postimg.cc/tnHy8qVZ)


### 5.1.1.1. Core Entities Unit Tests

#### PetCommandService Unit Test:

```java
package pe.upc.pawfectcarebackend.petmanagement;

import org.junit.jupiter.api.Test;
import org.mockito.Mockito;
import pe.upc.pawfectcarebackend.medicalrecords.domain.model.aggregates.MedicalHistory;
import pe.upc.pawfectcarebackend.petmanagement.application.PetCommandServicelmpl;
import pe.upc.pawfectcarebackend.petmanagement.application.acl.ExternalMedicalHistoryService;
import pe.upc.pawfectcarebackend.petmanagement.domain.model.aggregates.Owner;
import pe.upc.pawfectcarebackend.petmanagement.domain.model.aggregates.Pet;
import pe.upc.pawfectcarebackend.petmanagement.domain.model.commands.CreatePetCommand;
import pe.upc.pawfectcarebackend.petmanagement.domain.model.commands.UpdatePetCommand;
import pe.upc.pawfectcarebackend.petmanagement.domain.model.valueobjects.PetGender;
import pe.upc.pawfectcarebackend.petmanagement.domain.services.PetCommandService;
import pe.upc.pawfectcarebackend.petmanagement.infrastructure.persistence.jpa.repositories.OwnerRepository;
import pe.upc.pawfectcarebackend.petmanagement.infrastructure.persistence.jpa.repositories.PetRepository;

import java.time.LocalDate;
import java.util.Optional;

import static org.junit.jupiter.api.Assertions.assertEquals;
import static org.mockito.ArgumentMatchers.any;
import static org.mockito.Mockito.*;

public class PetCommandServiceTest {
    /**
     * Test for handleCreatePetCommand method
     */
    @Test
    void handleCreatePetCommand() {
        /*
          Arrange
          Mock the dependencies
         */
        PetRepository petRepository = Mockito.mock(PetRepository.class);
        OwnerRepository ownerRepository = Mockito.mock(OwnerRepository.class);
        ExternalMedicalHistoryService medicalHistoryService = Mockito.mock(ExternalMedicalHistoryService.class);

        // Create an instance of the PetCommandService
        PetCommandService petCommandService = new PetCommandServicelmpl(petRepository, ownerRepository, medicalHistoryService);

        // Simulate the creation of an Owner
        Owner mockOwner = Mockito.mock(Owner.class);
        when(mockOwner.getId()).thenReturn(1L);
        when(ownerRepository.findById(1L)).thenReturn(Optional.of(mockOwner));

        // Create the command to add a pet
        CreatePetCommand command = new CreatePetCommand(
                "Buddy",
                LocalDate.of(2020, 1, 1),
                LocalDate.now(),
                "Golden Retriever",
                PetGender.MALE,
                1L
        );

        // Simulate the behavior of PetRepository
        Pet mockPet = new Pet(command);
        mockPet.setOwner(mockOwner);
        when(petRepository.save(any(Pet.class))).thenReturn(mockPet);

        // Simulate the behavior of ExternalMedicalHistoryService
        MedicalHistory mockMedicalHistory = Mockito.mock(MedicalHistory.class);
        when(medicalHistoryService.createMedicalHistory(any(String.class)))
                .thenReturn(Optional.of(mockMedicalHistory));

        /*
          Act
          Call the method to be tested
         */
        Long petId = petCommandService.handle(command);

        // Debugging: Print the created pet details
        System.out.println("\nCreated Pet: \n------------------------------\n");
        System.out.println("Created Pet Name: " + mockPet.getPetName());
        System.out.println("Created Pet Breed: " + mockPet.getAnimalBreed());
        System.out.println("Created Pet Gender: " + mockPet.getPetGender());
        System.out.println("Created Pet Owner ID: " + mockPet.getOwner().getId());
        System.out.println("------------------------------\n");

        /*
          Assert
          Verify the results
         */
        assertEquals(mockPet.getId(), petId);
        verify(ownerRepository, times(1)).findById(command.ownerId());
        verify(petRepository, times(1)).save(any(Pet.class));
        verify(medicalHistoryService, times(1)).createMedicalHistory(any(String.class));
    }


    /**
     * Test for handleUpdatePetCommand method
     */
    @Test
    void handleUpdatePetCommand() {
    /*
      Arrange
      Mock the dependencies
     */
        PetRepository petRepository = Mockito.mock(PetRepository.class);

        // Create an instance of the PetCommandService
        PetCommandService petCommandService = new PetCommandServicelmpl(petRepository, null, null);

        // Simulate the existing Pet
        Pet mockPet = Mockito.mock(Pet.class);
        when(mockPet.getId()).thenReturn(1L);
        when(mockPet.getPetName()).thenReturn("Buddy");
        when(mockPet.getAnimalBreed()).thenReturn("Golden Retriever");
        when(mockPet.getPetGender()).thenReturn(PetGender.MALE);
        when(petRepository.existsById(1L)).thenReturn(true);
        when(petRepository.findById(1L)).thenReturn(Optional.of(mockPet));

        // Mock the updateInformation method
        when(mockPet.updateInformation(
                anyString(),
                any(LocalDate.class),
                any(LocalDate.class),
                anyString(),
                any(PetGender.class)
        )).thenAnswer(invocation -> {
            System.out.println("\nBefore Update:");
            System.out.println("Pet Name: " + mockPet.getPetName());
            System.out.println("Pet Breed: " + mockPet.getAnimalBreed());
            System.out.println("Pet Gender: " + mockPet.getPetGender());

            // Simulate updating the pet
            when(mockPet.getPetName()).thenReturn("Updated Buddy");
            when(mockPet.getAnimalBreed()).thenReturn("Updated Breed");
            when(mockPet.getPetGender()).thenReturn(PetGender.FEMALE);

            System.out.println("\nAfter Update:");
            System.out.println("Pet Name: Updated Buddy");
            System.out.println("Pet Breed: Updated Breed");
            System.out.println("Pet Gender: FEMALE");

            return mockPet;
        });

        // Simulate the updated Pet
        when(petRepository.save(any(Pet.class))).thenReturn(mockPet);

        // Create the command to update a pet
        UpdatePetCommand command = new UpdatePetCommand(
                1L,
                "Updated Buddy",
                LocalDate.of(2020, 1, 1),
                LocalDate.now(),
                "Updated Breed",
                PetGender.FEMALE
        );

    /*
      Act
      Call the method to be tested
     */
        Optional<Pet> result = petCommandService.handle(command);

    /*
      Assert
      Verify the expected behavior
     */
        assertEquals(mockPet.getId(), result.get().getId());
        verify(petRepository, times(1)).existsById(command.id());
        verify(petRepository, times(1)).findById(command.id());
        verify(petRepository, times(1)).save(any(Pet.class));
    }

}
```

##### US04: Creación de Perfil de Mascota<br>
	Como dueño, deseo crear un perfil de mi mascota para tener su información almacenada en la plataforma.

[![Captura-de-pantalla-2025-05-16-200025.png](https://i.postimg.cc/1z504cF1/Captura-de-pantalla-2025-05-16-200025.png)](https://postimg.cc/bZWSBnLm)


##### US05: Edición de Perfil de Mascota<br>
    Como dueño, deseo editar el perfil de mi mascota para actualizar su información cuando sea necesario.

[![Captura-de-pantalla-2025-05-16-195441.png](https://i.postimg.cc/Xv0c36jq/Captura-de-pantalla-2025-05-16-195441.png)](https://postimg.cc/nX0QY5Qf)<br><br>


#### AppointmentCommandService & MedicalAppointmentCommandService  Unit Test:

```java
package pe.upc.pawfectcarebackend.appointmentsscheduling;

import org.junit.jupiter.api.Test;
import org.mockito.Mockito;
import pe.upc.pawfectcarebackend.appointmentsscheduling.application.AppointmentCommandServicelmpl;
import pe.upc.pawfectcarebackend.appointmentsscheduling.application.acl.ExternalPetService;
import pe.upc.pawfectcarebackend.appointmentsscheduling.domain.model.aggregates.Appointment;
import pe.upc.pawfectcarebackend.appointmentsscheduling.domain.model.commands.CreateAppointmentCommand;
import pe.upc.pawfectcarebackend.appointmentsscheduling.domain.model.valueobjects.AppointmentStatus;
import pe.upc.pawfectcarebackend.appointmentsscheduling.domain.services.AppointmentCommandService;
import pe.upc.pawfectcarebackend.appointmentsscheduling.infrastructure.persistence.jpa.repositories.AppointmentRepository;
import pe.upc.pawfectcarebackend.appointmentsscheduling.infrastructure.persistence.jpa.repositories.MedicalAppointmentRepository;
import pe.upc.pawfectcarebackend.petmanagement.domain.model.aggregates.Pet;

import java.time.LocalDateTime;
import java.util.Optional;

import static org.junit.jupiter.api.Assertions.assertEquals;
import static org.mockito.ArgumentMatchers.any;
import static org.mockito.Mockito.*;

public class AppointmentCommandServiceTest {
    /**
     * Test for handleCreateAppointmentCommand method
     */
    @Test
    void handleCreateAppointmentCommand() {
        /*
          Arrange
          Mock the dependencies
         */
        AppointmentRepository appointmentRepository = Mockito.mock(AppointmentRepository.class);
        MedicalAppointmentRepository medicalAppointmentRepository = Mockito.mock(MedicalAppointmentRepository.class);
        ExternalPetService externalPetService = Mockito.mock(ExternalPetService.class);

        // Create an instance of the AppointmentCommandService
        AppointmentCommandService appointmentCommandService = new AppointmentCommandServicelmpl(
                appointmentRepository,
                externalPetService,
                medicalAppointmentRepository
        );

        // Simulate the creation of a Pet
        Pet mockPet = Mockito.mock(Pet.class);
        when(mockPet.getId()).thenReturn(1L);
        when(externalPetService.fetchPetById(1L)).thenReturn(Optional.of(mockPet));

        // Create the command to add an appointment
        CreateAppointmentCommand command = new CreateAppointmentCommand(
                "Vet Visit",
                LocalDateTime.of(2023, 10, 1, 10, 0),
                LocalDateTime.of(2023, 10, 1, 11, 0),
                true,
                AppointmentStatus.SCHEDULED, // Use the AppointmentStatus enum
                1L // Pass a Long instead of a long
        );

        // Simulate the behavior of AppointmentRepository
        Appointment mockAppointment = new Appointment(command);
        mockAppointment.setPet(mockPet);
        when(appointmentRepository.save(any(Appointment.class))).thenReturn(mockAppointment);

        /*
          Act
          Call the method to be tested
         */
        Long appointmentId = appointmentCommandService.handle(command);

        // Debugging: Print the created appointment details
        System.out.println("\nCreated Appointment: \n------------------------------\n");
        System.out.println("Appointment Name: " + mockAppointment.getAppointmentName());
        System.out.println("Registration Date: " + mockAppointment.getRegistrationDate());
        System.out.println("End Date: " + mockAppointment.getEndDate());
        System.out.println("Is Medical: " + mockAppointment.isMedical());
        System.out.println("Pet ID: " + mockAppointment.getPet().getId());
        System.out.println("------------------------------\n");

        /*
          Assert
          Verify the results
         */
        assertEquals(mockAppointment.getId(), appointmentId);
        verify(externalPetService, times(1)).fetchPetById(command.petId());
        verify(appointmentRepository, times(1)).save(any(Appointment.class));
    }
}
```

```java
package pe.upc.pawfectcarebackend.appointmentsscheduling;

import org.junit.jupiter.api.Test;
import org.mockito.Mockito;
import pe.upc.pawfectcarebackend.appointmentsscheduling.application.MedicalAppointmentCommandServiceImpl;
import pe.upc.pawfectcarebackend.appointmentsscheduling.domain.model.aggregates.Appointment;
import pe.upc.pawfectcarebackend.appointmentsscheduling.domain.model.aggregates.MedicalAppointment;
import pe.upc.pawfectcarebackend.appointmentsscheduling.domain.model.commands.CreateMedicalAppointmentCommand;
import pe.upc.pawfectcarebackend.appointmentsscheduling.infrastructure.persistence.jpa.repositories.AppointmentRepository;
import pe.upc.pawfectcarebackend.appointmentsscheduling.infrastructure.persistence.jpa.repositories.MedicalAppointmentRepository;
import pe.upc.pawfectcarebackend.petmanagement.application.acl.ExternalMedicalHistoryService;
import pe.upc.pawfectcarebackend.medicalrecords.domain.model.aggregates.MedicalHistory;
import pe.upc.pawfectcarebackend.petmanagement.domain.model.aggregates.Pet;

import java.util.Optional;

import static org.junit.jupiter.api.Assertions.assertEquals;
import static org.mockito.ArgumentMatchers.any;
import static org.mockito.Mockito.*;

public class MedicalAppointmentCommandServiceTest {

    @Test
    void handleCreateMedicalAppointmentCommand() {
        /*
          Arrange
          Mock the dependencies
         */
        MedicalAppointmentRepository medicalAppointmentRepository = Mockito.mock(MedicalAppointmentRepository.class);
        AppointmentRepository appointmentRepository = Mockito.mock(AppointmentRepository.class);
        ExternalMedicalHistoryService externalMedicalHistoryService = Mockito.mock(ExternalMedicalHistoryService.class);

        // Create an instance of the MedicalAppointmentCommandService
        MedicalAppointmentCommandServiceImpl medicalAppointmentCommandService = new MedicalAppointmentCommandServiceImpl(
                medicalAppointmentRepository,
                appointmentRepository,
                externalMedicalHistoryService
        );

        // Simulate the existing Appointment and Pet
        MedicalHistory mockMedicalHistory = Mockito.mock(MedicalHistory.class);
        when(mockMedicalHistory.getId()).thenReturn(1L);

        Pet mockPet = Mockito.mock(Pet.class);
        when(mockPet.getMedicalHistory()).thenReturn(mockMedicalHistory);

        Appointment mockAppointment = Mockito.mock(Appointment.class);
        when(mockAppointment.getPet()).thenReturn(mockPet);
        when(appointmentRepository.findById(1L)).thenReturn(Optional.of(mockAppointment));

        // Create the command to add a medical appointment
        CreateMedicalAppointmentCommand command = new CreateMedicalAppointmentCommand(
                "diagnosis",
                "Treatment Example",
                "Notes Example",
                1L,
                1L
        );

        // Simulate the behavior of MedicalAppointmentRepository
        MedicalAppointment mockMedicalAppointment = new MedicalAppointment(
                command.diagnosis(),
                command.treatment(),
                command.notes()
        );
        mockMedicalAppointment.setMedicalHistory(mockMedicalHistory);
        mockMedicalAppointment.setAppointment(mockAppointment);
        when(medicalAppointmentRepository.save(any(MedicalAppointment.class))).thenReturn(mockMedicalAppointment);

        /*
          Act
          Call the method to be tested
         */
        Long medicalAppointmentId = medicalAppointmentCommandService.handle(command);

        // Debugging: Print the created medical appointment details
        System.out.println("\nCreated Medical Appointment: \n------------------------------\n");
        System.out.println("Diagnosis: " + mockMedicalAppointment.getDiagnosis());
        System.out.println("Treatment: " + mockMedicalAppointment.getTreatment());
        System.out.println("Notes: " + mockMedicalAppointment.getNotes());
        System.out.println("Appointment ID: " + mockMedicalAppointment.getAppointment().getId());
        System.out.println("Medical History ID: " + mockMedicalAppointment.getMedicalHistory().getId());
        System.out.println("------------------------------\n");

        /*
          Assert
          Verify the results
         */
        assertEquals(mockMedicalAppointment.getId(), medicalAppointmentId);
        verify(appointmentRepository, times(1)).findById(command.appointmentId());
        verify(medicalAppointmentRepository, times(1)).save(any(MedicalAppointment.class));
        verify(externalMedicalHistoryService, times(1)).AddMedicalAppointmentToMedicalHistory(
                mockMedicalHistory.getId(),
                mockMedicalAppointment.getId()
        );
    }
}
```

#### US09:	Agendamiento de Citas<br>
    Como dueño de mascota, deseo agendar citas veterinarias para asegurar que mi mascota reciba atención médica en el momento adecuado.

[![Captura-de-pantalla-2025-05-16-201707.png](https://i.postimg.cc/Pq9Lhmz4/Captura-de-pantalla-2025-05-16-201707.png)](https://postimg.cc/Mc0ZmfLM)

[![Captura-de-pantalla-2025-05-16-201838.png](https://i.postimg.cc/PryPNGQN/Captura-de-pantalla-2025-05-16-201838.png)](https://postimg.cc/w7t6bGPd)<br><br>


### 5.1.1.2. Core Integration Tests

Las Core Integration Tests aseguran que los componentes clave del sistema trabajan bien juntos. Usar Postman te permite verificar manualmente y de forma visual que la API cumple con lo esperado antes o junto a las pruebas automatizadas. Es especialmente útil en etapas de desarrollo, debugging o cuando se integra un nuevo módulo.

#### HTTP GETS 

[![Captura-de-pantalla-2025-05-17-015437.png](https://i.postimg.cc/Cx5BtjRc/Captura-de-pantalla-2025-05-17-015437.png)](https://postimg.cc/3kMx00CG)

[![Captura-de-pantalla-2025-05-17-015531.png](https://i.postimg.cc/rF8tG6MX/Captura-de-pantalla-2025-05-17-015531.png)](https://postimg.cc/5jR01RXn)

[![Captura-de-pantalla-2025-05-17-015352.png](https://i.postimg.cc/FH6dQ7cN/Captura-de-pantalla-2025-05-17-015352.png)](https://postimg.cc/K1nvPcJH)

[![Captura-de-pantalla-2025-05-17-015105.png](https://i.postimg.cc/MGjcZqbR/Captura-de-pantalla-2025-05-17-015105.png)](https://postimg.cc/cK01Xqz4)

[![Captura-de-pantalla-2025-05-17-015016.png](https://i.postimg.cc/BQMPMhn8/Captura-de-pantalla-2025-05-17-015016.png)](https://postimg.cc/D84zzPsF)

#### HTTP POSTS

[![Captura-de-pantalla-2025-05-17-020125.png](https://i.postimg.cc/zfnJPBFd/Captura-de-pantalla-2025-05-17-020125.png)](https://postimg.cc/wtj819PJ)

#### HTTP UPDATE

[![Captura-de-pantalla-2025-05-17-020504.png](https://i.postimg.cc/02M1Bj8p/Captura-de-pantalla-2025-05-17-020504.png)](https://postimg.cc/BX0z8qP6)

#### HTTP DELETE

[![Captura-de-pantalla-2025-05-17-020559.png](https://i.postimg.cc/kXtLyHcs/Captura-de-pantalla-2025-05-17-020559.png)](https://postimg.cc/HVdSYBF8)


### 5.1.1.3 User Acceptance Tests

Pruebas de aceptación para las historias pertenecientes al core business son mostradas a continuación:

US01: Registro de Usuario

[![Captura-de-pantalla-2025-05-16-232803.png](https://i.postimg.cc/Dz8nc044/Captura-de-pantalla-2025-05-16-232803.png)](https://postimg.cc/Z9tGbTcJ)
<br>

US02: Autenticación de Usuarios

[![Captura-de-pantalla-2025-05-16-235349.png](https://i.postimg.cc/DZ1r82gR/Captura-de-pantalla-2025-05-16-235349.png)](https://postimg.cc/JD4DFCSQ)
<br>

US06: Visualización de Perfiles de Mascotas

[![Captura-de-pantalla-2025-05-17-003231.png](https://i.postimg.cc/G2vfdnsm/Captura-de-pantalla-2025-05-17-003231.png)](https://postimg.cc/1n5BrTHk)
<br>

US08: Gestión de Perfiles de Mascotas

[![Captura-de-pantalla-2025-05-17-000356.png](https://i.postimg.cc/4ydxjPmw/Captura-de-pantalla-2025-05-17-000356.png)](https://postimg.cc/vgJyVW76)
<br>

US09: Agendamiento de Citas

[![Captura-de-pantalla-2025-05-17-000651.png](https://i.postimg.cc/RZfZrNZr/Captura-de-pantalla-2025-05-17-000651.png)](https://postimg.cc/BjS0HZFN)
<br>

US10: Cancelación de citas

[![Captura-de-pantalla-2025-05-17-002801.png](https://i.postimg.cc/JnBLXFDf/Captura-de-pantalla-2025-05-17-002801.png)](https://postimg.cc/CBYXTm47)
<br>

### 5.1.1.4 Automated Tests

Para la ejecución de las pruebas automatizadas se tomaron en cuenta las historias de usuario primarias que formaban parte del core bussines y se utilizó la herramienta Selenium.

US02: Autenticación de Usuarios

[![Captura-de-pantalla-2025-05-17-031953.png](https://i.postimg.cc/C57hFLPF/Captura-de-pantalla-2025-05-17-031953.png)](https://postimg.cc/GTBwKrnN)
<br>

US06: Visualización de Mascotas

[![Captura-de-pantalla-2025-05-17-032251.png](https://i.postimg.cc/yYW4JPWh/Captura-de-pantalla-2025-05-17-032251.png)](https://postimg.cc/0bgHF7Yr)
<br>

US08: Gestión de Perfiles de Mascotas

[![Captura-de-pantalla-2025-05-17-032518.png](https://i.postimg.cc/QCH4MfSH/Captura-de-pantalla-2025-05-17-032518.png)](https://postimg.cc/CnpHPH3g)
<br>

US09: Agendamiento de Citas

[![Captura-de-pantalla-2025-05-17-032758.png](https://i.postimg.cc/7YN9k8qm/Captura-de-pantalla-2025-05-17-032758.png)](https://postimg.cc/svv7YLQh)
<br>

[![Captura-de-pantalla-2025-05-17-032809.png](https://i.postimg.cc/GtFQt6G3/Captura-de-pantalla-2025-05-17-032809.png)](https://postimg.cc/Zvq3D7wX)
<br>

### 5.1.1.5 Quality Attributes Tests

Para realizar pruebas no funcionales tomamos en cuenta evaluar los atributos de calidad de escalabilidad y rendimiento. Decidimos utilizar Google Lighthouse porque es una herramienta automatizada de código abierto que permite auditar aplicaciones web en aspectos clave como el rendimiento de carga, optimización para dispositivos móviles, accesibilidad, buenas prácticas de desarrollo y SEO. Lighthouse proporciona métricas cuantitativas y sugerencias de mejora, lo que nos permite identificar cuellos de botella en el rendimiento y oportunidades para optimizar la experiencia del usuario. Además, su integración con navegadores como Chrome facilita su uso en entornos de desarrollo y pruebas continuas.

**Backend**

[![Captura-de-pantalla-2025-05-17-011514.png](https://i.postimg.cc/br5pW2Dt/Captura-de-pantalla-2025-05-17-011514.png)](https://postimg.cc/ctfp8Ccx)

[![Captura-de-pantalla-2025-05-17-011503.png](https://i.postimg.cc/ZK9T3j2F/Captura-de-pantalla-2025-05-17-011503.png)](https://postimg.cc/XpbS6KVp)

**Frontend**

[![Captura-de-pantalla-2025-05-17-030840.png](https://i.postimg.cc/pTVV3vTK/Captura-de-pantalla-2025-05-17-030840.png)](https://postimg.cc/5HGMFZ8t)

[![Captura-de-pantalla-2025-05-17-030732.png](https://i.postimg.cc/R07qjGTx/Captura-de-pantalla-2025-05-17-030732.png)](https://postimg.cc/rdp841bf)


## 5.1.2. Pattern Based Backend Application(s)

Para el desarrollo del Backend se aplicaron los siguientes patrones:

<br>**Command Service**

Un Command Service es un patrón que agrupa y maneja todas las operaciones que modifican el estado de una entidad o del sistema, como crear, actualizar o eliminar datos. Estas operaciones se encapsulan en servicios específicos llamados Command Services, que se encargan de ejecutar la lógica necesaria para procesar esos cambios de forma ordenada y consistente. <br>

[![Captura-de-pantalla-2025-05-16-175210.png](https://i.postimg.cc/X7F5QDWg/Captura-de-pantalla-2025-05-16-175210.png)](https://postimg.cc/svj12mvB)
En esta imagen se puede visualizar la aplicación de este patrón para manejar la creación de una mascota.<br><br>

[![Captura-de-pantalla-2025-05-16-175559.png](https://i.postimg.cc/KY93R67m/Captura-de-pantalla-2025-05-16-175559.png)](https://postimg.cc/1gq3dYYd)
En esta figura se puede visualizar la aplicación del patrón Command Service para manejar la actualización y eliminación de una mascota.<br><br>


<br>**Query Service**

El Query Service se utiliza para realizar consultas y obtener datos del sistema sin modificar su estado, separando así la lógica de lectura de la lógica de escritura. Es especialmente útil en arquitecturas basadas en CQRS, ya que mejora la claridad del código, permite optimizar el rendimiento de las consultas y facilita el mantenimiento de la obtención de datos de la aplicación.<br>

[![Captura-de-pantalla-2025-05-16-180105.png](https://i.postimg.cc/ZRdY42V7/Captura-de-pantalla-2025-05-16-180105.png)](https://postimg.cc/wy9YkfKL)
En esta imagen se puede apreciar el uso del patron Query Service implementado para los métodos de listar todas las mascotas registradas, listar una mascota por su id y listar mascotas por el id del dueño.<br><br>


<br>**Builder**

El patrón Builder se utiliza para simplificar y controlar la creación de objetos complejos que pueden requerir múltiples pasos o configuraciones, separando el proceso de construcción de la representación final. Esto facilita la creación de instancias de manera clara, flexible y con código más legible, evitando constructores con muchos parámetros y permitiendo construir objetos configurables sin exponer detalles internos.<br>

[![Captura-de-pantalla-2025-05-16-180610.png](https://i.postimg.cc/8Py2Xwbj/Captura-de-pantalla-2025-05-16-180610.png)](https://postimg.cc/D8Xp8rHT)
En nuestro caso utilizamos builder para construir de manera ordenada y encapsulada el objeto de autenticación que Spring Security necesita para identificar al usuario y permitirle iniciar sesión. Para ello, utilizaremos un token.<br><br>


<br>**Context Facade**

[![Captura-de-pantalla-2025-05-16-182328.png](https://i.postimg.cc/XYt7mngG/Captura-de-pantalla-2025-05-16-182328.png)](https://postimg.cc/MnbSj2Nq)

Permite que otros servicios interactúen con el sistema de gestión de mascotas de manera más sencilla y directa, sin necesidad de conocer los detalles internos.<br><br>

## 5.1.3. Pattern Based Custom Software Library

### Domain Layer
Esta capa representa el núcleo del negocio. Aquí se define el **modelo de dominio** y se encapsulan las reglas de negocio más importantes. Contiene:

- **Entidades y Aggregates**: Representan objetos del dominio con identidad persistente y lógica interna.

[![Captura-de-pantalla-2025-05-17-004711.png](https://i.postimg.cc/vm0BhCmD/Captura-de-pantalla-2025-05-17-004711.png)](https://postimg.cc/LqZ26CLM)<br>

[![Captura-de-pantalla-2025-05-17-004548.png](https://i.postimg.cc/3xHdxg6r/Captura-de-pantalla-2025-05-17-004548.png)](https://postimg.cc/VdDY7bm2)<br>

- **Value Objects**: Elementos inmutables que encapsulan atributos relacionados.

[![Captura-de-pantalla-2025-05-17-004303.png](https://i.postimg.cc/0QHzkhgh/Captura-de-pantalla-2025-05-17-004303.png)](https://postimg.cc/sQ7jK6gJ)

- **Commands**: Representan acciones que modifican el estado del dominio (crear, actualizar, eliminar).

[![Captura-de-pantalla-2025-05-17-005021.png](https://i.postimg.cc/tRZdcGVK/Captura-de-pantalla-2025-05-17-005021.png)](https://postimg.cc/LhSZq7DD)

- **Queries**: Representan solicitudes de información sin intención de modificar el estado.

[![Captura-de-pantalla-2025-05-17-005210.png](https://i.postimg.cc/xCbk6YFg/Captura-de-pantalla-2025-05-17-005210.png)](https://postimg.cc/62t53sKG)

---

### ACL (Anti-Corruption Layer)
Esta capa protege el modelo de dominio de las dependencias externas. Actúa como una barrera para evitar la contaminación de modelos externos y traduce estructuras ajenas al lenguaje del dominio. Contiene:

- **Adaptadores de integración**: Clases que convierten objetos de sistemas externos a objetos del dominio.
- **Servicios externos**: Interfaces y sus implementaciones para comunicarse con otros sistemas (por ejemplo, APIs externas).
- **Traductores (Mappers/Transformers)**: Transforman modelos externos a modelos internos y viceversa.

[![Captura-de-pantalla-2025-05-17-005722.png](https://i.postimg.cc/FHRHPNYc/Captura-de-pantalla-2025-05-17-005722.png)](https://postimg.cc/jLpT2VQd)

---

### Infrastructure Layer
Se encarga de las dependencias técnicas del sistema. Aquí se implementan los detalles concretos definidos en las interfaces del dominio y se gestionan los recursos del entorno. Contiene:

- **Implementaciones de Repositorios (JPA)**: Persistencia de entidades y aggregates.

[![Captura-de-pantalla-2025-05-17-010046.png](https://i.postimg.cc/Y0hdn4BZ/Captura-de-pantalla-2025-05-17-010046.png)](https://postimg.cc/N2v8LjMk)

---

### Application Layer
Coordina los casos de uso del backend. Aquí no hay lógica de negocio profunda, sino la orquestación de las operaciones del sistema. Contiene:

- **Servicios de Aplicación**: Implementan comandos (crear, actualizar, eliminar) y consultas (lectura de datos).
- **Comandos (Commands)**: Objetos que encapsulan los datos necesarios para ejecutar una acción.
- **Consultas (Queries)**: Objetos que representan peticiones de lectura.
- **Manejadores de Casos de Uso**: Métodos que coordinan validaciones, llamadas al dominio y persistencia.

[![Captura-de-pantalla-2025-05-17-010600.png](https://i.postimg.cc/qBPFbLgG/Captura-de-pantalla-2025-05-17-010600.png)](https://postimg.cc/hh0MhVLJ)

---

### Interface Layer
Es la puerta de entrada al backend. Expone la funcionalidad del sistema a los clientes (por ejemplo, frontend, otros servicios) y gestiona la interacción con ellos. Contiene:

- **Controladores (Controllers/Handlers)**: Gestionan las solicitudes HTTP/REST.
- **Resources**: Representan estructuras de respuesta (DTOs de salida) que serán devueltas al cliente. Separan el modelo de dominio de lo que realmente se expone en la API.
- **Transform**: Encapsulan la lógica de mapeo entre los objetos del dominio o DTOs internos y los "Resources" que se exponen en la interfaz. Promueven una separación clara entre la representación interna y externa.
- **ACL Context Facade**: Se utiliza en casos donde es necesario invocar servicios o APIs externas desde la capa de interfaz de manera simplificada y desacoplada, actuando como fachada que esconde detalles técnicos.
- **Validaciones de entrada (Request Validation)**: Validan los datos que provienen del cliente (por ejemplo, con anotaciones "@Valid") antes de enviarlos al Application Layer. Aseguran que la entrada sea consistente.
- **Autenticación y Autorización**: Incluye filtros, interceptores o resolvers que gestionan quién accede a qué recurso (por ejemplo, con Spring Security), garantizando seguridad a nivel de endpoints.

[![Captura-de-pantalla-2025-05-17-010751.png](https://i.postimg.cc/9fg8GPvZ/Captura-de-pantalla-2025-05-17-010751.png)](https://postimg.cc/GBYxRD3m)


## 5.1.4. Framework Pattern Driven Refactoring Report

Actualmente, el sistema opera bajo una arquitectura monolítica con los siguientes Bounded Contexts:

- IAM (Identity & Access Management): Maneja autenticación, autorización y gestión de usuarios.

- Appointment Scheduling: Controla la programación de citas y disponibilidad de servicios.

- Pet Management: Encapsula la información y gestión de las mascotas dentro del sistema.

Si bien esta estructura es funcional, la falta de segmentación genera desafíos en mantenimiento y escalabilidad, dificultando la independencia de los módulos. Por ello, para abordar los retos de escalabilidad y modularidad, se adopta el principio de Decompose by Subdomain, permitiendo dividir el sistema en Bounded Contexts más granulares que reflejen mejor los distintos aspectos del dominio. La nueva estructura en la arquitectura de microservicios queda definida como:

- IAM: Se mantiene como un contexto independiente, proporcionando servicios de autenticación y gestión de identidades.

- Medical Appointment Management: Permanece como un servicio autónomo para la programación de citas; sin embargo, este bounded context conocido como Appointment Scheduling será refactorizado a un modelo coherente con la arquitectura expresada en el C4 y, por lo tanto, su nombre es cambiado.

Pet Management, que se divide en dos subdominios:

- Medical Record: Se encarga exclusivamente del historial clínico de la mascota, administrando diagnósticos, tratamientos y evolución médica. Separar esta funcionalidad permite un control más preciso sobre la información médica, facilitando integraciones con servicios especializados y asegurando la coherencia de los datos.

- Pet Management: Se enfoca en la administración de propietarios y mascotas, contemplando la relación entre ambos. Este subdominio maneja datos como información de identificación, historial de adopción, y características generales de la mascota, garantizando una gestión eficiente sin interferencias con aspectos clínicos.

Esta segmentación permite una mayor independencia entre servicios, reduciendo el acoplamiento y facilitando la evolución de cada módulo sin afectar el resto del sistema.

## 5.2  Software Configuration Management

### 5.2.1    Software Development Environment Configuration

En la presente sección se especifican las herramientas de software empleadas a lo largo de todas las fases del ciclo de vida del proyecto.
- Product UX/UI Design:
    - UXPressia: Se empleó para la creación de User Personas, Empathy Map e Impact Map.
    - Miro: Se utilizó para elaborar los As-Is Scenario Map y To-Be Scenario Map.
- Project Management:
    - Trello: Se utilizó esta herramienta para los Sprints y ADD Iterations.
- Software Documentation:
    - Visual Paradigm: Fue empleado para la elaboración del modelo C4 de la arquitectura de software.
    - LucidChart: Se empleó para la creación de los UML Diagrams.
    - Vertabelo: Se utilizó para elaborar nuestro Database Diagram.
    - Swagger: Se empleó para la documentación de la API.
- Software Development:
    - IntelliJ IDEA: Empleado para el desarrollo del frontend y backend.
- Software Testing:
    - Gherkin / Cucumber: Acceptance Tests
    - JUnit / Mockito: Unit Tests
    - Postman: Integration Tests
    - Google Light House: Performance Tests

### 5.2.2    Source Code Management

Para la gestión del control de versiones de nuestros proyectos de software, se emplea la plataforma GitHub. En dicha plataforma, se ha creado una organización que contiene los repositorios correspondientes.
- Organización: https://github.com/SI657-2501-Grupo-6-Fundamentos
- FrontEnd: https://github.com/SI657-2501-Grupo-6-Fundamentos/PawFect-Care-FrontEnd
- BackEnd: https://github.com/SI657-2501-Grupo-6-Fundamentos/PawFect-Care-BackEnd

Además, se implementa GitFlow como Workflow de control de versiones:

- La rama principal del repositorio es denominada *main* y representa la versión estable del software.

- A partir de *main*, se genera la rama *development*, en la cual se integran las funcionalidades que han sido completadas.

- Las ramas que se deriven de *development* deberán seguir un formato de nomenclatura claro y descriptivo, que permita identificar de manera precisa la funcionalidad en desarrollo.

- En cuanto al manejo del código, se establece como práctica utilizar letras minúsculas en los nombres de las ramas, con el objetivo de mantener la consistencia y evitar posibles inconvenientes en el control de versiones. Asimismo, se recomienda emplear nombres concisos para archivos y ramas, evitando términos genéricos o ambiguos.

### 5.2.3    Source Code Style Guide & Conventions
Para mantener un código limpio, legible y fácil de mantener en equipo, se definieron guías de estilo específicas por tecnología, complementadas con linters automáticos y convenciones de nomenclatura. Estas prácticas se alinean con los principios de *Clean Code* y las recomendaciones de la comunidad técnica para cada stack.

#### **Pruebas unitarias (Gherkin + Cucumber)**
- Se adoptó Gherkin, el cual es un lenguaje estructurado utilizado para describir el comportamiento esperado del software mediante ejemplos concretos. Utiliza una sintaxis simple basada en palabras clave como `Feature`, `Escenario`, `Dado`, `Cuando` y `Entonces`, lo que permite que tanto desarrolladores como personas no técnicas colaboren en la definición de requisitos. Cada especificación se escribe en archivos con extensión `.feature`, facilitando la automatización de pruebas y asegurando que el sistema cumpla con las expectativas funcionales del usuario.
    - Convenciones:
        - `Feature`: Describe la funcionalidad a probar.
        - `Escenario`: Describe una situación específica o caso de uso.
        - `Dado`: Estado inicial o precondición.
        - `Cuando`: Acción principal que se realiza.
        - `Entonces`: Resultado esperado tras la acción.
        - `Y`: Se usan para extender los pasos `Dado`, `Cuando` o `Entonces`.

#### **Frontend Web (Angular con TypeScript)**
- Se adoptó Angular, el cual es un framework de desarrollo web frontend basado en TypeScript. Está diseñado para construir aplicaciones web de una sola página (SPA) estructuradas y escalables, mediante el uso de componentes, inyección de dependencias, enrutamiento, servicios y un sistema de templates declarativo.
- Las convenciones usadas son:
  - Carpetas:
    - Separadas por módulos (`feature-modules`)
    - Nombres: Como `nombre.component.ts`, `nombre.service.ts`, `nombre.module.ts`.
  - Nombres:
    - Componentes, servicios, módulos: `PascalCase`.
    - Variables y funciones: `camelCase`.

#### **Backend (Spring Boot + Java)**
- Se adoptó la guía oficial de estilo de Java + convención de Spring:
  - Clases en **PascalCase** (`UserService`, `PublicationController`).
  - Variables y métodos en **camelCase** (`getPublications()`, `userId`).
  - Separación en paquetes según capa: `controller`, `service`, `repository`, `model`.
  - Uso de anotaciones estándar (`@RestController`, `@Autowired`, `@GetMapping`).
  - Código documentado con comentarios Javadoc (`/** */`) en servicios y endpoints principales.

#### **General**
- Todos los equipos usaron **pre-commit hooks** con `Husky` (para frontend) y scripts personalizados en backend para evitar commits con errores de formato o linters.
- Se definieron **convenciones de nomenclatura de commits** usando el formato:
  - `feat:` para nuevas funcionalidades.
  - `fix:` para corrección de errores.
  - `docs:` para documentación.
  - `refactor:` para mejoras internas sin cambios funcionales.
  - `style:` para cambios de formato sin alterar la lógica.
Estas convenciones fueron aplicadas de forma continua mediante integración con GitHub Actions y revisión manual por parte del líder técnico antes de cada merge a `develop` y luego a `feat/deploy` .

### 5.2.4    Software Deployment Configuration

#### 1. Landing Page

La página de entrada al producto, centrada en captar la atención de potenciales usuarios y presentar nuestra propuesta de valor:

- **Tecnologías**  
  - HTML5 semántico  
  - CSS3 con animaciones ligeras  
  - JavaScript vanilla para interactividad básica  

- **Despliegue**  
  - **Plataforma:** GitHub Pages  
  - **Branch:** `main`  
  - **Flujo:** mediante GitHub Actions, tras cada `push` a `main`, los archivos de la carpeta `docs/` se publican en el dominio configurado.  
  - **Beneficios:** publicación inmediata, versión de revisión histórica disponible, y control de versiones integrado con Git.  

Esta configuración asegura que la landing esté siempre al día, sirviendo como escaparate público y primer punto de contacto para nuevos usuarios e inversores.


#### 2. Frontend Web  
La Aplicacion web desarrollada en Angular que ofrece la experiencia de usuario rica e interactiva:

- **Tecnologías**  
  - Angular v19

- **Despliegue**  
  - **Plataforma:** Firebase Hosting  
  - **Branch:** `feat/deploy`  
  - **Flujo:** un `push` a la rama `feat/deploy` ejecuta un script de build y luego publica automáticamente los archivos estáticos en Firebase  para entregas ultrarrápidas.  
  - **Beneficios:** SSL automático, previews de despliegue y rollback sencillo en caso de rollback.  

Con esto cualquier mejora o corrección en la interfaz llega casi instantáneamente a los usuarios finales, sin interrupciones.


#### 3. Backend RESTful  
Un servicio construido con Spring Boot que gestiona toda la lógica de negocio y persistencia de datos:

- **Tecnologías**  
  - Spring Boot 3.2
  - Java 21  
  - PostgreSQL

- **Despliegue**  
  - **Plataforma:** Azure App Services  
  - **Branch:** `feat/deploy`  
  - **Flujo:** cada vez que se hace un `push` a `feat/deploy`, un pipeline en Azure se dispara automáticamente, compila y actualiza el entorno productivo.  
  - **Beneficios:** escalado automático, monitorización nativa, configuración de variables de entorno (como cadenas de conexión y claves secretas) directamente en el portal de Azure.  

Este esquema garantiza que el backend esté siempre disponible bajo HTTPS, con tolerancia a fallos y capacidad de crecer según la demanda.

Con estos tres componentes automatizados, AventuraPe dispone de un entorno de producción sólido y escalable, listo para crecer con cada nueva funcionalidad y mantener la continuidad del servicio sin fricciones.

## 5.3  Microservices Implementation
En esta sección explicamos y evidenciamos el proceso de implementación, pruebas, documentación y despliegue del Web Service.

### 5.3.1   Sprint 1

#### 5.3.1.1       Sprint Backlog 1
| **Sprint #**   | **Sprint 1**                                                                                                                                                                                                                  |     |     |                                                                                             |           |                    |     |
|-----------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----|-----|---------------------------------------------------------------------------------------------|-----------|--------------------|-----|
| **User Story**  |   |  **Work-item / Task**    |     |                                                                                             |           |                    |     |
| **ID**         | **Title**                        | **Id** | **Title**                        | **Description**                                                                             | **Estimation (hours)** | **Assigned To**    | **Status (To-do / In-Process / To-Review / Done)** |
| **US01**     | Registro de Usuario | **T01** | Registro de Usuario | Implementar el registro de usuarios |   1h   |  José Gutierrez  |  Done   |
| **US02**     | Autenticación de Usuarios | **T02** | Autenticación de Usuarios | Implementar la autenticación de usuarios |   1h   |  José Gutierrez  |  Done   |
| **US04**     | Creación de Perfil de Mascota | **T03** | Creación de Perfil de Mascota | Implementar el correcto formulario para la creción del perfil de la mascota |   2h   |  Rodrigo Chirinos  |  Done   |
| **US05**     | Edición de Perfil de Mascota | **T04** | Edición de Perfil de Mascota | Implementar el formulario adecuado para editar el perfil de la mascota |   2h   |  Rodrigo Chirinos  |  Done   |
| **US06**     | Visualización de Perfiles de Mascotas	 | **T05** | Visualización de Perfiles de Mascotas	 | Implementar la vista para la visualización de Perfiles de Mascotas	 |   2h   |  José Gutierrez  |  Done   |
| **US08**     | Gestión de Perfiles de Mascotas | **T06** | Gestión de Perfiles de Mascotas | Implementar la correcta gestión de los perfiles de las mascotas. |   2h   |  Oscar Aranda  |  Done   |
| **US09**     | Agendamiento de Citas | **T07** | Agendamiento de Citas | Implementar el formulario pertinente para que se puedan agendar las citas. |   2h   |  Rodrigo Chirinos  |  Done   |
| **US010**     | Cancelación de Citas | **T08** | Cancelación de Citas | Implementar la opción de cancelar una cita. |   2h   |  Oscar Aranda  |  Done   |
| **US12**     | Edición de Citas Veterinarias | **T09** | Edición de Citas Veterinarias | Implementar la opción de editar una cita programada. |   2h   |  Renzo Silva  |  Done   |
| **US13**     | Búsqueda de dueños de mascota | **T10** | Búsqueda de dueños de mascota | Implementar la opción de buscar a las mascotas. |   2h   |  José Gutierrez  |  Done   |
| **US14**     | Consulta sobre alimentación adecuada | **T11** | Consulta sobre alimentación adecuada | Implementar la opción para que la veterinaria registre este servicio. |   2h   |  Oscar Aranda  |  Done   |
| **US15**     | Consejos de higiene para mascotas | **T12** | Consejos de higiene para mascotas | Implementar la opción para que la veterinaria registre este servicio. |   3h   |  José Gutierrez  |  Done   |
| **US16**     | Preguntas frecuentes sobre salud | **T13** | Preguntas frecuentes sobre salud | Implementar la opción para que la veterinaria registre este servicio.|   2h   |  Renzo Silva  |  Done   |
| **US17**     | Consejos de entrenamiento básico | **T14** | Consejos de entrenamiento básico | Implementar la opción para que la veterinaria registre este servicio. |   3h   |  José Gutierrez  |  Done   |
| **US18**     | Recomendaciones según tipo de mascota | **T15** | Recomendaciones según tipo de mascota | Implementar la opción de las recomendaciones. |   2h   |  Renzo Silva  |  Done   |
| **US19**     | Visualización del Historial Médico | **T16** | Visualización del Historial Médico | Implementar la opción para visualizar el historial médico. |   2h   |  José Gutierrez  |  Done   |
| **US20**     | Actualización del Historial Médico | **T17** | Actualización del Historial Médico | Implementar la opción para editar y actualizar el historial médico. |   2h   |  Oscar Aranda  |  Done   |

#### 5.3.1.2       Development Evidence for Sprint Review

En esta sección, se presentan los commits realizados en el repositorio del front end, back end, back end testing y el reporte en GitHub. Estos commits reflejan el progreso y las mejoras implementadas durante el Sprint 1, proporcionando una visión detallada de las actividades de desarrollo y las contribuciones del equipo.

| **Repository**                                                                 | **Branch** | **Commit Id**                              | **Commit Message**                                                                                                                                                                                                                                                                        | **Commit Message Body** | **Committed on (Date)** |
|--------------------------------------------------------------------------------|------------|--------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------|-------------------------|
| [https://github.com/SI657-2501-Grupo-6-Fundamentos/PawFect-Care-BackEnd](https://github.com/SI657-2501-Grupo-6-Fundamentos/PawFect-Care-BackEnd) | main | `caa88605581ed16bfd96147b35a5b18537ae8b83` | feat: add backend | - | 09/05/25 |
| [https://github.com/SI657-2501-Grupo-6-Fundamentos/PawFect-Care-FrontEnd](https://github.com/SI657-2501-Grupo-6-Fundamentos/PawFect-Care-FrontEnd) | main | `074a0d5932e28c81ac7ac80d606c9cc04f49a15c` | feat: Add front end | - | 16/05/25 |
| [https://github.com/SI657-2501-Grupo-6-Fundamentos/Pawfect-Care-report/tree/tp](https://github.com/SI657-2501-Grupo-6-Fundamentos/Pawfect-Care-report/tree/tp) | tp | `3eb8bd4fafa5b9ee99a82119218cc3515e97aa7e` | feat(report): add chore | - | 16/05/25 |
| [https://github.com/SI657-2501-Grupo-6-Fundamentos/Pawfect-Care-report/tree/tp](https://github.com/SI657-2501-Grupo-6-Fundamentos/Pawfect-Care-report/tree/tp) | tp | `789d2a9aa0a238ad222e1ca100c421477bf49e39` | feat(report): add Pattern Based Backend Application(s) | - | 16/05/25 |
| [https://github.com/SI657-2501-Grupo-6-Fundamentos/Pawfect-Care-report/tree/tp](https://github.com/SI657-2501-Grupo-6-Fundamentos/Pawfect-Care-report/tree/tp) | tp | `bfdc851661e380af28a4b46efb65d8ad975c215f` | feat(docs): add Unit Test: CreatePetCommand | - | 16/05/25 |
| [Pawfect-Care-Backend-Testing](https://github.com/SI657-2501-Grupo-6-Fundamentos/Pawfect-Care-Backend-Testing) | `dev`     |  `f0ed7cc39cae8492ff5384a8288e3bf6ffdabaef`   | feat: add MedicalAppointmentCommandServiceTest | - | 16/05/25 |
| [Pawfect-Care-Backend-Testing](https://github.com/SI657-2501-Grupo-6-Fundamentos/Pawfect-Care-Backend-Testing) | `dev`     |  `16917e34ddb2f6769e48204bb1709b425e48c0ce`   | feat: add PetCommandServiceTest for updating a pet | - | 16/05/25 |
| [Pawfect-Care-Backend-Testing](https://github.com/SI657-2501-Grupo-6-Fundamentos/Pawfect-Care-Backend-Testing) | `dev`     | `16917e34ddb2f6769e48204bb1709b425e48c0ce` | feat: Add PetCommandServiceTest & OwnerCommandServiceTest | - | 16/05/25 |


#### 5.3.1.3       Testing Suite Evidence for Sprint Review

En este sprint, se han incorporado pruebas de aceptación escritas en **Gherkin**, asegurando que los requisitos del usuario se validen de manera efectiva. A continuación, se proporciona el enlace al repositorio de las pruebas de aceptación, donde se encuentra una descripción detallada de los escenarios de prueba y su implementación:

**Repositorio de pruebas de aceptación:**  
[https://github.com/SI657-2501-Grupo-6-Fundamentos/Pawfect-Care-Backend-Testing](https://github.com/SI657-2501-Grupo-6-Fundamentos/Pawfect-Care-Backend-Testing)

| **Repository**                                                                             | **Branch** | **Commit Id**                          | **Commit Message**                                                                                                                                                         | **Commit Message Body** | **Committed on (Date)** |
|--------------------------------------------------------------------------------------------|------------|----------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------|-------------------------|
| [Pawfect-Care-Acceptance-Tests](https://github.com/SI657-2501-Grupo-6-Fundamentos/Pawfect-Care-Acceptance-Tests) | `main`     | `5ba730d2580f106bf46ee74aa7d6b9baab668554` | feat: add gherkin files .feature | - | 16/05/25 |


#### 5.3.1.4       Execution Evidence for Sprint Review

En esta seccion mostramos la ejecucion de nuestros servicios:

#### Backend

![Evidence Back1](./assets/chapter05/sprint1/exceution_evidence/execution_back1.png)

![Evidence Back2](./assets/chapter05/sprint1/exceution_evidence/execution_back2.png)

![Evidence Back3](./assets/chapter05/sprint1/exceution_evidence/execution_back3.png)

![Evidence Back4](./assets/chapter05/sprint1/exceution_evidence/execution_back4.png)

![Evidence Back5](./assets/chapter05/sprint1/exceution_evidence/execution_back5.png)

#### FrontEnd

![Evidence Front](./assets/chapter05/sprint1/exceution_evidence/execution_front.jpg)

#### 5.3.1.5       Microservices Documentation Evidence for Sprint Review

En esta seccion presentamos las capturas de los endpoints de microservicios que tiene nuestro BackEnd:

![MicroService Evidence 1](./assets/chapter05/sprint1/microservices_evidence/microservice_evidence1.png)

![MicroService Evidence 2](./assets/chapter05/sprint1/microservices_evidence/microservice_evidence2.png)

![MicroService Evidence 3](./assets/chapter05/sprint1/microservices_evidence/microservice_evidence3.png)


En esta seccion presentamos las capturas de los servicios que tiene nuestro FrontEnd:

#### Inicio:
![Front1](./assets/chapter05/sprint1/microservices_evidence/Front1.png)

#### Vista para registrar clientes o para visualizarlos:
![Front2](./assets/chapter05/sprint1/microservices_evidence/Front2.png)

#### Vista para registrar mascotas o para visualizarlas:
![Front3](./assets/chapter05/sprint1/microservices_evidence/Front3.png)

#### Vista para registrar una cita o para visualizarlas:
![Front4](./assets/chapter05/sprint1/microservices_evidence/Front4.png)


Acá presentamos las capturas de los endpoints de microservicios que tiene nuestro BackEnd:

#### 5.3.1.6       Software Deployment Evidence for Sprint Review

En esta seccion mostramos las evidencias de nuestro deployment con azure app services:

#### Vista del servicio de Azure App Services:
![Deployment Evidence 1](./assets/chapter05/sprint1/deployment_evidence/deploy_evidence1.png)

#### Vista del servicio Servidor flexible de Azure Database for PostgreSQL :
![Deployment Evidence 2](./assets/chapter05/sprint1/deployment_evidence/deploy_evidence2.png)

#### Vista del dashboard del servicio de hosting Firebase para el web frontend

[![Captura-de-pantalla-2025-05-17-030141.png](https://i.postimg.cc/KYkDBXFr/Captura-de-pantalla-2025-05-17-030141.png)](https://postimg.cc/VSwtPVJd)


#### 5.3.1.7       Team Collaboration Insights during Sprint

En esta seccion Mostramos la colaboracion de todos los integrantes en todos nuestros repositorios.

#### Repositorio para el Report
![Team Insights 1](./assets/chapter05/sprint1/team_insights/insights1.png)

#### Repositorio para el BackEnd
![Team Insights 2](./assets/chapter05/sprint1/team_insights/insights2.png)

#### Repositorio para el FrontEnd
![Team Insights 3](./assets/chapter05/sprint1/team_insights/insights3.png)

#### Repositorio para el Acceptance-Tests
![Team Insights 4](./assets/chapter05/sprint1/team_insights/insights4.png)

#### Repositorio para el Testing del Backend
![Team Insights 5](./assets/chapter05/sprint1/team_insights/insights5.png)


#### 5.3.1.8       Kanban Board
A continuación presentamos nuestro Kanban Board Realizado en Trello, correspondiente al Sprint 1. En él se reflejan las distintas etapas del flujo de trabajo (To‑Do, In‑Process, Testing y Done) y la asignación de cada User Story a su estado actual, facilitando la visualización clara del avance del equipo y la identificación de cuellos de botella. Este tablero nos permitió coordinar esfuerzos, priorizar tareas y asegurar que todas las historias de usuario planificadas para el sprint se completaran con éxito.

![Kanban Board 1](./assets/chapter05/sprint1/kanbanboard1.png)
