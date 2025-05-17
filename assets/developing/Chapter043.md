## 4.3  ADD Iterations

### 4.3.1   Iteration N: 1

#### 4.3.1.1        Architectural Design Backlog N: 1

![ADD Desgin 1](./assets/chapter04/Addbacklog1.png)

#### 4.3.1.2       Establish Iteration Goal by Selecting Drivers

**Drivers:**

 - **Incorporación:** permitir que Pet Owners y Veterinarians se registren e inicien sesión.

 - **Integración:** validar envío de correos con Outlook API y respuesta de IA simulada.

 - **Usabilidad:** definir límites claros de contexto para usuarios primerizos.

**Meta de la Iteración:** <br>
Definir y validar el contexto del sistema: implementar los flujos básicos de registro/login, simular el envío de recordatorios por email y el módulo de consultoría IA, y asegurar que los dueños de las mascotas y veterinarias puedan interactuar correctamente con el sistema de Pawfect Care.

#### 4.3.1.3       Choose One or More Elements of the System to Refine

Ya que es la primera iteracion, se debe escojer elementos para refinar.

#### 4.3.1.4       Choose One or More Design Concepts That Satisfy the Selected Drivers

<table>
  <tr>
    <th>Desiciones</th>
    <th>Justificacion</th>
  </tr>
  <tr>
    <td>Arquitectura de Microservicios</td>
    <td>Hemos optado por descomponer la plataforma en microservicios independientes para maximizar la escalabilidad, la resiliencia y la autonomía de los equipos. Cada servicio (usuarios, mascotas, citas, chatbot) puede desarrollarse, desplegarse y escalarse de forma aislada, reduciendo el riesgo de impactos colaterales y acelerando la entrega continua. Además, facilita la adopción de distintas tecnologías y versiones sin afectar al resto del sistema.</td>
  </tr>
  <tr>
    <td>Solicitudes Asíncronas sobre Sincrónicas</td>
    <td> Priorizamos el uso de mensajería y colas para las operaciones de larga duración (por ejemplo, envío de emails o consultas de IA), de modo que el frontend nunca bloquee la experiencia de usuario. Esto mejora la capacidad de respuesta del sistema, permite gestionar picos de carga de forma eficiente y garantiza que las tareas intensivas se procesen en segundo plano, sin degradar el rendimiento percibido por el usuario.</td>
  </tr>
  <tr>
    <td>Diseño Impulsado por el Dominio (DDD)</td>
    <td> Adoptamos DDD para asegurar que la estructura del código refleje fielmente los conceptos de negocio: veterinarios, dueños, mascotas y citas. Esto establece un “lenguaje ubicuo” entre desarrolladores y stakeholders, facilita la evolución del modelo de dominio y reduce las brechas de comunicación. Cada microservicio habita su propio bounded context, evitando ambigüedades y permitiendo validar reglas de negocio de forma clara e inequívoca.</td>
  </tr>
  <tr>
    <td>Contenerización con Docker</td>
    <td>Decidimos empaquetar cada microservicio en un contenedor Docker para garantizar portabilidad, coherencia entre entornos (desarrollo, pruebas, producción) y despliegues reproducibles. Docker simplifica la configuración del entorno, acelera la provisión de instancias y minimiza la típica “funciona en mi máquina” al encapsular dependencias y configuraciones en imágenes ligeras y versionadas.</td>
  </tr>
  <tr>
    <td>Patrón CQRS en AppointmentService</td>
    <td>Aplicamos CQRS (Command Query Responsibility Segregation) en el servicio de citas para separar rutas de escritura (crear, editar, cancelar) de consultas (listar, filtrar por fecha o estado). Gracias a esta segregación, optimizamos el rendimiento de lectura en escenarios de alta concurrencia, podemos escalar independientemente cada lado y facilitar la implementación de mecanismos de event sourcing o materialized views que aceleren aún más la entrega de datos.</td>
  </tr>
</table>

#### 4.3.1.5       Instantiate Architectural Elements, Allocate Responsibilities, and Define Interfaces

<table>
  <tr>
    <th>Desiciones</th>
    <th>Justificacion</th>
  </tr>
  <tr>
    <td>Crear AuthService como microservicio independiente</td>
    <td>Separar el manejo de autenticación y generación de JWT en un servicio autónomo facilita el cumplimiento de políticas de seguridad, permite escalar el login de forma aislada y simplifica la integración con Spring Security OAuth para la emisión y validación de tokens.</td>
  </tr>
  <tr>
    <td>Implementar PetService con Spring Data JPA</td>
    <td>Encapsular toda la lógica de creación, edición, búsqueda y eliminación de perfiles de mascota en un microservicio con repositorios JPA garantiza coherencia transaccional, facilita la implementación de pruebas unitarias y reutiliza automáticamente CRUD básicos.</td>
  </tr>
  <tr>
    <td>Definir NotificationService que consuma Outlook API</td>
    <td>Centralizar el envío de correos de confirmación y recordatorios en un servicio dedicado que abstraiga el cliente de Outlook API reduce la repetición de código, optimiza la trazabilidad de envíos y facilita el cambio a otro proveedor de email si fuera necesario.</td>
  </tr>
  <tr>
    <td>Crear ChatbotService con interfaz REST hacia AI externa</td>
    <td>Instanciar un microservicio que exponga un endpoint /chatbot/consulta y consuma el servicio de consultoría AI permite aislar la lógica de procesamiento de lenguaje, gestionar cuotas y monitorizar llamadas al proveedor, y mantener la UI desacoplada.</td>
  </tr>
  <tr>
    <td>Asignar responsabilidad de UI a Angular Material</td>
    <td>Delegar al frontend en Angular con Material Design la responsabilidad de presentar formularios de registro, tablas de mascotas y diálogos de confirmación asegura una experiencia consistente y acelera el desarrollo de componentes reutilizables.</td>
  </tr>
  <tr>
    <td>Establecer DB per microservicio en PostgreSQL for Azure</td>
    <td>Proveer esquemas de base de datos independientes para usuarios, mascotas y citas en PostgreSQL desplegado en Azure evita cuellos de botella, permite políticas de respaldo y escalado granular, y alinea con los requisitos de alta disponibilidad.</td>
  </tr>
</table>

#### 4.3.1.6       Sketch Views (C4 & UML) and Record Design Decisions

[![Pawfect-Care-Context-Diagram.png](https://i.postimg.cc/PrKSpm8v/Pawfect-Care-Context-Diagram.png)](https://postimg.cc/LnYtGgDm)

<table>
  <tr>
    <th>Elemento</th>
    <th>Responsabilidad</th>
  </tr>
  <tr>
    <td>Pet Owners</td>
    <td> Representan a los usuarios finales que registran, gestionan y visualizan información de sus mascotas a través de la plataforma Pawfect Care.</td>
  </tr>
  <tr>
    <td>Veterinarians</td>
    <td>Usuarios profesionales que acceden al sistema para registrar tratamientos, consultas, diagnósticos y controlar los historiales clínicos de las mascotas. </td>
  </tr>
  <tr>
    <td>Pawfect Care System</td>
    <td>Sistema principal que centraliza toda la gestión de datos veterinarios y la interacción entre veterinarios y dueños de mascotas. Incluye módulos de autenticación, gestión de mascotas, historial clínico, y reportes.</td>
  </tr>
  <tr>
    <td>Outlook API</td>
    <td>Servicio externo encargado de facilitar el envío automatizado de correos electrónicos como recordatorios de citas y confirmaciones de registro.</td>
  </tr>
  <tr>
    <td>AI Automated Consulting Services</td>
    <td> Módulo de inteligencia artificial diseñado para analizar síntomas ingresados y proporcionar sugerencias preliminares de diagnóstico o urgencia, asistiendo tanto a veterinarios como a dueños de mascotas.</td>
  </tr>
</table>

#### 4.3.1.7   	Analysis of Current Design and Review Iteration Goal (Kanban Board)  (Avance 1)
![ADD Board](./assets/chapter04/addboard.png)


### 4.3.2   Iteration N: 2

#### 4.3.2.1        Architectural Design Backlog N: 2

#### 4.3.2.2       Establish Iteration Goal by Selecting Drivers

#### 4.3.2.3       Choose One or More Elements of the System to Refine
#### 4.3.2.4       Choose One or More Design Concepts That Satisfy the Selected Drivers
#### 4.3.2.5       Instantiate Architectural Elements, Allocate Responsibilities, and Define Interfaces
#### 4.3.2.6       Sketch Views (C4 & UML) and Record Design Decisions

#### 4.3.2.7   	Analysis of Current Design and Review Iteration Goal (Kanban Board)  (Avance 2)