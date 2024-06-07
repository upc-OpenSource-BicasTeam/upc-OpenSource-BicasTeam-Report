# Capítulo 5: Product Implementation, Validation & Deployment

## 5.1 Software Configuration Management.

Para administrar la configuración de software de nuestra app, nos centraremos en tres aspectos principales: el control del código fuente, que implica gestionar las versiones y establecer una estructura organizada para el código; la configuración del entorno de desarrollo, donde nos aseguramos de que todos los miembros del equipo cuenten con herramientas consistentes; y la configuración de implementación, que se ocupa del despliegue en entornos de producción. Estas decisiones garantizan la coherencia y eficacia a lo largo de todo el ciclo de vida de la aplicación.

### 5.1.1 Software Development Environment Configuration

En esta sección, detallaremos y explicaremos los productos utilizados en el proyecto digital, así como su propósito y cómo se accede a cada uno de ellos y siguiendo las restricciones establecidas.

1. Project Management:
Para gestionar el proyecto, se utilizaron herramientas de comunicación y control de versiones. Se estableció una organización en GitHub para gestionar el código y las versiones del proyecto. Además, para las reuniones de equipo y la comunicación interna, se utilizaron plataformas como Google Meet y Discord.
- Github: https://github.com/
- Google Meet: https://meet.google.com/
- Discord: https://discord.com/download

2. Requirements Management:
Para la gestión de requisitos se llevó a cabo mediante el uso de herramientas personalizadas que permitieron recopilar, organizar y priorizar los requisitos del proyecto de manera eficiente. Se utilizó Trello, una herramienta visual para la gestión de requisitos, permitiendo la creación tableros personalizados para organizar y priorizar las tareas del proyecto que permitió realizar los Task board y Pivotal Tracker, utilizado para gestionar y realizar un seguimiento del Product Backlog del proyecto.
- Trello: https://trello.com/es
- Pivotal Tracker: https://www.pivotaltracker.com/

3. Product UX/UI Design:
Para el diseño de la experiencia de usuario (UX) y diseño de interfaz de usuario (UI) del producto se utilizo la herramienta Figma, esta herrmienta permitio al equipo crear wireframes, mockups y prototipos interactivos para visualizar y validad el diseño del producto antes de la implementación.
Por otro lado, para la creación de User Personas, Empathy Maps, Journey Maps e Impact Maps se utilizó UXPressia y para la creación de As-Is y To-Be Scenario Maps se utilizó Miro.
- Figma: https://www.figma.com/downloads/
- UXPressia: https://uxpressia.com/
- Miro: https://miro.com/es/

4. Software Development:
Para el desarrollo de software se utilizó HTML5, CSS3 y JavaScript para el desarrollo de la Landing Page de la startup, por otro lado, para la creación del Web Application de la startup se utilizarán el framework de AngularJS por el lado del Frontend y en el Backend se utilizará SpringBoot con Java.
Para trabajar con estas tecnologías, se emplearon los siguientes IDEs:
Visual Studio Code: Herramienta principal para el desarrollo Frontend, que ofrece una amplia gama de extensiones para mejorar la productividad del equipo. (En nuestro caso solo fue utilizado para la Landing Page).
JetBrains Toolbox: Proporciona un entorno integrado para el desarrollo web, con características avanzadas de edición y depuración que faciitan la creación de aplicaciones web robustas tanto para el lado FrontEnd como BackEnd.
- Visual Studio Code: https://code.visualstudio.com/
- JetBrains Toolbox: https://www.jetbrains.com/toolbox-app/

5. Software Documentation:
La documentación del software se realizó utilizando GitHub, además de ser utilizado como plataforma de control de versiones, GitHub también se empleó para alojar la documentación técnica del proyecto. Se crearon repositorios específicos para almacenar toda la información. La documentación se gestionó mediante archivos Markdown para facilitar la creación y edición colaborativa.
- GitHub: https://github.com/

### 5.1.2 Source Code Management.

En este proyecto, utilizaremos GitHub como plataforma y sistema de control de versiones para gestionar el código fuente de nuestras diferentes partes del proyecto dentro de una organización.

**Repositorios en GitHub**
- Organización: https://github.com/upc-OpenSource-BicasTeam
- Landing Page: https://github.com/upc-OpenSource-BicasTeam/upc-opensource-bicasteam-landingpage.github.io.git
- Report : https://github.com/upc-OpenSource-BicasTeam/upc-OpenSource-BicasTeam-Report.git

**GitFlow Workflow**
Implementaremos el modelo GitFlow como Workflow de control de versiones, siguiendo las convenciones y prácticas establecidas para una gestión eficiente del desarrollo de software.
1. **Branches Principales:
- `main`: Rama principal del repositorio, contiene el código estable y liberado.
- `develop`: Rama de desarrollo deonde se integran las nuevas características y mejoras.

1. Branches de Funcionalidades (Feature Branches):
- Para cada nueva funcionalidad, se creará una rama de funcionalidad con el prefijo `feature/`, seguido del nombre descriptivo de la función o característica. En nuestro caso, creamos 5 branches de características correspondientes a los 5 capítulos de nuestro informe, donde se realizan los commits respectivos antes de fusionarlos con la rama develop cuando estén listos.

1. Branches de Lanzamiento (Release Branches) y Branches de Corrección (Hotfix Branches):
En nuestro caso, no hicimos uso de estas branches ya que no lo vimos necesario al ser solo documentacion del reporte.

**Versionado Semántico**
Seguimos la especificación Semantic Versioning 2.0.0 para nombrar nuestras versiones, siguiendo el formato: `MAJOR.MINOR.PATCH`.

**Conventional Commits**
Aplicamos el estándar de Conventional Commits para los mensajes de commit, siguiendo un formato estructurado que describe claramente los cambios realizados. Esto nos ayudó a automatizar la generación de notas de versión y facilitar la comprensión del historial de cambos del proyecto.

Con estas prácticas y convenciones adaptadas a una organización en GitHub, buscamos mantener un flujo de desarrollo ordenado, colaborativo y bien documentado.

### 5.1.3 Source Code Style Guide & Conventions.

En esta sección, se establece las convenciones y prácticas que seguiremos para nombrar elementos y programar en los lenguajes utilizados en la solución, que incluyen HTML, CSS, TypeScript, AngularJS, Java, y Gherkin para los archivos `.feature`. Todas las convenciones seguirán la nomenclatura en inglés y adoptarán convenciones estándares de codificación.

1. **HTML y CSS**:
- Basado en las recomendaciones de W3C y otras fuentes de la comunidad, se establecerán convenciones para el nombramiento de elemntos hTML y estilo de la codificación CSS.
- Se seguirán las convenciones recomendadas por Google para HTML y CSS, que incluyen el uso de identaciones de 2 espacios, el uso de comillas dobles para atributos y el uso de comentarios descriptivos.
- Se utilizará la metodologìa BEM para organizar las clases CSS en bloques, elementos y modificadores, lo que facilitará la modularidad y la reutilización del código. 
- Se debe utilizar los elementos HTML de manera semántica para una correcta descripción del contenido del sitio web, incluyendo el uso adecuado de etiquetas.
- Para el desarrollo con AngularJS, se adoptarán las convenciones recomendadas por la comunidad de Angular, que incluyen el uso de PascalCase para los nombres y componentes y el uso de camelCase para las propiedades y métodos de los componentes.

2. **TypeScript**:
- Se tomarán en cuenta las directrices proporcionadas por TypeScript Handbook para la escritura del superset JavaScript, que incluyen el uso de nombres descriptivos para variables y funciones en camelCase, el uso de declaración de variables con `let` o `const` en lugar de `var`, y el uso de punto y coma al final de cada declaración.
- Se seguirán las convenciones de codificación recomendadas por Google para JavaScript, que incluyen el uso de comillas simples para literales de cadena, el uso de comentarios descriptivos y el uso de funciones de flecha para expresiones de función.

3. **AngularJS**:
- Se adoptarán las convenciones de codificación recomendadas por la comunidad de aplicaciones de AngularJS, que incluyen el uso de directivas de flujo de control declarativas, manipualcion de componentes, el uso de ciclo de vida y la organización de los componentes en carpetas y subcarpetas según su función utilizando el Domain Driven Design (DDD).

4. **Java (SpringBoot)**:
- Se seguirán las convenciones de codificación establecidas por Manual de Código Limpio para el lenguaje Java, que incluyen el uso de PascalCase para nombres de clases y métodos, el uso de camelCase para nombres de variables locales y parámetros, y el uso de comentarios XML para documentar el código.
- Para el desarrollo en SpringBoot, se adoptarán las directrices proporcionadas por Spring en sus guías de codificación, que incluyen el uso de inyección de dependencias, la separación clara entre capas de la aplicación y el uso de modelos de vista para la comunicación entre el controlador y la vista.

5. **Gherkin**:
- Se aplicarán las convenciones recomendadas para escribir especificaciones legibles en Gherkin, que incluyen el uso de palabras clave como Given, When y Then para describir el comportamiento del sistema, el uso de un lenguaje sencillo y claro, y la organización de los escenarios en contextos, acciones y resultados.
- Se seguirán las mejores prácticas recomendadas por Cucumber para escribir escenarios de prueba en Gherkin, que incluyen la reutilización de pasos de prueba, la modularización de escenarios y la escritura de pruebas autoexplicativas.

Además de estas referencias, se promoverá el uso de buenas prácticas y metodologías estándar en el desarrollo de software, como la modularidad, la reutilización de código, la legibilidad del código, la optimización del rendimiento y la seguridad. 
Con estas guías de estilo y convenciones de codificación, buscamos asegurar la coherencia, la calidad y la mantenibilidad del código a lo largo de todo el proyecto.

### 5.1.4 Software Deployment Configuration.

En esta sección, describiremos la configuración necesaria para desplegar satisfactoriamente cada uno de los productos digitales de nuestra solución, incluyendo Landing Page, los Web Services y las Frontend Web Applications.

**Pasos para el despliegue**
1. Landing Page:
- Clonar o descargar el repositorio desde GitHub.
- Configurar el servidore web para alojar la Landing Page.
- Copiar los archivos HTMLS, CSS y JavaScript en el directorio correspondiente del servidor.
- Configurar cualquier dependencia adicional, como bibliotecas de JavaScript o imágenes.
- Verificar quue la Landing Page se cargue correctamente en el navegador.

2. Web Services (API):
- Preparar el código fuente del servicio web, asegurando que esté correctamente estructurado y documentado.
- Configurar un entorno de desarrolo o pruebas para realizar pruebas exhaustivas del servicio antes del desplieguee.
- Desplegar el código en un servidor adecuado para el entorno de producción.
- Configurar la seguridad y la autenticación según los requisitos del sistema.
- Documentar la API utilizando OpenAPI Specification para facilitar su integración y uso por parte de otros sistemas.

3. Frontend Web Applications:
- Clonar repositorio desde GitHub.
- Compilar y empaquetar las aplicaciones frontend. En nuestro caso, utilizamos el framework Vue.js, por lo que se debe ejecutar los comandos de construcción (`npm run build`) para generar los archivos estáticos.
- Una vez empaquetadas, las Frontend Web Applications se pueden servir utilizando un servidor de aplicaciones compatible con archivos estáticos, como Nginx o incluso GitHub Pages para proyectos estáticos más simples.
- Si es necesario, se deben configurar las rutas en el servidor de aplicaciones para que conincidan con las rutas esperadas por las aplicaciones frontend.

## 5.2 Landing Page, Services & Applications Implementation.

En esta sección, describiremos el proceso de implementación, pruebas, documentación y despliegue de la Landing Page, los Web Services y las Frontend Web Applications. Abordaremos cada componente de manera individual a lo largo de los diferentes sprints, comenzando en este Sprint 1 con la implementación específica de la Landing Page. Una vez establecido nuestro Product Backlog, cada sprint se dividirá en secciones internas para abordar cada aspecto de la implementación y la colaboración del equipo.

### 5.2.1 Sprint 1

En esta sección, documentaremos y explicaremos el progreso tanto en el desarrollo del producto como en la colaboración del equipo durante el Sprint 1. Seguimos un proceso definido que abarca desde la planificación hasta la revisión y documentación del trabajo realizado. A lo largo de las siguientes secciones, detallaremos cómo se llevó a cabo la planificación del sprint, qué tareas se incluyeron en el Sprint Backlog, las pruebas y evidencia de desarrollo para la revisión del sprint, así como la documentación de los servicios y las percepciones clave sobre la colaboración del equipo durante este periodo

### 5.2.1.1 Sprint Planning 1

En esta sección, se detallan los aspectos principales del Sprint Planning Meeting para el Sprint n. Este encuentro es crucial para establecer los objetivos del sprint, determinar las user stories que se abordarán y asignar tareas al equipo. A continuación, se presenta un resumen del Sprint Planning Meeting para este período.


| Sprint #                             | Sprint 1           |
|--------------------------------------|--------------------|
| Sprint Planning Background                                |
| Date                                 |  2024-03-23        |
| Time                                 |  01:30 PM          |
| Location                             |  Virtual (Discord) |
| Prepared By                          |   Miguel Huarcaya Chavez   |
| Attendees (to planning meeting)      |  Todo el equipo |
| Sprint 1 – 1 Review Summary          |  Durante el primer sprint, avanzamos significativamente en el desarrollo del producto y logramos una colaboración eficiente dentro del equipo. Alcanzamos hitos importantes y recopilamos retroalimentación valiosa que nos servirá como base para el próximo sprint.  |
| Sprint 1 – 1 Retrospective Summary   |  En la retrospectiva del primer sprint identificamos áreas para mejorar, como la comunicación y la estimación de tareas. Estamos comprometidos a implementar acciones correctivas y mejorar continuamente nuestro proceso de trabajo.  |
| Sprint Goal & User Stories                                |
| Sprint 1 Goal                        | Alcanzar una métrica de cumplimiento del 100%, lo que indicará que se ha logrado los objetivos del sprint 1.        |
| Sprint 1 Velocity                    | Acordamos aceptar 4 Story Points como nuestra capacidad de entrega para este sprint.     |
| Sum of Story Points                  | La suma de los Story Points para los User Stories que se están incluyendo en este Sprint 1 es 6 |

### 5.2.1.2 Sprint Backlog 1

El Sprint 1 está centrado en la implementación de las funcionalidades clave de la landing page del sitio web, priorizando las historias de usuario identificadas. Nuestro objetivo principal es proporcionar a los visitantes una experiencia inicial sólida al presentar de manera clara y concisa las características y beneficios del sitio, junto con una navegación intuitiva y acceso rápido a la información relevante. Al completar las tareas asociadas a las historias de usuario definidas, sentaremos las bases para futuras iteraciones, asegurando que la página de inicio cumpla con las expectativas de los usuarios y contribuya al éxito del proyecto.

URL del Board en Trello: https://trello.com/invite/b/9fFNzPVl/ATTId6d62a99d06e758b547d220c4b08a09131B77500/appweb

![Board Trello](/assets/chapter05/boardTrello.png)

<table>
    <tr>
        <td colspan="2">Sprint #</td>
        <td colspan="6">Sprint 1</td>
    </tr>
    <tr>
        <td colspan="2">User Story</td>
        <td colspan="6">Work-Item / Task</td>
    </tr>
    <tr>
        <td>Id</td>
        <td>Title</td>
        <td>Id</td>
        <td>Title</td>
        <td>Descripcion</td>
        <td>Estimation (Hours)</td>
        <td>Assigned To</td>
        <td>Status (To-do / In / Process / ToReview / Done)</td>
    </tr>
    <tr>
        <td>US17</td>
        <td>Landing - Resumen del sitio web</td>
        <td>T05</td>
        <td>Desarrollar resumen claro y conciso sobre las características y beneficios del sitio web en la página de inicio.</td>
        <td>Crear una sección de resumen en la página de inicio que presente de manera clara y concisa las principales características y beneficios del sitio web, destacando los puntos más relevantes de manera atractiva y fácil de entender.</td>
        <td>2 hora</td>
        <td>Jose Diego huamani</td>
        <td>Done</td>
    </tr>
    <tr>
        <td>US18</td>
        <td>Landing - Resumen de precios</td>
        <td>T06</td>
        <td>Implementar acceso claro y visible a la información detallada de los planes ofrecidos en la página de inicio.</td>
        <td>Integrar un acceso claro y visible en la página de inicio que permita a los visitantes buscar información detallada sobre los planes ofrecidos, incluyendo características, beneficios, limitaciones, términos y condiciones, precio y cualquier otra información relevante.</td>
        <td>3 hora</td>
        <td>Jose diego Huamani</td>
        <td>Done</td>
    </tr>
    <tr>
        <td>US19</td>
        <td>Landing - Información a pie de página</td>
        <td>T07</td>
        <td>Desarrollar un resumen claro y conciso del sitio web al final de la página de inicio.</td>
        <td>Crear un resumen al final de la página de inicio que destaque los aspectos más relevantes del sitio web, como las características principales, los servicios ofrecidos, la información de contacto y cualquier otra información importante para los visitantes.</td>
        <td>1 hora</td>
        <td>Miguel Huarcaya</td>
        <td>Done</td>
    </tr>
    <tr>
        <td>US20</td>
        <td>Landing - Ir a aplicación web directamente</td>
        <td>T08</td>
        <td>Integrar un llamado a la acción claro y visible para dirigir a los visitantes a la aplicación web principal.</td>
        <td>Presentar un llamado a la acción claro y visible en la página de inicio que guíe a los visitantes a explorar más a fondo el sitio web o tomar la acción deseada, como registrarse, suscribirse o contactar al equipo.</td>
        <td>1 hora</td>
        <td>Elias Torres</td>
        <td>Done</td>
    </tr>
    <tr>
        <td>US21</td>
        <td>Landing - Navegación de información</td>
        <td>T09</td>
        <td>Presentar contenido claro, detallado y preciso sobre lo que ofrece el sitio web en la página de inicio.</td>
        <td>Proporcionar contenido claro, detallado y preciso en la página de inicio que describa las características, funcionalidades y beneficios del sitio web de manera comprensible y convincente.</td>
        <td>1 hora</td>
        <td>Nestor velarde</td>
        <td>Done</td>
    </tr>
    <tr>
        <td>US22</td>
        <td>Landing - Navegación de contacto</td>
        <td>T10</td>
        <td>Mostrar información de contacto visible y accesible en la página de inicio.</td>
        <td>Mostrar claramente la información de contacto, como dirección de correo electrónico, número de teléfono y/o dirección física, en una sección destacada de la página de inicio para que los visitantes puedan comunicarse con el sitio web de manera efectiva.</td>
        <td>3 hora</td>
        <td>Elias Torres</td>
        <td>Done</td>
    </tr>
</table>

### 5.2.1.3 Development Evidence for Sprint Review.
Esta sección documenta y presenta la serie de commits realizados en el repositorio del Landing Page. Estos commits, que son una parte integral del proceso de desarrollo, se han gestionado utilizando la metodología GitFlow y siguiendo estrictamente las convenciones establecidas para los commits. Esta evidencia sirve como un registro transparente y trazable de nuestro progreso y esfuerzos de desarrollo a lo largo del sprint.

![Lista de commits](/assets/chapter05/commits.png)

| Repository                        | Branch              | Commit Id                          | Commit Message                   | Commit Message Body           |Commited on (Date) |
|-----------------------------------|---------------------|------------------------------------|----------------------------------|-------------------------------|-------------------|
| upc-OpenSource-BicasTeam-LandingPage.github.io   | main     | 4ad069c28a25992a9201a92858002309e0bf4df7 | chore: ...                      | initial commit         | 10-04             |
| upc-OpenSource-BicasTeam-LandingPage.github.io   | feature/section-about      | 9a37f7ee1756f0f868e45e7c1b3c71848007824a | feat: ...                      | create services         | 10-04             |
| upc-OpenSource-BicasTeam-LandingPage.github.io   | feature/section-footer      | | upc-OpenSource-BicasTeam-LandingPage.github.io   | feature/section-about      | 9a37f7ee1756f0f868e45e7c1b3c71848007824a | feat: ...           | create footer         | 10-04             | | feat: ...                      | create services         | 10-04             |
| upc-OpenSource-BicasTeam-LandingPage.github.io   | feature/section-footer service     | | upc-OpenSource-BicasTeam-LandingPage.github.io   | feature/section-about service     | d5e5a6eb2c9ad42feed3ed4f36c5aba0654202e5 | fix: ...        | fix footer         | 10-04             | | fix: ...                      | create services         | 10-04             |
| upc-OpenSource-BicasTeam-LandingPage.github.io   | feature/section-pricing      | | upc-OpenSource-BicasTeam-LandingPage.github.io   | feature/section-pricing      | d5e5a6eb2c9ad42feed3ed4f36c5aba0654202e5 | fix: ...   | fix footer         | 10-04             | | feat: ...                      | create services         | 10-04             |
| upc-OpenSource-BicasTeam-LandingPage.github.io   | feat     | cbb29c4b819970c09e9b3de1b84c0de61c758c4e | feat: ...                      | create section header       | 10-04             |
| upc-OpenSource-BicasTeam-LandingPage.github.io   | feat     | d7f5a246629c7aa309e2c2816d2fb1c38a953b85 | feat: ...                      | create section hero       | 10-04             |
| upc-OpenSource-BicasTeam-LandingPage.github.io   | feat     | 09ed97a86a2413031145c4413ec161ff07af625f | feat: ...                      | create section about team       | 10-04             |
| upc-OpenSource-BicasTeam-LandingPage.github.io   | feat     | 09ed97a86a2413031145c4413ec161ff07af625f | feat: ...                      | create section about us       | 10-04             |


### 5.2.1.4 Testing Suite Evidence for Sprint Review. 
En esta sección, presentamos la evidencia de las pruebas realizadas durante el sprint. Hemos utilizado Gherkin para definir los escenarios de prueba y hemos registrado cada prueba en commits específicos en nuestro repositorio. A continuación, se muestra un registro de estos commits:

| Repository                        | Branch              | Commit Id                          | Commit Message                   | Commit Message Body           |Commited on (Date) |
|-----------------------------------|---------------------|------------------------------------|----------------------------------|-------------------------------|-------------------|
| upc-OpenSource-BicasTeam-LandingPage.github.io   | feature/section-header  | 1fbb6f6                           | feat: ...                        | add tests for header section            | 10/04  |
| upc-OpenSource-BicasTeam-LandingPage.github.io   | feature/section-footer  | ee12b07                          | feat: ...                        | add test for footer section           | 10/04  |
| upc-OpenSource-BicasTeam-LandingPage.github.io   | feature/section-services  | e36977f                            | feat: ...                        | add test for pricing section            | 10/04  |      


### 5.2.1.5 Execution Evidence for Sprint Review. 

Durante el Sprint 1, se logró un progreso significativo en la implementación de las características clave de la página de inicio del sitio web. El equipo completó con éxito todas las historias de usuario asignadas para este sprint, que incluyeron el desarrollo de un resumen claro de las características y beneficios del sitio web, la integración de acceso visible a información detallada de precios, la adición de un resumen conciso al final de la página de inicio, la inclusión de un llamado a la acción prominente para dirigir a los visitantes a la aplicación web principal, la presentación de contenido informativo claro y detallado, y la integración de información de contacto visible en la página de inicio. El equipo trabajó de manera colaborativa para garantizar que las características implementadas cumplan con los requisitos y contribuyan a una experiencia de usuario positiva.
Capturas de pantalla:

- Sección de Resumen:

![Resumen](/assets/chapter05/resumen.png)

- Acceso a la Información de Precios:

![Precios](/assets/chapter05/precios.png)

- Resumen al Final:

![Footer](/assets/chapter05/footer.png)

- Contenido Informativo:

![Board Trello](/assets/chapter05/servicios.png)

- Llamado a la acción

![Board Trello](/assets/chapter05/calltoAction.png)

- Sección de Información de Contacto:

![Contacto](/assets/chapter05/contacto.png)


Video: https://upcedupe-my.sharepoint.com/:v:/g/personal/u202116207_upc_edu_pe/EcibyFqJONpAp8yWRYzs3c8BmX47KlQ4sjigq6VeGem_6g?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=CeppC1

### 5.2.1.6 Services Documentation Evidence for Sprint Review. 

Durante este Sprint 1, nos enfocamos en desarrollar el landing page, sin implementación de cualquier servicio. Por lo tanto, este punto quedará sin actividad en este aspecto.

### 5.2.1.7 Software Deployment Evidence for Sprint Review.

Durante el Sprint 1, llevamos a cabo el despliegue de nuestra landing page en GitHub Pages. A continuación, detallamos los pasos realizados:

1. Creación del Repositorio en GitHub: Iniciamos creando un repositorio dedicado en GitHub para nuestro proyecto de landing page.
2. Configuración de la Rama main: Aseguramos que la rama principal del repositorio se llamara main, ya que GitHub Pages toma esta rama como base para el despliegue automático.
3. Preparación del Contenido: Desarrollamos y diseñamos nuestra landing page, asegurándonos de que todos los archivos y recursos necesarios estuvieran presentes en el repositorio.
4. Generación del Enlace de GitHub Pages: Navegamos a la sección "Pages" en la configuración del repositorio en GitHub. Configuramos la fuente del GitHub Pages para que tomara el contenido de la rama main.
5. Despliegue Automático: GitHub Pages automáticamente detectó los cambios en la rama main y desplegó la landing page en la URL proporcionada por GitHub Pages.

### 5.2.1.8 Team Collaboration Insights during Sprint.

Durante este primer Sprint, hemos completado el desarrollo del landing page y hemos colaborado estrechamente en su implementación. La colaboración entre los miembros del equipo se refleja en los diversos commits realizados en el repositorio de GitHub, los cuales han sido debidamente documentados en las capturas de pantalla adjuntas.
Para asegurar una colaboración efectiva, hemos implementado GitFlow como nuestra metodología de trabajo colaborativo en Git. Con GitFlow, hemos creado ramas para cada una de las secciones de nuestra landing page. Esto nos ha permitido trabajar de manera organizada y centrarnos en completar correctamente las historias de usuario designadas para cada sección.
En cuanto a la elaboración del código, hemos asignado a cada miembro del equipo una sección específica del landing page. Esta estrategia nos ha permitido avanzar de manera más eficiente y completar el trabajo antes de la fecha de entrega.
Además, hemos realizado reuniones adicionales para intercambiar ideas y resolver cualquier duda o problema que pudiera surgir durante el desarrollo del landing page. Estas sesiones han contribuido de manera positiva al éxito del proyecto.
A continuación, presentamos algunas capturas de pantalla que muestran los commits realizados por los miembros del equipo en GitHub:



------
------
------
### 5.2.2 SPRINT 2
En esta sección, comentaremos y explicaremos el progreso tanto en el desarrollo del producto como en la colaboración del equipo durante el Sprint 2. Seguimos un proceso definido que abarca desde la planificación hasta la revisión y documentación del trabajo realizado. A lo largo de las siguientes secciones, detallaremos cómo se llevó a cabo la planificación del sprint, qué tareas se incluyeron en el Sprint Backlog, las pruebas y evidencia de desarrollo para la revisión del sprint, así como la documentación de los servicios y las percepciones clave sobre la colaboración del equipo durante este periodo.

#### 5.2.2.1 Sprint Planing 2
En esta sección, se detallan los aspectos principales del Sprint Planning Meeting para el Sprint n. Este encuentro es crucial para establecer los objetivos del sprint, determinar las user stories que se abordarán y asignar tareas al equipo. A continuación, se presenta un resumen del Sprint Planning Meeting para este período

![Sprint Planing 2](/assets/chapter05/sprintPlaning2.png)

#### 5.2.2.2 Sprint Backlog 2
El Sprint 2 está centrado en el frontend de nuestra aplicación web, priorizando las historias de usuario identificadas. Nuestro objetivo principal es proporcionar a los usuarios una experiencia inicial sólida al presentar una navegación intuitiva y acceso rápido a las funcionalidades relevantes. Al completar las tareas asociadas a las historias de usuario definidas, sentaremos una buena base para la aplicación web, asegurando que lo propuesto contribuya al éxito del proyecto.
URL del Board en Trello: 

Link Trello: https://trello.com/invite/b/5B5dHJXJ/ATTI89c324fa13b11e255137811b14e197e78549A8F8/appweb-sprinbacklog-2 

![ Trello Sprint Backlog 2](/assets/chapter05/trelloSprintPlaning2.png)

![ Sprint backlog 2](/assets/chapter05/sprint%20backlog%202.png)

#### 5.2.2.3 Development Evidence for Sprint review
Esta sección documenta y presenta la serie de commits realizados en el repositorio de la Aplicación Web. Estos commits, que son una parte integral del proceso de desarrollo, se han gestionado utilizando la metodología GitFlow y siguiendo estrictamente las convenciones establecidas para los commits. Esta evidencia sirve como un registro transparente y trazable de nuestro progreso y esfuerzos de desarrollo a lo largo del sprint.

![ development Evidence](/assets/chapter05/developmentEvidence.png)


#### 5.2.2.4 Testing Suite Evidence for Sprint Review
En esta sección, presentamos la evidencia de las pruebas realizadas durante el sprint. Hemos utilizado Gherkin para definir los escenarios de prueba y hemos registrado cada prueba en commits específicos en nuestro repositorio. A continuación, se muestra un registro de estos commits:
![ Test Sprint backlog](/assets/chapter05/testSprintBacklog2.png)


#### 5.2.2.5 Execution Evidence for Sprint Review
Durante el Sprint 2, se logró un progreso significativo en la implementación de las características clave del frontend en la aplicación web. El equipo completó con éxito las historias de usuario asignadas para este sprint, que incluyeron el desarrollo del frontend en nuestra aplicación web, también con la integración de acceso visible a todas las opciones, incluso de un llamado a la acción prominente para dirigir a los visitantes a la aplicación web. El equipo trabajó de manera colaborativa para garantizar que las características implementadas cumplan con los requisitos y contribuyan a una experiencia de usuario positiva.

![Evidence](/assets/chapter05/evidenceApp/homeBusinessman.png)
![Evidence](/assets/chapter05/evidenceApp/homeCarrier.png)
![Evidence](/assets/chapter05/evidenceApp/login.png)
![Evidence](/assets/chapter05/evidenceApp/profile.png)
![Evidence](/assets/chapter05/evidenceApp/registerInfo.png)
![Evidence](/assets/chapter05/evidenceApp/registerSucessfully.png)
![Evidence](/assets/chapter05/evidenceApp/registerType.png)
![Evidence](/assets/chapter05/evidenceApp/reportsBusinessman.png)
![Evidence](/assets/chapter05/evidenceApp/reportsCarrier.png)
![Evidence](/assets/chapter05/evidenceApp/shipmentsBusinessman.png)
![Evidence](/assets/chapter05/evidenceApp/shipmentsCarrier.png)
![Evidence](/assets/chapter05/evidenceApp/vehicleCarrier.png)
![Evidence](/assets/chapter05/evidenceApp/vehiclesBusinessman.png)



#### 5.2.2.6 Services Documentation Evidence for Sprint Review
Durante este Sprint 2, nos enfocamos en desarrollar el “App web Solution”, sin implementación de ningún servicio. Por lo tanto, este punto quedará sin actividad en este aspecto.

#### 5.2.2.7 Software Deployment Evidence for Sprint Review
Durante el Sprint 2, llevamos a cabo el despliegue de nuestra aplicación web en GitHub Pages. A continuación, detallamos los pasos realizados:
- Creación del Repositorio en GitHub: Iniciamos creando un repositorio dedicado en GitHub para nuestro proyecto de aplicación web.
- Configuración de la Rama main: Aseguramos que la rama principal del repositorio se llamará main, ya que GitHub Pages toma esta rama como base para el despliegue automático.
- Preparación del Contenido: Desarrollamos y diseñamos nuestra aplicación web, asegurándonos de que todos los archivos y recursos necesarios estuvieran presentes en el repositorio.
- Generación del enlace de GitHub Pages: Navegamos a la sección "Pages" en la configuración del repositorio en GitHub. Configuramos la fuente del GitHub Pages para que tomara el contenido de la rama main.
- Despliegue Automático: GitHub Pages automáticamente detectó los cambios en la rama main y desplegó la aplicación web en la URL proporcionada por GitHub Pages.


#### 5.2.2.8 Team Collaboration Insights during Sprint
Durante este segundo Sprint, hemos avanzado el desarrollo de la aplicación web y hemos colaborado estrechamente en su implementación. La colaboración entre los miembros del equipo se refleja en los diversos commits realizados en el repositorio de GitHub, los cuales han sido debidamente documentados en las capturas de pantalla adjuntas. Para asegurar una colaboración efectiva, hemos implementado GitFlow como nuestra metodología de trabajo colaborativo en Git. Con GitFlow, hemos creado ramas para cada una de las secciones de nuestra aplicación web. Esto nos ha permitido trabajar de manera organizada y centrarnos en completar correctamente las historias de usuario designadas para cada sección. En cuanto a la elaboración del código, hemos asignado a cada miembro del equipo una sección específica de la aplicación web. Esta estrategia nos ha permitido avanzar de manera más eficiente y completar el trabajo antes de la fecha de entrega. Además, hemos realizado reuniones adicionales para intercambiar ideas y resolver cualquier duda o problema que pudiera surgir durante el desarrollo del landing page. Estas sesiones han contribuido de manera positiva al éxito del proyecto. A continuación, presentamos algunas capturas de pantalla que muestran los commits realizados por los miembros del equipo en GitHub:

![ANALitica](/assets/chapter05/analityc1.png)
![ANALitica](/assets/chapter05/analityc2.png)
![ANALitica](/assets/chapter05/analityc3.png)

---

### 5.2.3 Sprint 3
En esta sección, comentaremos y explicaremos el progreso tanto en el desarrollo del producto como en la colaboración del equipo durante el Sprint 3. Seguimos un proceso definido que abarca desde la planificación hasta la revisión y documentación del trabajo realizado. A lo largo de las siguientes secciones, detallaremos cómo se llevó a cabo la planificación del sprint, qué tareas se incluyeron en el Sprint Backlog, las pruebas y evidencia de desarrollo para la revisión del sprint, así como la documentación de los servicios y las percepciones clave sobre la colaboración del equipo durante este periodo.

#### 5.2.3.1 Sprint Planning 3
En esta sección, se detallan los aspectos principales del Sprint Planning Meeting para el Sprint n. Este encuentro es crucial para establecer los objetivos del sprint, determinar las user stories que se abordarán y asignar tareas al equipo. A continuación, se presenta un resumen del Sprint Planning Meeting para este período.
|Sprint #|Sprint 3|
| :- | :- |
|Sprint Planning Background||
|Date|2024-05-24|
|Time|04:23 PM|
|Location|Google Meet|
|Prepared by|Miguel Huarcaya Chavez|
|Attendees (to planning meeting)|Nestor Velarde, Elias Torres, Miguel Huarcaya Chavez, Diego Huaman|
|Sprint 3 – 1 Review Summary|Después de realizar todos los procedimientos establecidos para la identificación de objetivos y áreas de retroalimentación, hemos podido concluir la reunión del sprint 3 con éxito en términos de avance en los productos de software y en la colaboración general del equipo. El proceso de mejora con la retroalimentación y la programación de varias secciones nuevas en el servicio web significó un gran proceso de mejora para la construcción y realización del sprint, además de reforzar el compromiso de nuestro equipo y la mejora exponencial de las actividades indicadas.|
|Sprint 3 – 1 Retrospective Summary|Para el proceso de la retrospectiva del Sprint 3, fue necesario que nuestro equipo revisará a detalle toda la retroalimentación recibida ante el primer sprint realizado, para luego generar un análisis a profundidad del desempeño general e individual de todos los miembros del equipo de trabajo. Después de ese proceso, pudimos identificar varias áreas de mejora en las cuales centrarnos para así poder garantizar la entrega de un mejor trabajo y un buen producto para todos nuestros clientes, promoviendo la mejora continua y optimizando los métodos de trabajo en los próximos sprints durante el ciclo de vida del proyecto.|
|Sprint Goal & User Stories||
|Sprint 3 Goal|Alcanzar una métrica de cumplimiento del 100%, lo que indicará que se ha logrado los objetivos del sprint 3.|
|Sprint 3 Velocity|Con el equipo para este sprint 3 decidimos aceptar 6 Story Points|
|Sum of Story Points|La suma de los Story Points para los User Stories que se están incluyendo en este Sprint es 32.|

#### 5.2.3.2 Sprint Backlog 3
El Sprint 3 está centrado en el servicio web, priorizando las historias de usuario identificadas. Nuestro objetivo principal es proporcionar a los usuarios una experiencia inicial sólida al presentar una navegación intuitiva y acceso rápido a las funcionalidades relevantes. Al completar las tareas asociadas a las historias de usuario definidas, sentaremos una buena base para el servicio web, asegurando que lo propuesto contribuya al éxito del proyecto.

URL del Board en Trello:

<https://trello.com/invite/b/vTLeIEal/ATTIa1968d7983179167e3fad507a5040fe21920F95D/appweb-sprintbacklog-3> 

![Trello Sprint 3](/assets/chapter05%20-%20spring%203/trello-sprint-3.png)

|&emsp;&emsp;&emsp;&emsp;<a name="_heading=h.kn5t1eh5nzqr"></a>Sprint #|&emsp;&emsp;&emsp;&emsp;Sprint 3|||||||
| :- | :- | :- | :- | :- | :- | :- | :- |
|&emsp;&emsp;&emsp;&emsp;User Story|&emsp;&emsp;&emsp;&emsp;Work-Item / Task|||||||
|&emsp;&emsp;&emsp;&emsp;Id|&emsp;&emsp;&emsp;&emsp;Title|&emsp;&emsp;&emsp;&emsp;Id|&emsp;&emsp;&emsp;&emsp;Title|&emsp;&emsp;&emsp;&emsp;Descripción|&emsp;&emsp;&emsp;&emsp;Estimation (Hours)|&emsp;&emsp;&emsp;&emsp;Assigned to|&emsp;&emsp;&emsp;&emsp;Status (To-do / In / Process / ToReview / Done)|
|&emsp;&emsp;&emsp;&emsp;US09|&emsp;&emsp;&emsp;&emsp;Asignación de flotas|&emsp;&emsp;&emsp;&emsp;T14|&emsp;&emsp;&emsp;&emsp;Desarrollo de interfaz y lógica de asignación de flotas|&emsp;&emsp;&emsp;&emsp;Crear una interfaz en la aplicación web que permita al gerente seleccionar y asignar flotas a los transportistas, junto con la lógica de backend necesaria para actualizar las bases de datos con las asignaciones realizadas.|&emsp;&emsp;&emsp;&emsp;4|&emsp;&emsp;&emsp;&emsp;Elias Torres|&emsp;&emsp;&emsp;&emsp;Done|
|&emsp;&emsp;&emsp;&emsp;US14|&emsp;&emsp;&emsp;&emsp;Reporte de accidentes en la carretera|&emsp;&emsp;&emsp;&emsp;T15|&emsp;&emsp;&emsp;&emsp;Implementación de sistema de reporte de accidentes|&emsp;&emsp;&emsp;&emsp;Crear un formulario en la aplicación móvil o web para que los transportistas reporten accidentes, junto con un endpoint en el servidor que reciba y almacene los reportes, e implemente notificaciones automáticas a los gerentes.|&emsp;&emsp;&emsp;&emsp;5|&emsp;&emsp;&emsp;&emsp;Diego huaman|&emsp;&emsp;&emsp;&emsp;Done|
|&emsp;&emsp;&emsp;&emsp;US15|&emsp;&emsp;&emsp;&emsp;Reporte de problemas con el paquete|&emsp;&emsp;&emsp;&emsp;T16|&emsp;&emsp;&emsp;&emsp;Implementación de sistema de reporte de problemas con el paquete|&emsp;&emsp;&emsp;&emsp;Crear un formulario en la aplicación móvil o web para reportar problemas con los paquetes, junto con un endpoint en el servidor que reciba y almacene los reportes, e implemente notificaciones automáticas a los gerentes y clientes.|&emsp;&emsp;&emsp;&emsp;4|&emsp;&emsp;&emsp;&emsp;Miguel Huarcaya|&emsp;&emsp;&emsp;&emsp;Done|
|&emsp;&emsp;&emsp;&emsp;US16|&emsp;&emsp;&emsp;&emsp;Reporte de problemas técnicos|&emsp;&emsp;&emsp;&emsp;T17|&emsp;&emsp;&emsp;&emsp;Implementación de sistema de reporte de problemas técnicos|&emsp;&emsp;&emsp;&emsp;Crear un formulario en la aplicación móvil o web para reportar problemas técnicos, junto con un endpoint en el servidor que reciba y almacene los reportes, e implementa notificaciones automáticas a los gerentes.|&emsp;&emsp;&emsp;&emsp;5|&emsp;&emsp;&emsp;&emsp;Elias Torres|&emsp;&emsp;&emsp;&emsp;Done|
|&emsp;&emsp;&emsp;&emsp;US23|&emsp;&emsp;&emsp;&emsp;Eliminar registro|&emsp;&emsp;&emsp;&emsp;T18|&emsp;&emsp;&emsp;&emsp;Desarrollo de endpoint para eliminar registro|&emsp;&emsp;&emsp;&emsp;Crear un endpoint en la API que permite eliminar registros específicos de la base de datos, incluyendo la lógica de backend para realizar las verificaciones necesarias antes de la eliminación.|&emsp;&emsp;&emsp;&emsp;4|&emsp;&emsp;&emsp;&emsp;Nestor Velarde|&emsp;&emsp;&emsp;&emsp;Done|
|<p>&emsp;&emsp;&emsp;&emsp;US24</p><p>&emsp;&emsp;&emsp;&emsp;</p>|&emsp;&emsp;&emsp;&emsp;Agregar registro|&emsp;&emsp;&emsp;&emsp;T19|&emsp;&emsp;&emsp;&emsp;Desarrollo de endpoint para agregar registro|&emsp;&emsp;&emsp;&emsp;Crear un endpoint en la API que permita agregar nuevos registros a la base de datos, incluyendo la lógica de backend para validar los datos antes de su inserción.|&emsp;&emsp;&emsp;&emsp;5|&emsp;&emsp;&emsp;&emsp;Elias Torres|&emsp;&emsp;&emsp;&emsp;Done|
|&emsp;&emsp;&emsp;&emsp;US25|&emsp;&emsp;&emsp;&emsp;Actualizar registro|&emsp;&emsp;&emsp;&emsp;T20|&emsp;&emsp;&emsp;&emsp;Desarrollo de endpoint para actualizar registro|&emsp;&emsp;&emsp;&emsp;Crear un endpoint en la API que permita actualizar registros existentes en la base de datos, incluyendo la lógica de backend para validar los datos antes de su actualización.|&emsp;&emsp;&emsp;&emsp;5|&emsp;&emsp;&emsp;&emsp;Diego Huaman|&emsp;&emsp;&emsp;&emsp;Done|

#### 5.2.3.3 Development Evidence for Sprint Review
Esta sección documenta y presenta la serie de commits realizados en el repositorio del Servicio Web. Estos commits, que son una parte integral del proceso de desarrollo, se han gestionado utilizando la metodología GitFlow y siguiendo estrictamente las convenciones establecidas para los commits. Esta evidencia sirve como un registro transparente y trazable de nuestro progreso y esfuerzos de desarrollo a lo largo del sprint.

TODO: Imagen Commits 
![Development Evidence fpr Spóinrt Review]()

|Repository|Branch|Commit Id|Commit Message|Commit Message Body|Committed on (Date)|
| :-: | :-: | :-: | :-: | :-: | :-: |
|upc-OpenSource-BicasTeam-Api|main|cc1ecb8|chore|create default project|27-05|
|upc-OpenSource-BicasTeam-Api|feature/profile-management|3c630b1|chore|implemented persistence base configuration|27-05|
|upc-OpenSource-BicasTeam-Api|feature/profile-management|46d523d|feat|added aggregate user|27-05|
|upc-OpenSource-BicasTeam-Api|feature/profile-management|05ef98f|feat|added user repository|27-05|
|upc-OpenSource-BicasTeam-Api|feature/profile-management|7b06c81|feat|implemented query service and command for user aggregate|27-05|
|upc-OpenSource-BicasTeam-Api|feature/profile-management|431353c|feat|added user controller|27-05|
|upc-OpenSource-BicasTeam-Api|feature/profile-management|554df5b|chore|implemented persistence base configuration|27-05|
|upc-OpenSource-BicasTeam-Api|feature/profile-management|5475552|fix|base configuration|27-05|
|upc-OpenSource-BicasTeam-Api|feature/shipments|cb61040|feat|added layers domain, infrastructure and application|28-05|
|upc-OpenSource-BicasTeam-Api|feature/shipments|b913385|feat|added resources and transform|28-05|
|upc-OpenSource-BicasTeam-Api|feature/shipments|9ee7c1c|feat|added shipment controller|28-05|
|upc-OpenSource-BicasTeam-Api|feature/shipments|8cdc129|chore|implemented interface layer base configuration, including configuration statements in main program|28-05|
|upc-OpenSource-BicasTeam-Api|feature/shipments|132998c|chore|added database context|28-05|
|upc-OpenSource-BicasTeam-Api|feature/communication-reports|49269c5|feat|added report aggregate|01-06|
|upc-OpenSource-BicasTeam-Api|feature/communication-reports|7c0c3ef|feat|added repositories and services for the model|01-06|
|upc-OpenSource-BicasTeam-Api|feature/communication-reports|328d93b|feat|added infrastructure and application for the report|01-06|
|upc-OpenSource-BicasTeam-Api|feature/communication-reports|77af4a6|feat|added resources and transform|01-06|
|upc-OpenSource-BicasTeam-Api|feature/communication-reports|a0a9813|chore|implemented interface layer base configuration, including configuration statements in main program|01-06|
|upc-OpenSource-BicasTeam-Api|feature/vehicles|0977fa1|feat|added aggregate vehicle|02-06|
|upc-OpenSource-BicasTeam-Api|feature/vehicles|0ce3c84|feat|added command and query services|02-06|
|upc-OpenSource-BicasTeam-Api|feature/vehicles|a6fac64|feat|added resources and transform|02-06|
|upc-OpenSource-BicasTeam-Api|feature/vehicles|ee78294|feat|added vehicle controller|02-06|
|upc-OpenSource-BicasTeam-Api|feature/vehicles|3395c27|chore|implemented interface layer base configuration in main program|02-06|

#### 5.2.3.4 Execution Evidence for Sprint Review
En esta sección, presentamos la evidencia de las pruebas realizadas durante el sprint. Hemos utilizado Gherkin para definir los escenarios de prueba y hemos registrado cada prueba en commits específicos en nuestro repositorio. A continuación, se muestra un registro de estos commits:

|Repository|Branch|Commit Id|Commit Message|Commit Message Body|Commited on (Date)|
| :- | :- | :- | :- | :- | :- |
|upc-OpenSource-BicasTeam-Api|feature/profile-management|328d93b|feat|add test for profile management|02-06|
|upc-OpenSource-BicasTeam-Api|feature/shipments|132998c|feat|add test for shipments|02-06|
|upc-OpenSource-BicasTeam-Api|feature/communication-reports|7c0c3ef|feat|add test for communication-reports|02-06|
|upc-OpenSource-BicasTeam-Api|feature/vehicles|e221a5b|feat|add test for vehicles|02-06|

#### 5.2.3.5 Services Documentation Evidence for Sprint Review
El equipo ha logrado despegar el web service de MoviGestion. Todas las historias de usuario asignadas para este sprint fueron completadas exitosamente. En primer lugar, nos enfocamos en el desarrollo y la implementación del web service que es fundamental para la aplicación MoviGestion. Este esfuerzo incluyó la creación de APIs RESTful, la integración segura y eficiente con la base de datos, y la implementación de pruebas exhaustivas para asegurar la fiabilidad y el rendimiento del servicio. 

Capturas de pantalla:

TODO: CAPTURAS DEL WEB SERVICE DESPLEGADO
![CAPTURAS DEL WEB SERVICE DESPLEGADO]()

#### 5.2.3.6 Software Deployment Evidence for Sprint Review
Durante el Sprint 3, el equipo ha trabajado intensamente en la documentación de los Web Services desarrollados. Utilizando OpenAPI, hemos documentado todos los endpoints relevantes, asegurando que cada uno de ellos esté claramente definido y accesible para los desarrolladores. Esta documentación es esencial para garantizar una integración fluida y eficiente del web service con otros componentes de la aplicación y con sistemas externos.

|&emsp;&emsp;&emsp;&emsp;Endpoint|&emsp;&emsp;&emsp;&emsp;Acción Implementada|&emsp;&emsp;&emsp;&emsp;Verbo HTTP|&emsp;&emsp;&emsp;&emsp;Sintaxis de Llamada|&emsp;&emsp;&emsp;&emsp;Parámetros|&emsp;&emsp;&emsp;&emsp;Ejemplo de Response|
| :- | :- | :- | :- | :- | :- |
|&emsp;&emsp;&emsp;&emsp;/report|&emsp;&emsp;&emsp;&emsp;Crear reporte|&emsp;&emsp;&emsp;&emsp;POST|&emsp;&emsp;&emsp;&emsp;/api/v1/report|&emsp;&emsp;&emsp;&emsp;|&emsp;&emsp;&emsp;&emsp;|
|&emsp;&emsp;&emsp;&emsp;/report/{id}|&emsp;&emsp;&emsp;&emsp;Obtener reporte por Id|&emsp;&emsp;&emsp;&emsp;GET|&emsp;&emsp;&emsp;&emsp;/api/v1/report/{id}|&emsp;&emsp;&emsp;&emsp;id|&emsp;&emsp;&emsp;&emsp;|
|&emsp;&emsp;&emsp;&emsp;/report/user/{userId}|&emsp;&emsp;&emsp;&emsp;Obtener reportes por id de usuario|&emsp;&emsp;&emsp;&emsp;GET|&emsp;&emsp;&emsp;&emsp;/api/v1/report/users/{userId}|&emsp;&emsp;&emsp;&emsp;userId|&emsp;&emsp;&emsp;&emsp;|
|&emsp;&emsp;&emsp;&emsp;/report|&emsp;&emsp;&emsp;&emsp;Obtener todo los reportes|&emsp;&emsp;&emsp;&emsp;GET|&emsp;&emsp;&emsp;&emsp;/api/v1/report|&emsp;&emsp;&emsp;&emsp;none|&emsp;&emsp;&emsp;&emsp;|
|&emsp;&emsp;&emsp;&emsp;/vehicle|&emsp;&emsp;&emsp;&emsp;Crear vehiculo|&emsp;&emsp;&emsp;&emsp;POST|&emsp;&emsp;&emsp;&emsp;/api/v1/vehicle|&emsp;&emsp;&emsp;&emsp;|&emsp;&emsp;&emsp;&emsp;|
|&emsp;&emsp;&emsp;&emsp;/vehicle/{id}|&emsp;&emsp;&emsp;&emsp;Obtener vehículo por Id|&emsp;&emsp;&emsp;&emsp;GET|&emsp;&emsp;&emsp;&emsp;/api/v1/vehicle/{id}|&emsp;&emsp;&emsp;&emsp;id|&emsp;&emsp;&emsp;&emsp;|
|&emsp;&emsp;&emsp;&emsp;/vehicle|&emsp;&emsp;&emsp;&emsp;Obtener todo los vehículos|&emsp;&emsp;&emsp;&emsp;GET|&emsp;&emsp;&emsp;&emsp;/api/v1/vehicle|&emsp;&emsp;&emsp;&emsp;none|&emsp;&emsp;&emsp;&emsp;|
|&emsp;&emsp;&emsp;&emsp;/shipment|&emsp;&emsp;&emsp;&emsp;Crear envío|&emsp;&emsp;&emsp;&emsp;POST|&emsp;&emsp;&emsp;&emsp;/api/v1/shipment|&emsp;&emsp;&emsp;&emsp;|&emsp;&emsp;&emsp;&emsp;|
|&emsp;&emsp;&emsp;&emsp;/shipment/{id}|&emsp;&emsp;&emsp;&emsp;Obtener envío por Id|&emsp;&emsp;&emsp;&emsp;GET|&emsp;&emsp;&emsp;&emsp;/api/v1/shipment/{id}|&emsp;&emsp;&emsp;&emsp;id|&emsp;&emsp;&emsp;&emsp;|
|<p>&emsp;&emsp;&emsp;&emsp;/shipment/user/{userId}</p><p>&emsp;&emsp;&emsp;&emsp;</p>|&emsp;&emsp;&emsp;&emsp;Obtener envíos por id de usuario|&emsp;&emsp;&emsp;&emsp;GET|&emsp;&emsp;&emsp;&emsp;/api/v1/shipment/users/{userId}|&emsp;&emsp;&emsp;&emsp;userId|&emsp;&emsp;&emsp;&emsp;|
|&emsp;&emsp;&emsp;&emsp;/shipment|&emsp;&emsp;&emsp;&emsp;Obtener todo los envíos|&emsp;&emsp;&emsp;&emsp;GET|&emsp;&emsp;&emsp;&emsp;/api/v1/shipment|&emsp;&emsp;&emsp;&emsp;none|&emsp;&emsp;&emsp;&emsp;|
|&emsp;&emsp;&emsp;&emsp;/user|&emsp;&emsp;&emsp;&emsp;Crear perfil|&emsp;&emsp;&emsp;&emsp;POST|&emsp;&emsp;&emsp;&emsp;/api/v1/user|&emsp;&emsp;&emsp;&emsp;|&emsp;&emsp;&emsp;&emsp;|
|&emsp;&emsp;&emsp;&emsp;/user/{id}|&emsp;&emsp;&emsp;&emsp;Obtener perfil por Id|&emsp;&emsp;&emsp;&emsp;GET|&emsp;&emsp;&emsp;&emsp;/api/v1/user/{id}|&emsp;&emsp;&emsp;&emsp;id|&emsp;&emsp;&emsp;&emsp;|
|&emsp;&emsp;&emsp;&emsp;/user|&emsp;&emsp;&emsp;&emsp;Obtener todo los perfil|&emsp;&emsp;&emsp;&emsp;GET|&emsp;&emsp;&emsp;&emsp;/api/v1/user|&emsp;&emsp;&emsp;&emsp;none|&emsp;&emsp;&emsp;&emsp;|

CAPTURAS DE INTERACCION CON LA DOCUMENTACION:
A continuación, se incluyen capturas de pantalla que muestran la interacción con la documentación de los web services, utilizando datos de muestra.

1. Endopoint de crear Reporte (/report) - POST

![1]()

Descripción: La captura muestra la documentación del endpoint para crear un nuevo reporte, incluyendo los parámetros requeridos y un ejemplo del response.

1. Endpoint de Obtener Reporte por ID (/report/{id}) - GET:

![2]()

Descripción: La captura presenta la documentación del endpoint para obtener un reporte por ID, con la sintaxis de llamada y un ejemplo de response.

1. Endpoint de Crear Vehículo (/vehicle) - POST:

![3]()

Descripción: La imagen muestra cómo documentamos la creación de un nuevo vehículo, especificando los parámetros y un ejemplo del response.

1. Endpoint de Obtener Envío por ID (/shipment/{id}) - GET:

![4]()

 Descripción: La captura ilustra la documentación del endpoint para obtener un envío por ID, incluyendo un ejemplo del request y response.

 #### <a name="_heading=h.ikcf394glpjk"></a>**URL del Repositorio:**
   El código fuente del Web Services se encuentran en el siguiente repositorio:

- **Repositorio de Web Service:** [https://github.com/upc-OpenSource-BicasTeam/upc-OpenSource-BicasTeam-api.git](https://github.com/upc-OpenSource-BicasTeam/upc-OpenSource-BicasTeam-api.git)

#### 5.2.3.7 Team Collaboration Insights during Sprint
Durante el Sprint 3, llevamos a cabo el despliegue de nuestra web service en GitHub Pages. A continuación, detallamos los pasos realizados:

- Creación del Repositorio en GitHub: Iniciamos creando un repositorio dedicado en GitHub para nuestro proyecto de web service.
- Configuración de la Rama main: Aseguramos que la rama principal del repositorio se llamará main, ya que esta rama sirve como base para el despliegue automático.
- Preparación del Contenido: Desarrollamos y diseñamos nuestra web service, asegurándonos de que todos los archivos y recursos necesarios estuvieran presentes en el repositorio.
- Generación del enlace del hosting: Creamos nuestra cuenta en el hosting, le asignamos un nombre y desplegamos el web service en la URL proporcionada por el hosting.

#### 5.2.3.8 Team Collaboration Insights During Sprint
Durante este segundo Sprint, hemos avanzado el desarrollo del web service y hemos colaborado estrechamente en su implementación. La colaboración entre los miembros del equipo se refleja en los diversos commits realizados en el repositorio de GitHub, los cuales han sido debidamente documentados en las capturas de pantalla adjuntas. Para asegurar una colaboración efectiva, hemos implementado GitFlow como nuestra metodología de trabajo colaborativo en Git. Con GitFlow, hemos creado ramas para cada una de las secciones de nuestro web service. Esto nos ha permitido trabajar de manera organizada y centrarnos en completar correctamente las historias de usuario designadas para cada sección. En cuanto a la elaboración del código, hemos asignado a cada miembro del equipo una sección específica del web service. Esta estrategia nos ha permitido avanzar de manera más eficiente y completar el trabajo antes de la fecha de entrega. Además, hemos realizado reuniones adicionales para intercambiar ideas y resolver cualquier duda o problema que pudiera surgir durante el desarrollo del web service. Estas sesiones han contribuido de manera positiva al éxito del proyecto. A continuación, presentamos algunas capturas de pantalla que muestran los commits realizados por los miembros del equipo en GitHub:

TODO: Captura gitHub de commits
![Team Collaobraiton]()

## 5.3  Validation Interviews

### 5.3.1 Diseño de Entrevsitas
**Para los Empresarios:**

- ¿Cuál es su opinión general sobre la plataforma MoviGestion tras la demostración?
- ¿Qué características de MoviGestion le resultaron más útiles para la gestión de su flota?
- ¿Hay alguna función que no encontró en MoviGestion y que consideraría esencial para su operación?
- ¿Cómo evalúa la interfaz de usuario en términos de facilidad de uso y navegación?
- ¿Cuánto tiempo cree que le tomaría a su equipo adaptarse al uso de MoviGestion?
- ¿Cuáles son los principales desafíos que enfrenta actualmente en la gestión de su flota?
- ¿Cómo cree que MoviGestion podría ayudarle a superar esos desafíos?
- ¿Qué tan útil considera la funcionalidad de registro de incidencias en la plataforma?
- ¿Qué aspectos de la gestión de envíos exitosos le parecen más críticos para su operación?
- ¿Está dispuesto a recomendar MoviGestion a otros empresarios del sector? ¿Por qué?
- ¿Cómo valora la seguridad de la información y los datos en la plataforma MoviGestion?

**Para los Transportistas:**

- ¿Cuál fue su impresión general de la plataforma MoviGestion después de la demostración?
- ¿Qué tan fácil le resultó navegar y utilizar las funciones de MoviGestion?
- ¿Qué características de MoviGestion le parecieron más útiles para su trabajo diario?
- ¿Hay alguna función que no encontró en MoviGestion y que consideraría útil para su labor?
- ¿Cómo cree que MoviGestion podría ayudarle a realizar su trabajo de manera más eficiente?
- ¿Qué tan útil considera la funcionalidad de registro de incidencias para reportar problemas en tiempo real?
- ¿Qué tan fácil le resultó el proceso de seguimiento de envíos en MoviGestion?
- ¿Cómo valora la capacidad de monitorear los sitios de entrega a través de la plataforma?
- ¿Le parece intuitiva la interfaz de usuario de MoviGestion? ¿Hay algo que cambiaría?
- ¿Cómo le gustaría que MoviGestion le notificara sobre nuevas tareas o cambios en las entregas?
- ¿Qué mejoras le gustaría ver en futuras actualizaciones de la plataforma?
- ¿Cómo valora la seguridad de la información y los datos en la plataforma MoviGestion?
- ¿Cree que MoviGestion le ayudaría a reducir el tiempo de inactividad y aumentar la productividad?
- ¿Estaría dispuesto a recomendar MoviGestion a otros transportistas? ¿Por qué?

### 5.3.2 Registro de Entrevistas
1. ### <a name="_heading=h.mqpm42spx03x"></a>***Segmento objetivo: Empresarios***
   **Entrevista N°1:**

![Entrevista 1](/assets/chapter05%20-%20reviews/entrevistaBussinesman1.png)

- **Datos principales:**
- **Nombre completo del entrevistado:** Vladimir Quique Espinoza
- **Edad:** 28 años
- **Distrito: Lima, San Isidro**
- **Link: [Aquí](https://upcedupe-my.sharepoint.com/:v:/g/personal/u20211c221_upc_edu_pe/EZVsHR_m-J1Hp3uOn85uHiYBdFAUAUr8A965BEV1SLvNzw?e=dtY7hW) **

- **Resumen:** Durante la entrevista con Vladimir nos comentan que él es actualmente el gerente de la empresa cargos express Espinoza,  una empresa familiar con una trayectoria de más de 10 años en el rubro de cargas,  la empresa fue fundada por su papá quien  era un antiguo trabajador en los puertos de callao al ver la necesidad de muchas cargas se le propuso formar una empresa de transporte de cargas.
En la primera parte Vladimir nos Comenta sobre nuestra aplicación web desarrollada los siguientes detalles, sobre el landing page  está bien diseñada con interfaz amigable y un color bien atractivo los botones funcionales,  tiene secciones bien organizadas más allá de eso me llama la atención el objetivo que tienen de su producto de software de mejorar la gestión y organización en rubros de transporte. Por otro lado, de la aplicación web es muy buena desde la Perspectiva de mi Visión también lo sección de botones están bien organizados y funcionales y tambien optaría nuestro software porque me ayudaría a gestionar y organizar mejor su empresa.


**Entrevista N°2:**

![Entrevsita 2](/assets/chapter05%20-%20reviews/entrevistaBussinesman2.png)

- **Datos principales:**
- **Nombre completo del entrevistado:** Abraham Quenta
- **Edad:** 28 años
- **Distrito:** Tacna
- **Link: [Video_20240605003047183_by_VideoShow.mp4**](https://upcedupe-my.sharepoint.com/:v:/g/personal/u20191a453_upc_edu_pe/EVoUsQcedjZHkRdxa-Z7_YUBLTmGiwmlqNwTjrWrYxZ4Bw?e=3pSUjY&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)**
- **Inicio de la entrevista:** 0:00
- **Duración:** 10:45
- **Resumen:** Abraham se presenta como un profesional del transporte con 5 años de experiencia en el sector transporte provincial, cuya ruta principal es de Tacna a Puno. Comenta sobre la página de destino de su servicio, que incluye información sobre los servicios ofrecidos y permite la personalización del idioma. Abraham explora las características y funcionalidades del sitio web, como la gestión de la flota, los informes de los conductores y la gestión de vehículos, y aprecia el aspecto organizativo de la plataforma, señalando que es fácil encontrar las funciones deseadas. Abraham menciona algunos problemas menores con la visibilidad del texto y la navegación, pero en general considera que la interfaz de usuario es clara y sencilla. información del vehículo, así como las estrategias de marketing y el diseño de la página de destino, pero en general. considera que la aplicación es valiosa, especialmente para monitorear las actividades de los conductores.

**Segmento objetivo: Transportistas**

**Entrevista N°1:**

![Entrevsita 3](/assets/chapter05%20-%20reviews/entrevistaCarrier1.png)

- **Datos principales:**
- **Nombre completo del entrevistado:** Martín Merino Ávila
- **Edad:** 50 años
- **Distrito:** Villa El Salvador
- **Link: [https://upcedupe-my.sharepoint.com/transportista-Martín Merino Ávila](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202217633_upc_edu_pe/EY5rIHwdoYJEo1060clcg08Bj9EUW4PKzVWG0qSQZ9iLKw?e=qVv4x8)**
- **Inicio de entrevista:** 0:00
- **Duración:** 7:50
- **Resumen:** El transportista Martín Merino Ávila expresó algunas dudas sobre la plataforma MoviGestion, especialmente en relación a la cantidad de tiempo que podría tomar adaptarse a una nueva herramienta, pero tras la demostración y uso práctico, encontró la interfaz más intuitiva de lo que esperaba. Nos comentó que las funciones de registro de incidencias eran lo mejor. Aunque cree que la plataforma podría beneficiarse de más opciones de personalización, le gusta la seguridad de la información. Al final, Martín reconoció que MoviGestion es una opción sólida y estaría dispuesta a recomendarla a otros transportistas.

**Entrevista N°2:**

![Entrevsita 4](/assets/chapter05%20-%20reviews/entrevistaCarrier2.png)

- **Datos principales:**
- **Nombre completo del entrevistado:** Ricardo Chate Flores
- **Edad:** 45 años
- **Distrito:** Cercado de Lima
- **Link: [https://upcedupe-my.sharepoint.com/transportista-Ricardo Chate Flores](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202217633_upc_edu_pe/EXSD46lHMXBHhtXU68u21MAB1k4GPVrGtb73aiHuhk-O4A?e=baM5qv)**
- **Inicio de entrevista:** 0:00
- **Duración:** 8:00
- **Resumen:** El transportista Ricardo Chate Flores expresó una opinión positiva sobre MoviGestion, destacando su facilidad de uso y navegación intuitiva. Consideró útiles las funciones de registro de incidencias y seguimiento de envíos para su trabajo diario. Valora la capacidad de monitorear los sitios de entrega y mencionó que la plataforma podría ayudarle a trabajar de manera más eficiente. Aunque satisfecho con las funcionalidades actuales, sugirió la necesidad de notificaciones más personalizables. José destacó la seguridad de la información y está dispuesto a recomendar MoviGestion a otros transportistas, ya que cree que puede reducir el tiempo de inactividad y aumentar la productividad.

**Entrevista N°3:**

![Entrevsita 5](/assets/chapter05%20-%20reviews/entrevistaCarrier3.png)

- **Datos principales:**
- **Nombre completo del entrevistado:** Víctor Cuba Bautista
- **Edad:** 42 años
- **Distrito:** Villa El Salvador
- **Link: [https://upcedupe-my.sharepoint.com/transportista-Víctor Cuba Bautista](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202217633_upc_edu_pe/Ee0tJI_1TaVDlx1FOyZIwjwBiTQSNEtbkeaMh9ggxyFgFQ?e=vercnA)**
- **Inicio de entrevista:** 0:00
- **Duración:** 4:50
- **Resumen:** El transportista Víctor Cuba Bautista tras probar la plataforma, reconoció que el uso de las funciones eran más sencillos de lo que esperaba. Encontró especialmente útil el registro de incidencias en tiempo real. Aunque le gustaría ver mejoras en algunas funcionalidades adicionales, valora la capacidad de monitorear los sitios de entrega y la seguridad de los datos proporcionada por la plataforma. Al final, Víctor concluyó que MoviGestion es una herramienta efectiva que puede mejorar su eficiencia y reducir el tiempo de inactividad, y estaría dispuesto a recomendarla a otros transportistas.

### 5.3.3 Evaluaciones segun heuristicas
Esta sección contiene el proceso de evaluación de las sesiones de validación basado en heurísticas, considerando heurísticas de usabilidad, arquitectura de información e inclusive design de la experiencia propuesta. Para esto la sección usamos la estructura del formato para evaluaciones de heurísticas indicado.

**UX Heuristics & Principles Evaluation**

**Usability – Inclusive Design – Information Architecture**
\***


**CARRERA                	: Ingeniería de Software**

**CURSO                    	: Aplicaciones Web**

**SECCIÓN                   	: SV54**

**AUDITOR                 	: Bicas Team**

**CLIENTE                  	: MoviGestion**
1. ## <a name="_heading=h.3ibjgvegxoc5"></a>** 
   **SITE o APP A EVALUAR:**

   **MoviGestion**

   **TAREAS A EVALUAR:**

   *El alcance de esta evaluación incluye la revisión de la usabilidad de las siguientes tareas:*

*1.* 	*Gestión y edición de perfil de usuario.*

*2.     Visualización de asignación de envíos que pertenecen a cada transportista*

*3. 	Agregar un nuevo vehículo a la flota de vehículos.*

*4. 	Eliminar un vehículo de la flota de vehículos.*

*5. 	Visualización de alertas de cada transportista.*

**ESCALA DE SEVERIDAD:**

*Los errores serán puntuados tomando en cuenta la siguiente escala de severidad*

|***Nivel***|***Descripción***|
| :- | :- |
|*1*|*Problema superficial: puede ser fácilmente superado o hasta ignorado por el usuario ó ocurre con muy poca frecuencia. El error no necesita ser arreglado de forma inmediata en la mayoría de las casos, a no ser que exista disponibilidad de tiempo.*|
|*2*|*Problema menor: puede ocurrir un poco más frecuentemente o es un poco más difícil de superar para el usuario. Se le debería asignar una prioridad baja para resolverlo de cara antes de la siguiente entrega o actualización.*|
|*3*|*Problema mayor: ocurre frecuentemente o los usuarios no son capaces de resolverlos. Es importante que sean corregidos y se les debe asignar una prioridad alta.*|
|*4*|*Problema muy grave: un error de gran impacto que impide al usuario continuar con el uso de la herramienta. Es imperativo que sea corregido antes del lanzamiento.*|


**TABLA RESUMEN:**

|*#*|*Problema*|*Escala de severidad*|*Heurística/Principio violada(o)*|
| :-: | :-: | :-: | :-: |
|*1*|*Incluye un botón “See More” pero no tiene funcionalidad*|*3*|*Information Architecture: Is it usable?*|
|*2*|*No parece haber consistencia en la forma en que se presentan las opciones para actualizar la información*|*2*|*Usability: Consistencia y estándares*|
|*3*|*Información de pagos no está claramente presentada*|*3*|*Usability: Visibilidad del estado del sistema*|
|*4*|*No funciona cancelar el agregado de un vehículo.*|*2*|*Usability: Libertad y control del usuario*|





**DESCRIPCIÓN DE PROBLEMAS:**

*PROBLEMA #1:* 

*Severidad: 3*

*Heurística violada: Information Architecture: Is it usable?*

*Problema:*

*La aplicación incluye un botón “See More” pero no tiene funcionalidad, lo que confunde a los usuarios y les impide acceder a contenido adicional esperado.*

![H1](/assets/chapter05%20-%20heuristc%20and%20final/h1.png)

*Recomendación:*

*Eliminar el botón “See More” si no hay contenido adicional disponible, o implementar la funcionalidad esperada para que los usuarios puedan acceder a más información.*

*PROBLEMA #2:* 

*Severidad: 2*

*Heurística violada: Usability - Consistencia y estándares*

*Problema:*

*La interfaz de Settings incluye campos para Nickname, Bio, Email y Avatar, pero no parece haber consistencia en la forma en que se presentan las opciones para actualizar la información. Por ejemplo, el botón ‘Choose’ para actualizar el avatar está separado del campo ‘Avatar’, lo que podría confundir a los usuarios.*

![H2](/assets/chapter05%20-%20heuristc%20and%20final/h2.png)

*Recomendación:*

*Asegurar que todos los campos de entrada y botones relacionados estén agrupados de manera coherente y clara para mejorar la comprensión y la facilidad de uso.*

*PROBLEMA #3:* 

*Severidad: 3*

*Heurística violada: Usability: Visibilidad del estado del sistema*

*Problema:*

*La información relacionada con Organization no está claramente presentada, lo que puede causar confusión a la hora de querer tener información y dificulta la asignación de envíos.*

![H3](/assets/chapter05%20-%20heuristc%20and%20final/h3.png)

*Recomendación:*

*Mejorar la presentación y accesibilidad de la información relacionada con "Organization" puede mejorar significativamente la experiencia del usuario y facilitar la asignación de envíos en la aplicación.* 

*PROBLEMA #4:* 

*Severidad: 2*

*Heurística violada: Usability: Libertad y control del usuario*

*Problema:*

*Al momento de ingresar los datos del nuevo vehículo, no se puede cerrar hasta darle darle al botón “Close” y luego se tiene que eliminar en el botón “Delete Vehicle”, esto obliga a agregar nuevos carros no deseados, también incrementando así la cantidad de esfuerzo del usuario.*

![H4](/assets/chapter05%20-%20heuristc%20and%20final/h4.png)

*Recomendación:*

*Hacer que el botón "Close" tenga la funcionalidad para cerrar la ventana emergente sin guardar los datos del vehículo ingresados.*

---

## 5.4 Video About The Product

<https://upcedupe-my.sharepoint.com/:v:/g/personal/u202116207_upc_edu_pe/EVzNfjl7ZRtAvgrVtGxeeSEB24lFo7SCNzRMpCjNjY7bRg?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=sBmRa5>

