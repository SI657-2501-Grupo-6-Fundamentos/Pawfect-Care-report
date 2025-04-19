# Capítulo III: Requirements Specification## 

## 3.1. To-Be Scenario Mapping.

- **Primer segmento: Médicos Veterinarios**

<br><img src="./assets/Chapter03/Tobe1.jpeg" alt="To Be Scenario Map 1" style="width: 1000px; height: auto;" ><br>

- **Segundo segmento: Dueños de Mascotas**

<br><img src="./assets/Chapter03/Tobe2.jpeg" alt="To Be Scenario Map 2" style="width: 1000px; height: auto;" ><br>


## 3.1.1. Requisitos Funcionales

### Gestión de Usuarios y Clientes
- **RF01.** El sistema debe permitir a los usuarios registrarse en la plataforma.
- **RF02.** El sistema debe permitir a los usuarios crear y editar su perfil.
- **RF03.** El administrador debe poder gestionar y editar los perfiles de los clientes.
- **RF04.** El administrador debe poder buscar clientes por su ID.

### Gestión de Mascotas
- **RF05.** El sistema debe permitir a los usuarios crear perfiles de sus mascotas.
- **RF06.** El sistema debe permitir a los usuarios editar la información de sus mascotas.
- **RF07.** El sistema debe permitir consultar los perfiles de mascotas.
- **RF08.** El administrador debe poder gestionar los perfiles de todas las mascotas.
- **RF09.** El administrador o el veterinario deben poder buscar mascotas por su ID.

### Gestión de Citas
- **RF10.** El sistema debe permitir a los usuarios agendar citas veterinarias.
- **RF11.** El sistema debe permitir a los usuarios cancelar sus citas.
- **RF12.** El sistema debe permitir al personal médico o administrativo gestionar y editar citas.
- **RF13.** El sistema debe permitir al administrador buscar citas por su ID.

### Historial Médico
- **RF14.** El sistema debe permitir a los usuarios visualizar el historial médico de sus mascotas.
- **RF15.** El sistema debe permitir a los veterinarios registrar actualizaciones en el historial médico de una mascota.

### Reseñas
- **RF16.** El sistema debe permitir a los usuarios publicar reseñas sobre la atención veterinaria recibida.
- **RF17.** El sistema debe permitir a los usuarios visualizar las reseñas publicadas por otros usuarios.

### Chatbot Informativo
- **RF18.** El sistema debe proporcionar un chatbot que brinde consejos sobre:
  - Alimentación de mascotas.
  - Higiene animal.
  - Salud y síntomas.
  - Entrenamiento básico.
  - Recomendaciones personalizadas según tipo de mascota.


## 3.1.2. Requisitos No Funcionales

- **RNF01:** El sistema debe tener alta disponibilidad al estar activo las 24 horas del día, los 7 días de la semana.
- **RNF02:** La interfaz debe ser intuitiva y fácil de usar para cualquier tipo de usuario, cumpliendo con la heurística de User Control and Freedom como mínimo.
- **RNF03:** El sistema debe estar desarrollado bajo una arquitectura web responsive.
- **RNF04:** Las respuestas del sistema no deben superar los 3 segundos en operaciones comunes.
- **RNF05:** El sistema debe enviar correos electrónicos de forma segura utilizando un proveedor confiable como Outlook o Gmail.
- **RNF06:** Toda la información de los usuarios y sus mascotas debe almacenarse en un proveedor de base de datos relacional como PostgreSQL o MySQL.
- **RNF07:** El frontend debe cargarse completamente en menos de 3 segundos con conexión de red promedio.
- **RNF08:** La landing page debe cargarse completamente en menos de 3 segundos con conexión de red promedio.
- **RNF09:** El frontend de la aplicación web debe ser implementado con Angular y TypeScript.
- **RNF10:** El backend de la aplicación web debe ser implementado con Java y Spring Boot.





## 3.2. User Stories
## Gestión de Usuarios
**EP01: Como administrador, deseo gestionar los usuarios para asegurar que solo personas autorizadas tengan acceso al sistema.**

| User Story ID | Título                     | Descripción                                                                                                                                                    |
|---------------|----------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| US01          | Registro de Usuario        | Como visitante, deseo registrarme en la plataforma para poder utilizar las funcionalidades del sistema                                                        |
| US02          | Gestión de Cuentas de Usuarios | Como administrador, deseo gestionar los cuentas de los usuarios para mantener la información y permisos actualizados.                                    |

---
# Gestión de Mascotas
**EP02: Como usuario, deseo gestionar la información de mis mascotas para mantener sus datos actualizados.**

| User Story ID | Título                     | Descripción                                                                                                                                                    |
|---------------|----------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| US03          | Creación de Perfil de Mascota | Como usuario, deseo crear un perfil de mi mascota para tener su información almacenada en la plataforma.                                                  |
| US04          | Edición de Perfil de Mascota | Como usuario, deseo editar el perfil de mi mascota para actualizar su información cuando sea necesario.                                                    |
| US05          | Visualización de Perfiles de Mascotas | Como usuario, deseo visualizar los perfiles de mis mascotas para revisar la información registrada.                                                    |
| US06          | Búsqueda de Mascotas por ID | Como administrador, deseo buscar mascotas por ID para acceder rápidamente a su información en el sistema.                                                   |
| US07          | Gestión de Perfiles de Mascotas | Como administrador, deseo gestionar los perfiles de mascotas para asegurarme de que la información esté correctamente registrada y actualizada.          |

---

# Gestión de Citas Veterinarias
**EP03: Como usuario, deseo gestionar las citas veterinarias de mis mascotas para asegurarme de que reciban atención médica a tiempo.**

| User Story ID | Título                     | Descripción                                                                                                                                                    |
|---------------|----------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| US08          | Agendamiento de Citas      | Como usuario, deseo agendar citas veterinarias para asegurar que mi mascota reciba atención médica en el momento adecuado.                                     |
| US09          | Cancelación de Citas       | Como usuario, deseo cancelar una cita si no puedo asistir, para evitar problemas de horario y reorganizar la atención.                                        |
| US10          | Gestión de Citas Veterinarias | Como administrador o médico veterinario, deseo gestionar las citas veterinarias para coordinar correctamente la atención de las mascotas.                                     |
| US11          | Búsqueda de Citas por ID   | Como administrador o médico veterinario, deseo buscar citas por ID para acceder rápidamente a la información de la cita.                                                           |
| US12          | Edición de Citas Veterinarias | Como administrador o médico veterinario, deseo editar las citas para hacer cambios en la fecha o estado cuando sea necesario.                                                 |

---

# Navegación y Funcionalidades de la Landing Page
**EP04: Como visitante, deseo explorar la página principal de Pawfect Care para entender los servicios y características que ofrece la plataforma.**

| User Story ID | Título                                     | Descripción                                                                                                                                                     |
|---------------|-------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| US13          | Barra de Navegación en la Landing Page     | Como visitante, deseo usar la barra de navegación para acceder fácilmente a las diferentes secciones de la plataforma.                                        |
| US14          | Visualización de la Sección "Why Choose Us?" | Como visitante, deseo revisar la sección "Why Choose Us?" para entender los beneficios y servicios de la plataforma.                                     |
| US15          | Envío de Mensajes de Contacto             | Como visitante, deseo enviar un mensaje de contacto a través de la landing page para comunicarme con el equipo de Pawfect Care.                             |
| US16          | Visualización de Videos en la Sección de Características | Como visitante, deseo ver los videos informativos sobre los productos y servicios para conocer más sobre Pawfect Care.                                    |

---

# Gestión de Clientes
**EP05: Como administrador, deseo gestionar la información de los clientes para mantener los datos actualizados y organizados.**

| User Story ID | Título                     | Descripción                                                                                                                                                    |
|---------------|----------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| US17          | Creación de Perfiles de Clientes | Como administrador, deseo crear perfiles de clientes para registrar la información de contacto y sus mascotas.                                            |
| US18          | Edición de Perfiles de Clientes | Como administrador, deseo editar los perfiles de clientes para actualizar su información personal y de contacto.                                          |
| US19          | Búsqueda de Clientes por ID | Como administrador, deseo buscar clientes por su ID para acceder rápidamente a su información.                                      |

---

# Consultas Automatizadas
**EP06: Como usuario, deseo realizar consultas simples para obtener información rápida sobre el cuidado y bienestar de mi mascota.

| User Story ID | Título                                | Descripción                                                                                                                                      |
|---------------|----------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|
| US20          | Consulta sobre alimentación adecuada   | Como usuario, deseo consultar al chatbot sobre qué tipo de comida es ideal para mi mascota según su especie, edad y tamaño.                      |
| US21          | Consejos de higiene para mascotas      | Como usuario, deseo recibir recomendaciones básicas de higiene para mantener saludable a mi mascota.                                            |
| US22          | Preguntas frecuentes sobre salud       | Como usuario, deseo obtener respuestas rápidas sobre síntomas comunes y saber cuándo debo acudir al veterinario.                                |
| US23          | Consejos de entrenamiento básico       | Como usuario, deseo consultar sobre técnicas de adiestramiento o corrección de comportamientos no deseados.                                     |
| US24          | Recomendaciones según tipo de mascota  | Como usuario, deseo que el chatbot me dé consejos generales adaptados al tipo de mascota que tengo (perro, gato, ave, etc).                    |

---

# Gestión de Historial Médico de las Mascotas
**EP07: Como usuario o administrador, deseo gestionar el historial médico de las mascotas para llevar un registro de sus atenciones y tratamientos.**

| User Story ID | Título                     | Descripción                                                                                                                                                    |
|---------------|----------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| US25          | Visualización del Historial Médico | Como usuario, deseo visualizar el historial médico de mi mascota para revisar su estado de salud y tratamientos previos.                                  |
| US26          | Actualización del Historial Médico | Como administrador o doctor veterinario, deseo actualizar el historial médico de las mascotas para que los usuarios tengan la información más reciente sobre sus tratamientos. |

---

# Reviews y Feedback
**EP08: Como usuario dueño de una mascota, deseo poder dejar reseñas y comentarios sobre un doctor veterinario.**

| User Story ID | Título                     | Descripción                                                                                                                                                    |
|---------------|----------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| US27          | Publicar Reseñas | Como usuario dueño de una mascota, deseo dejar una reseña sobre un doctor veterinario para compartir mi experiencia con otros 
usuarios.                   |
| US28          | Visualización de Reseñas | Como dueño de una mascota, deseo ver las reseñas de otros usuarios sobre un doctor veterinario para conocer la calidad del servicio y su calificación general. |

---

# Funcionalidades de Idioma en la App Web
**EP09: Como usuario, deseo cambiar el idioma de la plataforma para navegar entre las versiones en inglés y español de la app web.**

| User Story ID | Título                     | Descripción                                                                                                                                                    |
|---------------|----------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| US29          | Cambio de Idioma en la App Web | Como usuario, deseo cambiar el idioma de la app web para poder utilizarla en inglés o español según mi preferencia.                                        |

<br><br>
# Historias de Usuario y Criterios de Aceptación

## US01: Registro de Usuario
**Relacionado con (Epic ID):** EP01

**Descripción:**  
Como administrador, deseo gestionar los usuarios para asegurar que solo personas autorizadas tengan acceso al sistema.

### Criterios de Aceptación:
- **Escenario 1:** El usuario necesita registrarse en el sistema  
  - **Dado que** el usuario está en la página de registro,  
  - **Cuando** el usuario completa todos los campos requeridos (nombre completo, teléfono, correo electrónico, dirección y contraseña),  
  - **Entonces** el sistema debe permitir al usuario crear una cuenta y mostrar un mensaje de confirmación.

- **Escenario 2:** El usuario ingresa un correo electrónico ya registrado  
  - **Dado que** el usuario intenta registrarse con un correo electrónico ya asociado a una cuenta,  
  - **Cuando** el usuario ingresa el correo duplicado y envía el formulario,  
  - **Entonces** el sistema debe mostrar un mensaje de error indicando que el correo ya está registrado.

- **Escenario 3:** El usuario deja campos obligatorios sin llenar  
  - **Dado que** el usuario intenta registrarse sin completar todos los campos obligatorios,  
  - **Cuando** el usuario presiona el botón de registro sin llenar todos los campos,  
  - **Entonces** el sistema debe mostrar un mensaje de error solicitando que se completen todos los campos requeridos.

---

## US02: Gestión de Cuentas de Usuarios
**Relacionado con (Epic ID):** EP01

**Descripción:**  
Como administrador, deseo gestionar los cuentas de los usuarios para mantener la información y permisos actualizados.

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

## US03: Creación de Perfil de Mascota
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

## US04: Edición de Perfil de Mascota
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

## US05: Visualización de Perfiles de Mascotas  
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

## US06: Búsqueda de Mascotas por ID  
**Relacionado con (Epic ID):** EP02

**Descripción:**  
Como administrador, deseo buscar mascotas por ID para acceder rápidamente a su información en el sistema.

### Criterios de Aceptación:
- **Escenario 1:** El administrador busca una mascota por ID válido  
  - **Dado que** el administrador está en la sección de gestión de mascotas,  
  - **Cuando** ingresa un ID de mascota válido en el campo de búsqueda,  
  - **Entonces** el sistema debe mostrar el perfil correspondiente a ese ID.

- **Escenario 2:** El administrador ingresa un ID inexistente  
  - **Dado que** el administrador intenta buscar una mascota,  
  - **Cuando** ingresa un ID que no está registrado,  
  - **Entonces** el sistema debe mostrar un mensaje indicando que no se encontró ninguna mascota con ese ID.

---

## US07: Gestión de Perfiles de Mascotas  
**Relacionado con (Epic ID):** EP02

**Descripción:**  
Como administrador, deseo gestionar los perfiles de mascotas para asegurarme de que la información esté correctamente registrada y actualizada.

### Criterios de Aceptación:
- **Escenario 1:** El administrador edita un perfil de mascota  
  - **Dado que** el administrador está gestionando perfiles de mascotas,  
  - **Cuando** selecciona un perfil y actualiza la información,  
  - **Entonces** el sistema debe permitir guardar los cambios y mostrar una confirmación de éxito.

- **Escenario 2:** El administrador elimina un perfil de mascota  
  - **Dado que** el administrador está en la lista de mascotas,  
  - **Cuando** selecciona la opción de eliminar en un perfil,  
  - **Entonces** el sistema debe solicitar confirmación y, al aceptarse, eliminar permanentemente el perfil y sus datos.

- **Escenario 3:** El administrador visualiza el historial de cambios en un perfil  
  - **Dado que** el administrador desea verificar cambios anteriores,  
  - **Cuando** accede a un perfil de mascota,  
  - **Entonces** el sistema debe mostrar un historial con las modificaciones realizadas al perfil.

---

## US08: Agendamiento de Citas  
**Relacionado con (Epic ID):** EP03

**Descripción:**  
Como usuario, quiero agendar citas para que mi mascota reciba atención veterinaria a tiempo.

### Criterios de Aceptación:
- **Escenario 1:** El usuario necesita agendar una cita  
  - **Dado que** el usuario necesita una consulta veterinaria,  
  - **Cuando** acceda a la opción de "Agendar Cita" y seleccione la fecha, hora y tipo de servicio,  
  - **Entonces** la cita será agendada correctamente y recibirá una confirmación.

---

## US09: Cancelación de Citas  
**Relacionado con (Epic ID):** EP03

**Descripción:**  
Como usuario, quiero cancelar citas agendadas en caso de que no pueda asistir.

### Criterios de Aceptación:
- **Escenario 1:** El usuario necesita cancelar una cita previamente agendada  
  - **Dado que** el usuario ha reservado una cita,  
  - **Cuando** haga clic en "Cancelar Cita" en su historial de citas,  
  - **Entonces** la cita será eliminada y se enviará una notificación de cancelación.

---

## US10: Gestión de Citas Veterinarias
**Relacionado con (Epic ID):** EP03

**Descripción:**  
Como administrador, deseo gestionar las citas veterinarias para coordinar correctamente la atención de las mascotas.

### Criterios de Aceptación:
- **Escenario 1:** El administrador visualiza todas las citas  
  - **Dado que** el administrador está en la sección de gestión de citas,  
  - **Cuando** accede al listado de citas agendadas,  
  - **Entonces** el sistema debe mostrar todas las citas con detalles como fecha, hora, veterinario asignado, y estado de la cita (agendada, cancelada, etc.).

- **Escenario 2:** El administrador filtra las citas por estado o fecha  
  - **Dado que** el administrador está gestionando las citas,  
  - **Cuando** utiliza los filtros para buscar citas según estado (agendada, cancelada, completada) o fecha,  
  - **Entonces** el sistema debe mostrar solo las citas que coincidan con los criterios seleccionados.

---

## US11: Búsqueda de Citas por ID
**Relacionado con (Epic ID):** EP03

**Descripción:**  
Como administrador, deseo buscar citas por ID para acceder rápidamente a la información de la cita.

### Criterios de Aceptación:
- **Escenario 1:** El administrador busca una cita por su ID  
  - **Dado que** el administrador está en la sección de citas,  
  - **Cuando** ingresa el ID de una cita en el campo de búsqueda,  
  - **Entonces** el sistema debe mostrar la cita correspondiente al ID ingresado.

- **Escenario 2:** El administrador ingresa un ID inválido  
  - **Dado que** el administrador está buscando una cita por ID,  
  - **Cuando** ingresa un ID que no existe en el sistema,  
  - **Entonces** el sistema debe mostrar un mensaje de error indicando que no se encontró ninguna cita con ese ID.

---

## US12: Edición de Citas Veterinarias
**Relacionado con (Epic ID):** EP03

**Descripción:**  
Como administrador, deseo editar las citas para hacer cambios en la fecha o estado cuando sea necesario.

### Criterios de Aceptación:
- **Escenario 1:** El administrador edita la fecha de una cita  
  - **Dado que** el administrador está en la página de gestión de citas,  
  - **Cuando** selecciona una cita y cambia su fecha u hora,  
  - **Entonces** el sistema debe actualizar la cita y enviar una notificación al usuario afectado indicando el cambio.

- **Escenario 2:** El administrador cambia el estado de una cita  
  - **Dado que** el administrador está gestionando citas,  
  - **Cuando** selecciona una cita y cambia su estado (de agendada a completada o cancelada),  
  - **Entonces** el sistema debe reflejar el cambio y enviar una actualización al usuario de la cita.

---

## US13: Barra de Navegación en la Landing Page  
**Relacionado con (Epic ID):** EP04

**Descripción:**  
Como visitante, deseo usar la barra de navegación para acceder fácilmente a las diferentes secciones de la plataforma.

### Criterios de Aceptación:
- **Escenario 1:** Visualización de la barra de navegación  
  - **Dado que** un visitante accede a la landing page,  
  - **Cuando** se carga la página,  
  - **Entonces** el sistema debe mostrar una barra de navegación en la parte superior con enlaces a secciones clave (inicio, servicios, contacto, etc.).

- **Escenario 2:** Navegación mediante la barra  
  - **Dado que** un visitante visualiza la barra de navegación,  
  - **Cuando** hace clic en una de las secciones,  
  - **Entonces** el sistema debe redirigirlo correctamente a la sección correspondiente de la landing page.

---

## US14: Visualización de la Sección "Why Choose Us?"  
**Relacionado con (Epic ID):** EP04

**Descripción:**  
Como visitante, deseo revisar la sección "Why Choose Us?" para entender los beneficios y servicios de la aplicación.

### Criterios de Aceptación:
- **Escenario 1:** Acceso a la sección "Why Choose Us?"
  - **Dado que** el visitante se desplaza por la landing page,  
  - **Cuando** llega a la sección "Why Choose Us?",  
  - **Entonces** el visitante visualiza una sección destacada con información clara sobre los beneficios de la aplicación.

- **Escenario 2:** Visualización de contenido  
  - **Dado que** el visitante está en la sección "Why Choose Us?",  
  - **Cuando** revisa el contenido,  
  - **Entonces** el visitante debe encontrar íconos, textos o elementos visuales que expliquen los valores diferenciales de Pawfect Care.

---

## US15: Envío de Mensajes de Contacto  
**Relacionado con (Epic ID):** EP04

**Descripción:**  
Como visitante, deseo enviar un mensaje de contacto a través de la landing page para comunicarme con el equipo de Pawfect Care.

### Criterios de Aceptación:
- **Escenario 1:** Visualización del formulario de contacto  
  - **Dado que** el visitante está en la sección de contacto,  
  - **Cuando** la sección es visible,  
  - **Entonces** el sistema muestra un formulario con campos para nombre, correo electrónico, asunto y mensaje.

- **Escenario 2:** Envío exitoso del formulario  
  - **Dado que** el visitante ha llenado todos los campos requeridos,  
  - **Cuando** hace clic en el botón de enviar,  
  - **Entonces** el sistema debe enviar el mensaje y mostrar una confirmación de envío exitoso.

---

## US16: Visualización de Videos en la Sección de Características  
**Relacionado con (Epic ID):** EP04

**Descripción:**  
Como visitante, deseo ver los videos informativos sobre los productos y servicios para conocer más sobre Pawfect Care.

### Criterios de Aceptación:
- **Escenario 1:** Visualización de reproductores de video  
  - **Dado que** el visitante llega a la sección de características,  
  - **Cuando** se carga la página,  
  - **Entonces** el sistema muestra los reproductores de video que están disponibles.

- **Escenario 2:** Reproducción de video  
  - **Dado que** el visitante está en la sección de características,  
  - **Cuando** hace clic en el botón de reproducción de un video,  
  - **Entonces** el sistema comienza a reproducir el video correctamente sin errores.

---

## US17: Creación de Perfiles de Clientes  
**Relacionado con (Epic ID):** EP05

**Descripción:**  
Como administrador, deseo crear perfiles de clientes para registrar la información de contacto y sus mascotas.

### Criterios de Aceptación:
- **Escenario 1:** Visualización del formulario de creación  
  - **Dado que** el administrador accede a la sección de gestión de clientes,  
  - **Cuando** selecciona la opción de "crear cliente",  
  - **Entonces** el administrador debe visualizar un formulario con campos para nombre, correo, teléfono y datos de mascotas.

- **Escenario 2:** Envío exitoso del formulario  
  - **Dado que** el administrador completa todos los campos requeridos,  
  - **Cuando** hace clic en "Guardar",  
  - **Entonces** el administrador debe visualizar el nuevo perfil creado y añadido en la lista de clientes.

---

## US18: Edición de Perfiles de Clientes  
**Relacionado con (Epic ID):** EP05

**Descripción:**  
Como administrador, deseo editar los perfiles de clientes para actualizar su información personal y de contacto.

### Criterios de Aceptación:
- **Escenario 1:** Acceso a la edición de perfil  
  - **Dado que** el administrador se encuentra en la lista de clientes,  
  - **Cuando** selecciona un perfil y elige la opción "Editar",  
  - **Entonces** el administrador debe mostrarse un formulario editable con los datos actuales del cliente.

- **Escenario 2:** Actualización exitosa de la información  
  - **Dado que** el administrador modifica los datos del cliente,  
  - **Cuando** hace clic en "Guardar cambios",  
  - **Entonces** el sistema actualiza la información y la refleja correctamente en el perfil del cliente.

---

## US19: Búsqueda de Clientes por ID  
**Relacionado con (Epic ID):** EP05

**Descripción:**  
Como administrador, deseo buscar clientes por su ID para acceder rápidamente a su información.

### Criterios de Aceptación:
- **Escenario 1:** Ingreso del ID en el buscador  
  - **Dado que** el administrador se encuentra en la sección de búsqueda de clientes,  
  - **Cuando** introduce un ID válido en el campo de búsqueda,  
  - **Entonces** el sistema debe mostrar la información correspondiente al cliente con ese ID.

- **Escenario 2:** ID inexistente  
  - **Dado que** el administrador introduce un ID no registrado,  
  - **Cuando** ejecuta la búsqueda,  
  - **Entonces** el sistema debe mostrar un mensaje indicando que no se encontró ningún cliente con ese ID.

---

## US20: Consulta sobre Alimentación Adecuada  
**Relacionado con (Epic ID):** EP06

**Descripción:**  
Como usuario, deseo consultar al chatbot sobre qué tipo de comida es ideal para mi mascota según su especie, edad y tamaño.

### Criterios de Aceptación:
- **Escenario 1:** Consulta con datos completos  
  - **Dado que** el usuario ha proporcionado la especie, edad y tamaño de su mascota,  
  - **Cuando** el usuario pregunta por el tipo de comida adecuada,  
  - **Entonces** el chatbot debe proporcionar una recomendación personalizada basada en esos datos.

- **Escenario 2:** Consulta con datos incompletos  
  - **Dado que** el usuario no ha proporcionado todos los datos,  
  - **Cuando** el usuario pregunta por el tipo de comida adecuada,  
  - **Entonces** el chatbot debe pedir información adicional o proporcionar una respuesta más general.

---

## US21: Consejos de Higiene para Mascotas  
**Relacionado con (Epic ID):** EP06

**Descripción:**  
Como usuario, deseo recibir recomendaciones básicas de higiene para mantener saludable a mi mascota.

### Criterios de Aceptación:
- **Escenario 1:** Consulta sobre higiene  
  - **Dado que** el usuario pregunta por consejos de higiene,  
  - **Cuando** el chatbot responde,  
  - **Entonces** debe proporcionar consejos generales sobre el baño, cuidado de dientes y otras prácticas de higiene.

- **Escenario 2:** Consulta específica sobre problemas de higiene  
  - **Dado que** el usuario pregunta sobre un problema específico de higiene (por ejemplo, mal aliento, piel seca),  
  - **Cuando** el chatbot responde,  
  - **Entonces** debe dar recomendaciones más detalladas según el problema planteado.

---

## US22: Preguntas Frecuentes sobre Salud  
**Relacionado con (Epic ID):** EP06

**Descripción:**  
Como usuario, deseo obtener respuestas rápidas sobre síntomas comunes y saber cuándo debo acudir al veterinario.

### Criterios de Aceptación:
- **Escenario 1:** Consulta sobre síntomas comunes  
  - **Dado que** el usuario pregunta sobre síntomas comunes,  
  - **Cuando** el chatbot responde,  
  - **Entonces** debe proporcionar información sobre posibles causas y cuándo es necesario consultar a un veterinario.

- **Escenario 2:** Consulta sobre cuándo acudir al veterinario  
  - **Dado que** el usuario pregunta cuándo debería ir al veterinario,  
  - **Cuando** el chatbot responde,  
  - **Entonces** debe dar ejemplos de situaciones críticas en las que es importante buscar atención profesional.

---

## US23: Consejos de Entrenamiento Básico  
**Relacionado con (Epic ID):** EP06

**Descripción:**  
Como usuario, deseo consultar sobre técnicas de adiestramiento o corrección de comportamientos no deseados.

### Criterios de Aceptación:
- **Escenario 1:** Consulta sobre adiestramiento básico  
  - **Dado que** el usuario pregunta sobre técnicas de adiestramiento,  
  - **Cuando** el chatbot responde,  
  - **Entonces** debe proporcionar consejos sobre entrenamiento de comandos básicos como "sentado", "quieto", etc.

- **Escenario 2:** Consulta sobre corrección de comportamientos no deseados  
  - **Dado que** el usuario pregunta sobre cómo corregir un comportamiento no deseado (por ejemplo, ladridos excesivos),  
  - **Cuando** el chatbot responde,  
  - **Entonces** debe ofrecer sugerencias sobre cómo corregir ese comportamiento específico.

---

## US24: Recomendaciones Según Tipo de Mascota  
**Relacionado con (Epic ID):** EP06

**Descripción:**  
Como usuario, deseo que el chatbot me dé consejos generales adaptados al tipo de mascota que tengo (perro, gato, ave, etc).

### Criterios de Aceptación:
- **Escenario 1:** Consulta sobre tipo de mascota  
  - **Dado que** el usuario especifica el tipo de mascota (perro, gato, etc.),  
  - **Cuando** el usuario pide recomendaciones,  
  - **Entonces** el chatbot debe proporcionar consejos específicos según el tipo de mascota.

- **Escenario 2:** Consulta sin especificar tipo de mascota  
  - **Dado que** el usuario no especifica el tipo de mascota,  
  - **Cuando** el usuario pide recomendaciones,  
  - **Entonces** el chatbot debe pedir al usuario que indique el tipo de mascota para personalizar las recomendaciones.

---

## US25: Visualización del Historial Médico
**Relacionado con (Epic ID):** EP07

**Descripción:**  
Como usuario, deseo visualizar el historial médico de mi mascota para revisar su estado de salud y tratamientos previos.

### Criterios de Aceptación:
- **Escenario 1:** Visualización exitosa del historial médico  
  - **Dado que** soy un usuario autenticado en la plataforma,  
  - **Cuando** accedo al perfil de mi mascota y selecciono la opción de visualizar el historial médico,  
  - **Entonces** el sistema debe mostrarme todos los detalles del historial médico, incluyendo diagnósticos, tratamientos, y citas previas de mi mascota.

- **Escenario 2:** Historial médico sin información registrada  
  - **Dado que** soy un usuario autenticado accediendo al perfil de mi mascota,  
  - **Cuando** intento visualizar el historial médico y no existen registros previos de atención,  
  - **Entonces** el sistema debe mostrar un mensaje indicando que no hay información médica disponible en el historial de la mascota.

---

## US26: Actualización del Historial Médico
**Relacionado con (Epic ID):** EP07

**Descripción:**  
Como administrador o doctor veterinario, deseo actualizar el historial médico de las mascotas para que los usuarios tengan la información más reciente sobre sus tratamientos.

### Criterios de Aceptación:
- **Escenario 1:** Actualización exitosa del historial médico  
  - **Dado que** soy un administrador o doctor veterinario,  
  - **Cuando** realizo una actualización en el historial médico de una mascota (ej. registrar un nuevo diagnóstico o tratamiento),  
  - **Entonces** el sistema debe guardar los cambios y reflejar la nueva información en el perfil de la mascota, accesible para los usuarios.

- **Escenario 2:** Intento de actualización con campos obligatorios incompletos  
  - **Dado que** soy un administrador o doctor veterinario intentando actualizar el historial médico,  
  - **Cuando** dejo campos obligatorios sin completar (ej. fecha del tratamiento o diagnóstico),  
  - **Entonces** el sistema debe mostrar un mensaje de error solicitando que se completen los campos obligatorios antes de guardar los cambios.

- **Escenario 3:** Verificación de actualizaciones previas en el historial  
  - **Dado que** soy un administrador o doctor veterinario,  
  - **Cuando** accedo a un historial médico previamente actualizado,  
  - **Entonces** el sistema debe poder mostrar un registro detallado de todas las actualizaciones realizadas, incluyendo las fechas y los usuarios que realizaron cada modificación.

---

## US27: Publicar Reseñas  
**Relacionado con (Epic ID):** EP08  

**Descripción:**  
Como usuario dueño de una mascota, deseo dejar una reseña sobre un doctor veterinario para compartir mi experiencia con otros usuarios.

### Criterios de Aceptación:
- **Escenario 1:** Publicación de una reseña completa  
  - **Dado que** el usuario ha tenido una consulta con un doctor veterinario,  
  - **Cuando** accede al formulario de reseña y completa los campos requeridos (comentario, calificación, nombre del doctor),  
  - **Entonces** el sistema debe guardar la reseña y mostrarla públicamente en el perfil del doctor.

- **Escenario 2:** Publicación con campos incompletos  
  - **Dado que** el usuario intenta enviar la reseña sin llenar todos los campos obligatorios,  
  - **Cuando** hace clic en “Publicar”,  
  - **Entonces** el sistema debe mostrar un mensaje de error indicando qué campos están faltando.

---

## US28: Visualización de Reseñas  
**Relacionado con (Epic ID):** EP08  

**Descripción:**  
Como dueño de una mascota, deseo ver las reseñas de otros usuarios sobre un doctor veterinario para conocer la calidad del servicio y su calificación general.

### Criterios de Aceptación:
- **Escenario 1:** Visualización de reseñas existentes  
  - **Dado que** el usuario accede al perfil de un doctor veterinario,  
  - **Cuando** navega a la sección de reseñas,  
  - **Entonces** el sistema debe mostrar todas las reseñas publicadas, incluyendo comentarios y calificaciones.

- **Escenario 2:** Doctor sin reseñas  
  - **Dado que** el doctor veterinario no tiene reseñas aún,  
  - **Cuando** el usuario accede a su perfil,  
  - **Entonces** el sistema debe mostrar un mensaje indicando que aún no hay reseñas disponibles.

---

## US29: Cambio de Idioma en la App Web  
**Relacionado con (Epic ID):** EP09 

**Descripción:**  
Como usuario, deseo cambiar el idioma de la app web para poder utilizarla en inglés o español según mi preferencia.

### Criterios de Aceptación:

- **Escenario 1:** Cambio de idioma desde el menú  
  - **Dado que** el usuario está navegando en la app web,  
  - **Cuando** selecciona un idioma diferente desde el selector de idioma ("English" o "Español"),  
  - **Entonces** el sistema actualiza todo el contenido visible de la interfaz al idioma seleccionado.

- **Escenario 2:** Elementos no traducidos  
  - **Dado que** el usuario ha seleccionado un idioma,  
  - **Cuando** algún texto no esté disponible en el idioma elegido,  
  - **Entonces** el sistema debe mostrarlo en el idioma por defecto (español), acompañado de una alerta para los desarrolladores.


## 3.3. Impact Mapping.

Este Impact Map muestra cómo Pawfect Care alinea sus objetivos de negocio con los impactos deseados. Detalla los entregables específicos y las user stories que abordan estos impactos, asegurando que cada aspecto del desarrollo de la plataforma mejore la eficiencia y la experiencia del usuario.

[![Impactmap.png](https://i.postimg.cc/4df4zmDD/Impactmap.png)](https://postimg.cc/064qv22n)

## 3.4. Product Backlog.

Con el fin de simplificar la complejidad de las tareas, hemos utilizado la escala de Fibonacci (1/2/3/5/8) para crear nuestro product backlog.
Historia de usuario base:
Tomamos como referencia US06: Como usuario, quiero agendar citas para que mi mascota reciba atención veterinaria a tiempo. (Posee 3 puntos de historia).
Asimismo, utilizamos la herramienta “Planning Poker Online” para poder votar en grupo y decidir la dificultad de cada historia de usuario, tomando como punto intermedio el User Story 06

<table>
  <thead>
    <tr>
      <th># Orden</th>
      <th>User Story ID</th>
      <th>Título</th>
      <th>Descripción</th>
      <th>Story Points (1/2/3/5/8)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>US08</td>
      <td>Agendamiento de Citas</td>
      <td>Como usuario, deseo agendar citas para que mis mascotas reciban atención veterinaria.</td>
      <td>3</td>
    </tr>
    <tr>
      <td>2</td>
      <td>US09</td>
      <td>Cancelación de Citas</td>
      <td>Como usuario, deseo cancelar citas si no puedo asistir, para reorganizar la atención de mis mascotas.</td>
      <td>2</td>
    </tr>
    <tr>
      <td>3</td>
      <td>US17</td>
      <td>Creación de Perfiles de Clientes</td>
      <td>Como usuario, deseo registrar mi perfil para poder gestionar mis mascotas y citas.</td>
      <td>3</td>
    </tr>
    <tr>
      <td>4</td>
      <td>US03</td>
      <td>Creación de Perfil de Mascota</td>
      <td>Como usuario, deseo crear un perfil para cada una de mis mascotas y llevar el control de su información.</td>
      <td>3</td>
    </tr>
    <tr>
      <td>5</td>
      <td>US04</td>
      <td>Edición de Perfil de Mascota</td>
      <td>Como usuario, deseo editar la información de mis mascotas para mantenerla actualizada.</td>
      <td>3</td>
    </tr>
    <tr>
      <td>6</td>
      <td>US05</td>
      <td>Visualización de Perfiles de Mascotas</td>
      <td>Como usuario, deseo consultar los perfiles de mis mascotas en cualquier momento.</td>
      <td>2</td>
    </tr>
    <tr>
      <td>7</td>
      <td>US10</td>
      <td>Gestión de Citas (Admin/Doctor)</td>
      <td>Como personal médico o administrador, deseo gestionar las citas para atender a los clientes.</td>
      <td>5</td>
    </tr>
    <tr>
      <td>8</td>
      <td>US25</td>
      <td>Visualización del Historial Médico</td>
      <td>Como usuario, deseo consultar el historial médico de mis mascotas para conocer diagnósticos y tratamientos anteriores.</td>
      <td>3</td>
    </tr>
    <tr>
      <td>9</td>
      <td>US26</td>
      <td>Actualización del Historial Médico (Doctor)</td>
      <td>Como veterinario, deseo registrar el historial médico de una mascota para llevar un control clínico.</td>
      <td>3</td>
    </tr>
    <tr>
      <td>10</td>
      <td>US27</td>
      <td>Publicar Reseñas sobre Veterinarios</td>
      <td>Como usuario, deseo dejar reseñas sobre la atención recibida para compartir mi experiencia.</td>
      <td>2</td>
    </tr>
    <tr>
      <td>11</td>
      <td>US28</td>
      <td>Visualización de Reseñas</td>
      <td>Como usuario, deseo leer reseñas de otros para elegir al mejor profesional para mi mascota.</td>
      <td>2</td>
    </tr>
    <tr>
      <td>12</td>
      <td>US20</td>
      <td>Chatbot: Consejos de Alimentación</td>
      <td>Como usuario, deseo obtener consejos sobre la alimentación adecuada para mis mascotas mediante un chatbot.</td>
      <td>5</td>
    </tr>
    <tr>
      <td>13</td>
      <td>US21</td>
      <td>Chatbot: Higiene Animal</td>
      <td>Como usuario, deseo obtener consejos sobre higiene para cuidar mejor a mis mascotas.</td>
      <td>5</td>
    </tr>
    <tr>
      <td>14</td>
      <td>US22</td>
      <td>Chatbot: Salud y Síntomas</td>
      <td>Como usuario, deseo identificar síntomas comunes de enfermedades para actuar rápidamente.</td>
      <td>3</td>
    </tr>
    <tr>
      <td>15</td>
      <td>US23</td>
      <td>Chatbot: Entrenamiento Básico</td>
      <td>Como usuario, deseo obtener consejos básicos de entrenamiento para mejorar el comportamiento de mis mascotas.</td>
      <td>2</td>
    </tr>
    <tr>
      <td>16</td>
      <td>US24</td>
      <td>Chatbot: Recomendaciones según Mascota</td>
      <td>Como usuario, deseo obtener recomendaciones personalizadas para cada tipo de mascota.</td>
      <td>2</td>
    </tr>
    <tr>
      <td>17</td>
      <td>US06</td>
      <td>Búsqueda de Mascotas por ID</td>
      <td>Como administrador o médico veterinario, deseo buscar mascotas por su ID para facilitar su gestión interna.</td>
      <td>2</td>
    </tr>
    <tr>
      <td>18</td>
      <td>US07</td>
      <td>Gestión de Perfiles de Mascotas (Admin)</td>
      <td>Como administrador, deseo gestionar todos los perfiles de mascotas registrados en la plataforma.</td>
      <td>3</td>
    </tr>
    <tr>
      <td>19</td>
      <td>US11</td>
      <td>Búsqueda de Citas por ID</td>
      <td>Como administrador, deseo buscar citas médicas por su ID para controlar su trazabilidad.</td>
      <td>2</td>
    </tr>
    <tr>
      <td>20</td>
      <td>US12</td>
      <td>Edición de Citas (Admin/Doctor)</td>
      <td>Como personal médico o administrador, deseo editar las citas programadas para adaptarlas según disponibilidad.</td>
      <td>3</td>
    </tr>
    <tr>
      <td>21</td>
      <td>US13</td>
      <td>Barra de Navegación en la Landing Page</td>
      <td>Como usuario, quiero un menú para navegar entre las secciones principales de la página.</td>
      <td>2</td>
    </tr>
    <tr>
      <td>22</td>
      <td>US14</td>
      <td>Sección "Why Choose Us?"</td>
      <td>Como usuario, quiero conocer las razones para elegir esta plataforma y confiar en sus servicios.</td>
      <td>2</td>
    </tr>
    <tr>
      <td>23</td>
      <td>US15</td>
      <td>Formulario de Contacto</td>
      <td>Como usuario, deseo contactar a la clínica para resolver dudas o pedir ayuda.</td>
      <td>2</td>
    </tr>
    <tr>
      <td>24</td>
      <td>US16</td>
      <td>Videos de Características</td>
      <td>Como usuario, deseo ver videos informativos sobre el uso y beneficios de la aplicación.</td>
      <td>2</td>
    </tr>
    <tr>
      <td>25</td>
      <td>US29</td>
      <td>Cambio de Idioma</td>
      <td>Como usuario, deseo cambiar el idioma de la aplicación para entender mejor el contenido.</td>
      <td>3</td>
    </tr>
    <tr>
      <td>26</td>
      <td>US01</td>
      <td>Registro de Usuarios</td>
      <td>Como usuario, deseo registrarme en la plataforma para acceder a los servicios ofrecidos.</td>
      <td>3</td>
    </tr>
    <tr>
      <td>27</td>
      <td>US02</td>
      <td>Gestión de Perfiles de Usuario (Admin)</td>
      <td>Como administrador, deseo gestionar los cuentas de los usuarios para asegurar el correcto uso del sistema.</td>
      <td>5</td>
    </tr>
    <tr>
      <td>28</td>
      <td>US18</td>
      <td>Edición de Perfil de Cliente (Admin)</td>
      <td>Como administrador, deseo editar los datos de los clientes en caso de errores o cambios solicitados.</td>
      <td>3</td>
    </tr>
    <tr>
      <td>29</td>
      <td>US19</td>
      <td>Búsqueda de Clientes por ID</td>
      <td>Como administrador, deseo buscar a los clientes por su ID para dar seguimiento a sus casos.</td>
      <td>2</td>
    </tr>
  </tbody>
</table>
