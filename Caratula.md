<p align="center">
    <img src="./assets/UPC_logo_transparente.png" alt="upc-logo" width="80px" height="80px"/>
</p>

<h1 align="center">
    Universidad Peruana de Ciencias Aplicadas
</h1>

<h3 align="center">
    Carrera: Ingeniería de Software
    <br> <br>
    Curso: 1ASI0572 - Desarrollo de Soluciones IOT
    <br> <br>
    Sección: 8735
    <br> <br>
    Profesor: Marco Antonio Leon Baca
    <br> <br>
    Ciclo: 202620
    <br> <br>
    Informe de Trabajo Final
    <br> <br>
    Startup: SpaceUp
    <br> <br>
    Producto: Sentrya  
</h3>

<div align="center">

| <div style="width:300px">Alumno</div>       | <div style="width:125px">Código</div> |
|:-------------------------------------------:|:-------------------------------------:|
|  Martínez Valdivia, José Luis               |              u202213989               |
|  Taipe Sangama, Jorge Francisco             |                u202313458              | 
|  Serrano Uchuya, Gerald Patricio   | u202122876                           |
|    Martinez Gaona, Pablo Afranio         |   u202120011                          |
|  Ventosilla Trujillo, Anderson Ricardo | u202319025                            |
|  Torrejon Navarro, Braulio Rodrigo | u201711828                            |

</div>

<div align="center"> Setiembre 2026 </div>

<div style="page-break-before: always;"></div>

## Registro de Versiones del Informe

| Versión | Fecha      | Autor(es)      | Descripción de modificación       |
|-------|----------|--------------------------------------------------------|---------|
| 0.1     | 09/09/2026 |    Equipo SpaceUp       |     Se completaron los capitulos del 1 al 4     |
| 0.2     | 05/10/2026 |    Equipo SpaceUp       |     Se completaron los capitulos del 5 y 6     |

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





     


**ABET – EAC - Student Outcome 7**

La capacidad de adquirir y aplicar nuevos
conocimientos según sea necesario,
utilizando estrategias de aprendizaje
apropiadas.

En el siguiente cuadro se describe las acciones realizadas y enunciados de conclusiones por parte del grupo,
que permiten sustentar el haber alcanzado el logro del ABET – EAC - Student Outcome 7.


| Criterio específico | Acciones realizadas | Conclusiones |
| :--- | :--- | :--- |
| **Actualiza conceptos y conocimientos necesarios para su desarrollo profesional y en especial para su proyecto en soluciones de software.** | **Pablo Martinez Gaona:** <br/> **AV1:** Realicé todo el capítulo 1. Esta entrega me permitió ampliar mis conocimientos sobre el planteamiento de soluciones IoT y comprender mejor cómo relacionar las necesidades de los usuarios con dispositivos, funcionalidades y procesos de software. <br/>**TB1:** Lideré la corrección de los diagramas de arquitectura de software (C4 Model), asegurando coherencia con el diseño estratégico. Coordiné el Sprint Backlog 1 y la matriz de responsabilidades. <br> <br/>**Jose Luis Martínez Valdivia:**<br/> **AV1:** Contribuí en El desarrollo del capítulo 4 - Definición de Bounded Contexts y sus componentes El desarrollo del AV1 me permitió comentar y enriquecer mis conocimientos de DDD y la forma en la que se debaten ideas para implementar una solución de Servicio Web <br>**TB1:** Lideré la mejora de los User Stories en formato Gherkin para todos los stories del backlog. Coordiné la sección de Testing Suite Evidence para el Sprint Review.<br/> <br/> **Jorge Francisco Taipe Sangama:**<br/> **AV1:** Construí y refactoricé los Diagramas de contexto, de containers y diagramas ERD. El desarrollo del AV1 me permitió conocer la perspectiva de los usuarios que usarán la aplicación.Lideré la definición del lenguaje ubicuo y el registro de evidencias de investigación, orientando al equipo en el uso de terminología común.<br/> **TB1:** Lideré la corrección del Problem Statement y el Lean UX Canvas. Coordiné la redacción del Sprint Planning 1 y la priorización del Product Backlog por valor de negocio. <br><br> **Anderson Ricardo Ventosilla Trujillo:** <br/> **AV1:** Desarrollé el capítulo 3, elaborando las User Stories, el Impact Mapping y el Product Backlog del proyecto, además de realizar las entrevistas al segmento 2 (implementadores de hogar inteligente).  El desarrollo del AV1 me permitió profundizar en la construcción de artefactos clave como las user historias, el impact mapping y el product backlog. A través de este proceso, logré entender mejor cómo traducir necesidades del negocio en requerimientos claros y estructurados, facilitando una mejor organización del trabajo y priorización de funcionalidades dentro del proyecto.<br/> **TB1:** Lideré la elaboración del Capítulo V (UI/UX Design), guiando al equipo en la aplicación de principios de diseño inclusivo y accesibilidad. <br><br> **Gerald Serrano Uchuya:** <br/> **AV1:** Realicé la sección 4.1 relacionado al Event Storming, definición de Bounded Contexts, flujos y los diagramas de arquitectura de system landscape, context, container y despliegue. El desarrollo del AV1 me permitió reconocer los módulos core del negocio al que nuestro proyecto se enfocará, adicionalmente que permitió definir el diagrama arquitectónico base que servirá como guía para la implementación de Sentrya. <br/> **TB1:** Lideré el despliegue de la primera versión del Landing Page y definió el Source Code Style Guide y las convenciones de GitFlow.<br><br> **Braulio Torrejon:** Contribuí en el desarrollo del capítulo 2, realizando el análisis de las entrevistas a los segmentos objetivo, la identificación de necesidades de los usuarios y la elaboración de los User Personas, User Journey Mapping y Empathy Mapping. Además, incorporé los hallazgos obtenidos de las entrevistas para identificar oportunidades de mejora para la solución IoT. El desarrollo del capítulo 2 me permitió reforzar mis conocimientos sobre análisis de usuarios y levantamiento de requisitos. A través de las entrevistas y herramientas de UX, comprendí mejor cómo identificar problemas reales de los usuarios y transformarlos en necesidades y oportunidades que pueden ser consideradas durante el desarrollo de una solución de software. <br/> **TB1:** Lideré la mejora de los Lean UX Hypothesis Statements y guié al equipo en la elaboración de los Wireframes y Wireflows en Figma. <br><br>|<br><br> **AV1:** El desarrollo del AV1 me permitió reforzar mis conocimientos sobre la estructura inicial de un proyecto de software. Sentí que este proceso me ayudó a entender mejor cómo plantear una base sólida, lo cual considero clave para mi crecimiento profesional. El equipo demostró capacidad para distribuir el liderazgo de manera equitativa entre los siete integrantes, asumiendo guías en secciones clave del informe inaugural. Cada miembro lideró un dominio distinto — arquitectura de software, investigación y lenguaje ubicuo, visión de negocio, análisis estadístico e impact mapping, diseño estratégico DDD, needfinding competitivo y elicitación Lean UX — lo que permitió construir los Capítulos I y II, ejecutar entrevistas con sustento estadístico y sentar las bases metodológicas del proyecto SENTRYA sin depender de un único líder central. <br><br> **TB1:** Tras la retroalimentación del docente, cada integrante lideró mejoras específicas en su área de competencia, reforzando el liderazgo conjunto por dominios (diseño, arquitectura, UX, calidad y despliegue). Se corrigieron diagramas C4, User Stories en Gherkin, entregables del Capítulo V, Sprint Planning 1, Landing Page v1 y convenciones de GitFlow. La matriz de Aspect Leaders and Collaborators formalizó la rotación de responsabilidades y demostró que el equipo puede asumir liderazgo rotativo sin perder coherencia ni calidad documental. |
| **Reconoce la necesidad del aprendizaje permanente para el desempeño profesional y el desarrollo de proyectos en soluciones detecnologías de ingeniería de software** | **Pablo Martinez Gaona:** <br/> **AV1:** Contribuí realizando el capítulo 1,sedimentando las bases del proyecto. A lo largo del desarrollo del capítulo 1, comprendí que siempre hay aspectos que mejorar y aprender. Esta experiencia me hizo reflexionar sobre la importancia de mantenerme en constante actualización para poder aportar mejor en futuros proyectos. <br/> **TB1:** Establecí metas para la arquitectura y realizó el seguimiento mediante el Sprint Backlog. Validé los artefactos de otros integrantes para asegurar la calidad. <br><br> **Jose Luis Martínez Valdivia:**<br/> **AV1:** Contribuí en El desarrollo del capítulo 4 - Definición de Bounded Contexts y sus componentes. Durante El desarrollo de capítulo 4, logré entender los procesos y requerimientos que se deben llevar a cabo para poder delimitar el alcance y arquitectura de desarrollo del proyecto a implementar. <br/> **TB1:** Organizó sesiones de revisión de criterios de aceptación con el equipo y cumplió con la elaboración de los archivos feature para el Testing Suite<br><br> **Gerald Serrano Uchuya:** <br/> **AV1:** Fue necesario repasar los pasos para la identificación de bounded contexts y flujos, partiendo desde la lluvia de eventos hasta la definición de los módulos en los que se dividirá el proyecto. Adicionalmente, requerí repasar temas de diagramas c4 para ver cómo adaptar IoT a nuestro caso. Repasar esos temas me permitió identificar correctamente los BC de Sentrya de acuerdo a las necesidades de nuestros usuarios y permitir diagramar adecuadamente las diferentes capas del modelo C4 <br/> **TB1:** Fomentó la inclusión convocando retrospectivas tras cada artefacto UX. Entregó el prototipo navegable en Figma dentro de los plazos. <br><br> **Jorge Francisco Taipe Sangama:** <br/> **AV1:** Reconocí segmentos, funcionalidades y los convertí en bounded context para desarrollo.  El desarrollo de este capítulo me permitió aprender como segmentar bounded context en el contexto de desarrollo móvil. <br/> **TB1:** Planificó el Sprint Planning 1 estableciendo objetivos SMART. Actualizó el Product Backlog priorizando los User Stories por valor de negocio.<br><br> **Anderson Ricardo Ventosilla Trujillo:** <br/> **AV1:** Contribuí realizando parte del capítulo 3, con las user historias, el impact mapping y el product backlog.  Durante el desarrollo del capítulo 3, comprendí mejor cómo definir y organizar el alcance del proyecto. El uso de herramientas como el impact mapping y el product backlog me ayudó a estructurar las ideas, priorizar funcionalidades y tener una visión más clara del desarrollo del software.<br/> **TB1:** Organizó la implementación del Landing Page asignando secciones mediante la matriz de colaboradores. Cumplió con el despliegue en el plazo acordado. <br/> <br><br> **Braulio Torrejon:** <br/> **AV1:** Investigué y apliqué herramientas de análisis de usuarios y levantamiento de información, como entrevistas, User Personas, User Journey Mapping y Empathy Mapping, para comprender las necesidades de los dueños de hogar e implementadores de soluciones IoT.El desarrollo de este capítulo me permitió reconocer la importancia de continuar aprendiendo nuevas herramientas y metodologías para el desarrollo de software. En particular, comprendí que conocer las necesidades y dificultades de los usuarios es fundamental para plantear soluciones que respondan adecuadamente al contexto del proyecto. <br/> **TB1:**  Planificó las tareas de corrección del needfinding distribuyendo responsabilidades de análisis. Cumplió con el sustento estadístico requerido.<br><br>| **AV1:** Desde la primera entrega, el equipo construyó un ambiente colaborativo e inclusivo, cumpliendo el 100% de los entregables dentro del plazo establecido. Se definieron metas claras por sección, se estructuró el product backlog y se realizaron sesiones de EventStorming con participación equitativa de los siete integrantes. Las user personas garantizaron que el diseño considerara la diversidad de segmentos (familiares, cuidadores y administradores), manteniendo al equipo alineado en la documentación de los Capítulos I y II, las hipótesis UX y el journey mapping. <br/> <br/> **TB1:** En la segunda entrega se fortaleció la planificación mediante Scrum y GitFlow. El Sprint Planning 1 estableció objetivos SMART, el Product Backlog se priorizó por valor de negocio y la matriz de Aspect Leaders and Collaborators eliminó ambigüedades en roles y responsabilidades. Retrospectivas UX, revisiones de criterios de aceptación y validación cruzada de artefactos arquitectónicos permitieron cumplir en plazo el Landing Page v1, el prototipo navegable en Figma, el sustento estadístico del needfinding y los archivos .feature del Testing Suite.|