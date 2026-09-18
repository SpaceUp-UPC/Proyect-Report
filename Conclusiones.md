### Conclusiones

1. El análisis de la problemática, desarrollado mediante la técnica de las 5W y 2H y respaldado por indicadores del INEI y recomendaciones de Osinergmin, confirmó que existe una necesidad real de centralizar la implementación, el monitoreo y la administración de soluciones IoT en viviendas peruanas, tanto para los dueños de hogar como para los implementadores especializados.

2. El proceso de Lean UX permitió validar que la propuesta de valor de Setrya se sostiene sobre tres núcleos de protección —detección acústica y visual, monitoreo térmico y protección eléctrica inteligente— y que estos pueden ampliarse de forma modular sin reemplazar las soluciones ya instaladas, lo cual responde directamente a las hipótesis y suposiciones planteadas en el Capítulo I.

3. Las entrevistas, el needfinding y el análisis competitivo del Capítulo II evidenciaron que, a diferencia de alternativas como Samsung SmartThings, Home Assistant o Google Home, la principal oportunidad de diferenciación de Setrya no está en el control de dispositivos aislados, sino en integrar en una misma plataforma el monitoreo, las alertas, los históricos y la comunicación entre dueños de hogar e implementadores.

4. La especificación de requisitos del Capítulo III, compuesta por 12 épicas y 25 historias de usuario derivadas del Impact Mapping, tradujo de manera consistente los objetivos de negocio de ambos segmentos objetivo en funcionalidades concretas y priorizables dentro del Product Backlog.

5. El diseño estratégico y táctico del Capítulo IV, mediante Domain-Driven Design, permitió delimitar cinco bounded contexts (Identity & Access Management, Space Management, Payment Management, IoT Monitoring and Notifications, y Report Management) con responsabilidades claras, lo que reduce el acoplamiento entre módulos y facilita la evolución independiente de cada uno conforme el ecosistema de dispositivos se amplíe.

6. En conjunto, los cuatro capítulos muestran una trazabilidad coherente entre la problemática identificada, las hipótesis de negocio, los requisitos funcionales y la arquitectura de software propuesta, lo que sustenta la viabilidad de Setrya como solución para la gestión integral de hogares inteligentes.

### Recomendaciones

1. Validar con dueños de hogar reales las hipótesis planteadas en el Lean UX Canvas —en especial las asociadas al dashboard centralizado y al centro de alertas— antes de escalar el desarrollo de nuevos módulos IoT.

2. Priorizar en los primeros sprints las épicas de Registro y Autenticación (EP01), Dashboard Centralizado (EP02) y Centro de Alertas (EP06), dado que constituyen la base sobre la cual dependen funcionalmente el resto de módulos del backlog.

3. Establecer métricas de adopción y retención (por ejemplo, frecuencia de consulta del dashboard y tiempo de respuesta ante alertas) que permitan contrastar en producción los Business Outcomes definidos en el Impact Mapping del Capítulo III.

4. Mantener la separación de bounded contexts definida en el Capítulo IV al momento de implementar nuevas soluciones IoT, evitando dependencias directas entre los módulos de dominio y favoreciendo la comunicación a través de los contratos ya definidos en el Context Mapping.

5. Incorporar pruebas de integración y de carga sobre el módulo de IoT Monitoring and Notifications antes de ampliar el catálogo de dispositivos compatibles, considerando que este bounded context concentra el procesamiento de eventos y alertas en tiempo real.

6. Evaluar, en una siguiente iteración, la incorporación de nuevas categorías de dispositivos (por ejemplo, iluminación o sensores de movimiento) siguiendo el mismo enfoque modular validado para los tres núcleos iniciales, de modo que la expansión no afecte las soluciones ya instaladas por los usuarios.

### Bibliografía

- Instituto Nacional de Estadística e Informática. (2026). *Estadísticas de las tecnologías de información y comunicación en los hogares: Informe técnico N.º 1, primer trimestre de 2026*. INEI. https://www.gob.pe/inei

- Organismo Supervisor de la Inversión en Energía y Minería. (s.f.). *Recomendaciones para el uso seguro de la electricidad en el hogar*. Osinergmin. https://www.osinergmin.gob.pe

- Evans, E. (2003). *Domain-Driven Design: Tackling Complexity in the Heart of Software*. Addison-Wesley.

- Vernon, V. (2013). *Implementing Domain-Driven Design*. Addison-Wesley.

- Gothelf, J., & Seiden, J. (2016). *Lean UX: Designing Great Products with Agile Teams* (2.ª ed.). O'Reilly Media.

- Adzic, G. (2012). *Impact Mapping: Making a Big Impact with Software Products and Projects*. Provoking Thoughts.

- Samsung Electronics. (s.f.). *SmartThings*. https://www.smartthings.com

- Home Assistant. (s.f.). *Home Assistant: Awaken your home*. https://www.home-assistant.io

- Google. (s.f.). *Google Home*. https://home.google.com

## Anexos
#### Anexo A: Enlaces de Repositorios

A continuación se listan los enlaces a  los repositorios de código fuente utilizados en el proyecto.

| Recurso                                         | URL                                                                                                                                      |
|-------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------|
| **Repositorio Project Report**                  | [https://github.com/SpaceUp-UPC/Proyect-Report](https://github.com/SpaceUp-UPC/Proyect-Report) |
| **Repositorio Frontend** | [https://github.com/SpaceUp-UPC/Setrya-Frontend](https://github.com/SpaceUp-UPC/Setrya-Frontend)                                                                         |
| **Repositorio Backend**                         | [https://github.com/SpaceUp-UPC/Setrya-Backend](https://github.com/SpaceUp-UPC/Setrya-Backend)                                 |
| **Repositorio Mobile**                          | [https://github.com/SpaceUp-UPC/MultiPlatform-App-Sentrya-Flutter](https://github.com/SpaceUp-UPC/MultiPlatform-App-Sentrya-Flutter)                           |

#### Anexo B: Videos de Exposiciones

Registro histórico de las exposiciones durante el ciclo académico 2026-20.

| Entrega / Hito              | Plataforma       | URL                                                |
|-----------------------------|------------------|----------------------------------------------------|
| **Video de Entrevistas** | Microsoft Stream | [Entrevistas Unidas](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202313458_upc_edu_pe/IQCbt_6Mzl12SJq6qsfCFuxqAR2Ywpzb010_STXjIGtgn6c?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=c4k3Wn ) |
| **Video de Exposición AV1** | Microsoft Stream | [Video de Exposicion AV1](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202313458_upc_edu_pe/IQDW-q_HEu45Sp9Wbm3C4Zg7Ac9C_V1c2xJLPtEqpcPUyfQ?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=ssoFne) |

