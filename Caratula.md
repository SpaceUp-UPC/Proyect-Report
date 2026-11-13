<p align="center">
    <img src="./assets/UPC_logo_transparente.png" alt="UPC Logo" width="80"/>
</p>

<p align="center">
    Universidad Peruana de Ciencias Aplicadas
</p>

<p align="center">
    Carrera de Ingeniería de Software
</p>

<br>

<h2 align="center">1ASI0572</h2>

<h2 align="center">Desarrollo de Soluciones IoT</h2>

<p align="center">NRC</p>

<h3 align="center">8735</h3>

<h1 align="center">Informe del Trabajo Final</h1>

<p align="center">Docente</p>

<h3 align="center">León Baca, Marco Antonio</h3>

<br>

<p align="center">Equipo</p>

<h3 align="center">SpaceUp</h3>

<br>

<p align="center">Proyecto</p>

<h3 align="center">SENTRYA</h3>

<br>

<h3 align="center">Integrantes</h3>

<table align="center" border="0" style="border-collapse: collapse; border: none;">
    <thead>
        <tr>
            <th style="border: none; text-align: left; padding: 4px 15px;">Código</th>
            <th style="border: none; text-align: left; padding: 4px 15px;">Apellidos y Nombres</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td style="border: none; padding: 4px 15px;">u202213989</td>
            <td style="border: none; padding: 4px 15px;">Martínez Valdivia, José Luis</td>
        </tr>
        <tr>
            <td style="border: none; padding: 4px 15px;">u202313458</td>
            <td style="border: none; padding: 4px 15px;">Taipe Sangama, Jorge Francisco</td>
        </tr>
        <tr>
            <td style="border: none; padding: 4px 15px;">u202122876</td>
            <td style="border: none; padding: 4px 15px;">Serrano Uchuya, Gerald Patricio</td>
        </tr>
        <tr>
            <td style="border: none; padding: 4px 15px;">u202120011</td>
            <td style="border: none; padding: 4px 15px;">Martinez Gaona, Pablo Afranio</td>
        </tr>
        <tr>
            <td style="border: none; padding: 4px 15px;">u202319025</td>
            <td style="border: none; padding: 4px 15px;">Ventosilla Trujillo, Anderson Ricardo</td>
        </tr>
        <tr>
            <td style="border: none; padding: 4px 15px;">u201711828</td>
            <td style="border: none; padding: 4px 15px;">Torrejon Navarro, Braulio Rodrigo</td>
        </tr>
    </tbody>
</table>

<br>

<p align="center">
    Período 202620
</p>


<div style="page-break-before: always;"></div>

## Registro de Versiones del Informe

| Versión | Fecha      | Autor(es)      | Descripción de modificación       |
|-------|----------|--------------------------------------------------------|---------|
| 0.1     | 09/09/2026 |    Equipo SpaceUp       |     Se completaron los capitulos del 1 al 4     |
| 0.2     | 05/10/2026 |    Equipo SpaceUp       |     Se completaron los capitulos del 5 y 6     |
| 0.3     | 10/11/2026 |    Equipo SpaceUp       |     Se completo el capitulo 6     |

<div style="page-break-before: always;"></div>

# Tabla de Contenidos

- Capítulo I: Presentación   
  - [1.1 Startup Profile](#11-startup-profile)   
    - [1.1.1 Descripción de la Startup](#111-descripcion-de-la-startup)   
    - [1.1.2 Perfiles de integrantes del equipo](#112-perfiles-de-integrantes-del-equipo)   

  - [1.2 Solution Profile](#12-solution-profile)   
    - [1.2.1 Antecedentes y problemática](#121-antecedentes-y-problematica)   
    - [1.2.2 Lean UX Process](#122-lean-ux-process)   
      - [1.2.2.1 Lean UX Problem Statements](#1221-lean-ux-problem-statements)   
      - [1.2.2.2 Lean UX Assumptions](#1222-lean-ux-assumptions)   
      - [1.2.2.3 Lean UX Hypothesis Statements](#1223-lean-ux-hypothesis-statements)   
      - [1.2.2.4 Lean UX Canvas](#1224-lean-ux-canvas)   

  - [1.3 Segmentos Objetivo](#13-segmentos-objetivo)   


- Capítulo II: Requirements Development and Software Solution Design   
  - [2.1 Competidores](#21-competidores)   
    - [2.1.1 Análisis competitivo](#211-analisis-competitivo)   
    - [2.1.2 Estrategias y tácticas frente a competidores](#212-estrategias-y-tacticas-frente-a-competidores)   

  - [2.2 Entrevistas](#22-entrevistas)   
    - [2.2.1 Diseño de entrevistas](#221-diseno-de-entrevistas)   
    - [2.2.2 Registro de entrevistas](#222-registro-de-entrevistas)   
    - [2.2.3 Análisis de entrevistas](#223-analisis-de-entrevistas)   

  - [2.3 Needfinding](#23-needfinding)   
    - [2.3.1 User Personas](#231-user-personas)   
    - [2.3.2 User Task Matrix](#232-user-task-matrix)   
    - [2.3.3 User Journey Mapping](#233-user-journey-mapping)   
    - [2.3.4 Empathy Mapping](#234-empathy-mapping)   

  - [2.4 Big Picture EventStorming](#24-big-picture-eventstorming)   

  - [2.5 Ubiquitous Language](#25-ubiquitous-language)   


- Capítulo III: Requirements Specification   
  - [3.1 User Stories](#31-user-stories)   
  - [3.2 Impact Mapping](#32-impact-mapping)   
  - [3.3 Product Backlog](#33-product-backlog)   


- Capítulo IV: Solution Software Design   
  - [4.1 Strategic-Level Domain-Driven Design](#41-strategic-level-domain-driven-design)   
    - [4.1.1 Design-Level EventStorming](#411-design-level-eventstorming)   
      - [4.1.1.1 Candidate Context Discovery](#4111-candidate-context-discovery)   
      - [4.1.1.2 Domain Message Flows Modeling](#4112-domain-message-flows-modeling)   
      - [4.1.1.3 Bounded Context Canvases](#4113-bounded-context-canvases)   

    - [4.1.2 Context Mapping](#412-context-mapping)   

    - [4.1.3 Software Architecture](#413-software-architecture)   
      - [4.1.3.1 Software Architecture System Landscape Diagram](#4131-software-architecture-system-landscape-diagram)   
      - [4.1.3.2 Software Architecture Context Level Diagrams](#4132-software-architecture-context-level-diagrams)   
      - [4.1.3.3 Software Architecture Container Level Diagrams](#4133-software-architecture-container-level-diagrams)   
      - [4.1.3.4 Software Architecture Deployment Diagrams](#4134-software-architecture-deployment-diagrams)   

  - [4.2 Tactical-Level Domain-Driven Design](#42-tactical-level-domain-driven-design)   
    - [4.2.X Bounded Context: &lt;Bounded Context Name&gt;](#42x-bounded-context-bounded-context-name)   
      - [4.2.X.1 Domain Layer](#42x1-domain-layer)   
      - [4.2.X.2 Interface Layer](#42x2-interface-layer)   
      - [4.2.X.3 Application Layer](#42x3-application-layer)   
      - [4.2.X.4 Infrastructure Layer](#42x4-infrastructure-layer)   
      - [4.2.X.5 Bounded Context Software Architecture Component Level Diagrams](#42x5-bounded-context-software-architecture-component-level-diagrams)   
      - [4.2.X.6 Bounded Context Software Architecture Code Level Diagrams](#42x6-bounded-context-software-architecture-code-level-diagrams)   
        - [4.2.X.6.1 Bounded Context Domain Layer Class Diagrams](#42x61-bounded-context-domain-layer-class-diagrams)   
        - [4.2.X.6.2 Bounded Context Database Design Diagram](#42x62-bounded-context-database-design-diagram)   

  - [5.1 Style Guidelines](#51-style-guidelines)  
    - [5.1.1 General Style Guidelines](#511-general-style-guidelines)  
    - [5.1.2 Web, Mobile and IoT Style Guidelines](#512-web-mobile-and-iot-style-guidelines)  

  - [5.2 Information Architecture](#52-information-architecture)  
    - [5.2.1 Organization Systems](#521-organization-systems)  
    - [5.2.2 Labeling Systems](#522-labeling-systems)  
    - [5.2.3 SEO Tags and Meta Tags](#523-seo-tags-and-meta-tags)  
    - [5.2.4 Searching Systems](#524-searching-systems)  
    - [5.2.5 Navigation Systems](#525-navigation-systems)  

  - [5.3 Landing Page UI Design](#53-landing-page-ui-design)  
    - [5.3.1 Landing Page Wireframe](#531-landing-page-wireframe)  
    - [5.3.2 Landing Page Mock-up](#532-landing-page-mock-up)  

  - [5.4 Applications UX/UI Design](#54-applications-uxui-design)  
    - [5.4.1 Applications Wireframes](#541-applications-wireframes)  
    - [5.4.2 Applications Wireflow Diagrams](#542-applications-wireflow-diagrams)  
    - [5.4.3 Applications Mock-ups](#543-applications-mock-ups)  
    - [5.4.4 Applications User Flow Diagrams](#544-applications-user-flow-diagrams)  

  - [5.5 Applications Prototyping](#55-applications-prototyping)  

  - [5.6 IoT Device Design](#56-iot-device-design)  


  - [6.1 Software Configuration Management](#61-software-configuration-management)  
    - [6.1.1 Software Development Environment Configuration](#611-software-development-environment-configuration)  
    - [6.1.2 Source Code Management](#612-source-code-management)  
    - [6.1.3 Source Code Style Guide & Conventions](#613-source-code-style-guide--conventions)  
    - [6.1.4 Software Deployment Configuration](#614-software-deployment-configuration)  

- [6.2 Landing Page, Services & Applications Implementation](#62-landing-page-services--applications-implementation)  
  - [6.2.1 Sprint 1](#62x-sprint-n)  
    - [6.2.1.1 Sprint Planning 1. ](#62x1)  
    - [6.2.1.2 Aspect Leaders and Collaborators. ](#62x2)  
    - [6.2.1.3 Sprint Backlog 1. ](#62x3)  
    - [6.2.1.4 Development Evidence for Sprint Review. ](#62x4)  
    - [6.2.1.5 Testing Suite Evidence for Sprint Review.](#62x5)  
    - [6.2.1.6 Execution Evidence for Sprint Review. ](#62x6)  
    - [6.2.1.7 Services Documentation Evidence for Sprint Review. ](#62x7)  
    - [6.2.1.8 Software Deployment Evidence for Sprint Review. ](#62x8)  
    - [6.2.1.9 Team Collaboration Insights during Sprint. ](#62x9)
  - [6.2.2 Sprint 2](#62x-sprint-n)  
    - [6.2.2.1 Sprint Planning 1. ](#62x1)  
    - [6.2.2.2 Aspect Leaders and Collaborators. ](#62x2)  
    - [6.2.2.3 Sprint Backlog 1. ](#62x3)  
    - [6.2.2.4 Development Evidence for Sprint Review. ](#62x4)  
    - [6.2.2.5 Testing Suite Evidence for Sprint Review.](#62x5)  
    - [6.2.2.6 Execution Evidence for Sprint Review. ](#62x6)  
    - [6.2.2.7 Services Documentation Evidence for Sprint Review. ](#62x7)  
    - [6.2.2.8 Software Deployment Evidence for Sprint Review. ](#62x8)  
    - [6.2.2.9 Team Collaboration Insights during Sprint. ](#62x9)  





     


**ABET – EAC - Student Outcome 7**

La capacidad de adquirir y aplicar nuevos
conocimientos según sea necesario,
utilizando estrategias de aprendizaje
apropiadas.

En el siguiente cuadro se describe las acciones realizadas y enunciados de conclusiones por parte del grupo,
que permiten sustentar el haber alcanzado el logro del ABET – EAC - Student Outcome 7.


| Criterio específico | Acciones realizadas | Conclusiones |
| :--- | :--- | :--- |
| **Actualiza conceptos y conocimientos necesarios para su desarrollo profesional y en especial para su proyecto en soluciones de software.** | **Pablo Martinez Gaona:** <br/> **AV1:** Realicé todo el capítulo 1. Esta entrega me permitió ampliar mis conocimientos sobre el planteamiento de soluciones IoT y comprender mejor cómo relacionar las necesidades de los usuarios con dispositivos, funcionalidades y procesos de software. <br/> **TB1:** Lideré la corrección de los diagramas de arquitectura de software (C4 Model), asegurando coherencia con el diseño estratégico. Coordiné el Sprint Backlog 1 y la matriz de responsabilidades. <br/> **AV2:** Participé en el desarrollo del Sprint 2, contribuyendo a la implementación de los microservicios de SENTRYA y a la organización de sus componentes. Esta experiencia me permitió fortalecer mis conocimientos sobre arquitectura de microservicios, separación de responsabilidades y comunicación entre servicios, comprendiendo su importancia para construir soluciones escalables y mantenibles. <br/><br/> **Jose Luis Martínez Valdivia:** <br/> **AV1:** Contribuí en el desarrollo del capítulo 4 - Definición de Bounded Contexts y sus componentes. El desarrollo del AV1 me permitió comentar y enriquecer mis conocimientos de DDD y la forma en la que se debaten ideas para implementar una solución de Servicio Web. <br/> **TB1:** Lideré la mejora de los User Stories en formato Gherkin para todos los stories del backlog. Coordiné la sección de Testing Suite Evidence para el Sprint Review. <br/> **AV2:** Contribuí en el desarrollo del Sprint 2 mediante la implementación de microservicios, aplicando los conceptos de Domain-Driven Design (DDD) y la separación de responsabilidades entre los distintos componentes del sistema. Esta experiencia me permitió profundizar mis conocimientos sobre arquitectura de software, integración de servicios y desarrollo de APIs REST, fortaleciendo mis habilidades para implementar soluciones modulares y escalables. <br/><br/> **Jorge Francisco Taipe Sangama:** <br/> **AV1:** Construí y refactoricé los Diagramas de contexto, de containers y diagramas ERD. El desarrollo del AV1 me permitió conocer la perspectiva de los usuarios que usarán la aplicación. Lideré la definición del lenguaje ubicuo y el registro de evidencias de investigación, orientando al equipo en el uso de terminología común. <br/> **TB1:** Lideré la corrección del Problem Statement y el Lean UX Canvas. Coordiné la redacción del Sprint Planning 1 y la priorización del Product Backlog por valor de negocio. <br/> **AV2:** Participé en el desarrollo del Sprint 2, contribuyendo a la implementación e integración de los microservicios de SENTRYA. Durante esta etapa, reforcé mis conocimientos sobre la organización de componentes de software, comunicación mediante APIs y estructuración de servicios independientes, comprendiendo cómo estas tecnologías facilitan la evolución del sistema. <br/><br/> **Anderson Ricardo Ventosilla Trujillo:** <br/> **AV1:** Desarrollé el capítulo 3, elaborando las User Stories, el Impact Mapping y el Product Backlog del proyecto, además de realizar las entrevistas al segmento 2 (implementadores de hogar inteligente). El desarrollo del AV1 me permitió profundizar en la construcción de artefactos clave como las user historias, el impact mapping y el product backlog. A través de este proceso, logré entender mejor cómo traducir necesidades del negocio en requerimientos claros y estructurados, facilitando una mejor organización del trabajo y priorización de funcionalidades dentro del proyecto. <br/> **TB1:** Lideré la elaboración del Capítulo V (UI/UX Design), guiando al equipo en la aplicación de principios de diseño inclusivo y accesibilidad. <br/> **AV2:** Contribuí en el desarrollo del Sprint 2 mediante la implementación de funcionalidades del sistema utilizando una arquitectura basada en microservicios. Esta experiencia me permitió ampliar mis conocimientos sobre desarrollo backend, integración de servicios y aplicación de los requerimientos definidos en las User Stories, comprendiendo mejor cómo transformar las necesidades del negocio en funcionalidades operativas. <br/><br/> **Gerald Serrano Uchuya:** <br/> **AV1:** Realicé la sección 4.1 relacionada al Event Storming, definición de Bounded Contexts, flujos y los diagramas de arquitectura de system landscape, context, container y despliegue. El desarrollo del AV1 me permitió reconocer los módulos core del negocio al que nuestro proyecto se enfocará, adicionalmente permitió definir el diagrama arquitectónico base que servirá como guía para la implementación de SENTRYA. <br/> **TB1:** Lideré el despliegue de la primera versión del Landing Page y definí el Source Code Style Guide y las convenciones de GitFlow. <br/> **AV2:** Participé en el desarrollo del Sprint 2, contribuyendo a la implementación de microservicios a partir de los Bounded Contexts y diagramas arquitectónicos previamente definidos. Esta experiencia me permitió fortalecer mis conocimientos sobre arquitectura distribuida, diseño de servicios independientes e integración de componentes, comprendiendo la importancia de mantener coherencia entre el diseño arquitectónico y su implementación. <br/><br/> **Braulio Torrejon:** <br/> **AV1:** Contribuí en el desarrollo del capítulo 2, realizando el análisis de las entrevistas a los segmentos objetivo, la identificación de necesidades de los usuarios y la elaboración de los User Personas, User Journey Mapping y Empathy Mapping. Además, incorporé los hallazgos obtenidos de las entrevistas para identificar oportunidades de mejora para la solución IoT. El desarrollo del capítulo 2 me permitió reforzar mis conocimientos sobre análisis de usuarios y levantamiento de requisitos. A través de las entrevistas y herramientas de UX, comprendí mejor cómo identificar problemas reales de los usuarios y transformarlos en necesidades y oportunidades que pueden ser consideradas durante el desarrollo de una solución de software. <br/> **TB1:** Lideré la mejora de los Lean UX Hypothesis Statements y guié al equipo en la elaboración de los Wireframes y Wireflows en Figma. <br/> **AV2:** Contribuí en el desarrollo del Sprint 2, participando en la implementación de funcionalidades y microservicios de SENTRYA. Durante esta etapa, reforcé mis conocimientos sobre desarrollo de software, comunicación entre servicios y aplicación de requerimientos funcionales, comprendiendo cómo las necesidades identificadas durante la investigación de usuarios se transforman en componentes tecnológicos. | **AV1:** El desarrollo del AV1 me permitió reforzar mis conocimientos sobre la estructura inicial de un proyecto de software. Sentí que este proceso me ayudó a entender mejor cómo plantear una base sólida, lo cual considero clave para mi crecimiento profesional. El equipo demostró capacidad para distribuir el liderazgo de manera equitativa entre los siete integrantes, asumiendo guías en secciones clave del informe inaugural. Cada miembro lideró un dominio distinto — arquitectura de software, investigación y lenguaje ubicuo, visión de negocio, análisis estadístico e impact mapping, diseño estratégico DDD, needfinding competitivo y elicitación Lean UX — lo que permitió construir los Capítulos I y II, ejecutar entrevistas con sustento estadístico y sentar las bases metodológicas del proyecto SENTRYA sin depender de un único líder central. <br/><br/> **TB1:** Tras la retroalimentación del docente, cada integrante lideró mejoras específicas en su área de competencia, reforzando el liderazgo conjunto por dominios (diseño, arquitectura, UX, calidad y despliegue). Se corrigieron diagramas C4, User Stories en Gherkin, entregables del Capítulo V, Sprint Planning 1, Landing Page v1 y convenciones de GitFlow. La matriz de Aspect Leaders and Collaborators formalizó la rotación de responsabilidades y demostró que el equipo puede asumir liderazgo rotativo sin perder coherencia ni calidad documental. <br/><br/> **AV2:** Durante el desarrollo del Sprint 2, los integrantes del equipo fortalecieron sus conocimientos técnicos mediante la implementación de microservicios para el proyecto SENTRYA. Esta etapa permitió aplicar los conceptos de arquitectura de software, Domain-Driven Design (DDD), Bounded Contexts e integración mediante APIs REST, transformando los diseños y requerimientos previamente definidos en componentes funcionales. Asimismo, el trabajo colaborativo favoreció la comprensión de la arquitectura distribuida y la importancia de desarrollar soluciones modulares, escalables y mantenibles. |
| **Reconoce la necesidad del aprendizaje permanente para el desempeño profesional y el desarrollo de proyectos en soluciones de tecnologías de ingeniería de software.** | **Pablo Martinez Gaona:** <br/> **AV1:** Contribuí realizando el capítulo 1, sedimentando las bases del proyecto. A lo largo del desarrollo del capítulo 1, comprendí que siempre hay aspectos que mejorar y aprender. Esta experiencia me hizo reflexionar sobre la importancia de mantenerme en constante actualización para poder aportar mejor en futuros proyectos. <br/> **TB1:** Establecí metas para la arquitectura y realicé el seguimiento mediante el Sprint Backlog. Validé los artefactos de otros integrantes para asegurar la calidad. <br/> **AV2:** Durante el desarrollo del Sprint 2, reconocí la necesidad de continuar aprendiendo sobre arquitectura de microservicios y buenas prácticas de desarrollo. La implementación de servicios independientes me permitió comprender la importancia de actualizar constantemente mis conocimientos técnicos para afrontar los desafíos relacionados con la integración, organización y mantenimiento de sistemas distribuidos. <br/><br/> **Jose Luis Martínez Valdivia:** <br/> **AV1:** Contribuí en el desarrollo del capítulo 4 - Definición de Bounded Contexts y sus componentes. Durante el desarrollo del capítulo 4, logré entender los procesos y requerimientos que se deben llevar a cabo para poder delimitar el alcance y arquitectura de desarrollo del proyecto a implementar. <br/> **TB1:** Organicé sesiones de revisión de criterios de aceptación con el equipo y cumplí con la elaboración de los archivos feature para el Testing Suite. <br/> **AV2:** Durante el desarrollo del Sprint 2, reconocí la importancia de profundizar mis conocimientos sobre implementación de microservicios, integración mediante APIs REST y aplicación de principios de DDD. Esta experiencia me permitió comprender que el desarrollo de sistemas distribuidos requiere un aprendizaje constante para resolver problemas técnicos, mejorar la comunicación entre componentes y garantizar una arquitectura de software mantenible. <br/><br/> **Gerald Serrano Uchuya:** <br/> **AV1:** Fue necesario repasar los pasos para la identificación de Bounded Contexts y flujos, partiendo desde la lluvia de eventos hasta la definición de los módulos en los que se dividirá el proyecto. Adicionalmente, requerí repasar temas de diagramas C4 para ver cómo adaptar IoT a nuestro caso. Repasar esos temas me permitió identificar correctamente los BC de SENTRYA de acuerdo a las necesidades de nuestros usuarios y permitir diagramar adecuadamente las diferentes capas del modelo C4. <br/> **TB1:** Fomenté la inclusión convocando retrospectivas tras cada artefacto UX. Entregué el prototipo navegable en Figma dentro de los plazos. <br/> **AV2:** Durante el desarrollo del Sprint 2, fue necesario reforzar mis conocimientos sobre arquitectura de microservicios, separación de responsabilidades y comunicación entre servicios. Esta experiencia me permitió reconocer que los conceptos arquitectónicos deben complementarse con conocimientos prácticos de implementación, por lo que resulta fundamental mantener un aprendizaje continuo para desarrollar soluciones eficientes y escalables. <br/><br/> **Jorge Francisco Taipe Sangama:** <br/> **AV1:** Reconocí segmentos, funcionalidades y los convertí en Bounded Contexts para desarrollo. El desarrollo de este capítulo me permitió aprender cómo segmentar Bounded Contexts en el contexto de desarrollo móvil. <br/> **TB1:** Planifiqué el Sprint Planning 1 estableciendo objetivos SMART. Actualicé el Product Backlog priorizando los User Stories por valor de negocio. <br/> **AV2:** El desarrollo del Sprint 2 me permitió reconocer la necesidad de seguir aprendiendo sobre integración de microservicios y comunicación entre componentes. Durante la implementación, comprendí la importancia de investigar nuevas herramientas y buenas prácticas para resolver dificultades técnicas y asegurar que los diferentes servicios funcionen de manera coordinada. <br/><br/> **Anderson Ricardo Ventosilla Trujillo:** <br/> **AV1:** Contribuí realizando parte del capítulo 3, con las User Stories, el Impact Mapping y el Product Backlog. Durante el desarrollo del capítulo 3, comprendí mejor cómo definir y organizar el alcance del proyecto. El uso de herramientas como el Impact Mapping y el Product Backlog me ayudó a estructurar las ideas, priorizar funcionalidades y tener una visión más clara del desarrollo del software. <br/> **TB1:** Organicé la implementación del Landing Page asignando secciones mediante la matriz de colaboradores. Cumplí con el despliegue en el plazo acordado. <br/> **AV2:** Durante el desarrollo del Sprint 2, comprendí la importancia de mantenerme actualizado en tecnologías y metodologías de desarrollo backend. La implementación de microservicios me permitió identificar la necesidad de profundizar mis conocimientos sobre construcción de APIs, integración de funcionalidades y resolución de problemas técnicos, fortaleciendo mi capacidad de adaptación a nuevas tecnologías. <br/><br/> **Braulio Torrejon:** <br/> **AV1:** Investigué y apliqué herramientas de análisis de usuarios y levantamiento de información, como entrevistas, User Personas, User Journey Mapping y Empathy Mapping, para comprender las necesidades de los dueños de hogar e implementadores de soluciones IoT. El desarrollo de este capítulo me permitió reconocer la importancia de continuar aprendiendo nuevas herramientas y metodologías para el desarrollo de software. En particular, comprendí que conocer las necesidades y dificultades de los usuarios es fundamental para plantear soluciones que respondan adecuadamente al contexto del proyecto. <br/> **TB1:** Planifiqué las tareas de corrección del needfinding distribuyendo responsabilidades de análisis. Cumplí con el sustento estadístico requerido. <br/> **AV2:** El desarrollo del Sprint 2 me permitió reconocer la importancia del aprendizaje continuo durante la implementación de soluciones de software. A través del trabajo con microservicios, comprendí la necesidad de seguir investigando sobre desarrollo backend, integración de APIs y buenas prácticas de programación, con el objetivo de contribuir al desarrollo de funcionalidades que respondan adecuadamente a las necesidades de los usuarios. | **AV1:** Desde la primera entrega, el equipo construyó un ambiente colaborativo e inclusivo, cumpliendo el 100% de los entregables dentro del plazo establecido. Se definieron metas claras por sección, se estructuró el Product Backlog y se realizaron sesiones de EventStorming con participación equitativa de los siete integrantes. Las User Personas garantizaron que el diseño considerara la diversidad de segmentos (familiares, cuidadores y administradores), manteniendo al equipo alineado en la documentación de los Capítulos I y II, las hipótesis UX y el Journey Mapping. <br/><br/> **TB1:** En la segunda entrega se fortaleció la planificación mediante Scrum y GitFlow. El Sprint Planning 1 estableció objetivos SMART, el Product Backlog se priorizó por valor de negocio y la matriz de Aspect Leaders and Collaborators eliminó ambigüedades en roles y responsabilidades. Retrospectivas UX, revisiones de criterios de aceptación y validación cruzada de artefactos arquitectónicos permitieron cumplir en plazo el Landing Page v1, el prototipo navegable en Figma, el sustento estadístico del needfinding y los archivos .feature del Testing Suite. <br/><br/> **AV2:** El desarrollo del Sprint 2 permitió al equipo reconocer la importancia del aprendizaje permanente para afrontar los desafíos técnicos de la implementación de microservicios. Durante esta etapa, fue necesario reforzar conocimientos sobre desarrollo backend, comunicación entre servicios, integración de componentes y buenas prácticas de programación. La experiencia contribuyó al fortalecimiento de las habilidades de investigación, resolución de problemas y adaptación tecnológica, demostrando que la actualización continua de conocimientos resulta fundamental para el desarrollo profesional en ingeniería de software. |
