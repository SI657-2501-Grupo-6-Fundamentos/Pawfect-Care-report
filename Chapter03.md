
# Capítulo III: Requirements Specification

## 3.1. To-Be Scenario Mapping.

- **Primer segmento: Clinicas Veterinarias**

<br><img src="./assets/Chapter03/Tobe1.jpeg" alt="To Be Scenario Map 1" style="width: 1000px; height: auto;" ><br>

- **Segundo segmento: Dueños de Mascotas**

<br><img src="./assets/Chapter03/Tobe2.jpeg" alt="To Be Scenario Map 2" style="width: 1000px; height: auto;" ><br>


## 3.1.1. Requisitos Funcionales

### Gestión de Usuarios y Clientes
- **RF01.** El sistema debe permitir a los dueños de las mascotas y a los veterinarios registrarse en la plataforma. Para ello se requiere que ingresen su nombre completo, teléfono, correo electrónico y contraseña. Además, si el usuario es un médico veterinario se le pedirá ingresar su especialidad. Por otro lado, si es dueño de mascota, deberá añadir su dirección.
- **RF02.** El sistema debe permitir a los usuarios iniciar sesión, ingresando su correo electrónico y contraseña.
- **RF03.** El sistema debe permitir a los dueños de las mascotas y a los veterinarios crear y editar su perfil.

### Gestión de Mascotas
- **RF04.** El sistema debe permitir a los dueños crear perfiles de sus mascotas y asignarle un historial médico en blanco.
- **RF05.** El sistema debe permitir a los dueños editar la información de sus mascotas.
- **RF06.** El sistema debe permitir a los dueños de mascotas visualizar los perfiles de sus mascotas.
- **RF07.** El sistema debe permitir a los dueños de mascotas eliminar el perfil de su mascota
- **RF08.** El veterinario debe poder buscar mascotas primero por el nombre del dueño y luego por nombre de mascota.

### Gestión de Citas
- **RF09.** El sistema debe permitir a los dueños de mascotras agendar citas veterinarias.
- **RF10.** El sistema debe permitir a los dueños de mascotras cancelar sus citas.
- **RF11.** El sistema debe permitir al médico veterinario gestionar y editar citas.
- **RF12.** El sistema debe permitir que, tanto médicos veterinarios como dueños de mascotas, busquen citas por su fecha.
- **RF13.** El sistema debe permitir a los veterinarios poder buscar, por su nombre y dni, a un dueño de una mascota con los cuales se haya agendado una cita pendiente.

### Historial Médico
- **RF14.** El sistema debe permitir a los dueños visualizar el historial médico de sus mascotas.
- **RF15.** El sistema debe permitir a los veterinarios registrar actualizaciones en el historial médico de una mascota.
- **RF22.** El sistema debe permitir a los veterinarios registrar el historial médico de una mascota.

### Reseñas
- **RF16.** El sistema debe permitir a los dueños de las mascotas publicar reseñas sobre la atención veterinaria recibida.
- **RF17.** El sistema debe permitir a los dueños visualizar las reseñas publicadas por otros propietarios.

### Chatbot Informativo
- **RF18.** El sistema debe proporcionar un chatbot que brinde consejos a los dueños de mascotas sobre:
  - Alimentación de mascotas.
  - Higiene animal.
  - Salud y síntomas.
  - Entrenamiento básico.
  - Recomendaciones personalizadas según tipo de mascota.

### Gestión de Servicios
- **RF19.** El sistema debe permitir a los veterinarios ingresar el tarifario de cada uno de los servicios que ofrecen. Los servicios que puede realizar un veterinarios fueron seleccionados al momento de su registro y pueden ser los siguientes: Vacunación, Desparasitación interna y externa, Control antipulgas y antigarrapatas, Chequeo general de salud, Control de peso y nutrición, Evaluación geriátrica (para animales mayores), Esterilización o castración, Cirugías de tejidos blandos (tumores, hernias, etc), Cirugía ortopédica (fracturas, displasias), Cirugías oftalmológicas (cataratas, entropión), Cirugías odontológica, Suturas por heridas, Cesáreas y partos asistidos, Radiografías y Ecografías, etc.
- **RF20.** El sistema debe permitir a los dueños de mascotas seleccionar una tarifa que mejor se adapte a sus necesidades para que la cita sea agendada y recibir el servicio al precio que él desee. 
- **RF21.** El sistema debe permitir a los veterinarios publicar sus horarios disponibles para la atención para que el dueño de la mascota elija el de su preferencia y la cita sea agendada. 


## 3.1.2. Requisitos No Funcionales

Los Requisitos No Funcionales (RNF) establecen condiciones esenciales de calidad que el sistema debe cumplir, más allá de sus funciones básicas. A continuación se muestran los RNF alineados con los atributos de calidad definidos por Bass, Clements y Kazman (2012), los cuales se enfocan en las siguientes áreas.
1. **Disponibilidad**  
   Indica si el sistema está operable y accesible cuando los usuarios lo necesitan. Un sistema altamente disponible puede tolerar fallos y mantenerse en ejecución sin interrupciones.

2. **Seguridad**  
   Representa el grado de protección del sistema contra accesos no autorizados, uso indebido o ataques. Un sistema seguro protege tanto la información como sus servicios.

3. **Desempeño**  
   Evalúa la eficiencia con la que el sistema responde a solicitudes y realiza tareas, considerando el uso de recursos como CPU, memoria y tiempo de respuesta.

4. **Facilidad de prueba**  
   Mide cuán fácil es diseñar, ejecutar y evaluar pruebas efectivas del sistema. Esto incluye pruebas unitarias, de integración y de aceptación.

5. **Modificabilidad**  
   Describe el esfuerzo requerido para realizar cambios en el sistema, como agregar nuevas funcionalidades, corregir errores o adaptar el sistema a nuevos entornos.

6. **Usabilidad**  
   Indica qué tan fácil y eficiente es para los usuarios interactuar con el sistema. Incluye factores como intuición, accesibilidad y curva de aprendizaje.

7. **Interoperabilidad**  
   Se refiere a la capacidad del sistema para intercambiar información y trabajar conjuntamente con otros sistemas mediante interfaces bien definidas.

| Código | Descripción                                                                                            | Métrica (con Método de Evaluación)                                                                                                           | Atributo de Calidad       |
|--------|--------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------|---------------------------|
| RNF01  | El sistema debe estar disponible 24/7 para todos los usuarios.                                         | Debe tener más del 99.9% de disponibilidad mensual                                                                                           | Disponibilidad            |
| RNF02  | El sistema debe requerir contraseñas robustas para el inicio de sesión.                                | El 100% de contraseñas cumplen con política de tener más de 8 caracteres entre mayúsculas, minúsculas, números y un símbolo.                 | Seguridad                 |
| RNF03  | La información de los dni de los usuarios deben almacenarse cifrados.                                  | El 100% de los campos  sobre los dni de los veterinarios y dueños de una mascota deben estar cifrados con AES-256 en la base de datos.       | Seguridad                 |
| RNF04  | La información de los teléfonos de los usuarios deben almacenarse cifrados.                            | El 100% de los campos  sobre los teléfonos de los veterinarios y dueños de una mascota deben estar cifrados con AES-256 en la base de datos. | Seguridad                 |
| RNF05  | El 95% de las operaciones CRUD deben completarse en menos de 3 segundos. Esto incluye agregar, editar o eliminar un registro de historial medico, un registro de mascota, el perfil del dueño de mascota y el perfil del médico veterinario encargado             | El tiempo de respuesta de una operación CRUD debe ser, como mínimo, menor a 3 segundos en un 95% de 100 operaciones simuladas con Apache JMeter.                                                        | Desempeño                 |
| RNF06  | La pantalla de inicio debe cargar en menos de 2 segundos en conexión de 20 Mbps.                       | El tiempo de carga de la pantalla de inicio debe ser menor a 2 segundos en al menos 3 navegadores modernos (Edge, Chrome y Opera).                                                      | Desempeño                 |
| RNF07  | El sistema debe soportar al menos 100 usuarios simultáneos sin degradación.                            | Debe existir menos del 10% de degradación en los tiempos de carga de la pantalla principal de la aplicación durante prueba de carga con 100 usuarios concurrentes.                                                  | Desempeño                 |
| RNF08  | El código debe estar documentado para facilitar su comprensión.                                        | El 60% del código del backend  debe estar documentado con JavaDoc y en inglés, colocando información de propósito como mínimo.                                                   | Modificabilidad           |
| RNF09  | El sistema debe permitir añadir nuevas funcionalidades sin modificar más del 30% del código existente. | Debe haber menos del 30% de líneas modificadas, respecto al total de líneas, para agregar nueva funcionalidad. Esto se puede medir con Git diff.                                                                    | Modificabilidad           |
| RNF10  | El sistema debe ser calificado como fácil de usar por los usuarios.                                    | El 80% de usuarios califican  la facilidad de uso de la interfaz con un 4 en escala de 1 a 5 en encuestas post-prueba                                        | Usabilidad                |
| RNF11  | El sistema debe ser compatible con navegadores modernos.                                               | Funcionalidad completa debe poder realizarse en 3 navegadores como mínimo (Chrome, Edge, Opera).                                                                | Interoperabilidad         |
| RNF12  | El sistema debe escalar horizontalmente si la carga supera el 80%.                                     | Latencia media de 3 segundos durante escalamiento automático con 200 usuarios simultáneos.                                                           | Escalabilidad             |                                                     | Escalabilidad             |

## 3.1.3 Matriz User Stories vs Requisitos Funcionales

| Requisito | US01 | US02 | US03 | US04 | US05 | US06 | US07 | US08 | US09 | US10 | US11 | US12 |
|-----------|------|------|------|------|------|------|------|------|------|------|------|------|
| **RF01**  | ✔    |      |      |      |      |      |      |      |      |      |      |      |
| **RF02**  |      | ✔    |      |      |      |      |      |      |      |      |      |      |
| **RF03**  |      |      | ✔    |      |      |      |      |      |      |      |      |      |
| **RF04**  |      |      |      | ✔    |      |      |      |      |      |      |      |      |
| **RF05**  |      |      |      |      | ✔    |      |      |      |      |      |      |      |
| **RF06**  |      |      |      |      |      | ✔    |      |      |      |      |      |      |
| **RF07**  |      |      |      |      |      |      |      | ✔    |      |      |      |      |
| **RF08**  |      |      |      |      |      |      | ✔    |      |      |      |      |      |
| **RF09**  |      |      |      |      |      |      |      |      | ✔    |      |      |      |
| **RF10**  |      |      |      |      |      |      |      |      |      | ✔    |      |      |
| **RF11**  |      |      |      |      |      |      |      |      |      |      |      | ✔    |
| **RF12**  |      |      |      |      |      |      |      |      |      |      | ✔    |      |

| Requisito | US13 | US14 | US15 | US16 | US17 | US18 | US19 | US20 | US21 | US22 | US23 | US24 |
|-----------|------|------|------|------|------|------|------|------|------|------|------|------|
| **RF13**  | ✔    |      |      |      |      |      |      |      |      |      |      |      |
| **RF14**  |      |      |      |      |      |      | ✔    |      |      |      |      |      |
| **RF15**  |      |      |      |      |      |      |      | ✔    |      |      |      |      |
| **RF16**  |      |      |      |      |      |      |      |      | ✔    |      |      |      |
| **RF17**  |      |      |      |      |      |      |      |      |      | ✔    |      |      |
| **RF18**  |      | ✔    | ✔    | ✔    | ✔    | ✔    |      |      |      |      |      |      |
| **RF19**  |      |      |      |      |      |      |      |      |      |      | ✔    |      |
| **RF20**  |      |      |      |      |      |      |      |      |      |      |      | ✔    |



## 3.2. User Stories
## Gestión de Usuarios
**EP01: Como administrador, deseo gestionar los usuarios para asegurar que solo personas autorizadas tengan acceso al sistema.**

| User Story ID | Título                     | Descripción                                                                                                                                                    |
|---------------|----------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| US01          | Registro de Usuario        | Como visitante, deseo registrarme en la plataforma para poder utilizar las funcionalidades del sistema.                                                        |
| US02          | Autenticación de Usuarios | Como usuario registrado, deseo poder iniciar sesión, ingresando mi correo electrónico y contraseña para poder utilizar los servicios de la aplicación.     |
| US03          | Gestión de Cuentas de Usuarios | Como dueño de mascota y médico veterinario, deseo gestionar el perfil de mi cuenta para mantener la información actualizada.                                    |

---
# Gestión de Mascotas
**EP02: Como usuario, deseo gestionar la información de mis mascotas para mantener sus datos actualizados.**

| User Story ID | Título                     | Descripción                                                                                                                                                    |
|---------------|----------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| US04          | Creación de Perfil de Mascota | Como dueño, deseo crear un perfil de mi mascota para tener su información almacenada en la plataforma.                                                  |
| US05          | Edición de Perfil de Mascota | Como dueño, deseo editar el perfil de mi mascota para actualizar su información cuando sea necesario.                                                    |
| US06          | Visualización de Perfiles de Mascotas | Como dueño, deseo visualizar los perfiles de mis mascotas para revisar la información registrada.                                                    |
| US07          | Búsqueda de Mascotas por nombre del dueño y luego por el nombre de la mascota | Como médico veterinario, deseo buscar mascotas por su nombre para acceder rápidamente a su información en el sistema.                                                   |
| US08          | Gestión de Perfiles de Mascotas | Como dueño de mascota, deseo gestionar y poder eliminar los perfiles de mis mascotas para asegurarme de que la información esté correctamente registrada y actualizada.      |

---

# Gestión de Citas Veterinarias
**EP03: Como usuario, deseo gestionar las citas veterinarias de mis mascotas para asegurarme de que reciban atención médica a tiempo.**

| User Story ID | Título                     | Descripción                                                                                                                                                    |
|---------------|----------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| US09         | Agendamiento de Citas      | Como usuario, deseo agendar citas veterinarias para asegurar que mi mascota reciba atención médica en el momento adecuado.                                     |
| US10          | Cancelación de Citas       | Como usuario, deseo cancelar una cita si no puedo asistir para evitar problemas de horario y reorganizar la atención.                                        |
| US11          | Búsqueda de Citas por fecha   | Como dueño de mascota o médico veterinario, deseo poder buscar citas por fecha para acceder rápidamente a la información de la cita.                                                           |
| US12          | Edición de Citas Veterinarias | Como médico veterinario, deseo editar las citas para hacer cambios en la fecha o estado cuando sea necesario.                                                 |
| US13          | Búsqueda de dueños de mascota | Como  médico veterinario, deseo poder buscar citas de clientes agendados por su nombre y DNI para poder ubicarlos rápidamente.    |

---

# Consultas Automatizadas
**EP04: Como usuario, deseo realizar consultas simples para obtener información rápida sobre el cuidado y bienestar de mi mascota.**

| User Story ID | Título                                | Descripción                                                                                                                                      |
|---------------|----------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|
| US14         | Consulta sobre alimentación adecuada   | Como dueño, deseo consultar al asistente artificial (chatbot) sobre qué tipo de comida es ideal para mi mascota según su especie, edad y tamaño.                      |
| US15         | Consejos de higiene para mascotas      | Como dueño, deseo recibir recomendaciones básicas de higiene para mantener saludable a mi mascota mediante el asistente artificial (chatbot).                                            |
| US16         | Preguntas frecuentes sobre salud       | Como dueño de mascota, deseo obtener respuestas rápidas sobre síntomas comunes y saber cuándo debo acudir al veterinario.                                |
| US17          | Consejos de entrenamiento básico       | Como dueño de mascota, deseo consultar sobre técnicas de adiestramiento o corrección de comportamientos no deseados.                                     |
| US18          | Recomendaciones según tipo de mascota  | Como dueño, deseo que el chatbot me dé consejos generales adaptados al tipo de mascota que tengo (perro, gato, ave, etc).                    |

---

# Gestión de Historial Médico de las Mascotas
**EP05: Como usuario o administrador, deseo gestionar el historial médico de las mascotas para llevar un registro de sus atenciones y tratamientos.**

| User Story ID | Título                     | Descripción                                                                                                                                                    |
|---------------|----------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| US19          | Visualización del Historial Médico | Como dueño, deseo visualizar el historial médico de mi mascota para revisar su estado de salud y tratamientos previos.                                  |
| US20          | Creación del Historial Médico | Como doctor veterinario, deseo crear el historial médico de las mascotas para que los dueños tengan la información de sus mascotas en el sistema. |
| US21          | Actualización del Historial Médico | Como doctor veterinario, deseo actualizar el historial médico de las mascotas para que los dueños tengan la información más reciente sobre sus tratamientos. |

---

# Reviews y Feedback
**EP06: Como usuario dueño de una mascota, deseo poder dejar reseñas y comentarios sobre un doctor veterinario.**

| User Story ID | Título                     | Descripción                                                                                                                                                    |
|---------------|----------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| US22          | Publicar Reseñas | Como usuario dueño de una mascota, deseo dejar una reseña sobre un doctor veterinario para compartir mi experiencia con otros usuarios.                   |
| US23          | Visualización de Reseñas | Como dueño de una mascota, deseo ver las reseñas de otros usuarios sobre un doctor veterinario para conocer la calidad del servicio y su calificación general. |

---

# Gestión de Servicios y Tarifas
**EP07: Como médico veterinario, deseo ingresar tarifas por los servicios requeridos por un dueño de mascota para que él pueda conocer los precios que le ofrezco.**

| User Story ID | Título                           | Descripción                                                                                                                                                                  |
|---------------|----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| US24          | Ofrecer tarifa por servicio      | Como médico veterinario, deseo ofrecer una tarifa personalizada para un servicio solicitado por un dueño de mascota mediante una cita, para que él pueda evaluar mi propuesta. |
| US25          | Visualización de Reseñas y Tarifas | Como dueño de una mascota, deseo ver las reseñas y tarifas ofrecidas por distintos veterinarios para un servicio específico solicitado en una cita, y así elegir la mejor opción. |
| US26          | Registro de horarios | Como médico veterinario, deseo publicar mis horarios disponibles para un servicio solicitado por un dueño de mascota mediante una cita, para que él pueda elegir.  |


---

# Navegación y Funcionalidades de la Landing Page
**EP08: Como visitante, deseo explorar la página principal de Pawfect Care para entender los servicios y características que ofrece la plataforma.**

| User Story ID | Título                                     | Descripción                                                                                                                                                      |
|---------------|-------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| TS01          | Barra de Navegación en la Landing Page     | Como visitante, deseo usar la barra de navegación para acceder fácilmente a las diferentes secciones de la plataforma.                                        |
| TS02          | Visualización de la Sección "Why Choose Us?" | Como visitante, deseo revisar la sección "Why Choose Us?" para entender los beneficios y servicios de la plataforma.                                     |
| TS03          | Envío de Mensajes de Contacto             | Como visitante, deseo enviar un mensaje de contacto a través de la landing page para comunicarme con el equipo de Pawfect Care.                             |
| TS04          | Visualización de Videos en la Sección de Características | Como visitante, deseo ver los videos informativos sobre los productos y servicios para conocer más sobre Pawfect Care.                                    |

---

# Funcionalidades de Idioma en la App Web
**EP09: Como usuario, deseo cambiar el idioma de la plataforma para navegar entre las versiones en inglés y español de la app web.**

| User Story ID | Título                     | Descripción                                                                                                                                                    |
|---------------|----------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| TS05         | Cambio de Idioma en la App Web | Como usuario, deseo cambiar el idioma de la app web para poder utilizarla en inglés o español según mi preferencia.                                        |

<br><br>

# Historias de Usuario y Criterios de Aceptación

## US01: Registro de Usuario
**Relacionado con (Epic ID):** EP01

**Descripción:**  
Como administrador, deseo gestionar los usuarios para asegurar que solo personas autorizadas tengan acceso al sistema.

### Criterios de Aceptación:
- **Escenario 1:** El dueño de mascota necesita registrarse en el sistema  
  - **Dado que** el dueño de mascota está en la página de registro,  
  - **Cuando** el dueño de mascota completa todos los campos requeridos (nombre completo, teléfono, correo electrónico, dirección y contraseña),  
  - **Entonces** el sistema debe permitir al usuario crear una cuenta y mostrar un mensaje de confirmación.

  - **Escenario 2:** El veterinario necesita registrarse en el sistema  
  - **Dado que** el veterinario está en la página de registro,  
  - **Cuando** el veterinario completa todos los campos requeridos (nombre completo, teléfono, correo electrónico, especialidad y contraseña),  
  - **Entonces** el sistema debe permitir al usuario crear una cuenta y mostrar un mensaje de confirmación.

- **Escenario 3:** El usuario ingresa un correo electrónico ya registrado  
  - **Dado que** el usuario intenta registrarse con un correo electrónico ya asociado a una cuenta,  
  - **Cuando** el usuario ingresa el correo duplicado y envía el formulario,  
  - **Entonces** el sistema debe mostrar un mensaje de error indicando que el correo ya está registrado.

- **Escenario 4:** El usuario deja campos obligatorios sin llenar  
  - **Dado que** el usuario intenta registrarse sin completar todos los campos obligatorios,  
  - **Cuando** el usuario presiona el botón de registro sin llenar todos los campos,  
  - **Entonces** el sistema debe mostrar un mensaje de error solicitando que se completen todos los campos requeridos.

---

## US02: Autenticación de Usuarios
**Relacionado con (Epic ID):** EP01

**Descripción:**
Como usuario registrado, deseo poder iniciar sesión, ingresando mi correo electrónico y contraseña para poder utilizar los servicios de la aplicación.

### Criterios de Aceptación:

- **Escenario 1: Inicio de sesión exitoso**  
  - **Dado que** el usuario está registrado en el sistema  
  - **Y** se encuentra en la pantalla de inicio de sesión  
  - **Cuando** ingresa un correo electrónico y una contraseña válidos  
  - **Y** hace clic en el botón "Iniciar sesión"  
  - **Entonces** el sistema debe autenticar al usuario  
  - **Y** redirigirlo al panel principal de la aplicación  

- **Escenario 2: Credenciales inválidas**  
  - **Dado que** el usuario está en la pantalla de inicio de sesión  
  - **Cuando** ingresa un correo electrónico o una contraseña incorrectos  
  - **Y** hace clic en el botón "Iniciar sesión"  
  - **Entonces** el sistema debe mostrar un mensaje de error indicando que las credenciales son inválidas  
  - **Y** permanecer en la misma pantalla  

- **Escenario 3: Campos vacíos**  
  - **Dado que** el usuario está en la pantalla de inicio de sesión  
  - **Cuando** deja el campo de correo electrónico o contraseña vacío  
  - **Y** hace clic en el botón "Iniciar sesión"  
  - **Entonces** el sistema debe mostrar un mensaje de validación indicando que los campos son obligatorios


## US03: Gestión de Cuentas de Usuarios
**Relacionado con (Epic ID):** EP01

**Descripción:**  
Como usuario registrado, deseo poder iniciar sesión, ingresando mi correo electrónico y contraseña para poder utilizar los servicios de la aplicación.

### Criterios de Aceptación:
- **Escenario 1:** El administrador edita el perfil de un usuario  
  - **Dado que** el administrador está en la sección de gestión de usuarios,  
  - **Cuando** selecciona el perfil de un usuario y edita su información (nombre, correo, teléfono, dirección),  
  - **Entonces** el sistema debe permitir que el administrador guarde los cambios y mostrar un mensaje de confirmación.

- **Escenario 2:** El administrador desactiva una cuenta de usuario  
  - **Dado que** el administrador desea desactivar la cuenta de un usuario,  
  - **Cuando** selecciona la opción de desactivar en la lista de usuarios,  
  - **Entonces** el sistema debe cambiar el estado del usuario a "inactivo" y el usuario no podrá acceder al sistema hasta ser reactivado.

- **Escenario 3:** El administrador elimina un cuenta de usuario  
  - **Dado que** el administrador está gestionando cuentas de usuarios,  
  - **Cuando** selecciona la opción de eliminar el perfil de un usuario,  
  - **Entonces** el sistema debe eliminar permanentemente el perfil y todos sus datos asociados, mostrando una advertencia antes de la eliminación.

---

## US04: Creación de Perfil de Mascota
**Relacionado con (Epic ID):** EP02

**Descripción:**  
Como usuario, deseo crear un perfil de mi mascota para tener su información almacenada en la plataforma.

### Criterios de Aceptación:
- **Escenario 1:** El usuario crea un perfil para su mascota  
  - **Dado que** el usuario está en la página de creación de perfil de mascota,  
  - **Cuando** ingresa toda la información requerida (nombre de la mascota, fecha de nacimiento, raza, género, historial clínico),  
  - **Entonces** el sistema debe permitir la creación del perfil y mostrar un mensaje de confirmación de éxito.

- **Escenario 2:** El usuario deja campos obligatorios sin llenar  
  - **Dado que** el usuario está intentando crear el perfil de una mascota,  
  - **Cuando** deja uno o más campos obligatorios vacíos,  
  - **Entonces** el sistema debe mostrar un mensaje de error indicando que debe completar todos los campos requeridos antes de crear el perfil.

- **Escenario 3:** El usuario introduce un nombre de mascota duplicado  
  - **Dado que** el usuario está creando un perfil de mascota,  
  - **Cuando** ingresa un nombre de mascota que ya existe en su cuenta,  
  - **Entonces** el sistema debe mostrar una advertencia solicitando al usuario que elija un nombre único o que diferencie entre mascotas con nombres similares.

---

## US05: Edición de Perfil de Mascota
**Relacionado con (Epic ID):** EP02

**Descripción:**  
Como usuario, deseo editar el perfil de mi mascota para actualizar su información cuando sea necesario.

### Criterios de Aceptación:
- **Escenario 1:** El usuario edita el perfil de su mascota  
  - **Dado que** el usuario está en la página de edición del perfil de su mascota,  
  - **Cuando** realiza cambios en la información del perfil (por ejemplo, actualiza el historial clínico o cambia la raza),  
  - **Entonces** el sistema debe permitir guardar los cambios y mostrar un mensaje de confirmación de éxito.

- **Escenario 2:** El usuario intenta guardar un perfil con información incompleta  
  - **Dado que** el usuario está editando el perfil de una mascota,  
  - **Cuando** intenta guardar el perfil sin haber completado todos los campos requeridos,  
  - **Entonces** el sistema debe mostrar un mensaje de error solicitando que complete toda la información requerida.

---

## US06: Visualización de Perfiles de Mascotas  
**Relacionado con (Epic ID):** EP02

**Descripción:**  
Como usuario, deseo visualizar los perfiles de mis mascotas para revisar la información registrada.

### Criterios de Aceptación:
- **Escenario 1:** El usuario accede a la lista de sus mascotas  
  - **Dado que** el usuario ha iniciado sesión,  
  - **Cuando** accede a la sección de “Mis Mascotas”,  
  - **Entonces** el sistema debe mostrar una lista con los perfiles de sus mascotas registradas.

- **Escenario 2:** El usuario visualiza los detalles de una mascota  
  - **Dado que** el usuario está en la lista de mascotas,  
  - **Cuando** selecciona una mascota,  
  - **Entonces** el sistema debe mostrar toda la información registrada sobre esa mascota (nombre, raza, historial clínico, etc.).

---

## US07: Búsqueda de Mascotas por el nombre del dueño y de la mascota  
**Relacionado con (Epic ID):** EP02

**Descripción:**  
Como médico veterinario, deseo buscar mascotas por el nombre del dueño y de la mascota para acceder rápidamente a su información en el sistema.

### Criterios de Aceptación:

- **Escenario 1: El médico veterinario busca una mascota por nombre del dueño y nombre de la mascota válidos**  
  - **Dado que** el médico veterinario está en la sección de gestión de mascotas  
  - **Cuando** ingresa el nombre del dueño y el nombre de la mascota en el campo de búsqueda  
  - **Entonces** el sistema debe mostrar el perfil correspondiente a la combinación de esos datos

- **Escenario 2: El médico veterinario ingresa un nombre de dueño o mascota inexistente**  
  - **Dado que** el médico veterinario intenta buscar una mascota  
  - **Cuando** ingresa un nombre de dueño y/o nombre de mascota que no están registrados  
  - **Entonces** el sistema debe mostrar un mensaje indicando que no se encontró ninguna mascota con esos datos

- **Escenario 3: El médico veterinario deja uno o ambos campos vacíos**  
  - **Dado que** el médico veterinario se encuentra en la sección de búsqueda de mascotas  
  - **Cuando** deja el campo del nombre del dueño, el nombre de la mascota, o ambos vacíos  
  - **Entonces** el sistema debe mostrar un mensaje de validación indicando que ambos campos son obligatorios para realizar la búsqueda

---

## US08: Gestión de Perfiles de Mascotas  
**Relacionado con (Epic ID):** EP02

**Descripción:**  
Como dueño de mascota, deseo gestionar y poder eliminar los perfiles de mis mascotas (de ser necesario) para asegurarme de que la información esté correctamente registrada y actualizada.

### Criterios de Aceptación:
- **Escenario 1:** El dueño edita un perfil de mascota  
  - **Dado que** el dueño está gestionando perfiles de mascotas,  
  - **Cuando** selecciona un perfil y actualiza la información,  
  - **Entonces** el sistema debe permitir guardar los cambios y mostrar una confirmación de éxito.

- **Escenario 2:** El dueño elimina un perfil de mascota  
  - **Dado que** el dueño está en la lista de mascotas,  
  - **Cuando** selecciona la opción de eliminar en un perfil,  
  - **Entonces** el sistema debe solicitar confirmación y, al aceptarse, eliminar permanentemente el perfil y sus datos.

- **Escenario 3:** El dueño visualiza el historial de cambios en un perfil  
  - **Dado que** el dueño desea verificar cambios anteriores,  
  - **Cuando** accede a un perfil de mascota,  
  - **Entonces** el sistema debe mostrar un historial con las modificaciones realizadas al perfil.

---

## US09: Agendamiento de Citas  
**Relacionado con (Epic ID):** EP03

**Descripción:**  
Como dueño, quiero agendar citas para que mi mascota reciba atención veterinaria a tiempo.

### Criterios de Aceptación:
- **Escenario 1:** El dueño necesita agendar una cita  
  - **Dado que** el dueño necesita una consulta veterinaria,  
  - **Cuando** acceda a la opción de "Agendar Cita" y seleccione la fecha, hora y tipo de servicio,  
  - **Entonces** la cita será agendada correctamente y recibirá una confirmación.

---

## US10: Cancelación de Citas  
**Relacionado con (Epic ID):** EP03

**Descripción:**  
Como dueño de mascota, quiero cancelar citas agendadas en caso de que no pueda asistir.

### Criterios de Aceptación:
- **Escenario 1:** El dueño de mascota necesita cancelar una cita previamente agendada  
  - **Dado que** el dueño de mascota ha reservado una cita,  
  - **Cuando** haga clic en "Cancelar Cita" en su historial de citas,  
  - **Entonces** la cita será eliminada y se enviará una notificación de cancelación.

---

## US11: Búsqueda de Citas por fecha 
**Relacionado con (Epic ID):** EP03

**Descripción:**  
Como dueño de mascota o médico veterinario, deseo poder buscar citas por fecha para acceder rápidamente a la información de la cita.

### Criterios de Aceptación:

- **Escenario 1: El usuario busca citas por una fecha válida**  
  - **Dado que** el usuario (dueño o veterinario) está en la sección de citas  
  - **Cuando** ingresa una fecha válida en el campo de búsqueda  
  - **Entonces** el sistema debe mostrar todas las citas correspondientes a esa fecha

- **Escenario 2: El usuario ingresa una fecha sin citas registradas**  
  - **Dado que** el usuario desea buscar citas por fecha  
  - **Cuando** ingresa una fecha para la cual no hay citas registradas en el sistema  
  - **Entonces** el sistema debe mostrar un mensaje indicando que no se encontraron citas para esa fecha

- **Escenario 3: El usuario deja el campo de fecha vacío o con un formato incorrecto**  
  - **Dado que** el usuario está en la sección de búsqueda de citas  
  - **Cuando** deja el campo vacío o introduce una fecha con un formato inválido  
  - **Entonces** el sistema debe mostrar un mensaje de validación indicando que debe ingresar una fecha válida

---

## US12: Edición de Citas Veterinarias
**Relacionado con (Epic ID):** EP03

**Descripción:**  
Como médico veterinario, deseo editar las citas para hacer cambios en la fecha o estado cuando sea necesario.

### Criterios de Aceptación:
- **Escenario 1:** El médico veterinario edita la fecha de una cita  
  - **Dado que** el médico veterinario está en la página de gestión de citas,  
  - **Cuando** selecciona una cita y cambia su fecha u hora,  
  - **Entonces** el sistema debe actualizar la cita y enviar una notificación al usuario afectado indicando el cambio.

---

## US13: Búsqueda de dueño de mascota  
**Relacionado con (Epic ID):** EP03

**Descripción:**  
Como  médico veterinario, deseo poder buscar citas de clientes agendados por su nombre y DNI para poder ubicarlos rápidamente.

### Criterios de Aceptación:

- **Escenario 1: Búsqueda por nombre y DNI válidos**  
  - **Dado que** el médico veterinario está en la sección de búsqueda de citas  
  - **Cuando** ingresa el nombre completo y el DNI de un cliente que tiene citas registradas  
  - **Entonces** el sistema debe mostrar todas las citas asociadas a ese cliente

- **Escenario 2: Búsqueda sin resultados**  
  - **Dado que** el médico veterinario desea buscar citas por nombre y DNI  
  - **Cuando** ingresa un nombre y/o DNI que no corresponde a ningún cliente con citas registradas  
  - **Entonces** el sistema debe mostrar un mensaje indicando que no se encontraron citas para ese cliente

- **Escenario 3: Campos incompletos o inválidos**  
  - **Dado que** el médico veterinario intenta realizar una búsqueda  
  - **Cuando** deja uno de los campos vacío o introduce un formato inválido en el campo del DNI  
  - **Entonces** el sistema debe mostrar un mensaje de validación solicitando que complete correctamente los campos

---

## US14: Consulta sobre alimentación adecuada  
**Relacionado con (Epic ID):** EP04

**Descripción:**  
Como dueño, deseo consultar al asistente artificial (chatbot) sobre qué tipo de comida es ideal para mi mascota según su especie, edad y tamaño.

### Criterios de Aceptación:

- **Escenario 1:** Consulta exitosa de alimentación adecuada
  - **Dado que** soy un dueño que accede al chatbot del sistema
  - **Y** proporciono la especie, edad y tamaño de mi mascota
  - **Cuando** solicito una recomendación de alimentación adecuada
  - **Entonces** el chatbot debe responder con una sugerencia de comida específica
  - **Y** debe explicar por qué es adecuada para la especie, edad y tamaño de la mascota
  - **Y** debe incluir recomendaciones generales sobre cantidad y frecuencia de alimentación

- **Escenario 2:** Información incompleta proporcionada
  - **Dado que** soy un dueño que accede al chatbot del sistema
  - **Y** no proporciono todos los datos requeridos 
  - **Cuando** solicito una recomendación de alimentación
  - **Entonces** el chatbot debe pedirme que complete la información faltante

- **Escenario 3:** Especie de mascota no soportada
  - **Dado que** ingreso una especie de mascota poco común o no registrada en el sistema
  - **Cuando** solicito recomendaciones de alimentación
  - **Entonces** el chatbot debe indicar que no tiene información disponible para esa especie
  - **Y** debe sugerirme consultar con un veterinario

- **Escenario 4:** Recomendación personalizada según condiciones especiales
  - **Dado que** mi mascota tiene condiciones especiales de salud conocidas 
  - **Cuando** incluyo esta información en la consulta
  - **Entonces** el chatbot debe adaptar la recomendación de alimentación teniendo en cuenta dichas condiciones
  - **Y** debe advertir que se consulte con un especialista si es necesario

- **Escenario 5:** Consulta repetida para diferentes mascotas
  - **Dado que** tengo más de una mascota
  - **Cuando** realizo varias consultas sobre alimentación para distintas mascotas
  - **Entonces** el chatbot debe permitir gestionar múltiples consultas de forma continua y sin reiniciar la conversación


## US15: Consejos de higiene para mascotas  
**Relacionado con (Epic ID):** EP04

**Descripción:**  
Como dueño, deseo recibir recomendaciones básicas de higiene para mantener saludable a mi mascota mediante el asistente artificial (chatbot).

### Criterios de Aceptación:

- **Escenario 1:** Consulta exitosa de consejos de higiene
  - **Dado que** soy un dueño que accede al chatbot del sistema
  - **Y** proporciono la especie de mi mascota
  - **Cuando** solicito recomendaciones de higiene
  - **Entonces** el chatbot debe responder con consejos básicos de higiene específicos para esa especie
  - **Y** debe explicar por qué son importantes para la salud de la mascota

- **Escenario 2:** Información incompleta
  - **Dado que** soy un dueño que accede al chatbot
  - **Y** no proporciono la especie de la mascota
  - **Cuando** solicito consejos de higiene
  - **Entonces** el chatbot debe pedirme que proporcione la especie para ofrecer recomendaciones adecuadas

- **Escenario 3:** Especie no registrada
  - **Dado que** ingreso una especie no común o no registrada en el sistema
  - **Cuando** pido consejos de higiene
  - **Entonces** el chatbot debe informar que no tiene recomendaciones específicas para esa especie
  - **Y** debe sugerirme consultar con un veterinario

- **Escenario 4:** Consejos personalizados según edad o condición
  - **Dado que** mi mascota es muy joven, anciana o tiene una condición especial de salud
  - **Cuando** incluyo esta información en la consulta
  - **Entonces** el chatbot debe adaptar los consejos de higiene a las necesidades especiales de la mascota

- **Escenario 5:** Solicitud de consejos para múltiples mascotas
  - **Dado que** soy dueño de varias mascotas de diferentes especies
  - **Cuando** realizo múltiples consultas de higiene en una misma sesión
  - **Entonces** el chatbot debe responder adecuadamente sin necesidad de reiniciar la conversación

---

## US16: Preguntas frecuentes sobre salud  
**Relacionado con (Epic ID):** EP04

**Descripción:**  
Como dueño de mascota, deseo obtener respuestas rápidas sobre síntomas comunes y saber cuándo debo acudir al veterinario.

### Criterios de Aceptación:

- **Escenario 1:** Consulta exitosa sobre síntoma común
  - **Dado que** soy un dueño preocupado por un síntoma en mi mascota
  - **Y** accedo al chatbot del sistema
  - **Cuando** describo un síntoma común (como vómitos, diarrea, letargo, pérdida de apetito, etc.)
  - **Entonces** el chatbot debe brindarme una respuesta rápida explicando posibles causas
  - **Y** debe indicarme si es necesario acudir al veterinario de inmediato o monitorear en casa

- **Escenario 2:** Síntoma no reconocido
  - **Dado que** proporciono un síntoma poco común o ambiguo
  - **Cuando** realizo la consulta al chatbot
  - **Entonces** el chatbot debe indicar que no puede brindar una respuesta precisa
  - **Y** debe recomendarme acudir a un veterinario para una evaluación profesional

- **Escenario 3:** Solicitud de lista de síntomas frecuentes
  - **Dado que** quiero estar preparado ante problemas de salud comunes
  - **Cuando** solicito al chatbot información general sobre síntomas frecuentes
  - **Entonces** el chatbot debe mostrarme una lista de los síntomas más comunes por especie
  - **Y** debe explicar brevemente qué hacer en cada caso

- **Escenario 4:** Consulta sobre cuándo acudir al veterinario
  - **Dado que** no sé cuándo un síntoma es realmente grave
  - **Cuando** le pregunto al chatbot si debo llevar a mi mascota al veterinario
  - **Entonces** el chatbot debe brindar criterios generales de urgencia
  - **Y** debe recomendar acudir a un especialista si el síntoma persiste o empeora

- **Escenario 5:** Consulta para distintas especies
  - **Dado que** tengo varias mascotas de diferentes especies
  - **Cuando** hago preguntas sobre síntomas en cada una
  - **Entonces** el chatbot debe identificar la especie y dar respuestas apropiadas para cada caso

---

## US17: Consejos de entrenamiento básico  
**Relacionado con (Epic ID):** EP04

**Descripción:**  
Como dueño de mascota, deseo consultar sobre técnicas de adiestramiento o corrección de comportamientos no deseados.

### Criterios de Aceptación:

- **Escenario 1:** Consulta exitosa sobre entrenamiento básico
  - **Dado que** soy un dueño que desea entrenar a su mascota
  - **Y** accedo al chatbot del sistema
  - **Cuando** solicito consejos sobre técnicas de adiestramiento
  - **Entonces** el chatbot debe proporcionarme recomendaciones básicas específicas según la especie y edad de la mascota
  - **Y** debe incluir ejemplos de comandos comunes o técnicas positivas de refuerzo

- **Escenario 2:** Corrección de comportamiento no deseado
  - **Dado que** mi mascota presenta un comportamiento no deseado (como morder, ladrar mucho, hacer sus necesidades en lugares inadecuados)
  - **Cuando** describo este comportamiento al chatbot
  - **Entonces** el chatbot debe brindarme consejos prácticos para corregir dicha conducta
  - **Y** debe explicar cómo aplicar la técnica y cuánto tiempo podría tomar ver resultados

- **Escenario 3:** Información insuficiente proporcionada
  - **Dado que** realizo una consulta de entrenamiento sin indicar la especie o edad de la mascota
  - **Cuando** envío mi mensaje al chatbot
  - **Entonces** el chatbot debe pedirme que complete esa información antes de brindar recomendaciones

- **Escenario 4:** Técnicas según etapa de vida
  - **Dado que** mi mascota es un cachorro, adulto o anciano
  - **Cuando** solicito orientación sobre entrenamiento
  - **Entonces** el chatbot debe adaptar los consejos a la etapa de vida correspondiente

- **Escenario 5:** Consulta para distintas mascotas
  - **Dado que** tengo más de una mascota con comportamientos distintos
  - **Cuando** hago múltiples preguntas en una misma sesión
  - **Entonces** el chatbot debe gestionar cada caso por separado
  - **Y** brindar respuestas adecuadas a cada especie, comportamiento y situación


---

## US18: Recomendaciones según tipo de mascota  
**Relacionado con (Epic ID):** EP04

**Descripción:**  
Como dueño, deseo que el chatbot me dé consejos generales adaptados al tipo de mascota que tengo (perro, gato, ave, etc).

### Criterios de Aceptación:

- **Escenario 1:** Recomendaciones generales exitosas según tipo de mascota
  - **Dado que** soy un dueño que accede al chatbot del sistema
  - **Y** proporciono el tipo de mascota que tengo (por ejemplo, perro, gato, ave)
  - **Cuando** solicito consejos generales para el cuidado de mi mascota
  - **Entonces** el chatbot debe responder con recomendaciones adaptadas a ese tipo de mascota
  - **Y** debe cubrir aspectos como alimentación, higiene, salud y actividad física

- **Escenario 2:** Tipo de mascota no registrado
  - **Dado que** ingreso un tipo de mascota que no está en la base de datos del sistema
  - **Cuando** pido recomendaciones
  - **Entonces** el chatbot debe informarme que no tiene información disponible para ese tipo de mascota
  - **Y** debe sugerirme consultar a un veterinario u otro especialista


---

## US19: Visualización del Historial Médico  
**Relacionado con (Epic ID):** EP05

**Descripción:**  
Como dueño, deseo visualizar el historial médico de mi mascota para revisar su estado de salud y tratamientos previos.

### Criterios de Aceptación:

- **Escenario 1:** Visualización exitosa del historial médico
  - **Dado que** soy un dueño autenticado en el sistema
  - **Y** tengo registrada a mi mascota
  - **Cuando** accedo a la opción de historial médico
  - **Entonces** el sistema debe mostrar una lista organizada con las visitas veterinarias, diagnósticos, tratamientos y vacunas aplicadas

- **Escenario 2:** Mascota sin historial registrado
  - **Dado que** soy un dueño autenticado
  - **Y** la mascota aún no tiene historial médico cargado
  - **Cuando** intento visualizar el historial
  - **Entonces** el sistema debe mostrar un mensaje indicando que aún no hay datos disponibles
  - **Y** debe sugerir registrar la primera visita médica

- **Escenario 3:** Acceso sin autenticación
  - **Dado que** intento acceder al historial médico sin iniciar sesión
  - **Cuando** ingreso a la sección de historial
  - **Entonces** el sistema debe redirigirme a la pantalla de autenticación o mostrar un mensaje de acceso restringido

---

## US20: Creación del Historial Médico  
**Relacionado con (Epic ID):** EP05

**Descripción:**  
Como doctor veterinario, deseo crear el historial médico de las mascotas para que los dueños tengan la información de sus mascotas en el sistema.

### Criterios de Aceptación:

- **Escenario 1:** Creación exitosa del historial médico
  - **Dado que** ccedo al perfil de una mascota que no tiene historial médico registrado
  - **Y** tengo acceso al perfil de una mascota registrada
  - **Cuando** ingreso los datos iniciales del historial
  - **Entonces** el sistema debe crear un nuevo historial médico para la mascota
  - **Y** mostrar un mensaje de confirmación

- **Escenario 2:** Intento de registro sin autenticación
  - **Dado que** no he iniciado sesión como veterinario
  - **Cuando** intento acceder a la función para registrar el historial médico de una mascota
  - **Entonces** el sistema debe denegar el acceso
  - **Y** debe mostrar un mensaje indicando que se requiere autenticación como profesional autorizado

- **Escenario 3:** Datos obligatorios incompletos o inválidos
  - **Dado que** soy un veterinario autenticado
  - **Cuando** intento crear un historial médico sin completar campos obligatorios
  - **Entonces** el sistema debe mostrar un mensaje de error
  - **Y** no debe permitir guardar el historial hasta que los datos requeridos sean completados correctamente

---

## US21: Actualización del Historial Médico  
**Relacionado con (Epic ID):** EP05

**Descripción:**  
Como doctor veterinario, deseo actualizar el historial médico de las mascotas para que los dueños tengan la información más reciente sobre sus tratamientos.

### Criterios de Aceptación:

- **Escenario 1:** Actualización exitosa del historial médico
  - **Dado que** soy un doctor veterinario autenticado en el sistema
  - **Y** tengo acceso al perfil de una mascota registrada
  - **Cuando** ingreso nuevos datos médicos (como diagnóstico, tratamiento o vacuna)
  - **Entonces** el sistema debe guardar correctamente la información en el historial médico de la mascota
  - **Y** debe estar disponible para ser consultada por el dueño

- **Escenario 2:** Intento de actualización sin autenticación
  - **Dado que** no he iniciado sesión como veterinario
  - **Cuando** intento acceder o modificar el historial médico de una mascota
  - **Entonces** el sistema debe denegar el acceso
  - **Y** debe mostrar un mensaje indicando que se requiere autenticación como profesional autorizado

- **Escenario 3:** Ingreso de datos incompletos o inválidos
  - **Dado que** soy un veterinario autenticado
  - **Cuando** intento registrar un historial sin llenar campos obligatorios (como fecha o diagnóstico)
  - **Entonces** el sistema debe mostrar un mensaje de error
  - **Y** no debe guardar la información hasta que todos los campos requeridos sean completados

---

## US22: Publicar Reseñas  
**Relacionado con (Epic ID):** EP06

**Descripción:**  
Como usuario dueño de una mascota, deseo dejar una reseña sobre un doctor veterinario para compartir mi experiencia con otros usuarios.

### Criterios de Aceptación:

- **Escenario 1:** Publicación exitosa de una reseña
  - **Dado que** soy un usuario autenticado en el sistema
  - **Y** he tenido una consulta con un doctor veterinario registrado
  - **Cuando** accedo a la sección de reseñas y escribo mi opinión junto con una calificación
  - **Entonces** el sistema debe guardar y mostrar la reseña públicamente en el perfil del doctor

- **Escenario 2:** Intento de publicación sin autenticación
  - **Dado que** no he iniciado sesión
  - **Cuando** intento dejar una reseña sobre un doctor veterinario
  - **Entonces** el sistema debe redirigirme a la pantalla de inicio de sesión
  - **Y** mostrar un mensaje indicando que solo usuarios autenticados pueden dejar reseñas

- **Escenario 3:** Ingreso de reseña incompleta
  - **Dado que** estoy autenticado
  - **Cuando** intento publicar una reseña sin completar campos obligatorios (como texto o calificación)
  - **Entonces** el sistema debe notificarme qué campos faltan
  - **Y** no debe permitir publicar la reseña hasta que esté completa

---

## US23: Visualización de Reseñas  
**Relacionado con (Epic ID):** EP06

**Descripción:**  
Como dueño de una mascota, deseo ver las reseñas de otros usuarios sobre un doctor veterinario para conocer la calidad del servicio y su calificación general.

### Criterios de Aceptación:

- **Escenario 1:** Visualización exitosa de reseñas
  - **Dado que** soy un usuario autenticado en el sistema
  - **Y** busco un doctor veterinario específico
  - **Cuando** accedo a su perfil
  - **Entonces** el sistema debe mostrar todas las reseñas publicadas por otros usuarios
  - **Y** debe incluir la calificación promedio y las reseñas individuales con texto y puntuación

- **Escenario 2:** No hay reseñas disponibles
  - **Dado que** soy un usuario autenticado
  - **Y** el doctor veterinario no tiene reseñas publicadas
  - **Cuando** accedo al perfil del doctor
  - **Entonces** el sistema debe mostrar un mensaje indicando que no hay reseñas disponibles para este doctor

- **Escenario 3:** Visualización de reseñas sin autenticación
  - **Dado que** no he iniciado sesión en el sistema
  - **Cuando** intento acceder a las reseñas de un doctor veterinario
  - **Entonces** el sistema debe permitir la visualización pública de las reseñas, si están disponibles

---

## US24: Ofrecer tarifa por servicio  
**Relacionado con (Epic ID):** EP07

**Descripción:**  
Como médico veterinario, deseo ofrecer una tarifa personalizada para un servicio solicitado por un dueño de mascota mediante una cita, para que él pueda evaluar mi propuesta.

### Criterios de Aceptación:

- **Escenario 1:** Oferta de tarifa exitosa por servicio
  - **Dado que** soy un médico veterinario autenticado en el sistema
  - **Y** un dueño de mascota ha solicitado una cita para un servicio específico
  - **Cuando** ingreso la tarifa personalizada para dicho servicio
  - **Entonces** el sistema debe guardar la tarifa y mostrarla al dueño de la mascota en su solicitud de cita

- **Escenario 2:** Modificación de tarifa para un servicio existente
  - **Dado que** soy un veterinario autenticado y ya he ofrecido una tarifa para un servicio
  - **Cuando** decido modificar la tarifa propuesta
  - **Entonces** el sistema debe permitir la modificación
  - **Y** debe notificar al dueño de la mascota sobre el cambio en la tarifa

- **Escenario 3:** Intento de ofrecer tarifa sin autenticación
  - **Dado que** no estoy autenticado como médico veterinario
  - **Cuando** intento ofrecer una tarifa por un servicio
  - **Entonces** el sistema debe redirigirme a la pantalla de inicio de sesión
  - **Y** mostrar un mensaje indicando que solo los veterinarios autenticados pueden ofrecer tarifas por servicio

---

## US25: Visualización de Reseñas y Tarifas  
**Relacionado con (Epic ID):** EP07

**Descripción:**  
Como dueño de una mascota, deseo ver las reseñas y tarifas ofrecidas por distintos veterinarios para un servicio específico solicitado en una cita, y así elegir la mejor opción.

### Criterios de Aceptación:

- **Escenario 1:** Visualización de reseñas y tarifas para un servicio específico
  - **Dado que** soy un dueño de mascota autenticado en el sistema
  - **Y** he solicitado un servicio específico de veterinario (por ejemplo, consulta, vacunación)
  - **Cuando** accedo a las opciones de veterinarios disponibles para este servicio
  - **Entonces** el sistema debe mostrar las reseñas de otros usuarios sobre cada veterinario
  - **Y** debe mostrar la tarifa personalizada ofrecida por cada veterinario para el servicio solicitado

- **Escenario 2:** No hay reseñas o tarifas disponibles
  - **Dado que** soy un dueño de mascota autenticado
  - **Y** el veterinario no tiene reseñas publicadas o no ha ofrecido una tarifa para el servicio solicitado
  - **Cuando** accedo a su perfil
  - **Entonces** el sistema debe mostrar un mensaje indicando que no hay reseñas o tarifas disponibles

- **Escenario 3:** Acceso sin autenticación
  - **Dado que** no he iniciado sesión como dueño de mascota
  - **Cuando** intento ver las reseñas y tarifas de los veterinarios
  - **Entonces** el sistema debe redirigirme a la pantalla de inicio de sesión
  - **Y** mostrar un mensaje indicando que solo los usuarios autenticados pueden acceder a esta información

---

## US26: Registro de horarios
**Relacionado con (Epic ID):** EP07

**Descripción:**  
Como médico veterinario, deseo publicar mis horarios disponibles para un servicio solicitado por un dueño de mascota mediante una cita, para que él pueda elegir.

### Criterios de Aceptación:

- **Escenario 1:** Registro exitoso de horarios disponibles
  - **Dado que** soy un médico veterinario autenticado en el sistema
  - **Cuando** ingreso horarios disponibles para atención
  - **Entonces** el sistema debe registrar correctamente los horarios
  - **Y** mostrarlos como opciones disponibles al dueño de mascota cuando solicite una cita

- **Escenario 2:** Intento de registro de horarios sin autenticación
  - **Dado que** no he iniciado sesión como veterinario
  - **Cuando** intento acceder a la funcionalidad de registrar horarios
  - **Entonces** el sistema debe denegar el acceso
  - **Y** mostrar un mensaje indicando que se requiere autenticación como profesional autorizado

- **Escenario 3:** Registro con datos incompletos o inválidos
  - **Dado que** soy un médico veterinario autenticado
  - **Cuando** intento registrar un horario sin completar campos obligatorios o ingreso un rango horario inválido
  - **Entonces** el sistema debe mostrar un mensaje de error
  - **Y** no debe guardar el horario hasta que los datos sean corregidos

## 3.3. Impact Mapping.

Este Impact Map muestra cómo Pawfect Care alinea sus objetivos de negocio con los impactos deseados. Detalla los entregables específicos y las user stories que abordan estos impactos, asegurando que cada aspecto del desarrollo de la plataforma mejore la eficiencia y la experiencia del usuario.

[![Impactmap.png](https://i.postimg.cc/4df4zmDD/Impactmap.png)](https://postimg.cc/064qv22n)

## 3.4. Product Backlog.

Con el fin de simplificar la complejidad de las tareas, hemos utilizado la escala de Fibonacci (1/2/3/5/8) para crear nuestro product backlog.
Historia de usuario base:
Tomamos como referencia US06: Como usuario, quiero agendar citas para que mi mascota reciba atención veterinaria a tiempo. (Posee 3 puntos de historia).
Asimismo, utilizamos la herramienta “Planning Poker Online” para poder votar en grupo y decidir la dificultad de cada historia de usuario, tomando como punto intermedio el User Story 06

| # Orden | User Story ID | Título                                   | Descripción                                                                                                     | Story Points |
|--------|----------------|-------------------------------------------|-----------------------------------------------------------------------------------------------------------------|--------------|
| 1      | US09           | Agendamiento de Citas                     | Como usuario, deseo agendar citas veterinarias para asegurar que mi mascota reciba atención médica en el momento adecuado. | 5            |
| 2      | US19           | Visualización del Historial Médico        | Como dueño, deseo visualizar el historial médico de mi mascota para revisar su estado de salud y tratamientos previos. | 3            |
| 3      | US20           | Actualización del Historial Médico        | Como doctor veterinario, deseo actualizar el historial médico de las mascotas para que los dueños tengan la información más reciente sobre sus tratamientos. | 3            |
| 4      | US07           | Búsqueda de Mascotas                      | Como médico veterinario, deseo buscar mascotas por su nombre para acceder rápidamente a su información en el sistema. | 2            |
| 5      | US05           | Edición de Perfil de Mascota              | Como dueño, deseo editar el perfil de mi mascota para actualizar su información cuando sea necesario.           | 2            |
| 6      | US06           | Visualización de Perfiles de Mascotas     | Como dueño, deseo visualizar los perfiles de mis mascotas para revisar la información registrada.               | 2            |
| 7      | US13           | Búsqueda de dueño de mascota                     | Como médico veterinario, deseo poder buscar citas de clientes agendados por su nombre y DNI para poder ubicarlos rápidamente. | 2            |
| 8      | US11           | Búsqueda de Citas por fecha               | Como dueño de mascota o médico veterinario, deseo poder buscar citas por fecha para acceder rápidamente a la información de la cita. | 2            |
| 9      | US12           | Edición de Citas Veterinarias             | Como médico veterinario, deseo editar las citas para hacer cambios en la fecha o estado cuando sea necesario.  | 3            |
|10      | US10           | Cancelación de Citas                      | Como usuario, deseo cancelar una cita si no puedo asistir para evitar problemas de horario y reorganizar la atención. | 2            |
|11      | US14           | Consulta sobre alimentación adecuada      | Como dueño, deseo consultar al chatbot sobre qué tipo de comida es ideal para mi mascota según su especie, edad y tamaño. | 5            |
|12      | US15           | Consejos de higiene para mascotas         | Como dueño, deseo recibir recomendaciones básicas de higiene para mantener saludable a mi mascota mediante el asistente artificial (chatbot). | 3            |
|13      | US16           | Preguntas frecuentes sobre salud          | Como dueño de mascota, deseo obtener respuestas rápidas sobre síntomas comunes y saber cuándo debo acudir al veterinario. | 3            |
|14      | US17           | Consejos de entrenamiento básico          | Como dueño de mascota, deseo consultar sobre técnicas de adiestramiento o corrección de comportamientos no deseados. | 3            |
|15      | US18           | Recomendaciones según tipo de mascota     | Como dueño, deseo que el chatbot me dé consejos generales adaptados al tipo de mascota que tengo (perro, gato, ave, etc). | 3            |
|16      | US23           | Ofrecer tarifa por servicio               | Como médico veterinario, deseo ofrecer una tarifa personalizada para un servicio solicitado por un dueño de mascota mediante una cita, para que él pueda evaluar mi propuesta. | 3            |
|17      | US24           | Visualización de Tarifas                  | Como dueño de una mascota, deseo ver las tarifas ofrecidas por distintos veterinarios para un servicio específico solicitado en una cita, y así elegir la mejor opción. | 3            |
|18      | US21           | Publicar Reseñas                          | Como usuario dueño de una mascota, deseo dejar una reseña sobre un doctor veterinario para compartir mi experiencia con otros usuarios. | 3            |
|19      | US22           | Visualización de Reseñas                  | Como dueño de una mascota, deseo ver las reseñas de otros usuarios sobre un doctor veterinario para conocer la calidad del servicio y su calificación general. | 3            |
|20      | US04           | Creación de Perfil de Mascota             | Como dueño, deseo crear un perfil de mi mascota para tener su información almacenada en la plataforma.         | 2            |
|21      | US08           | Gestión de Perfiles de Mascotas           | Como dueño de mascota, deseo gestionar y poder eliminar los perfiles de mis mascotas para asegurarme de que la información esté correctamente registrada y actualizada. | 2            |
|22      | US01           | Registro de Usuario                       | Como visitante, deseo registrarme en la plataforma para poder utilizar las funcionalidades del sistema.         | 3            |
|23      | US02           | Autenticación de Usuarios                 | Como usuario registrado, deseo poder iniciar sesión, ingresando mi correo electrónico y contraseña para poder utilizar los servicios de la aplicación. | 3            |
|24      | US03           | Gestión de Cuentas de Usuarios            | Como dueño de mascota y médico veterinario, deseo gestionar el perfil de mi cuenta para mantener la información actualizada. | 2            |

---