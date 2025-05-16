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

---

## 2. Pruebas no funcionales
Evalúan atributos del sistema **como rendimiento, seguridad o usabilidad**.

### 🔹 Pruebas de rendimiento (Quality Attributes Tests)
Miden tiempos de respuesta, velocidad, escalabilidad. Para ello, utilizaremos la herramientas Lighthouse.

[![lighthouse2.jpg](https://i.postimg.cc/Wzd3FtNn/lighthouse2.jpg)](https://postimg.cc/tnHy8qVZ)


### 5.1.1.1. Core Entities Unit Tests




### 5.1.1.2. Core Integration Tests



### 5.1.1.3 User Acceptance Tests




### 5.1.1.4 Quality Attributes Tests

Para realizar pruebas no funcionales tomamos en cuenta evaluar los atributos de calidad de escalabilidad y rendimiento. Decidimos utilizar Google Lighthouse porque es una herramienta automatizada de código abierto que permite auditar aplicaciones web en aspectos clave como el rendimiento de carga, optimización para dispositivos móviles, accesibilidad, buenas prácticas de desarrollo y SEO. Lighthouse proporciona métricas cuantitativas y sugerencias de mejora, lo que nos permite identificar cuellos de botella en el rendimiento y oportunidades para optimizar la experiencia del usuario. Además, su integración con navegadores como Chrome facilita su uso en entornos de desarrollo y pruebas continuas.




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
- **Value Objects**: Elementos inmutables que encapsulan atributos relacionados.
- **Commands**: Representan acciones que modifican el estado del dominio (crear, actualizar, eliminar).
- **Queries**: Representan solicitudes de información sin intención de modificar el estado.

---

### ACL (Anti-Corruption Layer)
Esta capa protege el modelo de dominio de las dependencias externas. Actúa como una barrera para evitar la contaminación de modelos externos y traduce estructuras ajenas al lenguaje del dominio. Contiene:

- **Adaptadores de integración**: Clases que convierten objetos de sistemas externos a objetos del dominio.
- **Servicios externos**: Interfaces y sus implementaciones para comunicarse con otros sistemas (por ejemplo, APIs externas).
- **Traductores (Mappers/Transformers)**: Transforman modelos externos a modelos internos y viceversa.

---

### Infrastructure Layer
Se encarga de las dependencias técnicas del sistema. Aquí se implementan los detalles concretos definidos en las interfaces del dominio y se gestionan los recursos del entorno. Contiene:

- **Implementaciones de Repositorios (JPA)**: Persistencia de entidades y aggregates.

---

### Application Layer
Coordina los casos de uso del backend. Aquí no hay lógica de negocio profunda, sino la orquestación de las operaciones del sistema. Contiene:

- **Servicios de Aplicación**: Implementan comandos (crear, actualizar, eliminar) y consultas (lectura de datos).
- **Comandos (Commands)**: Objetos que encapsulan los datos necesarios para ejecutar una acción.
- **Consultas (Queries)**: Objetos que representan peticiones de lectura.
- **Manejadores de Casos de Uso**: Métodos que coordinan validaciones, llamadas al dominio y persistencia.

---

### Interface Layer
Es la puerta de entrada al backend. Expone la funcionalidad del sistema a los clientes (por ejemplo, frontend, otros servicios) y gestiona la interacción con ellos. Contiene:

- **Controladores (Controllers/Handlers)**: Gestionan las solicitudes HTTP/REST.
- **Resources**: Representan estructuras de respuesta (DTOs de salida) que serán devueltas al cliente. Separan el modelo de dominio de lo que realmente se expone en la API.
- **Transform**: Encapsulan la lógica de mapeo entre los objetos del dominio o DTOs internos y los "Resources" que se exponen en la interfaz. Promueven una separación clara entre la representación interna y externa.
- **ACL Context Facade**: Se utiliza en casos donde es necesario invocar servicios o APIs externas desde la capa de interfaz de manera simplificada y desacoplada, actuando como fachada que esconde detalles técnicos.
- **Validaciones de entrada (Request Validation)**: Validan los datos que provienen del cliente (por ejemplo, con anotaciones "@Valid") antes de enviarlos al Application Layer. Aseguran que la entrada sea consistente.
- **Autenticación y Autorización**: Incluye filtros, interceptores o resolvers que gestionan quién accede a qué recurso (por ejemplo, con Spring Security), garantizando seguridad a nivel de endpoints.


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

