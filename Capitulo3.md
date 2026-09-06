# Capítulo III: Requirements Specification

## 3.1. User Stories

En esta sección se detallan las Épicas y las User Stories que guiarán el desarrollo de Setrya. Las épicas agrupan las historias de usuario según las soluciones IoT y funcionalidades definidas en el Capítulo I (dashboard centralizado, monitoreo térmico, detección acústica y visual, protección eléctrica, centro de alertas, mediciones e históricos, catálogo de soluciones IoT, solicitud de implementadores, gestión de clientes e instalaciones, gestión de dispositivos IoT, control remoto y expansión modular).

### 3.1.1. Épicas

| Epic ID | Título | Descripción |
|---------|--------|--------------|
| EP01 | Registro y Autenticación | Como usuario de Setrya (dueño de hogar o implementador), quiero crear una cuenta, iniciar/cerrar sesión y recuperar mi contraseña, para acceder de forma segura a la plataforma según mi rol. |
| EP02 | Dashboard Centralizado del Hogar | Como dueño de hogar, quiero visualizar en un solo entorno el estado general de mis dispositivos y soluciones IoT, para conocer rápidamente la situación de mi vivienda. |
| EP03 | Monitoreo Térmico | Como dueño de hogar, quiero monitorear la temperatura de mi vivienda con distintos niveles de alerta, para prevenir riesgos asociados a incrementos anómalos. |
| EP04 | Detección Acústica y Visual | Como dueño de hogar, quiero recibir alertas ante eventos anómalos de seguridad detectados por sensores acústicos y visuales, para responder oportunamente ante posibles intrusiones. |
| EP05 | Protección Eléctrica Inteligente | Como dueño de hogar, quiero que el sistema detecte condiciones eléctricas anómalas y actúe automáticamente, para proteger mis dispositivos y mi vivienda. |
| EP06 | Centro de Alertas y Notificaciones | Como dueño de hogar, quiero recibir y consultar todas las alertas generadas por mis dispositivos en un solo lugar, para atender rápidamente lo que requiere mi atención. |
| EP07 | Mediciones e Históricos | Como usuario de Setrya, quiero consultar el historial de mediciones y eventos de mi vivienda, para comprender el comportamiento de mis dispositivos a lo largo del tiempo. |
| EP08 | Catálogo de Soluciones IoT | Como dueño de hogar, quiero explorar un catálogo de soluciones IoT disponibles, para ampliar progresivamente el ecosistema inteligente de mi vivienda. |
| EP09 | Solicitud de Implementadores | Como dueño de hogar, quiero buscar y solicitar el servicio de un implementador especializado, para instalar, ampliar o mantener mis soluciones IoT. |
| EP10 | Gestión de Clientes e Instalaciones | Como implementador, quiero administrar mis clientes, viviendas e instalaciones desde un mismo entorno, para organizar mi trabajo de forma centralizada. |
| EP11 | Gestión de Dispositivos IoT | Como implementador, quiero registrar y consultar los dispositivos asociados a cada vivienda y ambiente, para mantener trazabilidad de cada instalación. |
| EP12 | Control Remoto y Expansión Modular | Como dueño de hogar, quiero controlar remotamente los dispositivos compatibles e incorporar nuevas categorías de dispositivos, para administrar y ampliar mi hogar inteligente sin reemplazar lo ya instalado. |

### 3.1.2. Historias de Usuario

| Epic / Story ID | Título | Descripción | Criterios de Aceptación | Epic ID |
|------------------|--------|--------------|---------------------------|---------|
| Registro y Autenticación / US01 | Registro de usuario | Como usuario de Setrya, quiero crear una cuenta seleccionando mi rol (dueño de hogar o implementador), para acceder a las funcionalidades correspondientes. | Dado que el usuario accede a la pantalla de registro <br> Cuando completa el formulario con sus datos y selecciona un rol <br> Entonces el sistema crea la cuenta y lo redirige a su dashboard según el rol elegido. | EP01 |
| Registro y Autenticación / US02 | Inicio de sesión | Como usuario de Setrya, quiero iniciar sesión con mis credenciales, para acceder a mi cuenta personalizada. | Escenario 1: <br> Dado que el usuario ingresa credenciales válidas <br> Cuando presiona "Iniciar sesión" <br> Entonces accede a su dashboard. <br><br> Escenario 2: <br> Dado que el usuario ingresa credenciales inválidas <br> Cuando presiona "Iniciar sesión" <br> Entonces el sistema muestra un mensaje de error y no permite el acceso. | EP01 |
| Registro y Autenticación / US03 | Recuperar contraseña | Como usuario de Setrya, quiero recuperar mi contraseña, para volver a acceder a mi cuenta en caso la olvide. | Dado que el usuario no recuerda su contraseña <br> Cuando presiona "Recuperar contraseña" e ingresa su correo <br> Entonces el sistema envía un enlace para restablecerla. | EP01 |
| Dashboard Centralizado / US04 | Visualización del estado general del hogar | Como dueño de hogar, quiero ver un resumen del estado de todos mis dispositivos IoT al ingresar a la aplicación, para identificar rápidamente si existe alguna alerta activa. | Dado que el dueño de hogar tiene dispositivos registrados <br> Cuando ingresa a su dashboard <br> Entonces el sistema muestra el estado general de cada módulo (térmico, seguridad, eléctrico) y las alertas activas. | EP02 |
| Dashboard Centralizado / US05 | Organización por ambientes | Como dueño de hogar, quiero visualizar mis dispositivos agrupados por ambiente de la vivienda, para ubicar rápidamente el dispositivo que necesito revisar. | Dado que el dueño de hogar tiene ambientes configurados <br> Cuando accede a la sección "Mis ambientes" <br> Entonces el sistema lista los dispositivos asociados a cada ambiente. | EP02 |
| Monitoreo Térmico / US06 | Configuración de niveles de alerta térmica | Como dueño de hogar, quiero configurar los umbrales de temperatura que activan una alerta, para adaptar el monitoreo a las condiciones de mi vivienda. | Dado que el dueño de hogar tiene un sensor térmico instalado <br> Cuando define los umbrales de alerta (normal, moderado, crítico) <br> Entonces el sistema guarda la configuración y la aplica a las lecturas futuras. | EP03 |
| Monitoreo Térmico / US07 | Recepción de alerta térmica | Como dueño de hogar, quiero recibir una notificación cuando la temperatura supere el umbral configurado, para tomar acción antes de que represente un riesgo. | Dado que un sensor térmico registra una lectura fuera de los umbrales definidos <br> Cuando se supera el umbral configurado <br> Entonces el sistema genera una alerta y notifica al dueño de hogar indicando el nivel alcanzado. | EP03 |
| Detección Acústica y Visual / US08 | Recepción de alerta de seguridad | Como dueño de hogar, quiero recibir una alerta cuando un sensor acústico o visual detecte un evento anómalo, para conocer oportunamente una posible situación de riesgo. | Dado que los sensores de seguridad están activos <br> Cuando se detecta un evento anómalo <br> Entonces el sistema genera una alerta con la evidencia disponible y notifica al dueño de hogar. | EP04 |
| Detección Acústica y Visual / US09 | Revisión de evidencia de un evento | Como dueño de hogar, quiero revisar la evidencia asociada a una alerta de seguridad, para comprender qué originó la notificación. | Dado que existe una alerta de seguridad generada <br> Cuando el dueño de hogar accede al detalle de la alerta <br> Entonces el sistema muestra la evidencia (imagen o registro) asociada al evento. | EP04 |
| Protección Eléctrica / US10 | Detección de condición eléctrica anómala | Como dueño de hogar, quiero que el sistema identifique condiciones eléctricas anómalas (sobrecarga o cortocircuito), para proteger los dispositivos conectados a mi vivienda. | Dado que el protector eléctrico inteligente está instalado <br> Cuando se detecta una condición anómala predefinida <br> Entonces el sistema registra el evento y ejecuta la acción de protección configurada. | EP05 |
| Protección Eléctrica / US11 | Consulta de acción ejecutada | Como dueño de hogar, quiero consultar qué acción ejecutó el sistema ante una condición eléctrica anómala, para conocer el estado actual del suministro. | Dado que se generó un evento de protección eléctrica <br> Cuando el dueño de hogar accede al detalle del evento <br> Entonces el sistema muestra la condición detectada, el dispositivo afectado y la acción ejecutada. | EP05 |
| Centro de Alertas / US12 | Listado centralizado de alertas | Como dueño de hogar, quiero ver todas mis alertas (térmicas, de seguridad y eléctricas) en un mismo centro de notificaciones, para atender rápidamente lo más relevante. | Dado que existen alertas generadas por distintos módulos <br> Cuando el dueño de hogar accede al "Centro de alertas" <br> Entonces el sistema lista las alertas ordenadas por prioridad y fecha. | EP06 |
| Centro de Alertas / US13 | Configuración de preferencias de notificación | Como dueño de hogar, quiero elegir el canal por el que recibo mis notificaciones (push, correo), para enterarme de los eventos de la forma que prefiera. | Dado que el dueño de hogar accede a "Preferencias de notificaciones" <br> Cuando selecciona los canales deseados <br> Entonces el sistema aplica la configuración a las futuras alertas. | EP06 |
| Mediciones e Históricos / US14 | Consulta de histórico de mediciones | Como dueño de hogar, quiero consultar el histórico de mediciones de un dispositivo en un periodo determinado, para comprender su comportamiento a lo largo del tiempo. | Dado que un dispositivo tiene mediciones registradas <br> Cuando el usuario selecciona un rango de fechas <br> Entonces el sistema muestra las mediciones y una tendencia básica del periodo. | EP07 |
| Mediciones e Históricos / US15 | Consulta de histórico de eventos | Como implementador, quiero consultar el historial de eventos de las instalaciones que administro, para dar seguimiento a su comportamiento. | Dado que una instalación tiene eventos registrados <br> Cuando el implementador accede al historial de la instalación <br> Entonces el sistema lista los eventos ordenados por fecha. | EP07 |
| Catálogo de Soluciones IoT / US16 | Exploración del catálogo | Como dueño de hogar, quiero explorar un catálogo de soluciones IoT disponibles, para identificar nuevas soluciones acordes a las necesidades de mi vivienda. | Dado que el dueño de hogar accede al "Catálogo de soluciones" <br> Cuando filtra por categoría (seguridad, monitoreo, automatización) <br> Entonces el sistema muestra las soluciones disponibles para esa categoría. | EP08 |
| Catálogo de Soluciones IoT / US17 | Detalle de una solución del catálogo | Como dueño de hogar, quiero ver el detalle de una solución del catálogo, para conocer sus características antes de solicitarla. | Dado que el dueño de hogar selecciona una solución del catálogo <br> Cuando accede a su detalle <br> Entonces el sistema muestra la descripción, requisitos y beneficios de la solución. | EP08 |
| Solicitud de Implementadores / US18 | Búsqueda de implementadores | Como dueño de hogar, quiero buscar implementadores especializados disponibles en mi zona, para solicitar la instalación o el mantenimiento de una solución. | Dado que el dueño de hogar accede a "Buscar implementador" <br> Cuando filtra por ubicación y especialidad <br> Entonces el sistema muestra una lista de implementadores disponibles. | EP09 |
| Solicitud de Implementadores / US19 | Solicitud de servicio a un implementador | Como dueño de hogar, quiero enviar una solicitud de servicio a un implementador, para coordinar la instalación de una solución IoT. | Dado que el dueño de hogar seleccionó un implementador <br> Cuando completa y envía el formulario de solicitud <br> Entonces el sistema notifica al implementador y registra la solicitud como pendiente. | EP09 |
| Gestión de Clientes e Instalaciones / US20 | Registro de una nueva instalación | Como implementador, quiero registrar una nueva instalación asociada a un cliente, para llevar control de los servicios que realizo. | Dado que el implementador acepta una solicitud de servicio <br> Cuando registra los datos de la instalación <br> Entonces el sistema la asocia al cliente correspondiente y la agrega a su listado de instalaciones. | EP10 |
| Gestión de Clientes e Instalaciones / US21 | Consulta de instalaciones por cliente | Como implementador, quiero consultar las instalaciones que he realizado agrupadas por cliente, para ubicar rápidamente la información que necesito. | Dado que el implementador tiene instalaciones registradas <br> Cuando accede a "Mis clientes" <br> Entonces el sistema lista los clientes junto con sus instalaciones asociadas. | EP10 |
| Gestión de Dispositivos IoT / US22 | Registro de dispositivo IoT | Como implementador, quiero registrar un dispositivo IoT y asociarlo a una vivienda y ambiente, para mantener organizada la información de cada instalación. | Dado que el implementador está configurando una instalación <br> Cuando registra un dispositivo indicando vivienda y ambiente <br> Entonces el sistema guarda el dispositivo y lo asocia correctamente. | EP11 |
| Gestión de Dispositivos IoT / US23 | Identificación de dispositivos que requieren atención | Como implementador, quiero identificar qué dispositivos presentan alertas o fallas, para priorizar mi trabajo de mantenimiento. | Dado que existen dispositivos con alertas activas <br> Cuando el implementador accede a su panel de dispositivos <br> Entonces el sistema resalta los dispositivos que requieren revisión. | EP11 |
| Control Remoto / US24 | Control remoto de un dispositivo compatible | Como dueño de hogar, quiero ejecutar acciones remotas sobre un dispositivo compatible, para administrar mi vivienda sin necesidad de estar físicamente junto al dispositivo. | Dado que el dueño de hogar tiene un dispositivo compatible con control remoto <br> Cuando ejecuta una acción desde la aplicación <br> Entonces el sistema aplica la acción y actualiza el estado del dispositivo. | EP12 |
| Control Remoto / US25 | Incorporación de una nueva categoría de dispositivo | Como dueño de hogar, quiero incorporar una nueva categoría de dispositivo a mi ecosistema, para ampliar mi hogar inteligente sin reemplazar lo ya instalado. | Dado que el dueño de hogar selecciona una nueva solución del catálogo <br> Cuando confirma su incorporación <br> Entonces el sistema la agrega a su ecosistema manteniendo activas las soluciones previas. | EP12 |

## 3.2. Impact Mapping

El Impact Mapping se elaboró a partir de los objetivos de negocio (Business Outcomes) definidos en el Lean UX Canvas del Capítulo I, distinguiendo los dos segmentos objetivo de Setrya: dueños de hogar e implementadores de hogar inteligente.

### 3.2.1. Impact Mapping — Segmento: Dueño de hogar

- **Goal (¿Por qué?):** Incrementar el uso recurrente de Setrya y la ampliación progresiva del ecosistema IoT de la vivienda.
  - **Actor (¿Quién?): Dueño de hogar**
    - **Impact (¿Cómo debe cambiar su comportamiento?):** Consultar el estado de su hogar con frecuencia y confiar en las alertas generadas.
      - **Deliverable (¿Qué podemos construir?):** Dashboard Centralizado del Hogar (EP02)
      - **Deliverable:** Centro de Alertas y Notificaciones (EP06)
      - **Deliverable:** Mediciones e Históricos (EP07)
    - **Impact:** Reconocer oportunamente eventos de riesgo (térmicos, de seguridad y eléctricos) y responder ante ellos.
      - **Deliverable:** Monitoreo Térmico (EP03)
      - **Deliverable:** Detección Acústica y Visual (EP04)
      - **Deliverable:** Protección Eléctrica Inteligente (EP05)
    - **Impact:** Ampliar su ecosistema inteligente incorporando nuevas soluciones sin reemplazar lo instalado.
      - **Deliverable:** Catálogo de Soluciones IoT (EP08)
      - **Deliverable:** Control Remoto y Expansión Modular (EP12)
    - **Impact:** Solicitar apoyo especializado cuando lo necesite, sin depender de medios externos.
      - **Deliverable:** Solicitud de Implementadores (EP09)

### 3.2.2. Impact Mapping — Segmento: Implementador de hogar inteligente

- **Goal (¿Por qué?):** Incrementar la adopción profesional de Setrya y mejorar la organización y trazabilidad de las instalaciones realizadas.
  - **Actor (¿Quién?): Implementador de hogar inteligente**
    - **Impact (¿Cómo debe cambiar su comportamiento?):** Administrar clientes e instalaciones desde una misma herramienta en lugar de registros externos.
      - **Deliverable:** Gestión de Clientes e Instalaciones (EP10)
    - **Impact:** Registrar y ubicar con rapidez los dispositivos que ha instalado para cada vivienda.
      - **Deliverable:** Gestión de Dispositivos IoT (EP11)
    - **Impact:** Priorizar su trabajo identificando primero las instalaciones o dispositivos que requieren atención.
      - **Deliverable:** Centro de Alertas y Notificaciones (EP06)
      - **Deliverable:** Mediciones e Históricos (EP07)
    - **Impact:** Aceptar y dar seguimiento a nuevas solicitudes de servicio generadas por los dueños de hogar.
      - **Deliverable:** Solicitud de Implementadores (EP09)

## 3.3. Product Backlog

| # Orden | User Story ID | Título | Story Points (1/2/3/5/8) |
|---------|----------------|--------|----------------------------|
| 1 | US01 | Registro de usuario | 3 |
| 2 | US02 | Inicio de sesión | 2 |
| 3 | US03 | Recuperar contraseña | 2 |
| 4 | US04 | Visualización del estado general del hogar | 5 |
| 5 | US05 | Organización por ambientes | 3 |
| 6 | US06 | Configuración de niveles de alerta térmica | 3 |
| 7 | US07 | Recepción de alerta térmica | 5 |
| 8 | US08 | Recepción de alerta de seguridad | 5 |
| 9 | US09 | Revisión de evidencia de un evento | 3 |
| 10 | US10 | Detección de condición eléctrica anómala | 5 |
| 11 | US11 | Consulta de acción ejecutada | 2 |
| 12 | US12 | Listado centralizado de alertas | 3 |
| 13 | US13 | Configuración de preferencias de notificación | 2 |
| 14 | US14 | Consulta de histórico de mediciones | 3 |
| 15 | US15 | Consulta de histórico de eventos | 3 |
| 16 | US16 | Exploración del catálogo | 2 |
| 17 | US17 | Detalle de una solución del catálogo | 1 |
| 18 | US18 | Búsqueda de implementadores | 3 |
| 19 | US19 | Solicitud de servicio a un implementador | 3 |
| 20 | US20 | Registro de una nueva instalación | 3 |
| 21 | US21 | Consulta de instalaciones por cliente | 2 |
| 22 | US22 | Registro de dispositivo IoT | 3 |
| 23 | US23 | Identificación de dispositivos que requieren atención | 5 |
| 24 | US24 | Control remoto de un dispositivo compatible | 5 |
| 25 | US25 | Incorporación de una nueva categoría de dispositivo | 3 |
