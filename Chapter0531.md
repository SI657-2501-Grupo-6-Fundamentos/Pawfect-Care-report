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