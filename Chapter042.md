## 4.2  Architectural Drivers
### 4.2.1    Design Purpose 
Para el desarrollo de la aplicación "Pawfect Care", que conecta a las veterinarias y sus servicios con los dueños de mascotas. Se sugiere adoptar la arquitectura de microservicios, ya que favorece una estructura organizada y eficiente, simplificando la gestión, el mantenimiento y el desarrollo continuo gracias a sus componentes pequeños e independientes. Además, cada microservicio puede ser desarrollado con diferentes lenguajes y marcos de trabajo, lo que proporciona una gran flexibilidad tecnológica que se ajusta perfectamente a la naturaleza innovadora de Pawfect Care.  En un entorno en línea, es esencial que la aplicación tenga alta resistencia a fallos y capacidad para escalar según la demanda, debido a la variabilidad del tráfico. Por ejemplo, cuando se lanzan nuevas versiones o se implementan actualizaciones importantes, la aplicación debe ser capaz de gestionar el aumento en el uso sin afectar la calidad de la experiencia del usuario. Además, la arquitectura de microservicios posibilita despliegues independientes y específicos para cada servicio. Este enfoque también favorece la experimentación y la implementación rápida de nuevas funcionalidades sin afectar los servicios ya establecidos, permitiendo a "Pawfect Care" adaptarse rápidamente a las necesidades cambiantes de sus usuarios y a las tendencias del mercado.
### 4.2.2    Primary Functionality (Primary User Stories)
| User Story Id | Título | Descripción |
|----------|----------|----------|
| US09 | Agendamiento de Citas | Como usuario, deseo agendar citas veterinarias para asegurar que mi mascota reciba atención médica en el momento adecuado.
| US19 | Visualización del Historial Médico | Como dueño, deseo visualizar el historial médico de mi mascota para revisar su estado de salud y tratamientos previos. |
| US20 | Actualización del Historial Médico | Como doctor veterinario, deseo actualizar el historial médico de las mascotas para que los dueños tengan la información más reciente sobre sus tratamientos. |
| US07  | Búsqueda de Mascotas | Como médico veterinario, deseo buscar mascotas por su nombre para acceder rápidamente a su información en el sistema. |
| | | 
| | | 

### 4.2.3 Quality Attribute Scenarios
### 4.2.4  Constraints
//MySQL, Angular, Spring Boot
### 4.2.5  Architectural Concerns
