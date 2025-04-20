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
    - [**3.1.2. Requisitos No Funcionales**](#311-requisitos-no-funcionales)
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
            - <strong>Segmento 1 – Médicos Veterinarios:</strong> Clínicas de diferentes tamaños que necesitan mejorar la gestión de información médica, citas e inventarios.<br>
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

**Entrevistado:** [Nonmbre] <br>
**Sexo:** [masculino o femenino] <br>
**Edad:** [n] años<br>
**Domicilio:** [Distrito] <br>
**Inicio de la Entrevista:** 0:00<br>
**Duración de la Entrevista:** 6:58<br>

<img src="./assets/Chapter02/entrevista3.png" alt="Entrevista con [Nombre]" style="width: 600px; height: auto;"><br>

**Enlace:** [``]()

**Resumen de la Entrevista:** <br>

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
- **RF01.** El sistema debe permitir a los dueños de las mascotas y a los veterinarios registrarse en la plataforma.
- **RF02.** El sistema debe permitir a los dueños de las mascotas y a los veterinarios crear y editar su perfil.
- **RF03.** El administrador debe poder gestionar y editar los perfiles de los clientes.
- **RF04.** El administrador debe poder buscar a los dueños por su nombre.

### Gestión de Mascotas
- **RF05.** El sistema debe permitir a los dueños crear perfiles de sus mascotas.
- **RF06.** El sistema debe permitir a los dueños editar la información de sus mascotas.
- **RF07.** El sistema debe permitir consultar los perfiles de mascotas.
- **RF08.** El administrador debe poder gestionar los perfiles de todas las mascotas.
- **RF09.** El administrador o el veterinario deben poder buscar mascotas primero por el nombre del dueño y luego por nombre de mascota.

### Gestión de Citas
- **RF10.** El sistema debe permitir a los dueños de mascotras agendar citas veterinarias.
- **RF11.** El sistema debe permitir a los dueños de mascotras cancelar sus citas.
- **RF12.** El sistema debe permitir al personal médico o administrativo gestionar y editar citas.
- **RF13.** El sistema debe permitir al administrador buscar citas por su fecha.

### Historial Médico
- **RF14.** El sistema debe permitir a los dueños visualizar el historial médico de sus mascotas.
- **RF15.** El sistema debe permitir a los veterinarios registrar actualizaciones en el historial médico de una mascota.

### Reseñas
- **RF16.** El sistema debe permitir a los dueños de las mascotas publicar reseñas sobre la atención veterinaria recibida.
- **RF17.** El sistema debe permitir a los dueños visualizar las reseñas publicadas por otros propietarios.

### Chatbot Informativo
- **RF18.** El sistema debe proporcionar un chatbot que brinde consejos sobre:
  - Alimentación de mascotas.
  - Higiene animal.
  - Salud y síntomas.
  - Entrenamiento básico.
  - Recomendaciones personalizadas según tipo de mascota.

### Gestión de Servicios
- **RF19.** El sistema debe permitir a los veterinarios ingresar cada servicio que brindan.
- **RF20.** El sistema debe permitir a los veterinarios ingresar el tarifario de cada uno de los servicios que ofrecen.



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
      <th>Story Points</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>1</td><td>US01</td><td>Registro de Usuarios</td><td>Como usuario, deseo registrarme en la plataforma para acceder a los servicios ofrecidos.</td><td>3</td></tr>
    <tr><td>2</td><td>US17</td><td>Creación de Perfiles de Clientes</td><td>Como usuario, deseo registrar mi perfil para poder gestionar mis mascotas y citas.</td><td>3</td></tr>
    <tr><td>3</td><td>US03</td><td>Creación de Perfil de Mascota</td><td>Como usuario, deseo crear un perfil para cada una de mis mascotas y llevar el control de su información.</td><td>3</td></tr>
    <tr><td>4</td><td>US08</td><td>Agendamiento de Citas</td><td>Como usuario, deseo agendar citas para que mis mascotas reciban atención veterinaria.</td><td>3</td></tr>
    <tr><td>5</td><td>US09</td><td>Cancelación de Citas</td><td>Como usuario, deseo cancelar citas si no puedo asistir, para reorganizar la atención de mis mascotas.</td><td>2</td></tr>
    <tr><td>6</td><td>US10</td><td>Gestión de Citas (Admin/Doctor)</td><td>Como personal médico o administrador, deseo gestionar las citas para atender a los clientes.</td><td>5</td></tr>
    <tr><td>7</td><td>US04</td><td>Edición de Perfil de Mascota</td><td>Como usuario, deseo editar la información de mis mascotas para mantenerla actualizada.</td><td>3</td></tr>
    <tr><td>8</td><td>US05</td><td>Visualización de Perfiles de Mascotas</td><td>Como usuario, deseo consultar los perfiles de mis mascotas en cualquier momento.</td><td>2</td></tr>
    <tr><td>9</td><td>US25</td><td>Visualización del Historial Médico</td><td>Como usuario, deseo consultar el historial médico de mis mascotas para conocer diagnósticos y tratamientos anteriores.</td><td>3</td></tr>
    <tr><td>10</td><td>US26</td><td>Actualización del Historial Médico (Doctor)</td><td>Como veterinario, deseo registrar el historial médico de una mascota para llevar un control clínico.</td><td>3</td></tr>
    <tr><td>11</td><td>US07</td><td>Gestión de Perfiles de Mascotas (Admin)</td><td>Como administrador, deseo gestionar todos los perfiles de mascotas registrados en la plataforma.</td><td>3</td></tr>
    <tr><td>12</td><td>US06</td><td>Búsqueda de Mascotas por ID</td><td>Como administrador o médico veterinario, deseo buscar mascotas por su ID para facilitar su gestión interna.</td><td>2</td></tr>
    <tr><td>13</td><td>US12</td><td>Edición de Citas (Admin/Doctor)</td><td>Como personal médico o administrador, deseo editar las citas programadas para adaptarlas según disponibilidad.</td><td>3</td></tr>
    <tr><td>14</td><td>US11</td><td>Búsqueda de Citas por ID</td><td>Como administrador, deseo buscar citas médicas por su ID para controlar su trazabilidad.</td><td>2</td></tr>
    <tr><td>15</td><td>US28</td><td>Visualización de Reseñas</td><td>Como usuario, deseo leer reseñas de otros para elegir al mejor profesional para mi mascota.</td><td>2</td></tr>
    <tr><td>16</td><td>US27</td><td>Publicar Reseñas sobre Veterinarios</td><td>Como usuario, deseo dejar reseñas sobre la atención recibida para compartir mi experiencia.</td><td>2</td></tr>
    <tr><td>17</td><td>US02</td><td>Gestión de Perfiles de Usuario (Admin)</td><td>Como administrador, deseo gestionar los cuentas de los usuarios para asegurar el correcto uso del sistema.</td><td>5</td></tr>
    <tr><td>18</td><td>US18</td><td>Edición de Perfil de Cliente (Admin)</td><td>Como administrador, deseo editar los datos de los clientes en caso de errores o cambios solicitados.</td><td>3</td></tr>
    <tr><td>19</td><td>US19</td><td>Búsqueda de Clientes por ID</td><td>Como administrador, deseo buscar a los clientes por su ID para dar seguimiento a sus casos.</td><td>2</td></tr>
    <tr><td>20</td><td>US22</td><td>Chatbot: Salud y Síntomas</td><td>Como usuario, deseo identificar síntomas comunes de enfermedades para actuar rápidamente.</td><td>3</td></tr>
    <tr><td>21</td><td>US20</td><td>Chatbot: Consejos de Alimentación</td><td>Como usuario, deseo obtener consejos sobre la alimentación adecuada para mis mascotas mediante un chatbot.</td><td>5</td></tr>
    <tr><td>22</td><td>US21</td><td>Chatbot: Higiene Animal</td><td>Como usuario, deseo obtener consejos sobre higiene para cuidar mejor a mis mascotas.</td><td>5</td></tr>
    <tr><td>23</td><td>US23</td><td>Chatbot: Entrenamiento Básico</td><td>Como usuario, deseo obtener consejos básicos de entrenamiento para mejorar el comportamiento de mis mascotas.</td><td>2</td></tr>
    <tr><td>24</td><td>US24</td><td>Chatbot: Recomendaciones según Mascota</td><td>Como usuario, deseo obtener recomendaciones personalizadas para cada tipo de mascota.</td><td>2</td></tr>
    <tr><td>25</td><td>US13</td><td>Barra de Navegación en la Landing Page</td><td>Como usuario, quiero un menú para navegar entre las secciones principales de la página.</td><td>2</td></tr>
    <tr><td>26</td><td>US14</td><td>Sección "Why Choose Us?"</td><td>Como usuario, quiero conocer las razones para elegir esta plataforma y confiar en sus servicios.</td><td>2</td></tr>
    <tr><td>27</td><td>US15</td><td>Formulario de Contacto</td><td>Como usuario, deseo contactar a la clínica para resolver dudas o pedir ayuda.</td><td>2</td></tr>
    <tr><td>28</td><td>US16</td><td>Videos de Características</td><td>Como usuario, deseo ver videos informativos sobre el uso y beneficios de la aplicación.</td><td>2</td></tr>
    <tr><td>29</td><td>US29</td><td>Cambio de Idioma</td><td>Como usuario, deseo cambiar el idioma de la aplicación para entender mejor el contenido.</td><td>3</td></tr>
  </tbody>
</table>

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

