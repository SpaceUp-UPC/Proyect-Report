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
    Ciclo: 2026-02
    <br> <br>
    Informe de Trabajo Final
    <br> <br>
    Startup: SpaceUp
    <br> <br>
    Producto: Sentraya  
</h3>

<div align="center">

| <div style="width:300px">Alumno</div>       | <div style="width:125px">Código</div> |
|:-------------------------------------------:|:-------------------------------------:|
|  Martínez Valdivia, José Luis               |              u202213989               |
|  Taipe Sangama, Jorge Francisco             |                u202313458              |
|                 |                            |
|    Martinez Gaona, Pablo Afranio         |   u202120011                          |
|  Ventosilla Trujillo, Anderson Ricardo | u202319025                            |

</div>

<div align="center"> Setiembre 2026 </div>


## Registro de Versiones del Informe

| Versión | Fecha      | Autor(es)      | Descripción de modificación       |
|-------|----------|--------------------------------------------------------|---------|
| 0.1     | 22/04/2026 |              |          |





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



**ABET – EAC - Student Outcome 7**

La capacidad de adquirir y aplicar nuevos
conocimientos según sea necesario,
utilizando estrategias de aprendizaje
apropiadas.

En el siguiente cuadro se describe las acciones realizadas y enunciados de conclusiones por parte del grupo,
que permiten sustentar el haber alcanzado el logro del ABET – EAC - Student Outcome 7.


| Criterio específico | Acciones realizadas | Conclusiones |
| :--- | :--- | :--- |
| **Actualiza conceptos y conocimientos necesarios para su desarrollo profesional y en especial para su proyecto en soluciones de software.** |  **Pablo Martinez Gaona:** Realicé todo el capítulo 1 <br><br> **Jose Luis Martínez Valdivia:** Contribui en El desarrollo del capitulo 4 - Definicion de Bounded Contexts y sus componentes <br><br> **Jorge Francisco Taipe Sangama:** Construi y refactorize los Diagramas de contexto, de containers y diagramas ERD <br><br> **XXXXX:** SDSDSDSDSDSD  <br><br> **XXXXX:** SDDSDSDSDSDSDSD. <br><br>| **Pablo Martinez Gaona:** **TB1** Esta entrega me permitió ampliar mis conocimientos sobre el planteamiento de soluciones IoT y comprender mejor cómo relacionar las necesidades de los usuarios con dispositivos, funcionalidades y procesos de software. <br><br>  **XXXX:** **TB1:** El desarrollo del AV1 me permitió reforzar mis conocimientos sobre la estructura inicial de un proyecto de software. Sentí que este proceso me ayudó a entender mejor cómo plantear una base sólida, lo cual considero clave para mi crecimiento profesional. <br><br>   <br><br> **Jose Luis Martínez Valdivia:** El desarrollo del AV1 me permitió comentar y enriquecer mis conocimientos de DDD y la forma en la que se debaten ideas para implementar una solución de Servicio Web <br><br> **Jorge Francisco Taipe Sangama:** El desarrollo del AV1 me permitió conocer la perspectiva de los usuarios que usarán la aplicación. <br><br>  **XXXXX:** El desarrollo del AV1 permitirá a los desarrolladores asignar los bounded context y hacer consultas de funcionamiento e interconexión. <br><br> **XXXXXX:** El desarrollo del AV1 me permitió profundizar en la construcción de artefactos clave como las user historias, el impact mapping y el product backlog. A través de este proceso, logré entender mejor cómo traducir necesidades del negocio en requerimientos claros y estructurados, facilitando una mejor organización del trabajo y priorización de funcionalidades dentro del proyecto. <br><br>|
| **Reconoce la necesidad del aprendizaje permanente para el desempeño profesional y el desarrollo de proyectos en soluciones detecnologías de ingeniería de software** | **Pablo Martinez Gaona:** Contribuí realizando el capítulo 1,sedimentando las bases del proyecto <br><br> **Jose Luis Martínez Valdivia:** Contribui en El desarrollo del capitulo 4 - Definicion de Bounded Contexts y sus componentes <br><br> **XXXXXXXXXXXXX** Reconocí las necesidades de los usuarios a través de entrevistas, así como sus gustos y molestias <br><br> **Jorge Francisco Taipe Sangama:** Reconocí segmentos, funcionalidades y los convertí en bounded context para desarrollo  <br><br> **XXXXXXX:** Contribui realizando parte del capítulo 2, con las user historias, el impact mapping y el product backlog. <br><br>| **Pablo Martinez Gaona** **TB1:** A lo largo del desarrollo del capítulo 1, comprendí que siempre hay aspectos que mejorar y aprender. Esta experiencia me hizo reflexionar sobre la importancia de mantenerme en constante actualización para poder aportar mejor en futuros proyectos. <br><br> **Jose Luis Martínez Valdivia:** Durante El desarrollo de capitulo 4, logre entender los procesos y requerimientos que se deben llevar acabo para poder delimitar el alcance y arquitectura de desarrollo del proyecto a implementar <br><br> **XXXXXXX: :** Este conocimiento me permitió hacer un análisis y crear personas para enfocarnos en posibles requisitos funcionales <br><br> **Jorge Francisco Taipe Sangama:** El desarrollo de este capítulo me permitió aprender como segmentar bounded context en el contexto de desarrollo móvil <br><br> **XXXXXX:** Durante el desarrollo del capítulo 2, comprendí mejor cómo definir y organizar el alcance del proyecto. El uso de herramientas como el impact mapping y el product backlog me ayudó a estructurar las ideas, priorizar funcionalidades y tener una visión más clara del desarrollo del software.<br><br>|

