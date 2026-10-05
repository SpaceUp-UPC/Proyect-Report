# Capítulo V: Solution UI/UX Design 
## 5.1. Style Guidelines. 
### 5.1.1. General Style Guidelines. 

| Color | Uso |
|---|---|
| Primary | Botones principales, navegación, elementos importantes |
| Accent | Destacar acciones, indicadores y elementos seleccionados |
| Background | Fondo general de la aplicación |
| Surface | Cards, formularios y contenedores |
| Text | Textos principales |
| Success | Estados correctos |
| Warning | Alertas preventivas |
| Error/Critical | Situaciones críticas |

### 5.1.2. Web, Mobile and IoT Style Guidelines. 
## 5.2. Information Architecture. 
La arquitectura de información de Sentrya organiza y estructura el contenido disponible en el Landing Page y en la aplicación Web, permitiendo que los usuarios encuentren de forma clara y eficiente la información y funcionalidades de la solución. La estructura considera las necesidades de los principales usuarios de la plataforma, principalmente dueños de hogar e implementadores.

### 5.2.1. Organization Systems. 


### 5.2.2. Labeling Systems. 
Etiquetas del Landing Page
| Etiqueta | Descripción |
|---|---|
| **Inicio** | Acceso a la sección principal de la Landing Page. |
| **Problema** | Presenta las principales necesidades que busca resolver Sentrya. |
| **Soluciones** | Presenta las soluciones IoT ofrecidas por Sentrya. |
| **Cómo funciona** | Explica el funcionamiento de la solución mediante tres pasos. |
| **Equipo** | Presenta a los integrantes responsables del proyecto. |
| **Contacto** | Permite al usuario comunicarse con el equipo de Sentrya. |
| **Descargar app** | Acceso a las opciones disponibles para utilizar Sentrya. |

Aplicación Web — Dueño de hogar
| Etiqueta | Descripción |
|---|---|
| **Inicio** | Muestra el resumen general del estado del hogar. |
| **Mis ambientes** | Permite consultar los ambientes y dispositivos asociados al hogar. |
| **Alertas** | Permite consultar y revisar eventos que requieren atención. |
| **Históricos** | Permite consultar mediciones y eventos registrados anteriormente. |
| **Catálogo** | Muestra las soluciones y servicios disponibles. |
| **Implementadores** | Permite buscar especialistas para instalación o mantenimiento. |
| **Ver detalle** | Permite consultar información ampliada de una solución o elemento. |
| **Solicitar servicio** | Permite iniciar una solicitud a un implementador. |
| **Control remoto** | Permite ejecutar acciones sobre los dispositivos compatibles. |

Aplicación Web — Implementador
| Etiqueta | Descripción |
|---|---|
| **Panel** | Presenta un resumen de las actividades pendientes del implementador. |
| **Solicitudes** | Permite gestionar solicitudes de servicio recibidas. |
| **Clientes** | Permite consultar los clientes asociados al implementador. |
| **Instalaciones** | Permite gestionar las instalaciones realizadas o pendientes. |
| **Dispositivos** | Permite consultar los dispositivos asociados a las instalaciones. |
| **Históricos** | Permite consultar los registros históricos de las instalaciones y dispositivos. |
| **Aceptar** | Permite aceptar una solicitud pendiente. |
| **Revisar** | Permite consultar el detalle de una solicitud antes de tomar una decisión. |
| **Ver perfil** | Permite consultar la información del implementador. |

Criterios utilizados
Las etiquetas se definieron considerando los siguientes criterios:
- Claridad: utilizan términos que describen directamente la función.
- Consistencia: se mantiene el mismo término para una misma funcionalidad en las diferentes pantallas.
- Brevedad: se evita utilizar textos innecesariamente extensos en menús y botones.
- Orientación al usuario: se emplean términos comprensibles para dueños de hogar e implementadores.
- Diferenciación por rol: las etiquetas de la aplicación cambian según las necesidades del dueño de hogar o del implementador.

### 5.2.3. SEO Tags and Meta Tags 

| Página / sección | Title | Description | Keywords | Author |
|---|---|---|---|---|
| **Inicio** | Sentrya \| Hogar inteligente y seguro | Convierte tu vivienda en un hogar inteligente con soluciones IoT para seguridad, monitoreo y protección. | Sentrya, IoT, hogar inteligente, seguridad, monitoreo | SpaceUp |
| **Problema** | Problema \| Sentrya | Conoce los principales problemas relacionados con la seguridad, temperatura y consumo dentro del hogar. | seguridad del hogar, IoT, temperatura, consumo eléctrico | SpaceUp |
| **Soluciones** | Soluciones IoT \| Sentrya | Conoce las soluciones de seguridad, monitoreo térmico y protección eléctrica de Sentrya. | soluciones IoT, seguridad, temperatura, energía, Smart Home | SpaceUp |
| **Cómo funciona** | Cómo funciona \| Sentrya | Descubre cómo Sentrya permite seleccionar, instalar y monitorear soluciones inteligentes para el hogar. | IoT, Smart Home, instalación, monitoreo | SpaceUp |
| **Contacto** | Contacto \| Sentrya | Comunícate con el equipo de Sentrya para conocer más sobre nuestras soluciones para el hogar. | contacto, Sentrya, soporte, hogar inteligente | SpaceUp |

Ejemplo de Meta Tags
```html
<title>Sentrya | Hogar inteligente y seguro</title>

<meta
    name="description"
    content="Convierte tu vivienda en un hogar inteligente
    con soluciones IoT para seguridad, monitoreo y protección."
>

<meta
    name="keywords"
    content="Sentrya, IoT, hogar inteligente,
    seguridad, monitoreo, temperatura, energía"
>

<meta
    name="author"
    content="SpaceUp"
>
```

Open Graph
Para mejorar la presentación de la Landing Page cuando sea compartida mediante plataformas sociales o aplicaciones de mensajería, también pueden definirse etiquetas Open Graph:
```html
<meta
    property="og:title"
    content="Sentrya | Hogar inteligente y seguro"
>

<meta
    property="og:description"
    content="Soluciones IoT para proteger,
    monitorear y controlar tu hogar."
>

<meta
    property="og:type"
    content="website"
>

<meta
    property="og:site_name"
    content="Sentrya"
>
```


### 5.2.4. Searching Systems. 
El sistema de búsqueda de Sentrya se encuentra principalmente en la aplicación Web, dentro del módulo de Implementadores. Su objetivo es permitir que el usuario encuentre de manera rápida a especialistas que puedan realizar servicios relacionados con la instalación y mantenimiento de las soluciones IoT.
La búsqueda se organiza mediante criterios y filtros, permitiendo reducir los resultados de acuerdo con las necesidades del usuario. Los resultados presentan información resumida del implementador y permiten acceder posteriormente a su perfil para consultar información más detallada.

| Criterio | Descripción |
|---|---|
| **Nombre o servicio** | Permite buscar un implementador mediante texto relacionado con su nombre o servicio ofrecido. |
| **Ubicación** | Permite encontrar implementadores disponibles en una determinada zona. |
| **Especialidad** | Permite filtrar según el tipo de solución o servicio que puede realizar el implementador. |
| **Disponibilidad** | Permite identificar implementadores que se encuentran disponibles para atender una solicitud. |
| **Calificación** | Permite considerar la valoración obtenida por el implementador. |



Los resultados de búsqueda se presentan mediante tarjetas que permiten identificar rápidamente al implementador, su especialidad, ubicación y valoración. Desde el resultado seleccionado, el usuario puede acceder al perfil correspondiente y continuar con el proceso de solicitud del servicio.


### 5.2.5. Navigation Systems

El sistema de navegación de Sentrya permite a los usuarios desplazarse de manera clara y organizada entre las diferentes secciones de la Landing Page y de la aplicación Web. La navegación se estructura de acuerdo con las funcionalidades disponibles y el rol del usuario, facilitando el acceso a la información y reduciendo desplazamientos innecesarios.

#### Navegación de la Landing Page

La Landing Page cuenta con un menú de navegación principal que permite acceder a las diferentes secciones informativas de Sentrya:

| Elemento | Función |
|---|---|
| Inicio | Acceso a la sección principal de la Landing Page. |
| Problema | Presenta las necesidades que busca solucionar Sentrya. |
| Soluciones | Presenta las soluciones IoT ofrecidas por Sentrya. |
| Cómo funciona | Explica el funcionamiento general de la solución. |
| Equipo | Presenta información relacionada con el equipo. |
| Contacto | Permite acceder a los medios de contacto. |

#### Navegación de la aplicación Web

La aplicación Web utiliza un menú lateral para organizar las funcionalidades disponibles según el rol del usuario.

**Usuario propietario del hogar:**

- Inicio
- Mis ambientes
- Alertas
- Históricos
- Catálogo
- Implementadores

**Usuario implementador:**

- Panel
- Solicitudes
- Clientes
- Instalaciones
- Dispositivos
- Históricos

Esta organización permite que cada usuario acceda principalmente a las funcionalidades relacionadas con sus actividades dentro de Sentrya.

#### Técnicas de navegación

| Técnica | Aplicación en Sentrya |
|---|---|
| Menú lateral | Permite acceder a las principales funcionalidades de la aplicación Web. |
| Navegación jerárquica | Organiza las funcionalidades de acuerdo con el rol del usuario. |
| Botones de acción | Permiten ejecutar acciones específicas dentro de cada sección. |
| Enlaces internos | Permiten desplazarse entre contenidos y vistas relacionadas. |
| Navegación contextual | Presenta acciones relacionadas con la sección en la que se encuentra el usuario. |

La estructura de navegación busca que el usuario pueda identificar fácilmente las secciones disponibles y acceder a las funcionalidades necesarias de acuerdo con su rol.

## 5.3. Landing Page UI Design. 
### 5.3.1. Landing Page Wireframe. 
### 5.3.2. Landing Page Mock-up. 
## 5.4. Applications UX/UI Design. 
### 5.4.1. Applications Wireframes. 
### 5.4.2. Applications Wireflow Diagrams. 
### 5.4.2. Applications Mock-ups. 
### 5.4.3. Applications User Flow Diagrams. 
## 5.5. Applications Prototyping. 
## 5.6. IoT Device Design.
La solución IoT propuesta está orientada al monitoreo preventivo de seguridad, consumo eléctrico y condiciones ambientales dentro de una vivienda. El diseño considera tres dispositivos principales: un sistema de detección mediante cámara y sonido, un sensor de flujo/consumo eléctrico y un sensor de temperatura.
Las decisiones de diseño se basan principalmente en los siguientes criterios:
- Procesamiento en el borde (Edge Computing): las lecturas críticas y reglas de emergencia se procesan localmente para reducir la dependencia de la conexión a Internet.
- Baja latencia: las situaciones consideradas críticas requieren que el dispositivo pueda actuar inmediatamente.
- Disponibilidad: ciertas acciones, como interrumpir la alimentación eléctrica, pueden ejecutarse localmente aun cuando el servicio cloud no se encuentre disponible.
- Privacidad: el procesamiento de imágenes y sonido debe realizarse preferentemente en el dispositivo Edge, enviándose al backend únicamente eventos y evidencias estrictamente necesarias.
- Seguridad: toda comunicación entre los dispositivos IoT y el backend debe utilizar conexiones autenticadas y cifradas, por ejemplo MQTT sobre TLS o HTTPS.
- Interacción mínima: siguiendo los principios de IoT Device Physical Interfaces, el dispositivo debe comunicar sus estados mediante indicadores simples como LEDs, sonidos o notificaciones en la aplicación.
- Prevención de falsos positivos: las acciones de escalamiento externo, particularmente aquellas relacionadas con servicios de emergencia, requieren la correlación y validación de múltiples señales antes de ejecutarse.
La arquitectura considera un IoT Edge Controller como elemento central encargado de recibir información de los sensores, aplicar reglas locales y comunicarse con la plataforma backend.

### 5.6.1 UML Deployment Diagram
Este diagrama representa físicamente dónde se encuentran los sensores y cómo se comunican con el Edge Controller y la infraestructura cloud.

<img src="assets/IOTDD.png" alt="IOT DD">


Los tres dispositivos se encuentran dentro de la vivienda y se comunican con un IoT Edge Controller.
El Edge Controller permite que determinadas decisiones críticas se ejecuten localmente. Por ejemplo, si existe un incremento peligroso de consumo eléctrico, el controlador puede abrir el relé sin esperar una respuesta del servidor.

### 5.6.2 UML Component Diagram
El diagrama de componentes muestra la organización lógica de la solución IoT y las responsabilidades de cada módulo. Los dispositivos físicos capturan información del entorno y la envían al controlador Edge, donde se ejecutan servicios de análisis, detección y aplicación de reglas. Posteriormente, los eventos relevantes son enviados al backend, el cual se encarga del almacenamiento, generación de notificaciones y escalamiento de situaciones críticas. Esta separación facilita el mantenimiento y permite desacoplar la lógica de sensores, procesamiento y servicios cloud.
<img src="assets/IOTCD.png" alt="IOT CD">



Aquí la parte importante de la arquitectura es el Rules Engine.
Por ejemplo:

```IF unknown_person = true
AND suspicious_sound = true
THEN SECURITY_ALERT
```


Mientras que para temperatura:


```
IF temperature >= WARNING_THRESHOLD
    -> WARNING
```

```IF temperature >= CRITICAL_THRESHOLD
    -> CRITICAL_ALERT
```


Y para consumo eléctrico:

```IF power > NORMAL_THRESHOLD
OR sudden_power_spike = true
    -> CUT_POWER
    -> ALERT_USER
```


### 5.6.3 Camera + Sound Detector
Este diagrama describe el flujo de detección de posibles incidentes de seguridad utilizando información proveniente de la cámara y del sensor de sonido. El sistema analiza primero si existe una persona en el área supervisada y determina si esta puede ser reconocida. En caso de tratarse de una persona desconocida, se analiza adicionalmente el entorno sonoro. Cuando ambas condiciones, persona desconocida y sonido sospechoso, ocurren de manera simultánea, se genera un evento de alta prioridad, se notifica al usuario y se inicia un proceso de validación antes de realizar un posible escalamiento hacia las autoridades:

<img src="assets/IOTCSD.png" alt="IOT CSD">


### 5.6.4 Power Flow Sensor
Este diagrama representa el proceso de monitoreo del consumo eléctrico de los dispositivos conectados. El sensor obtiene valores de voltaje y corriente, a partir de los cuales se calcula el consumo energético. Si se detecta una variación anómala, el sistema determina si se trata únicamente de un consumo inusual o de un pico potencialmente peligroso. En el segundo caso, el controlador Edge puede abrir el relé inteligente para interrumpir de manera inmediata la alimentación del dispositivo afectado y posteriormente notificar al usuario:

<img src="assets/IOTPFS.png" alt="IOT PFS">



### 5.6.5 Temperature Sensor
El diagrama muestra el comportamiento del sistema de monitoreo de temperatura considerando dos niveles configurables de alerta. Mientras la temperatura permanezca por debajo del primer umbral, el sistema continúa operando en estado normal. Al superar el primer nivel, se genera una advertencia dirigida al usuario y se incrementa la frecuencia de monitoreo. Si la temperatura alcanza el segundo umbral, el evento pasa a ser crítico, generándose una alerta prioritaria y un proceso de validación para determinar si es necesario realizar un escalamiento hacia los servicios de emergencia:

<img src="assets/IOTTS.png" alt="IOT TS">




### 5.6.6 Overall IoT Interaction

El diagrama presenta una visión integrada del funcionamiento de los tres subsistemas IoT. Cada sensor opera de manera concurrente, supervisando de forma independiente la seguridad, el consumo eléctrico y la temperatura. Cuando se detecta una condición anómala, el subsistema correspondiente ejecuta las acciones definidas, tales como generar alertas, interrumpir la alimentación eléctrica o solicitar una validación de emergencia. Finalmente, los eventos generados y la telemetría son almacenados para su posterior consulta y análisis:

<img src="assets/IOTALL.png" alt="IOT ALL">

Este diagrama de secuencia muestra el intercambio de mensajes entre un sensor IoT, el controlador Edge, el backend, el servicio de notificaciones y la aplicación móvil. Dependiendo de la severidad del evento, el flujo puede limitarse al registro de telemetría, generar una advertencia o escalar hacia una situación crítica. La comunicación permite evidenciar cómo los eventos detectados en el entorno físico son procesados y convertidos en acciones visibles para el usuario:

<img src="assets/IOTECS.png" alt="IOT ECS">




