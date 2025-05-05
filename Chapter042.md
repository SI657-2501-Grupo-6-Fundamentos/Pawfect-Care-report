## 4.2  Architectural Drivers
### 4.2.1    Design Purpose 
Para el desarrollo de la aplicación "Pawfect Care", que conecta a las veterinarias y sus servicios con los dueños de mascotas. Se sugiere adoptar la arquitectura de microservicios, ya que favorece una estructura organizada y eficiente, simplificando la gestión, el mantenimiento y el desarrollo continuo gracias a sus componentes pequeños e independientes. Además, cada microservicio puede ser desarrollado con diferentes lenguajes y marcos de trabajo, lo que proporciona una gran flexibilidad tecnológica que se ajusta perfectamente a la naturaleza innovadora de Pawfect Care.  En un entorno en línea, es esencial que la aplicación tenga alta resistencia a fallos y capacidad para escalar según la demanda, debido a la variabilidad del tráfico. Por ejemplo, cuando se lanzan nuevas versiones o se implementan actualizaciones importantes, la aplicación debe ser capaz de gestionar el aumento en el uso sin afectar la calidad de la experiencia del usuario. Además, la arquitectura de microservicios posibilita despliegues independientes y específicos para cada servicio. Este enfoque también favorece la experimentación y la implementación rápida de nuevas funcionalidades sin afectar los servicios ya establecidos, permitiendo a "Pawfect Care" adaptarse rápidamente a las necesidades cambiantes de sus usuarios y a las tendencias del mercado.
### 4.2.2    Primary Functionality (Primary User Stories)
| USER STORY ID | TÍTULO | DESCRIPCIÓN |
|----------|----------|----------|
| US01 | Registro de Usuario | Como visitante, deseo registrarme en la plataforma para poder utilizar las funcionalidades del sistema. | 
| US02 | Autenticación de Usuarios | Como usuario registrado, deseo poder iniciar sesión, ingresando mi correo electrónico y contraseña para poder utilizar los servicios de la aplicación. |
| US03 | Gestión de Cuentas de Usuarios | Como dueño de mascota y médico veterinario, deseo gestionar el perfil de mi cuenta para mantener la información actualizada. |
| US04 | Creación de Perfil de Mascota | Como dueño, deseo crear un perfil de mi mascota para tener su información almacenada en la plataforma. |
| US05 | Edición de Perfil de Mascota | Como dueño, deseo editar el perfil de mi mascota para actualizar su información cuando sea necesario. |
| US06 | Visualización de Perfiles de Mascotas | Como dueño, deseo visualizar los perfiles de mis mascotas para revisar la información registrada.|
| US07 | Búsqueda de Mascotas | Como médico veterinario, deseo buscar mascotas por su nombre para acceder rápidamente a su información en el sistema. |
| US08 | Gestión de Perfiles de Mascotas | Como dueño de mascota, deseo gestionar y poder eliminar los perfiles de mis mascotas para asegurarme de que la información esté correctamente registrada y actualizada. |
| US09 | Agendamiento de Citas | Como usuario, deseo agendar citas veterinarias para asegurar que mi mascota reciba atención médica en el momento adecuado. |
| US10 | Cancelación de Citas | Como usuario, deseo cancelar una cita si no puedo asistir para evitar problemas de horario y reorganizar la atención. |
| US11 | Búsqueda de Citas por fecha | Como dueño de mascota o médico veterinario, deseo poder buscar citas por fecha para acceder rápidamente a la información de la cita. |
| US12 | Edición de Citas Veterinarias | Como médico veterinario, deseo editar las citas para hacer cambios en la fecha o estado cuando sea necesario. |
| US13 | Búsqueda de dueño de mascota | Como médico veterinario, deseo poder buscar citas de clientes agendados por su nombre y DNI para poder ubicarlos rápidamente. |
| US19 | Visualización del Historial Médico | Como dueño, deseo visualizar el historial médico de mi mascota para revisar su estado de salud y tratamientos previos. |
| US20 | Actualización del Historial Médico | Como doctor veterinario, deseo actualizar el historial médico de las mascotas para que los dueños tengan la información más reciente sobre sus tratamientos. |

### 4.2.3 Quality Attribute Scenarios
| ID | ATRIBUTO DE CALIDAD | ESCENARIO | HISTORIA DE USUARIO USADA |
|----|---------------------|-----------|---------------------------|
| QA01 | Rendimiento | Cuando un veterinario agenda una cita, el sistema debe mostrar la confirmación y los horarios disponibles en menos de 1 segundo. | US09 (Agendamiento de Citas) |
| QA02 | Seguridad | Al iniciar sesión, la aplicación debe validar credenciales. | US02 (Autenticación de Usuarios) |
| QA03 | Disponibilidad | Durante el horario de atención, la plataforma debe estar disponible al menos 99.9% del tiempo para consultar historiales. | US19 (Visualización del Historial Médico) |
| QA04 | Usabilidad | Un veterinario o dueño debe poder buscar y acceder al perfil de una mascota en máximo 3 clics. | US07 (Búsqueda de Mascotas) |
| QA05 | Escalabilidad | El sistema debe soportar hasta 1 000 usuarios concurrentes (veterinarios y dueños) sin degradar tiempos de respuesta. | US19 (Visualización del Historial Médico) - US20 (Actualización del Historial Médico) |
### 4.2.4  Constraints
| ID | CONSTRAINTS | DESCRIPCIÓN |
|----|-------------|-------------|
| CONS01 | Tecnológico – Front-end | La UI debe implementarse con Angular y TypeScript, siguiendo las buenas prácticas de modularidad, lazy-loading y responsive design. |
| CONS02 | Tecnológico – Base de datos | Debe usarse MySQL para almacenar toda la información clínica, citas y perfiles, garantizando compatibilidad con los sistemas internos. |
| CONS03 | Regulatorio – Protección de datos | Debe cumplir con la Ley N° 29733 de Protección de Datos Personales de Perú y sus modificatorias, así como permitir solicitudes de eliminación (“derecho al olvido”). |
| CONS04 | Operacional – Conectividad | Debe funcionar correctamente con conexiones de hasta 3G y degradarse de forma manejable (sin pérdida de datos) en casos de latencia alta. |
### 4.2.5  Architectural Concerns
| ID | ARQUITECTURAL CONCERNS |
|----|------------------------|
| ARC01 |  Los datos personales de los usuarios podrían estar expuestos a riesgos si no se implementan adecuadamente medidas de seguridad robustas. |
| ARC02 | Utilizar lo aprendido en tecnologías en proyectos previos como Java Spring Boot, Angular, MySQL y Github |
| ARC03 | Asignar responsabilidades cada integrante según su mejor especialidad para un mejor desempeño. |
| ARC04 | Lograr un rendimiento óptimo en términos de tiempos de respuesta y eficiencia del procesamiento podría ser difícil, particularmente bajo cargas de trabajo elevadas. |
| ARC05 | Integrar microservicios de manera que se mantenga la cohesión y se facilite el mantenimiento podría ser un desafío, especialmente si se busca mantener una alta modularidad y flexibilidad en la arquitectura. |