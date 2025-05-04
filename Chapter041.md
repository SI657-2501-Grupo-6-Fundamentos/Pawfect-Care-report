# Capítulo IV: Product Architecture Design

## 4.1. Desing Concepts, ViewPoints & ER Diagrams

## 4.1.1. Principles Statements

A partir de la visión de la arquitectura de negocio, se han identificado los siguientes principios que guiarán el desarrollo del proyecto. Estos principios están diseñados para garantizar que las decisiones técnicas y de diseño estén alineadas con los objetivos a largo plazo:

1. **Solicitudes asincrónicas sobre las sincrónicas**: Siempre que sea posible, se priorizará el uso de requests asincrónicas para mejorar la escalabilidad y la capacidad de respuesta del sistema.

2. **Programación orientada a objetos**: Se fomentará el uso de paradigmas de programación orientada a objetos para estructurar el código en torno a entidades y sus interacciones, mejorando la modularidad y la reutilización.

3. **Uso de bibliotecas con soporte comercial**: Se priorizará el uso de bibliotecas y herramientas que cuenten con soporte comercial para garantizar estabilidad y soporte a largo plazo.

4. **Diseño impulsado por el dominio (DDD)**: Se utilizará el enfoque de Diseño Impulsado por el Dominio para garantizar que el modelo de negocio esté en el centro de las decisiones de diseño, promoviendo una alineación clara entre los requisitos del negocio y la implementación técnica.

5. **Adopción de principios SOLID**: Para garantizar un diseño de software robusto, flexible y fácil de mantener, se aplicarán los siguientes principios:

   - **Principio de Responsabilidad Única (SRP)**: Cada clase o módulo del sistema estará alineado a una única responsabilidad. Esto permitirá que el código sea más fácil de testear, mantener y extender.

   - **Principio Abierto/Cerrado (OCP)**: Las clases y módulos estarán diseñados para ser abiertos a la extensión pero cerrados a la modificación. Esto permitirá añadir funcionalidad al negocio sin alterar el funcionamiento de otros componentes, evitando que se produzcan comportamientos inesperados en el sistema.
   
   - **Principio de Sustitución de Liskov (LSP)**: Las clases derivadas podrán sustituir a sus clases base sin alterar la lógica del negocio. Esto garantizará que las implementaciones específicas sean coherentes con los objetivos del proyecto y la aplicación.

   - **Principio de Segregación de Interfaces (ISP)**: Se diseñarán interfaces pequeñas y específicas para cada funcionalidad, evitando interfaces grandes y genéricas. Esto asegurará que los componentes del sistema solo implementen las interfaces que realmente se necesiten, promoviendo modularidad y simplicidad.

   - **Principio de Inversión de Dependencias (DIP)**: Los módulos de alto nivel dependerán de abstracciones en lugar de implementaciones concretas. Esto permitirá desacoplar los componentes del sistema, facilitando la reutilización y el mantenimiento del código a largo plazo.

Estos principios se aplicarán de manera consistente en el desarrollo del proyecto, asegurando un diseño alineado con los objetivos estratégicos y las mejores prácticas de ingeniería de software.

## 4.1.2. Approaches Statements Architectural Styles & Patterns

En el desarrollo del software, se considerarán enfoques arquitectónicos y patrones que permitan abordar la complejidad del sistema y garantizar su alineación con los objetivos del negocio. Uno de los enfoques principales será el uso del patrón Domain Driven Design (DDD), que ofrece los siguientes beneficios:

1. **Enfoque en el dominio del negocio**: Prioriza entender y modelar el dominio central del negocio, asegurando un desarrollo de software orientado a los procesos del negocio y sus objetivos.

2. **Lenguaje ubicuo**: Utiliza un lenguaje común entre desarrolladores y partes interesadas, garantizando una adecuada comprensión con los principales skateholders.

3. **Modelado centrado en el dominio**: Se desarrolla un modelo que representa con precisión las entidades y relaciones clave del negocio, sirviendo como base para estructurar y construir el software.

4. **Colaboración continua**: Fomenta una interacción constante entre los desarrolladores y los expertos en el dominio, lo que permite realizar ajustes progresivos al software conforme evolucionan las necesidades del negocio.

5. **División en contextos específicos**: Los sistemas se organizan en contextos claramente definidos, cada uno con su propio modelo de dominio, lo que simplifica la gestión de la complejidad y permite que los equipos trabajen de manera autónoma.

6. **Gestión eficaz de la complejidad**: Facilita el control de la lógica de negocio al identificar y estructurar de forma clara las entidades, valores y eventos, asegurando que las reglas del negocio se mantengan consistentes.

7. **Flexibilidad y evolución**: Gracias a su enfoque iterativo, el software puede ajustarse fácilmente a los cambios o al crecimiento del negocio, garantizando su sostenibilidad y capacidad de escalar a largo plazo.

Además del enfoque DDD, se considerarán otros patrones arquitectónicos y estilos como:

- **Arquitectura en capas**: Para separar responsabilidades en diferentes capas (presentación, lógica de negocio, acceso a datos), promoviendo modularidad y facilidad de mantenimiento.
- **Microservicios**: Dado que el sistema requiere escalabilidad y despliegue independiente, se evaluará la adopción de una arquitectura basada en microservicios.
- **CQRS (Command Query Responsibility Segregation)**: Para separar las operaciones de lectura y escritura, optimizando el rendimiento y la escalabilidad en sistemas con alta concurrencia.

Estos enfoques y patrones serán evaluados y aplicados según las necesidades específicas del proyecto, asegurando un diseño arquitectónico robusto.

## 4.1.3. Context Diagram

El diagrama de contexto es un recurso clave para analizar las conexiones entre Pawfect Care y los elementos externos que lo rodean. Este enfoque permite identificar posibles áreas de mejora e integración, proporcionando una visión clara de cómo el sistema interactúa con su entorno.

[![Pawfect-Care-Context-Diagram.png](https://i.postimg.cc/PrKSpm8v/Pawfect-Care-Context-Diagram.png)](https://postimg.cc/LnYtGgDm)

## 4.1.4. Approach driven ViewPoints Diagrams

### Container Diagram

En este diagrama se expresa una representación visual que muestra los principales contenedores de software que componen un sistema. Por ejemplo, aplicaciones, bases de datos y microservicios que interactúan entre sí.

[![Pawfect-Care-Containers-Diagram.png](https://i.postimg.cc/sD3ngn1R/Pawfect-Care-Containers-Diagram.png)](https://postimg.cc/ThHjkJrk)


### Pet Management Component Diagram
A continuación, se presenta el diagrama de componentes para el microservicio de gestión de mascotas.
[![Pet-Management-Component.png](https://i.postimg.cc/15Rf7PnN/Pet-Management-Component.png)](https://postimg.cc/NLVsL3xg)

### Medical Appointment Management Component Diagram
A continuación, se presenta el diagrama de componentes para el microservicio de gestión de citas.
[![Pawfect-Care-Appointment-Microservice-Component-Diagram.png](https://i.postimg.cc/L8LhQVBn/Pawfect-Care-Appointment-Microservice-Component-Diagram.png)](https://postimg.cc/PCftPY7j)

### Reviews & Feedback Component Diagram
A continuación, se presenta el diagrama de componentes para el microservicio de Feedback y reviews.
[![Feedback-Component.png](https://i.postimg.cc/N08tw9ZG/Feedback-Component.png)](https://postimg.cc/3ywVXRKz)

### UML Activity Diagrams
#### Bounded Context: Pet Management
[![Diagrama-Actividades-Pet-Management.png](https://i.postimg.cc/Dw7JYVLm/Diagrama-Actividades-Pet-Management.png)](https://postimg.cc/QHndHy6r)

#### Bounded Context: Medical Appointment Management 
[![Diagrama-Actividades-Medical-Appointment-Management.png](https://i.postimg.cc/xjHXfjPc/Diagrama-Actividades-Medical-Appointment-Management.png)](https://postimg.cc/z3zzpr6r)

## 4.1.5. Relational/Non Relational Database Diagram
Optamos por utilizar MySQL como sistema de gestión de bases de datos, gestionado mediante MySQL Workbench. Esta elección se basa en la experiencia previa del equipo con el lenguaje SQL y en la eficacia de esta herramienta para cubrir las necesidades de nuestro proyecto.
[![Pawfect-Care-Database-Diagram.png](https://i.postimg.cc/Xq40Bx5y/Pawfect-Care-2025-05-04-15-45.png)](https://postimg.cc/FdW62yD9)

## 4.1.6. Design Patterns

Los patrones de diseño identificados para el desarrollo del sistema son los siguientes:

### Command

Este patrón encapsula una solicitud como un objeto, permitiendo parametrizar clientes con diferentes solicitudes, encolar o registrar solicitudes, y soportar operaciones como deshacer. Es especialmente útil para desacoplar el objeto que envía una solicitud del que la recibe.

**Aplicación en el sistema:**

- **En Pet Management:**
  - `CreatePetCommand`
  - `EditPetCommand`
  - `DeletePetCommand`
  - `CreateMedicalRecordCommand`
  - `EditMedicalRecordCommand`
  - `DeleteMedicalRecordCommand`

- **En Medical Appointment:**
  - `CreateMedicalAppointmentCommand`
  - `EditMedicalAppointmentCommand`
  - `DeleteMedicalAppointmentCommand`

- **En Reviews & Feedback:**
  - `CreateReviewCommand`
  - `EditReviewCommand`
  - `DeleteReviewCommand`

Con ello se permite implementar de forma flexible la gestión de operaciones (como creación, edición o eliminación) y facilita características futuras como el historial de acciones o deshacer cambios.

---

### Builder

Este patrón permite construir un objeto complejo paso a paso. Es ideal cuando el proceso de construcción debe permitir diferentes representaciones del objeto que se está construyendo.

**Aplicación en el sistema:**

- Para construir objetos de tipo perfil (Profile) tanto de **pet owners** como de **veterinarians**, ya que estos pueden contener múltiples atributos opcionales como la foto de perfil para dueños de mascotas y veterinarios.

Con ello se permite crear perfiles personalizados de forma clara y escalable, evitando constructores con demasiados parámetros y mejorando la legibilidad del código.

## 4.1.7. Tactics
