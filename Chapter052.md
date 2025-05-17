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

#### **Frontend Web (Angular con TypeScript)**
- 


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
