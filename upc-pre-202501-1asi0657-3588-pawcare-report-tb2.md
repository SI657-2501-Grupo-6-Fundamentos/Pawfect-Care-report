# COURSE PROJECT

---

<p align="center">
    <strong>Universidad Peruana de Ciencias Aplicadas (UPC)</strong><br>    
    <img src="https://upload.wikimedia.org/wikipedia/commons/f/fc/UPC_logo_transparente.png"></img><br>
    <strong>Carrera de Ingeniería de Software - Ciclo VII</strong><br><br>
    <strong>Fundamentos de Arquitectura de Software - SI729</strong><br>
    <br><strong>Profesor: Ernesto Ocampo Tello</strong><br>
    <br><strong><b>INFORME DEL TRABAJO FINAL</strong></b><br>
</p>

<p align="center">
    <strong>Startup del Proyecto: PawCare</strong><br>
    <strong>Producto: Pawfect Care</strong><br>
</p>

<div>
    <h3 align="center">Team Members:</h3>
</div>

<div>
    <table align="center">
        <tr>
            <th style="text-align:center;">Member</th>
            <th style="text-align:center;">Code</th>
        </tr>
        <tr>
            <td>Aranda Vallejos, Oscar Gabriel</td>
            <td>U202218167</td>
        </tr>
        <tr>
            <td>Chirinos Zúñiga, Rodrigo Manuel</td>
            <td>U202217804</td>
        </tr>
        <tr>
            <td>Gutierrez Garcia, Jose Eduardo</td>
            <td>U202221518</td>
        </tr>
        <tr>
            <td>Silva Morales, Renzo Cesar</td>
            <td>U20221C362</td>
        </tr>
    </table>
    </div>
</body>

<p align="center">
<br><strong>2025-01</strong></p>
<br>

---

# Registro de Versiones del Informe

| Versión | Fecha | Autor | Descripción de la modificación |
|----|----|----|----|
| TB1 | 19/04/2025 | PawCare | Redacción de los Capítulos I: Introduction, II: Requirements Elicitation & Analysis, III: Requirements Specification. |


# Contenido
## Tabla de contenidos
- [**Registro de Versiones del Informe**](#registro-de-versiones-del-informe)
- [**Contenido**](#contenido)
    - [Tabla de contenidos](#tabla-de-contenidos)
- [**Student Outcome**](#student-outcome)
- ## [ **Capítulo I: Introducción** ](#-capítulo-i-introducción-)
  - [**1.1. Startup Profile**](#11-startup-profile)
    - [**1.1.1. Descripción de la Startup**](#112-descripción-de-la-startup)
    - [**1.1.2. Perfiles de integrantes del equipo**](#113-perfiles-de-integrantes-del-equipo)
  - [**1.2. Solution Profile**](#12-solution-profile)
    - [**1.2.1. Nombre del Producto**](#121-nombre-del-producto)
    - [**1.2.2 Antecedentes y problemática**](#122-antecedentes-y-problemática)
    - [What (¿Qué?)](#what-qué)
    - [Who (¿Quién?)](#who-quién)
    - [Where (¿Dónde?)](#where-dónde)
    - [When (¿Cuándo?)](#when-cuándo)
    - [Why (¿Por qué?)](#why-por-qué)
    - [How (¿Cómo?)](#how-cómo)
    - [How much (¿Cuánto?)](#how-much-cuánto)
    - [**1.2.3 Lean UX Process**](#122-lean-ux-process)
    - [**1.2.3.1. Lean UX Problem Statements**](#1221-lean-ux-problem-statements)
    - [**1.2.3.2. Lean UX Assumptions**](#1222-lean-ux-assumptions)
    - [**1.2.3.3. Lean UX Hypothesis Statements**](#1223-lean-ux-hypothesis-statements)
    - [**1.2.3.4. Lean UX Canvas**](#1224-lean-ux-canvas)
  - [**1.3. Segmentos objetivo**](#13-segmentos-objetivo)
- ## [ **Capítulo II: Requirements Elicitation \& Analysis**](#-capítulo-ii-requirements-elicitation--analysis)
  - [**2.1. Competidores**](#21-competidores)
    - [**2.1.1. Análisis competitivo**](#211-análisis-competitivo)
    - [**2.1.2. Estrategias y tácticas frente a competidores**](#212-estrategias-y-tácticas-frente-a-competidores)
  - [**2.2. Entrevistas**](#22-entrevistas)
    - [**2.2.1. Diseño de entrevistas**](#221-diseño-de-entrevistas)
    - [**2.2.2. Registro de entrevistas**](#222-registro-de-entrevistas)
    - [**2.2.3. Análisis de entrevistas**](#223-análisis-de-entrevistas)
  - [**2.3. Needfinding**](#23-needfinding)
    - [**2.3.1. User Personas**](#231-user-personas)
    - [**2.3.2. User Task Matrix**](#232-user-task-matrix)
    - [**2.3.3. User Journey Mapping**](#233-user-journey-mapping)
    - [**2.3.4. Empathy Mapping**](#234-empathy-mapping)
    - [**2.3.5. As-is Scenario Mapping**](#235-as-is-scenario-mapping)
  - [**2.4. Ubiquitous Language**](#24-ubiquitous-language)
- ## [ **Capítulo III: Requirements Specification**](#-capítulo-iii-requirements-specification)
  - [**3.1. To-Be Scenario Mapping**](#31-to-be-scenario-mapping)
    - [**3.1.1. Requisitos Funcionales**](#311-requisitos-funcionales)
    - [**3.1.2. Requisitos No Funcionales**](#312-requisitos-no-funcionales)
    - [**3.1.3. User Stories vs Requisitos Funcionales y No Funcionales**](#313-user-stories-vs-requisitos-funcionales-y-no-funcionales)
  - [**3.2. User Stories**](#32-user-stories)
  - [**3.3. Impact Mapping**](#33-impact-mapping)
  - [**3.4. Product Backlog**](#34-product-backlog)
- [**Conclusiones**](#conclusiones)
- [**Conclusiones y recomendaciones**](#conclusiones-y-recomendaciones)
- [**Video About-the-Team**](#video-about-the-team)
- [**Bibliografía**](#bibliografía)
- [**Anexos**](#anexos)

# Student Outcome

| Criterio específico | Acciones realizadas | Conclusiones |
|----|----|----|
|Actualiza conceptos y conocimientos necesarios para su desarrollo profesional y en especial para su proyecto en soluciones de software.| **Aranda Vallejos, Oscar Gabriel**<br>*TB1*<br> A partir de la etapa del Needfinding pude definir nuestros requisitos funcionales y no funcionales. Estos fueron fundamentales para identificar nuestras historias de usuario y establecer un product backlog consistente. <br>**Chirinos Zúñiga, Rodrigo Manuel**<br>*TB1*<br> Al hacer las preguntas para las entrevistas se pudo mapear las funcionalidades del proyecto y realizar de la mejor manera el product backlog, junto con los requisitos funcionales bien especificados. <br>**Gutierrez Garcia, Jose Eduardo**<br>*TB1*<br>Durante la elaboración del Capítulo 1 (Introducción y análisis de la problemática) y del Capítulo 2 (Especificación de requisitos), profundicé en metodologías de Lean UX, mapeo de impacto y definición de segmentos de usuarios. Me capacité en el uso de herramientas colaborativas (Git, Markdown, GitFlow) y en buenas prácticas de documentación técnica, lo que me permitió estructurar el informe de manera coherente y profesional. Gracias a este proceso, fortalecí mi comprensión de cómo alinear las necesidades del negocio con soluciones de software efectivas. <br>**Silva Morales, Renzo Cesar**<br>*TB1*<br> Mediante el desarrollo de entrevistas logré interpretar las funcionalidades que debería incluir nuestra propuesta y las necesidades del cliente. <br> | TB1: <br> El equipo ha demostrado una actualización efectiva de conceptos y conocimientos clave para el desarrollo de PawFect Care. Al profundizar en metodologías ágiles (Lean UX, mapeo de impacto), herramientas de control de versiones (Git, GitFlow) y documentación técnica ( Markdown), cada miembro fortaleció su base profesional y aportó soluciones más alineadas con las necesidades del proyecto. Esto se traduce en una implementación más sólida, coherente y escalable de la plataforma veterinaria.|


| Criterio específico | Acciones realizadas | Conclusiones |
|----|----|----|
|Reconoce la necesidad del aprendizaje permanente para el desempeño profesional y el desarrollo de proyectos en soluciones de software.| **Aranda Vallejos, Oscar Gabriel**<br>*TB1*<br> Al desarrollar las historias de usuario, identifiqué y reconocí áreas clave para ser implementadas en bounded contexts. Para ello, utilicé el product backlog con el fin de extraer las historias de usuario más relevantes para el core del negocio y visualizar los futuros bounded context en base a sus epics. <br>**Chirinos Zúñiga, Rodrigo Manuel**<br>*TB1*<br> En el desarrollo de esta parte inicial del proyecto el product backlog y los requisitos funcionales y no funcionales fueron lo fundamental para desarrollar el servicio en base a las necesidades de los usuarios. <br>**Gutierrez Garcia, Jose Eduardo**<br>*TB1*<br>Al enfrentar nuevos desafíos—como definir los bounded contexts, redactar user stories y diseñar el backlog—identifiqué áreas donde debía profundizar: gestión de proyectos ágiles, documentación   y diseño de experiencia de usuario. Para ello, consulté tutoriales, documentación oficial y prácticas recomendadas en foros especializados. Este proceso reafirmó mi compromiso con el aprendizaje continuo, indispensable para mantener la calidad y escalabilidad de cualquier solución de software. <br>**Silva Morales, Renzo Cesar**<br>*TB1*<br> Con el análisis de entrevistas pude reconocer otros competidores y factores clave que nos ayudarían a ofrecer un valor agregado superior. <br> | TB1: <br> El proyecto reforzó en todos nosotros la importancia del aprendizaje permanente. Identificamos brechas en áreas como gestión de APIs, diseño UX y despliegue en la nube, y las abordamos mediante investigación, auto‑formación y consulta de fuentes especializadas. Este compromiso con la mejora continua asegura que, más allá de esta entrega, mantendremos la capacidad de adaptarnos a nuevas tecnologías y mejores prácticas en el desarrollo de soluciones de software.|

----

# **Capítulo I: Introducción**

## 1.1. Startup Profile

### 1.1.1. Descripción de la Startup
“Pawfect Care” es una plataforma integral destinada a la gestión veterinaria y a la visualización de historiales clínicos. La idea fundamental detrás de esta plataforma es simplificar y optimizar la administración de diversos aspectos relacionados con el cuidado de las mascotas. Esto incluye la gestión de usuarios, clientes, productos y servicios, así como la organización de historiales clínicos. El objetivo es proporcionar una herramienta que facilite tanto a los propietarios de mascotas como a los veterinarios en el manejo de la información y las tareas diarias.

- **Misión:** Nuestra misión es mejorar la calidad de vida de las mascotas y sus dueños, ofreciendo una plataforma que simplifique la gestión veterinaria y el acceso a la información de salud de las mascotas

- **Visión:** Ser la plataforma líder en la gestión veterinaria, reconocida por su eficiencia, confiabilidad y facilidad de uso.


### 1.1.2. Perfiles de integrantes del equipo

|           Photo                        |                                                                                                                                                                                                                                                                                                    Description                                                                                                                                                                                                                                                                                                    |
| :------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
| Oscar Gabriel Aranda Vallejos <img src="https://i.postimg.cc/6qRCcvNF/Captura-de-pantalla-2024-09-08-151747.png"> | Tengo 20 años y soy estudiante de la carrera de Ingeniería de Software, poseo conocimientos básicos en Unity, C++ y diseño web. Me considero una persona preparada y perseverante en cumplir con los objetivos del proyecto; además, siempre estoy dispuesto a aprender nuevos conceptos.            |
| Rodrigo Chirinos Zúñiga<img src="https://github.com/user-attachments/assets/9895e794-a88f-4436-a332-8d5c8112f9cb" width="200" height="150"> |     Tengo 20 años, soy un estudiante de la carrera de Ingeniería de Software, considero que soy una persona responsable y de escucha activa. Estoy comprometido con mis compañeros en realizar un buen trabajo y así aprender todos en el proceso. También tengo conocimientos en programación en C++, HTML, CSS y JavaScript.      |
| Jose Eduardo Gutierrez Garcia ![C](./assets/chapter01/Josepfp.png) |    Mi Tengo 21 años, actualmente me encuentro cruzando mi 7mo ciclo de la carrera de ingeniería de software en la UPC. Me gusta jugar videojuegos y practicar natación, soy un gran aficionado de la tecnología y del ensamblaje de computadoras. Me considero una persona dispuesta siempre a aprender tecnologías nuevas, creativa y responsable.         |
| Renzo Cesar Silva Morales ![D](./assets/chapter01/Renzopfp.jpg) |  Tengo 20 años y soy estudiante de la carrera de Ingeniería de Software. Me considero un estudiante atento y responsable con los trabajos. Poseo conocimientos en programación en lenguajes como C++, C# y Python. Estoy dispuesto y me comprometo a ayudar al equipo en el proyecto.       |


## 1.2. Solution Profile

Pawfect Care es una aplicación diseñada específicamente para el uso en clínicas veterinarias, enfocada en la gestión interna de todas sus operaciones y en facilitar el acceso a la información clínica para los dueños de las mascotas. Esta aplicación no solo permite a los veterinarios manejar de manera más eficiente y organizada los historiales clínicos de sus pacientes, sino que también ofrece herramientas para gestionar recordatorios, controlar el inventario de productos y realizar otras tareas esenciales para el funcionamiento de la veterinaria. La interfaz de Pawfect Care ha sido diseñada para ser intuitiva y amigable, lo que permite a los veterinarios llevar un control detallado y preciso de cada aspecto de su práctica sin complicaciones. Además, la aplicación proporciona una funcionalidad adicional: la posibilidad de publicar las historias clínicas para que los dueños de las mascotas puedan acceder a ellas cuando lo necesiten. Esto garantiza que los propietarios estén siempre informados sobre el estado de salud de sus mascotas y puedan consultar los detalles médicos en cualquier momento, mejorando así la comunicación y la transparencia entre la clínica y sus clientes.


### 1.2.1. Nombre del Producto

Pawfect Care es el nombre de nuestra plataforma digital, una combinación de las palabras en inglés “paw” (pata) y “perfect” (perfecto), lo que transmite el concepto de “cuidado perfecto para las mascotas”. El nombre refleja el compromiso del producto con la salud, el bienestar y la atención responsable de los animales, a través de una solución tecnológica intuitiva, profesional y centrada tanto en veterinarias como en dueños de mascotas.

### 1.2.2. Antecedentes y problemática

Con la finalidad de poder conocer y comprender con mayor precisión las necesidades de nuestros usuarios, en este caso universitarios, hemos hecho un estudio por medio de la técnica 5w’s & 2H’s. Según el sitio web Rockcontent (2019) 5w’s & 2H’s es una de las metodologías de gestión empresarial más utilizadas. Puede aplicarse en muchos momentos, empresas y proyectos, ayuda a responder una serie de preguntas decisivas para hacer que las acciones de un negocio sean más estratégicas y precisas. Sin más preámbulos, por siguiente mostraremos la información que hemos logrado recopilar por medio de esta técnica.


#### Uso de la técnica The 5'W's w Y 2'H's

| LAS 5W y 2H | Pregunta                                                | Descripción                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| ----------- | ------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| What?        | ¿Cuál es el problema?                                     |      El problema radica en la ausencia de una aplicación que sea tanto intuitiva como fácil de usar en el entorno veterinario, y que, además, permita integrar y gestionar eficazmente los múltiples aspectos que involucra esta práctica                                                                                                           |
| When?       | ¿Cuándo sucede el problema?                                   |           El problema surge cuando las clínicas veterinarias carecen de una aplicación que sea intuitiva y sencilla de usar, lo que dificulta la integración y gestión eficiente de los diversos aspectos necesarios para su funcionamiento diario.                                                                                                                                                                                          |
| Where?       | ¿Dónde sucede el problema?                             |          El problema ocurre en las clínicas veterinarias, donde la falta de una aplicación complica la integración y gestión de las múltiples áreas necesarias para su funcionamiento. Esto no solo afecta a los veterinarios en su labor diaria, sino que también impacta a los dueños de mascotas, quienes necesitan una forma sencilla de acceder a la información y los servicios relacionados con la salud de sus animales.                                                                                                                               |
| Why?      | ¿Por qué sucede el problema?                               |        El problema se debe al desconocimiento de aplicaciones que estén específicamente diseñadas para atender las necesidades complejas y diversas de una clínica veterinaria. Existen muchas aplicaciones pero no son lo suficientemente flexibles o integrales para abarcar todos los campos necesarios, como la gestión de historiales clínicos, el control de inventario, y la comunicación con los dueños de las mascotas. Esto crea dificultades tanto para los veterinarios, que se ven obligados a utilizar múltiples herramientas o procesos manuales, como para los dueños de mascotas, que enfrentan limitaciones en el acceso a la información relevante.                                                                                                                                                                        |
| Who?        | ¿Qué llevara a las personas a usar nuestro producto?                         | Las personas optarán por Pawfect Care debido a la facilidad con la que podrán completar los campos necesarios, la amplia difusión que la aplicación tendrá en redes sociales, y especialmente por lo sencillo que resulta rellenar las historias clínicas sin la complicación de tener que llenar campos obligatorios. |
| How?        | ¿En qué condiciones los clientes usaran nuestro producto?               |                                     Los clientes utilizarán nuestro producto en condiciones donde necesiten una solución eficiente y fácil de usar para gestionar las operaciones de su clínica veterinaria. Esto incluye situaciones en las que buscan una herramienta que simplifique el manejo de historiales clínicos, controle el inventario, y facilite la comunicación con los dueños de las mascotas. Además, lo usarán cuando requieran una aplicación que les permita acceder y compartir información médica de manera rápida y sin complicaciones, especialmente en un entorno donde el tiempo y la precisión son esenciales.                                                                                                                                    |
| How Much?   | ¿Con qué frecuencia o en qué cantidad se utilizará nuestro producto? |                                                           Nuestro producto está diseñado para ser utilizado diariamente por las clínicas veterinarias. El sistema de gestión clínica se utilizará en la mayoría de las interacciones clínicas, desde la admisión de pacientes hasta el seguimiento post-tratamiento. Dado que el acceso a la información clínica y la gestión de citas es una necesidad recurrente, esperamos que el personal utilice la plataforma constantemente a lo largo del día. Además, los dueños de mascotas podrán acceder a la información relevante de sus mascotas, lo que también incentivará un uso frecuente por parte de ellos, especialmente para verificar el historial clínico y programar citas.                                 |


## 1.2.3. Lean UX Process.

#### 1.2.3.1. Lean UX Problem Statements.

La aplicación Pawfect Care busca resolver la necesidad de una herramienta integral que facilite la gestión diaria de las clínicas veterinarias. Al ofrecer una interfaz intuitiva y fácil de usar, la aplicación trata de eliminar las complejidades y dificultades asociadas con la administración de múltiples aspectos de la práctica veterinaria en un solo lugar, permitiendo que tanto veterinarios como propietarios de mascotas tengan acceso rápido y sencillo a la información relevante.

#### 1.2.3.2. Lean UX Assumptions.

Para desarrollar la aplicación Pawfect Care, partimos de varias suposiciones clave que guiarán nuestro proceso de diseño y desarrollo. Estas suposiciones están basadas en una comprensión inicial de las necesidades y problemas de nuestros usuarios objetivo, así como en los resultados esperados para el negocio. A medida que avanzamos en el desarrollo, estas suposiciones se validarán mediante pruebas y retroalimentación continua para asegurar que la solución propuesta cumpla con las expectativas y resuelva eficazmente los desafíos identificados.

**Features:**

- Sistema de gestión de citas para facilitar la organización del tiempo en las clínicas.
- Almacenamiento y visualización de historiales clínicos de las mascotas de forma rápida y segura.
- Notificaciones automáticas para recordatorios de vacunas, tratamientos o revisiones.
- Sección para la venta de productos veterinarios, integrando un catálogo accesible para los clientes.
- Sistema de reportes de ingresos, control de inventario, y análisis de datos para mejorar la eficiencia administrativa.
- Interfaz intuitiva y adaptable para ser utilizada tanto en dispositivos móviles como en computadoras.


**Business Outcomes:**

- Aumento de la eficiencia operativa de las clínicas, reduciendo el tiempo en tareas administrativas.
- Mejora en la satisfacción del cliente, permitiendo un acceso rápido a la información médica de sus mascotas y facilitando la interacción con la clínica.
- Generación de ingresos adicionales a través de suscripciones premium que ofrezcan funciones avanzadas y comisiones por la venta de productos veterinarios.
- Reducción de errores y tiempos de espera en la gestión clínica, lo que aumentará la retención de clientes y atraerá nuevos usuarios.

**Users:**
- **Segmento 1 – Clinicas Veterinarias:** Veterinarias de distintos tamaños, desde consultorios individuales hasta centros de atención con varios especialistas. Este segmento se enfoca en mejorar el manejo de la información médica, el control de inventarios y la programación de citas, con el objetivo de incrementar su eficiencia y brindar un servicio de mayor calidad a sus clientes.

- **Segmento 2 – Dueños de Mascotas:** Propietarios que necesitan gestionar de manera eficiente la salud de sus mascotas, incluyendo jóvenes acostumbrados a usar aplicaciones móviles y también aquellos poco familiarizados con la tecnología. Este segmento busca acceder a una forma más accesible de organizar la información médica de sus animales.

**User Outcomes & Benefits:**

- Reducción de tiempo en la gestión de citas y actualización de historiales médicos.
- Mejor organización en el manejo de inventarios y productos.
- Mejora en la relación con los clientes, ofreciendo un acceso directo a la información de salud de sus mascotas.
- Simplificación en la administración de las clínicas veterinarias, reduciendo errores y tiempos de espera.

**User Assumptions:**

- **¿Quién es el usuario?**
  Los usuarios principales son las clínicas veterinarias y los dueños de mascotas.<br>

- **¿Dónde encaja la aplicación en su vida?**
  La aplicación se integra en la rutina diaria de las clínicas veterinarias y en la vida cotidiana de las mascotas, facilitando su tratamiento y cuidado.<br>

- **¿Qué problemas tienen nuestros usuarios y como se puede resolver?**
  Los usuarios enfrentan la falta de una aplicación especializado para la gestión integral de clínicas veterinarias y la ausencia de un portal donde se pueda acceder fácilmente a la historia clínica de una mascota. Nuestra aplicación resuelve estos problemas proporcionando una plataforma única para administrar todos los aspectos de la clínica y facilitar el acceso a la información médica.<br>

- **¿Dónde y cuándo es usada nuestra aplicación?**
  La aplicación se utiliza principalmente en clínicas veterinarias. Los momentos clave para su uso son durante las consultas veterinarias y cuando los dueños deciden cambiar de veterinario y necesitan trasladar el historial clínico o el registro de vacunas a otro establecimiento.<br>

- **¿Qué características son importantes?**
  Las características esenciales incluyen una interfaz fácil de usar en dispositivos móviles, computadoras y laptops. Además, es crucial la eliminación de campos innecesarios u obligatorios que puedan complicar el proceso de registro.<br>

- **¿Cómo debe verse nuestra aplicación y como debe comportarse?**
 Nuestra aplicación debe tener un diseño funcional y amigable, tanto para veterinarios como para dueños de mascotas. Debe permitir un registro rápido y sencillo de nuevos pacientes y la actualización de historiales clínicos, evitando campos obligatorios que no aporten valor al proceso de registro y atención.<br>

**Business Assumptions**

- Los veterinarios y asistentes están dispuestos a adoptar herramientas digitales si mejoran la eficiencia en sus clínicas.
- Los dueños de mascotas valorarán una aplicación que les permita acceder a la información de salud de sus animales en cualquier momento.
- Las clínicas veterinarias estarán dispuestas a pagar por suscripciones premium o herramientas avanzadas de gestión si aumentan la productividad.
- El mercado de clínicas veterinarias aún utiliza métodos manuales o desactualizados, lo que genera ineficiencias que la aplicación puede resolver.
- Habrá una aceptación de la aplicación tanto por usuarios jóvenes familiarizados con la tecnología como por aquellos menos habituados al uso de herramientas digitales.


#### 1.2.3.3. Lean UX Hypothesis Statements.

Para asegurar que nuestra solución esté alineada con las necesidades y expectativas de nuestros usuarios, hemos formulado las siguientes hipótesis utilizando el enfoque Lean UX. Este enfoque nos permitirá validar nuestras suposiciones a través de iteraciones constantes y ajustes basados en el feedback de los usuarios


**Creemos que** si diseñamos una aplicación intuitiva que permita a los veterinarios gestionar historiales clínicos y recordatorios de manera eficiente.
**Sabremos** que hemos tenido éxito cuando observemos un aumento en la eficiencia operativa y una reducción en el tiempo dedicado a tareas administrativas en las clínicas veterinarias
**cuando** las clínicas adopten nuestra aplicación y reporten mejoras en su flujo de trabajo diario, habremos validado nuestra hipótesis.


**Creemos que** lal ofrecer una plataforma que facilite el acceso a la historia clínica de las mascotas para los dueños
**Sabremos** que nuestra solución es efectiva cuando recibamos comentarios positivos de los usuarios sobre la facilidad de acceso y la utilidad de la información médica compartida
**cuando** los dueños de mascotas utilicen la aplicación para consultar y manejar la salud de sus animales sin problemas, habremos confirmado que estamos resolviendo una necesidad real.


**Creemos que** que si eliminamos los campos obligatorios innecesarios y simplificamos el proceso de registro en la aplicación.
**Sabremos** que hemos logrado nuestro objetivo cuando los usuarios experimenten una mayor satisfacción y una reducción en los errores de entrada de datos.
**cuando** tanto veterinarios como propietarios de mascotas reporten una experiencia de usuario fluida y sin frustraciones, habremos validado que nuestra aplicación cumple con las expectativas de simplicidad y funcionalidad..


#### 1.2.3.4. Lean UX Canvas

<table border="1" cellpadding="10" cellspacing="0">
    <tr>
        <td><strong>Lean UX Canvas</strong></td>
        <td><strong>Fecha:</strong> 18/04/2025</td>
        <td><strong>Primera Iteración</strong></td>
    </tr>
    <tr>
        <td>
            <strong>Business Problem</strong><br>
            La gestión de clínicas veterinarias enfrenta desafíos significativos debido al uso de métodos manuales o sistemas desactualizados, lo que resulta en ineficiencias operativas, errores en la documentación y una experiencia insatisfactoria tanto para los veterinarios como para los propietarios de mascotas. La falta de una herramienta integral complica la administración de citas, historiales clínicos y la venta de productos veterinarios.
        </td>
        <td>
            <strong>Solutions</strong><br>
            - Gestión de citas.<br>
            - Almacenamiento y visualización de historiales clínicos.<br>
            - Notificaciones automáticas para recordatorios de vacunas y tratamientos.<br>
            - Venta de productos veterinarios.<br>
            - Reportes de ingresos y control de inventario.
        </td>
        <td>
            <strong>Business Outcomes</strong><br>
            - Incremento de la eficiencia operativa en las clínicas veterinarias.<br>
            - Mejora en la satisfacción del cliente con acceso rápido a la información médica.<br>
            - Generación de ingresos adicionales a través de suscripciones premium y ventas de productos.<br>
            - Reducción de errores y tiempos de espera en la gestión clínica.
        </td>
    </tr>
    <tr>
        <td>
            <strong>Users</strong><br>
            - <strong>Segmento 1 – Clinicas Veterinarias:</strong> Clínicas de diferentes tamaños que necesitan mejorar la gestión de información médica, citas e inventarios.<br>
            - <strong>Segmento 2 – Dueños de Mascotas:</strong> Propietarios que buscan una forma eficiente de gestionar la salud de sus mascotas y acceder a la información médica de manera digital.
        </td>
        <td>
            <strong>Hypotheses</strong><br>
            - Creemos que diseñar una aplicación intuitiva para veterinarios mejorará la eficiencia en la gestión clínica.<br>
            - Sabemos que hemos tenido éxito cuando observamos una mejora en la eficiencia operativa y una reducción en el tiempo dedicado a tareas administrativas.<br>
            - Creemos que una plataforma que facilite el acceso a la historia clínica para los dueños será bien recibida.<br>
            - Sabemos que nuestra solución es efectiva cuando recibimos comentarios positivos sobre la facilidad de acceso a la información médica.<br>
            - Creemos que simplificar el proceso de registro eliminará campos innecesarios y mejorará la experiencia del usuario.<br>
            - Sabemos que hemos logrado nuestro objetivo cuando reportan una experiencia de usuario fluida y sin frustraciones.
        </td>
        <td>
            <strong>User Outcomes & Benefits</strong><br>
            - Reducción del tiempo en la gestión de citas y actualización de historiales.<br>
            - Mejor organización en inventarios y productos.<br>
            - Mejora en la relación con los clientes mediante acceso directo a la información médica.<br>
            - Simplificación en la administración de las clínicas, reduciendo errores y tiempos de espera.
        </td>
    </tr>
    <tr>
        <td>
            <strong>What's the most important thing we need to learn first?</strong><br>
            Validar si la aplicación realmente mejora la eficiencia operativa de las clínicas veterinarias y facilita el acceso a la información médica para los dueños de mascotas.
        </td>
        <td colspan="2">
            <strong>What's the least amount of work we need to do to learn the next most important?</strong><br>
            Desarrollar un prototipo funcional que permita a un grupo selecto de usuarios (veterinarios y propietarios de mascotas) probar las características clave de la aplicación y proporcionar retroalimentación sobre su efectividad en la mejora de la eficiencia y la satisfacción del usuario.
        </td>
    </tr>
</table>

## 1.3. Segmentos objetivo.

Para asegurar el éxito de Pawfect Care, hemos identificado dos segmentos clave que serán el foco principal de nuestras estrategias de desarrollo y marketing. Estos segmentos representan a nuestros usuarios ideales y nos permitirán adaptar nuestras funcionalidades y servicios a sus necesidades específicas, maximizando así el impacto de la plataforma.

**Segmento Objetivo 1 - Clínicas Veterinarias**

El primer segmento objetivo incluye a las clínicas veterinarias de diversos tamaños, desde pequeñas clínicas independientes hasta grandes centros especializados con múltiples profesionales. Pawfect Care les ofrece una plataforma que simplifica la gestión interna de sus operaciones, permitiendo una mayor eficiencia en la programación de citas, gestión de historiales médicos y la comunicación con los dueños de las mascotas. Estas clínicas buscan una herramienta que facilite el acceso a información clínica y mejore la administración de sus recursos, todo bajo una interfaz intuitiva y accesible. El valor de Pawfect Care radica en su capacidad para optimizar procesos, lo que se traduce en un mejor servicio y atención para los animales.

**Segmento Objetivo 2 - Dueño de Mascotas:**

El segundo segmento está compuesto por los dueños de mascotas, quienes son responsables del bienestar y la salud de sus animales. Este grupo de usuarios busca soluciones prácticas que les permitan manejar de manera eficiente la salud de sus mascotas, incluyendo la programación de citas, acceso a historiales médicos y recordatorios de vacunación. Pawfect Care les proporciona una plataforma que centraliza toda esta información y facilita el acceso desde cualquier dispositivo, brindándoles tranquilidad y control sobre el cuidado de sus animales. La conveniencia y facilidad de uso son elementos clave para este segmento, que espera una experiencia fluida y personalizada.

---


# **Capítulo II: Requirements Elicitation & Analysis**

## 2.1. Competidores.

<table>
    <thead>
        <tr>
            <th>Nombre</th>
            <th>Descripción</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td rowspan align="center">VetPraxis<img src="https://i.postimg.cc/8cHpQXqN/vetpraxis.png" alt="VetPraxis Logo" style="width: 250px; height: auto;" </td>
            <td>Es una solución de gestión para clínicas veterinarias, diseñada para optimizar la administración de operaciones diarias. Ofrece funcionalidades que incluyen la gestión de citas, historias clínicas electrónicas, administración de inventario, y facturación. También proporciona herramientas para la comunicación con los clientes y el seguimiento de tratamientos.<br>
            Página web:<a href="https://vetpraxis.net/"> https://vetpraxis.net/</a>
        </tr>
        <tr>
            <td align="center">VetApp<img src="https://i.postimg.cc/RFx43zmv/vetapp.jpg"alt="VetApp Logo" style="width: 700px; height: auto;"</td>
            <td> Es una plataforma desarrollada para la gestión de clínicas veterinarias. Proporciona características como la programación de citas, el manejo de historias clínicas electrónicas, y la administración de inventario.<br>
            Página web:<a href="https://vetapp.app/en"> https://vetapp.app/en</a>
        </tr>
        <tr>
           <td rowspan align="center">PetClinic<br><img src="https://i.postimg.cc/fRgbRFkb/petclinic.jpg"alt="PetClinic Logo" style="width: 250px; height: auto;"</td> 
           <td>Es una aplicación diseñada para gestionar clínicas veterinarias y consultas de mascotas. Incluye funciones para la gestión de citas, el manejo de historias clínicas electrónicas, y la administración de inventario y facturación. La plataforma está orientada a mejorar la organización y eficiencia dentro de las clínicas, ofreciendo herramientas para el seguimiento de tratamientos y la comunicación con los clientes. PetClinic está adaptada a las necesidades específicas del sector veterinario en Perú.<br>
           Página web:<a href="https://petclinic.es/"> https://petclinic.es/</a>
    </tbody>
</table>

### 2.1.1. Análisis competitivo.
<table style="width: 100%;">
  <tr>
    <th colspan="6" style="padding: 8px; text-align: center;"> Competitive Analysis Landscape</th>
  </tr>
  <tr>
    <td>¿Por qué llevar a cabo este análisis?</td>
    <td colspan="5">Para comparar las características tanto internas como externas de los productos que compiten con nosotros.</td>
  </tr>
  <tr>
    <td colspan="2"></td>
    <td align="center">Pawfect Care<br><img src="https://i.postimg.cc/2ymktN90/pawfect.png" alt="Pawfect Logo"></td>
    <td align="center">VetPraxis<br><img src="https://i.postimg.cc/8cHpQXqN/vetpraxis.png" alt="VetPraxis Logo"></td>
    <td align="center">VetApp<br><img src="https://i.postimg.cc/RFx43zmv/vetapp.jpg"alt="VetApp Logo"></td>
    <td align="center">PetClinic<br><img src="https://i.postimg.cc/fRgbRFkb/petclinic.jpg"alt="PetClinic Logo"></td> 
  </tr>
  <tr>
    <td rowspan="2" align="center">Perfil</td>
    <td align="center">Overview</td>
    <td>
    Plataforma para clínicas veterinarias que simplifica la gestión de historiales clínicos, recordatorios e inventarios con una interfaz fácil de usar.</td>
    <td>Software de gestión veterinaria que optimiza citas, historiales clínicos y facturación con una interfaz amigable.</td>
    <td>Aplicación móvil para gestionar citas, recordatorios, historiales médicos de mascotas, facilitando la comunicación entre veterinarios y propietarios.</td>
    <td>Plataforma que integra administración de historiales clínicos, citas e inventario para mejorar la eficiencia en clínicas veterinarias.</td>
  </tr>
  <tr>
    <td>Ventaja competitiva<br>¿Qué valor ofrece a los clientes?</td>
    <td>Interfaz intuitiva que facilita la gestión de historiales, recordatorios e inventario.</td>
    <td>Gestión integral de citas, historiales y facturación con una interfaz amigable.</td>
    <td>Gestión móvil de citas e historiales médicos que mejora la comunicación entre veterinarios y propietarios.</td>
    <td>Plataforma única para administrar historiales, citas e inventario en clínicas veterinarias.</td>
  </tr>
  <tr>
    <td rowspan="2" align="center">Perfil de Marketing</td>
    <td>Mercado objetivo</td>
    <td>
    Clínicas veterinarias y dueños de mascotas.</td>
    <td>Clínicas veterinarias medianas y grandes.</td>
    <td>Propietarios de mascotas y veterinarios móviles.</td>
    <td>Clínicas veterinarias pequeñas y medianas.</td>
  </tr>
  <tr>
    <td>Estrategias de marketing</td>
    <td>Redes sociales y colaboraciones con clínicas.</td>
    <td>Marketing de contenido y webinars.</td>
    <td>Redes sociales.</td>
    <td>Publicidad dirigida y promociones.</td>
  </tr>
  <tr>
    <td rowspan="3" align="center">Perfil del Producto</td>
    <td>Productos & Servicios</td>
    <td>Gestión de historiales clínicos, recordatorios e inventarios.</td>
    <td>Gestión de citas, historiales clínicos y facturación.</td>
    <td>Aplicación móvil para gestionar citas e historiales médicos.</td>
    <td>Plataforma de administración de historiales, citas e inventario.</td>
  </tr>
  <tr>
    <td>Precios & Costos</td>
    <td>Suscripción mensual con diferentes niveles.</td>
    <td>Licencia de software con tarifas anuales.</td>
    <td>Descarga gratuita con compras dentro de la app.</td>
    <td>Suscripción con tarifas basadas en el tamaño de la clínica.</td>
  </tr>
  <tr>
    <td>Canales de distribución (Web y/o Móvil)</td>
    <td>Web y móvil.</td>
    <td>Web.</td>
    <td>Móvil (App stores)</td>
    <td>Web.</td>
  </tr>
  <tr>
    <td rowspan="4" align="center">Análisis SWOT</td>
    <td>Fortalezas</td>
    <td>Interfaz intuitiva y fácil de usar; integración de múltiples funciones.</td>
    <td>Gestión integral y amigable; adaptado para clínicas medianas y grandes.</td>
    <td>Acceso móvil conveniente; mejora la comunicación con propietarios de mascotas.</td>
    <td>Plataforma integral para clínicas pequeñas y medianas; fácil de usa.</td>
  </tr>
  <tr>
    <td>Debilidades</td>
    <td>Dependencia de la adopción por parte de clínicas veterinarias.</td>
    <td>Costos potencialmente altos para pequeñas clínicas.</td>
    <td>Funcionalidades limitadas comparadas con plataformas completas.</td>
    <td>Limitado a clínicas de menor tamaño; menos atractivo para grandes clínicas.</td>
  </tr>
  <tr>
    <td>Oportunidades</td>
    <td>
    Expansión en el mercado de clínicas veterinarias pequeñas y medianas.</td>
    <td>Crecimiento en el segmento de clínicas grandes y asociaciones veterinarias.</td>
    <td>Expansión en el mercado de usuarios móviles y propietarios de mascotas.</td>
    <td>Penetración en el mercado de clínicas veterinarias pequeñas</td>
  </tr>
  <tr>
    <td>Amenazas</td>
    <td>Competencia de otras plataformas con características similares.</td>
    <td>Competencia con soluciones de bajo costo o gratuitas.</td>
    <td>Alta competencia en aplicaciones móviles para la salud de mascotas.</td>
    <td>Competencia de soluciones más avanzadas para clínicas grandes.</td>
  </tr>
<table>

### 2.1.2. Estrategias y tácticas frente a competidores.
<strong> Estrategias:</strong><br>
- <strong>Interfaz Intuitiva y Fácil de Usar:</strong> Pawfect Care se diferenciará por su interfaz amigable y fácil de usar, lo que simplifica la gestión diaria para los veterinarios y dueños de mascotas. Esto contrasta con muchas soluciones existentes que pueden ser complicadas o difíciles de navegar.
- <strong>Características Exclusivas:</strong> La aplicación ofrecerá características únicas como la personalización de historiales clínicos y recordatorios adaptados a las necesidades específicas de cada clínica y propietario de mascotas, lo cual no está comúnmente disponible en otras plataformas.
- <strong>Valor Agregado:</strong> Se enfocará en agregar valor a través de un sistema integral que combina gestión de citas, control de inventarios, notificaciones automáticas y una sección para la venta de productos veterinarios, abordando múltiples necesidades en una sola plataforma.
- <strong>Adaptabilidad: </strong>Pawfect Care se adaptará a diferentes tamaños de clínicas y será accesible tanto en dispositivos móviles como en computadoras, lo que la convierte en una solución flexible para diversas necesidades.

<strong>Tácticas: </strong><br>
- <strong>Demostraciones Personalizadas:</strong> Se organizarán demostraciones en vivo en clínicas veterinarias para mostrar de manera práctica cómo la plataforma mejora la eficiencia y facilita la gestión clínica. Estas demostraciones permitirán a los clientes potenciales experimentar la funcionalidad de Pawfect Care en su entorno de trabajo.
- <strong>Períodos de Prueba Gratuita:</strong> Se ofrecerán períodos de prueba gratuita para que las clínicas puedan experimentar los beneficios de la aplicación sin compromiso. Esto permitirá a los usuarios evaluar la utilidad y el impacto de la plataforma en su operación diaria.
- <strong>Testimonios y Casos de Éxito:</strong> Se recopilarán y publicarán testimonios y casos de éxito de usuarios satisfechos que hayan experimentado mejoras significativas en su gestión veterinaria. Estos testimonios se utilizarán en campañas de marketing, en el sitio web de la aplicación y en materiales promocionales para construir credibilidad y atraer nuevos clientes.
-<strong> Soporte Proactivo y Capacitación:</strong> Se proporcionará soporte proactivo y capacitación personalizada para ayudar a las clínicas a integrar la plataforma de manera eficiente. Esto asegurará que los usuarios obtengan el máximo provecho de las características avanzadas y reduzcan el tiempo de adaptación.
- <strong>Optimización Continua:</strong> Se implementará un proceso de retroalimentación continua para identificar áreas de mejora y responder rápidamente a las necesidades cambiantes del mercado. Esto permitirá a Pawfect Care mantenerse a la vanguardia y adaptarse a nuevas tendencias y demandas.
- <strong>Partnerships Estratégicos:</strong> Se explorarán asociaciones estratégicas con proveedores de productos veterinarios y organizaciones de salud animal para ampliar la red de distribución y aumentar la visibilidad de la plataforma.


## 2.2. Entrevistas.

El objetivo de las entrevistas es obtener una comprensión profunda de las experiencias, perspectivas y opiniones de los segmentos de mercado seleccionados. Nuestra meta es recopilar información valiosa que nos permita entender mejor a nuestro público objetivo y mejorar nuestra comprensión de los usuarios. Estas conversaciones nos proporcionarán una visión más clara de las necesidades y deseos de nuestros usuarios, lo que nos ayudará a adaptar nuestros productos o servicios de manera más efectiva a sus requisitos.

### 2.2.1. Diseño de entrevistas.

En esta parte, se han formulado varias preguntas destinadas a nuestros segmentos de interés con el fin de obtener información cualitativa, como opiniones o descripciones. Esta información será crucial para el desarrollo de nuestra solución.

<strong>Breve descripción de nuestra aplicación</strong>

RideFind es una plataforma que facilita el alquiler de vehículos alternativos y sostenibles, como autos eléctricos, motos eléctricas, scooters y bicicletas. Nuestra misión es ofrecer una solución de transporte eficiente, ecológica y accesible, ayudando a reducir la congestión vehicular y la contaminación en las ciudades. Ya sea que necesites un medio de transporte flexible y rápido, o que quieras alquilar un vehículo que no utilizas con frecuencia para obtener ingresos adicionales, RideFind está diseñada para satisfacer esas necesidades de manera segura y conveniente.


**Preguntas Generales:**

- ¿Cuál es tu nombre?
- ¿Cuántos años tienes?
- ¿Donde resides?
- ¿Cuál es tu ocupación?

**Preguntas para el Segmento Objetivo 1 - Clinicas Veterinarias:**

- ¿Conoces alguna aplicación de gestión veterinaria? ¿Cuál es?
- ¿Lo escogieron por alguna razón es especial?
- ¿Fue la primera aplicación que usaron?
- ¿Qué es lo que te gusta de esa aplicación?
- ¿Qué te disgusta de esa aplicación?
- ¿Qué sería una de las cosas que si o si cambiarias?


**Preguntas para el Segmento Objetivo 2 - Dueños de Mascotas:**


- ¿Con que frecuencia lleva a su mascota al veterinario?
- ¿Qué método usas para llevar el control de tu mascota?
- ¿Alguna vez perdiste los documentos?
- ¿En medio de algún tratamiento cambiaste de veterinario?
- ¿Qué opinas de tener la historia clínica en una aplicación?
- ¿Usarías una aplicación como la descrita?


### 2.2.2. Registro de entrevistas.

**Entrevista para el Segmento Objetivo 1 - Clinicas Veterinarias:**

---

Entrevista N°1:

**Entrevistado:** Elvia Garcia<br>
**Sexo:** Femenino <br>
**Edad:** 44 años<br>
**Domicilio:** Magdalena del Mar<br>
**Inicio de la Entrevista:** 0:09<br>
**Duración de la Entrevista:** 3:44<br>

<img src="./assets/Chapter02/entrevista-elvia.png" alt="Entrevista con Nasthya" style="width: 600px; height: auto;"><br>

**Enlace:** [`https://upcedupe-my.sharepoint.com/:v:/g/personal/u202221518_upc_edu_pe/EYevHRw9GQ5PmnarGePq9lsB9kIXpRvegYORyQnQLeUsQg?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=wTtOfn`](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202221518_upc_edu_pe/EYevHRw9GQ5PmnarGePq9lsB9kIXpRvegYORyQnQLeUsQg?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=wTtOfn)

**Resumen de la Entrevista:** <br>
La Doctora Elvia García, médico veterinaria con 20 años de experiencia, actualmente trabaja en una clínica donde utilizan la aplicación VetPraxis para la gestión veterinaria. Eligieron esta herramienta por ser una de las más reconocidas en el mercado y por las buenas referencias que recibieron. Valora que la plataforma permite tener un historial clínico bien organizado y accesible, además de facilitar la programación de citas y el seguimiento de tratamientos. Sin embargo, Elvia señala como una gran desventaja la cantidad excesiva de campos obligatorios en los formularios, muchos de los cuales considera innecesarios, como el RUC del cliente o sus redes sociales. Esto complica la atención en situaciones de emergencia, donde se necesita rapidez. Como mejora clave, propone reducir o eliminar estos campos para hacer el sistema más ágil y funcional en el día a día.

---

Entrevista N°2:

**Entrevistado:** Carlos <br>
**Sexo:** Masculino <br>
**Edad:** 30 años<br>
**Domicilio:** San Martín de Porres <br>
**Inicio de la Entrevista:** 0:00<br>
**Duración de la Entrevista:** 4:44<br>

[![image.png](https://i.postimg.cc/6qhMgd0d/image.png)](https://postimg.cc/BPX51PR6)

**Enlace:** [`https://upcedupe-my.sharepoint.com/:v:/g/personal/u20221c362_upc_edu_pe/EenhPQh7QtNJv8TMRTHvYP0BzjPaqB_rTUv0wqjPt7JQIQ?e=FNTg1h&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D`](https://upcedupe-my.sharepoint.com/:v:/g/personal/u20221c362_upc_edu_pe/EenhPQh7QtNJv8TMRTHvYP0BzjPaqB_rTUv0wqjPt7JQIQ?e=FNTg1h&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)

**Resumen de la Entrevista:** <br>
El Doctor Carlos menciona que en su lugar de trabajo utilizan VetPraxis, principalmente por ser una aplicación ampliamente conocida y adoptada por muchas clínicas veterinarias. No obstante, destaca que presenta algunas limitaciones, sobre todo en términos de eficiencia. Una de sus principales observaciones es la presencia de numerosos campos obligatorios que, desde su perspectiva, no son necesarios. Esto provoca que la elaboración de historias clínicas tome aproximadamente 5 minutos, lo cual resulta problemático, especialmente en contextos de urgencia donde se requiere actuar con rapidez. Por su parte, subraya que una de las modificaciones que haría con mayor urgencia sería eliminar estos campos innecesarios, con el fin de optimizar el proceso y mejorar el desempeño de la aplicación.

---

Entrevista N°3:

**Entrevistado:** Carlos Ventura <br>
**Sexo:** Masculino <br>
**Edad:** 38 años<br>
**Domicilio:** Lima <br>
**Inicio de la Entrevista:** 0:00<br>
**Duración de la Entrevista:** 2:49<br>

[![image.png](https://i.postimg.cc/J7YGL53T/image.png)](https://postimg.cc/fkXw7XrX)

**Enlace:** [`https://upcedupe-my.sharepoint.com/:v:/g/personal/u20221c362_upc_edu_pe/EVHJf-z0S_xLmFGdEM4xjqgBlsb3F-q3hD-1zjTQ1UHpLA?e=kZdvhS&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D`](https://upcedupe-my.sharepoint.com/:v:/g/personal/u20221c362_upc_edu_pe/EVHJf-z0S_xLmFGdEM4xjqgBlsb3F-q3hD-1zjTQ1UHpLA?e=kZdvhS&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)

**Resumen de la Entrevista:** <br>
El Dr. Carlos Ventura, médico veterinario de 38 años residente en Lima, Perú, trabaja en una clínica especializada en animales pequeños. Actualmente utiliza la aplicación VetClinic Manager para la gestión veterinaria, principalmente por su capacidad de almacenar historiales médicos digitalmente. Antes de usar esta app, probó herramientas como Excel y agendas físicas, pero estas se volvieron poco prácticas con el crecimiento de su clientela. Lo que más valora de VetClinic Manager es que centraliza el historial clínico, la agenda de citas y la facturación. Sin embargo, critica que el sistema es lento, confuso en ciertas áreas y carece de una interfaz amigable. Como mejora principal, propondría una interfaz más limpia, con accesos más rápidos a información clave, y una mejor gestión del inventario.

---

<br>

**Entrevista para el Segmento Objetivo 2 - Dueños de Mascotas:**

---
Entrevista N°1:

**Entrevistado:** Ana <br>
**Sexo:** Femenino <br>
**Edad:** 55 años<br>
**Domicilio:** Puente Piedra <br>
**Inicio de la Entrevista:** 0:00<br>
**Duración de la Entrevista:** 2:20<br>

[![entrevista-ana.png](https://i.postimg.cc/025jhjYD/entrevista-ana.png)](https://postimg.cc/z3MqgJPG)

**Enlace:** [`https://upcedupe-my.sharepoint.com/:v:/g/personal/u202217804_upc_edu_pe/EW0OxQboN91CuWYKpGd_4MwBlAsR0SZe-MXv2JYI9tr2sA?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=hOaFtS`](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202217804_upc_edu_pe/EW0OxQboN91CuWYKpGd_4MwBlAsR0SZe-MXv2JYI9tr2sA?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=hOaFtS)

**Resumen de la Entrevista:** <br>
 Ana nos comenta que lleva a su mascota al veterinario cada vez que nota algún comportamiento raro en su mascota o cuando lo ve enfermo. Explica que siempre lleva los documentos que le da el veterinario, como su tarjeta de vacunas o chequeos, aunque ha habido el caso donde ha perdido dichos documentos. Ella considera que una aplicación que le permita ver la historia clínica sería excelente porque toda la información lo tendría en su pc o laptop y podría ingresar a revisar desde cualquier navegador. 

---

Entrevista N°2:

**Entrevistado:** Diego <br>
**Sexo:** Masculino <br>
**Edad:** 20 años<br>
**Domicilio:** San Miguel <br>
**Inicio de la Entrevista:** 0:00<br>
**Duración de la Entrevista:** 3:25<br>

[![image.png](https://i.postimg.cc/ZRsk2z5b/image.png)](https://postimg.cc/R6tbJ8ty)

**Enlace:** [`https://upcedupe-my.sharepoint.com/:v:/g/personal/u20221c362_upc_edu_pe/Ee5rXgJAqnREmSoDnOD-WfUBGOscyXbOLMpNCqAw-zoysg?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=SSRBR3`](https://upcedupe-my.sharepoint.com/:v:/g/personal/u20221c362_upc_edu_pe/Ee5rXgJAqnREmSoDnOD-WfUBGOscyXbOLMpNCqAw-zoysg?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=SSRBR3)

**Resumen de la Entrevista:** <br>
 Diego es un estudiantes de 20 años que solo lleva a su mascota al veterinario cada vez que necesita bañarlo, ya que menciona que su mascota no se suele enfermar. Además, menciona que usa una cartilla física para llevar el control de su mascota. Por otro lado, explica que jamás a perdido la cartilla de control de su mascota, y que nunca ha cambiado de veterinario. Él considera que tener una app para ver la historia clínica de su mascota sería excelente, ya que podría ver toda la información desde su celular.

---

Entrevista N°3:

**Entrevistado:** Sergio <br>
**Sexo:** Masculino <br>
**Edad:** 20 años<br>
**Domicilio:** Comas <br>
**Inicio de la Entrevista:** 0:00<br>
**Duración de la Entrevista:** 4:11<br>

[![Captura-de-pantalla-2025-04-18-232019.png](https://i.postimg.cc/k4DsmRv9/Captura-de-pantalla-2025-04-18-232019.png)](https://postimg.cc/DJkLQZNY)

**Enlace:** [`https://upcedupe-my.sharepoint.com/:v:/g/personal/u202218167_upc_edu_pe/ESaf-2VJ0zJGpLnNv2DsVwsBl6m8PtmuTuQSefq_dH90YQ?e=lp9DhQ`](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202218167_upc_edu_pe/ESaf-2VJ0zJGpLnNv2DsVwsBl6m8PtmuTuQSefq_dH90YQ?e=lp9DhQ)

**Resumen de la Entrevista:**<br>

Sergio es un estudiante de 20 años que acude al veterinario con su mascota para hacerle revisiones generales y control de vacunas cada 4 meses. Además, se menciona que debe utilizar una aplicación de block de notas en su celular para anotar fechas de citas importantes y que en raras ocasiones suele perder documentos de vacunación importantes. Él considera que una aplicación sería vital para gestionar de manera eficiente todos los documentos relacionados a su mascota y no volver a perder algún registro que podría necesitar más adelante.


### 2.2.3. Análisis de entrevistas.

***Segmento 1:  Clinicas Veterinarias***

- El 100% de los entrevistados utilizan software de gestión en sus clínicas veterinarias. Dos de ellos (66.7%) emplean VetPraxis debido a su reconocimiento en el mercado, mientras que uno (33.3%) utiliza otro software específico para veterinarias.
- El 100% de los veterinarios expresaron preocupaciones sobre el tiempo que toma completar las historias clínicas. El 66.7% de ellos reportaron que el proceso puede tomar entre 7 y 15 minutos, lo cual consideran excesivo. Esto destaca la necesidad de soluciones más eficientes.
- El 100% de los entrevistados mencionaron insatisfacción con la eficiencia del software que utilizan. Todos ellos señalaron la presencia de campos innecesarios que complican el proceso de creación de historias clínicas.
- El 33.3% de los entrevistados aprecian que el software esté adaptado a las necesidades específicas de las veterinarias, con campos diseñados para cada especie o raza. Sin embargo, incluso en estos casos, la eficiencia sigue siendo una preocupación.

***Segmento 2: Dueños de Mascotas***

- El 50% de los entrevistados lleva a sus mascotas al veterinario entre una y dos veces al año, generalmente por chequeos rutinarios o situaciones de salud menores. El otro 50% visita al veterinario con mayor regularidad, cada tres meses para una gata y una vez al mes para bañar a su perra. Esto sugiere que el uso de servicios veterinarios puede variar considerablemente según las necesidades específicas de la mascota. 
- Todos los entrevistados tienen dificultades para mantener organizados los documentos médicos de sus mascotas. Uno de los participantes no recuerda dónde guardó la carpeta con la documentación médica, mientras que otro ha perdido documentos importantes como cartillas de vacunación y exámenes. 
- El 66.7% de los entrevistados ha cambiado de veterinario alguna vez, lo que ha generado confusión sobre los productos o medicamentos utilizados en sus mascotas.
## 2.3. Needfinding.

El Needfinding es una metodología cualitativa centrada en captar las opiniones y sentimientos de los usuarios. Su propósito, como su nombre sugiere, es identificar, explorar, analizar, descubrir, y valorar de manera sencilla las necesidades que pueden dirigir y orientar el desarrollo y diseño de cualquier proyecto.

En este proyecto, hemos optado por interactuar con posibles usuarios a través de entrevistas y cuestionarios. A continuación, se presentan diversos análisis derivados de estas entrevistas en los siguientes artefactos.

### 2.3.1. User Personas.

- **Segmento Objetivo 1 - Clinicas Veterinarias**

[![user-Persona1.png](https://i.postimg.cc/8zy7rcXN/user-Persona1.png)](https://postimg.cc/VJCfxfcV)

- **Segmento Objetivo 2 - Dueños de Mascotas**

[![user-Persona2.png](https://i.postimg.cc/x8S8Sz8y/user-Persona2.png)](https://postimg.cc/KkJxP4nR)


### 2.3.2. User Task Matrix.

***Segmento 1: Clinicas Veterinarias***

|**Vanesa Gómez Suarez**|||
| :-: | :- | :- |
|**Actividades**|**Frecuencia**|**Importancia**|
|Elaborar y mantener actualizadas las historias clínicas de los pacientes.|Alta|Alta|
|Rellenar los campos requeridos en el software.|Alta|Alta|
|Acceder y buscar los registros médicos de las mascotas.|Alta|Alta|
|Programar y administrar citas veterinarias.|Media|Alta|
|Guardar y organizar los documentos médicos.|Media|Media|
|Solucionar problemas relacionados con la legibilidad y el extravío de documentos.|Media|Alta|
|Optimizar la eficiencia en el proceso de documentación.|Media|Alta|
|<p>Atender a los clientes de forma rápida y eficiente.</p><p></p>|Alta|Alta|

***Segmento 2: Dueños de Mascotas***

|**Lucerito Guzmán León**|||
| :-: | :- | :- |
|**Actividades**|**Frecuencia**|**Importancia**|
|Llevar a sus mascotas al veterinario.|Alta|Alta|
|Agendar y administrar citas veterinarias.|Alta|Alta|
|Mantener y ordenar la documentación médica de sus mascotas.|Alta|Alta|
|Consultar los historiales clínicos de sus mascotas.|Media|Alta|
|Cambiar de veterinario cuando sea necesario.|Baja|Media|
|Responder rápidamente ante emergencias médicas.|Media|Alta|
|Guardar y respaldar la información médica en formatos digital y físico.|Alta|Alta|
---


### 2.3.3. Empathy Mapping.

- **Primer segmento: Clinicas Veterinarias**
[![Empathy-Map1.png](https://i.postimg.cc/mZM16bky/Empathy-Map1.png)](https://postimg.cc/jCxjDYzD)

- **Segundo segmento: Dueños de Mascotas**
[![Empathy-Map2.png](https://i.postimg.cc/L6pYcrZK/Empathy-Map2.png)](https://postimg.cc/Z0w53scV)

### 2.3.4. As-is Scenario Mapping.

- **Primer segmento: Clinicas Veterinarias**
[![Asis1.jpg](https://i.postimg.cc/fR59jBy4/Asis1.jpg)](https://postimg.cc/Sn2RmLcV)

- **Segundo segmento: Dueños de Mascotas**
[![Asis2.jpg](https://i.postimg.cc/kgP6dL6P/Asis2.jpg)](https://postimg.cc/qzQMsbx1)


---

# Capítulo III: Requirements Specification

## 3.1. To-Be Scenario Mapping.

- **Primer segmento: Clinicas Veterinarias**

<br><img src="./assets/Chapter03/Tobe1.jpeg" alt="To Be Scenario Map 1" style="width: 1000px; height: auto;" ><br>

- **Segundo segmento: Dueños de Mascotas**

<br><img src="./assets/Chapter03/Tobe2.jpeg" alt="To Be Scenario Map 2" style="width: 1000px; height: auto;" ><br>


## 3.1.1. Requisitos Funcionales

### Gestión de Usuarios y Clientes
- **RF01.** El sistema debe permitir a los dueños de las mascotas y a los veterinarios registrarse en la plataforma. Para ello se requiere que ingresen su nombre completo, teléfono, correo electrónico, dirección y contraseña. Además, si el usuario es un médico veterinario se le pedirá ingresar el tipo de servicio que ofrece.
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
| US20          | Actualización del Historial Médico | Como doctor veterinario, deseo actualizar el historial médico de las mascotas para que los dueños tengan la información más reciente sobre sus tratamientos. |

---

# Reviews y Feedback
**EP06: Como usuario dueño de una mascota, deseo poder dejar reseñas y comentarios sobre un doctor veterinario.**

| User Story ID | Título                     | Descripción                                                                                                                                                    |
|---------------|----------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| US21          | Publicar Reseñas | Como usuario dueño de una mascota, deseo dejar una reseña sobre un doctor veterinario para compartir mi experiencia con otros usuarios.                   |
| US22          | Visualización de Reseñas | Como dueño de una mascota, deseo ver las reseñas de otros usuarios sobre un doctor veterinario para conocer la calidad del servicio y su calificación general. |

---

# Gestión de Servicios y Tarifas
**EP07: Como médico veterinario, deseo ingresar tarifas por los servicios requeridos por un dueño de mascota para que él pueda conocer los precios que le ofrezco.**

| User Story ID | Título                           | Descripción                                                                                                                                                                  |
|---------------|----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| US23          | Ofrecer tarifa por servicio      | Como médico veterinario, deseo ofrecer una tarifa personalizada para un servicio solicitado por un dueño de mascota mediante una cita, para que él pueda evaluar mi propuesta. |
| US24          | Visualización de Reseñas y Tarifas | Como dueño de una mascota, deseo ver las reseñas y tarifas ofrecidas por distintos veterinarios para un servicio específico solicitado en una cita, y así elegir la mejor opción. |


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

## US20: Actualización del Historial Médico  
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

## US21: Publicar Reseñas  
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

## US22: Visualización de Reseñas  
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

## US23: Ofrecer tarifa por servicio  
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

## US24: Visualización de Reseñas y Tarifas  
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

## Bibliografía

- Sedano, L. (2024). _Manual para la gestión eficaz de clínicas veterinarias: Estrategias administrativas y organizativas._ Recuperado de https://puntomedic.cl/blogs/manuales-y-guias/manual-para-la-gestion-eficaz-de-clinicas-veterinarias-estrategias-administrativas-y-organizativas 

- BioSystems S.A. (s.f.). _Guía de buenas prácticas en veterinaria._ Barcelona, España: ioSystems S.A. Recuperado de https://covetrioja.org/wp-content/uploads/2021/10/VET_GuiaBuenasPracticas_ESP.pdf 


## Anexos

**Anexo 1:**

**Entrevias de Needfinding**

Entrevistas a Clinicas Veterinarias:<br>
- [`https://upcedupe-my.sharepoint.com/:v:/g/personal/u202221518_upc_edu_pe/EYevHRw9GQ5PmnarGePq9lsB9kIXpRvegYORyQnQLeUsQg?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=wTtOfn`](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202221518_upc_edu_pe/EYevHRw9GQ5PmnarGePq9lsB9kIXpRvegYORyQnQLeUsQg?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=wTtOfn)

- [`https://upcedupe-my.sharepoint.com/:v:/g/personal/u20221c362_upc_edu_pe/EenhPQh7QtNJv8TMRTHvYP0BzjPaqB_rTUv0wqjPt7JQIQ?e=FNTg1h&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D`](https://upcedupe-my.sharepoint.com/:v:/g/personal/u20221c362_upc_edu_pe/EenhPQh7QtNJv8TMRTHvYP0BzjPaqB_rTUv0wqjPt7JQIQ?e=FNTg1h&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)

- 

Entrevistas a Dueños de Mascotas:<br>

- [`https://upcedupe-my.sharepoint.com/:v:/g/personal/u202217804_upc_edu_pe/EW0OxQboN91CuWYKpGd_4MwBlAsR0SZe-MXv2JYI9tr2sA?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=hOaFtS`](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202217804_upc_edu_pe/EW0OxQboN91CuWYKpGd_4MwBlAsR0SZe-MXv2JYI9tr2sA?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=hOaFtS)

- [`https://upcedupe-my.sharepoint.com/:v:/g/personal/u20221c362_upc_edu_pe/Ee5rXgJAqnREmSoDnOD-WfUBGOscyXbOLMpNCqAw-zoysg?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=SSRBR3`](https://upcedupe-my.sharepoint.com/:v:/g/personal/u20221c362_upc_edu_pe/Ee5rXgJAqnREmSoDnOD-WfUBGOscyXbOLMpNCqAw-zoysg?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=SSRBR3)

- [`https://upcedupe-my.sharepoint.com/:v:/g/personal/u202218167_upc_edu_pe/ESaf-2VJ0zJGpLnNv2DsVwsBl6m8PtmuTuQSefq_dH90YQ?e=lp9DhQ`](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202218167_upc_edu_pe/ESaf-2VJ0zJGpLnNv2DsVwsBl6m8PtmuTuQSefq_dH90YQ?e=lp9DhQ)

**Anexo 2:**
Respositorio en GitHub para el reporte:
[`https://github.com/SI657-2501-Grupo-6-Fundamentos/Pawfect-Care-report`](https://github.com/SI657-2501-Grupo-6-Fundamentos/Pawfect-Care-report)

**Anexo 3:**
Link del video exposicion TB1:
[`https://upcedupe-my.sharepoint.com/:v:/g/personal/u202221518_upc_edu_pe/EV8nUrFcwaZAt8-tHcVyjD8BxwXYykDanbxqxVP1HawhyA?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=OHKn0E`](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202221518_upc_edu_pe/EV8nUrFcwaZAt8-tHcVyjD8BxwXYykDanbxqxVP1HawhyA?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=OHKn0E)

