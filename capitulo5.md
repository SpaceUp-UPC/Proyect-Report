# Capítulo V: Solution UI/UX Design 
## 5.1. Style Guidelines. 
### 5.1.1. General Style Guidelines. 


Las guías generales de estilo de Sentrya establecen los criterios visuales y de comunicación utilizados en la Landing Page y en la aplicación Web. Su finalidad es mantener una experiencia visual consistente, clara y reconocible en todos los puntos de interacción de la solución.

#### Branding

Sentrya utiliza una identidad visual moderna y tecnológica orientada a transmitir seguridad, confianza, protección y control del hogar mediante soluciones IoT.

#### Iconography

Se emplean iconos simples y reconocibles para representar funcionalidades como dispositivos, alertas, ambientes, históricos, soluciones e implementadores.

#### Typography

Se utiliza una tipografía sans-serif que prioriza la legibilidad y establece una jerarquía visual mediante títulos, subtítulos, textos descriptivos, etiquetas y botones.

#### Colors

<img src="Capitulo5/Colors.PNG" style="max-width:700px; max-height:800px; width:auto; height:auto;">

La interfaz utiliza una paleta basada principalmente en tonos oscuros, neutros y acentos cálidos, manteniendo contraste suficiente para diferenciar acciones, estados y alertas.

#### Spacing

Se mantiene un sistema de espaciado consistente entre tarjetas, botones, formularios y secciones para evitar saturación visual y facilitar la lectura.

#### Communication Tone

El lenguaje utilizado por Sentrya es claro, directo, profesional y cercano, especialmente en mensajes relacionados con seguridad, alertas y estado de los dispositivos.

### 5.1.2. Web, Mobile and IoT Style Guidelines

Las guías específicas de plataforma de Sentrya establecen los criterios visuales y de interacción que deben mantenerse en los diferentes componentes de la solución. Para el alcance actual del proyecto se consideran principalmente la aplicación Web y los dispositivos IoT, debido a que la aplicación móvil aún no forma parte de la implementación actual.

#### Web Style Guidelines

La aplicación Web de Sentrya mantiene los lineamientos definidos en el sistema de diseño general, adaptándolos a una interfaz orientada al monitoreo y gestión del hogar.

Los principales criterios son:

- **Navegación:** se utiliza un menú lateral para acceder a las principales funcionalidades de acuerdo con el rol del usuario.
- **Componentes:** se utilizan tarjetas para representar ambientes, dispositivos, alertas, soluciones e implementadores.
- **Botones:** las acciones principales utilizan botones visualmente diferenciados para facilitar su identificación.
- **Estados:** los estados de los dispositivos y alertas se representan mediante indicadores visuales que permiten distinguir situaciones normales, preventivas y críticas.
- **Información:** los datos de sensores, históricos y alertas se presentan mediante tarjetas, indicadores y gráficos para facilitar su interpretación.
- **Consistencia:** los colores, tipografías, iconos, espaciados y componentes mantienen el mismo estilo en las diferentes pantallas del Web Front.

#### IoT Style Guidelines

Los dispositivos IoT de Sentrya utilizan una interacción física mínima, priorizando indicadores simples y fácilmente reconocibles para comunicar su estado.

Los principales criterios son:

- **Indicadores de estado:** los dispositivos pueden utilizar LEDs u otros indicadores para comunicar estados de funcionamiento.
- **Interacción mínima:** se reduce la necesidad de interacción física del usuario, priorizando la automatización.
- **Alertas:** las situaciones detectadas por los sensores son comunicadas mediante el sistema Web y los mecanismos de notificación definidos.
- **Seguridad:** la comunicación entre los dispositivos, el Edge Service y el backend debe realizarse mediante conexiones autenticadas y cifradas.
- **Baja latencia:** las situaciones críticas deben poder procesarse localmente mediante el Edge Service.
- **Consistencia:** los estados mostrados físicamente por los dispositivos deben corresponder con los estados representados en la aplicación Web.

De esta manera, los lineamientos de estilo permiten mantener una experiencia consistente entre la interfaz Web y los dispositivos físicos que forman parte de la solución IoT.


## 5.2. Information Architecture. 
La arquitectura de información de Sentrya organiza y estructura el contenido disponible en el Landing Page y en la aplicación Web, permitiendo que los usuarios encuentren de forma clara y eficiente la información y funcionalidades de la solución. La estructura considera las necesidades de los principales usuarios de la plataforma, principalmente dueños de hogar e implementadores.

### 5.2.1. Organization Systems

La arquitectura de información de Sentrya organiza el contenido de la Landing Page y de la aplicación Web de acuerdo con su función, contexto y tipo de usuario. Para ello, se consideran diferentes sistemas de organización que permiten estructurar la información de manera clara y facilitar su comprensión.

#### Jerárquico

La información se organiza desde los contenidos generales hacia las funcionalidades específicas de la solución.

<img src="Capitulo5/5.2.1.png" style="max-width:700px; max-height:800px; width:auto; height:auto;">

Secuencial
La organización secuencial se utiliza en procesos que requieren que el usuario complete diferentes pasos para alcanzar un objetivo.
En Sentrya, este tipo de organización se aplica principalmente en procesos como:
- Registro de usuario.
- Inicio de sesión.
- Búsqueda de un implementador.
- Consulta del perfil de un implementador.
- Solicitud de un servicio.
- Gestión de una solicitud de instalación.

Por tópicos
La información de Sentrya se agrupa según el tema o funcionalidad que representa. En la aplicación Web se consideran principalmente los siguientes tópicos:
Tópico	Información relacionada
Monitoreo	Ambientes, dispositivos y mediciones
Seguridad	Alertas y eventos detectados
Históricos	Registros y mediciones anteriores
Soluciones	Catálogo de soluciones IoT
Servicios	Implementadores y solicitudes
Gestión	Clientes, instalaciones y dispositivos


Esta organización permite que el usuario encuentre información relacionada dentro de una misma categoría funcional.
Según audiencia
La aplicación Web organiza sus funcionalidades de acuerdo con el tipo de usuario. Se consideran principalmente dos perfiles:
- Dueño de hogar: accede a funcionalidades relacionadas con el monitoreo, gestión y seguridad de su vivienda.
- Implementador: accede a funcionalidades relacionadas con la atención de solicitudes, clientes, instalaciones y dispositivos.
De esta manera, cada usuario visualiza una estructura de información acorde con las actividades que puede realizar dentro de Sentrya.

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

<img src="Capitulo5/5.3.png" style="max-width:700px; max-height:800px; width:auto; height:auto;">

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

<img src="Capitulo5/LandingPageWireframe1.png" style="max-width:700px; max-height:800px; width:auto; height:auto;">

<img src="Capitulo5/LandingPageWireframe2.png" style="max-width:700px; max-height:800px; width:auto; height:auto;">

### 5.3.2. Landing Page Mock-up. 
<img src="Capitulo5/LandingMockup1.png" style="max-width:700px; max-height:800px; width:auto; height:auto;">

<img src="Capitulo5/LandingMockup2.png" style="max-width:700px; max-height:800px; width:auto; height:auto;">

## 5.4. Applications UX/UI Design. 
### 5.4.1. Applications Wireframes. 

<img src="Capitulo5/Wireframe1.png" style="max-width:700px; max-height:800px; width:auto; height:auto;">
<img src="Capitulo5/Wireframe2.png" style="max-width:700px; max-height:800px; width:auto; height:auto;">
<img src="Capitulo5/Wireframe3.png" style="max-width:700px; max-height:800px; width:auto; height:auto;">
<img src="Capitulo5/Wireframe4.png" style="max-width:700px; max-height:800px; width:auto; height:auto;">
<img src="Capitulo5/Wireframe5.png" style="max-width:700px; max-height:800px; width:auto; height:auto;">
<img src="Capitulo5/Wireframe6.png" style="max-width:700px; max-height:800px; width:auto; height:auto;">
<img src="Capitulo5/Wireframe7.png" style="max-width:700px; max-height:800px; width:auto; height:auto;">
<img src="Capitulo5/Wireframe8.png" style="max-width:700px; max-height:800px; width:auto; height:auto;">
<img src="Capitulo5/Wireframe9.png" style="max-width:700px; max-height:800px; width:auto; height:auto;">

### 5.4.2. Applications Wireflow Diagrams. 
<img src="Capitulo5/Wireflow UX de Sentrya en español.png" style="max-width:700px; max-height:800px; width:auto; height:auto;">

### 5.4.3. Applications Mock-ups. 

<img src="Capitulo5/Mockup1.PNG" style="max-width:700px; max-height:800px; width:auto; height:auto;">
<img src="Capitulo5/Mockup2.PNG" style="max-width:700px; max-height:800px; width:auto; height:auto;">
<img src="Capitulo5/Mockup3.PNG" style="max-width:700px; max-height:800px; width:auto; height:auto;">
<img src="Capitulo5/Mockup4.PNG" style="max-width:700px; max-height:800px; width:auto; height:auto;">
<img src="Capitulo5/Mockup5.PNG" style="max-width:700px; max-height:800px; width:auto; height:auto;">
<img src="Capitulo5/Mockup6.PNG" style="max-width:700px; max-height:800px; width:auto; height:auto;">
<img src="Capitulo5/Mockup7.PNG" style="max-width:700px; max-height:800px; width:auto; height:auto;">
<img src="Capitulo5/Mockup8.PNG" style="max-width:700px; max-height:800px; width:auto; height:auto;">
<img src="Capitulo5/Mockup9.PNG" style="max-width:700px; max-height:800px; width:auto; height:auto;">
<img src="Capitulo5/Mockup10.PNG" style="max-width:700px; max-height:800px; width:auto; height:auto;">
<img src="Capitulo5/Mockup11.PNG" style="max-width:700px; max-height:800px; width:auto; height:auto;">


### 5.4.4. Applications User Flow Diagrams. 
<img src="Capitulo5/Flujo UX de Sentrya para Hogar e Implementadores.png" style="max-width:700px; max-height:800px; width:auto; height:auto;">

## 5.5. Applications Prototyping. 
[Link a Prototipo](https://www.figma.com/proto/mhFUTeLhAmlhVzSYXVqVsk/Sentrya?node-id=4-64&p=f&t=Zn6KBqUbSSFouWeO-0&scaling=min-zoom&content-scaling=fixed&page-id=0%3A1)

<img src="Capitulo5/prototipo.PNG" style="max-width:700px; max-height:800px; width:auto; height:auto;">

## 5.6. IoT Device Design.

La solución IoT propuesta para Sentrya está orientada al monitoreo preventivo de seguridad y condiciones ambientales dentro de una vivienda. El diseño considera tres subsistemas principales, cada uno compuesto por sensores encargados de recopilar información del entorno y actuadores capaces de ejecutar acciones automáticas ante determinadas condiciones.

Los subsistemas definidos son: seguridad mediante detección acústica y visual, monitoreo de temperatura y control de humedad ambiental mediante un humidificador. Estos dispositivos se integran mediante un controlador IoT Edge que procesa las mediciones, aplica reglas de automatización y establece comunicación con la plataforma Sentrya.

| Dispositivo | Sensores (magnitud y unidad) | Actuadores |
|---|---|---|
| Seguridad | Cámara (resolución en px, tasa en fps) y sensor de sonido (nivel sonoro en dB(A), muestreo en kHz) | Sirena (≈ 95 dB a 1 m), cerradura inteligente de puertas (bloqueo electromecánico) y LED de estado |
| Monitoreo de humedad | Sensor de humedad relativa (% HR) | Humidificador ultrasónico (encendido/apagado mediante módulo relé o interfaz de control compatible) y LED de estado |
| Monitoreo de temperatura | Sensor de temperatura (°C) | Ventilador / extractor (control por relé o PWM, 0–100 %), aire acondicionado inteligente (encendido y consigna en °C), buzzer y LED de estado |

Las decisiones de diseño se basan principalmente en los siguientes criterios:

- **Procesamiento en el borde (Edge Computing):** Las lecturas de los sensores y las reglas de automatización se procesan localmente para reducir la dependencia de la conexión a Internet. Esto permite responder a eventos de seguridad, cambios de temperatura y variaciones de humedad sin depender exclusivamente de los servicios cloud.

- **Baja latencia:** Las situaciones críticas requieren que los dispositivos actúen oportunamente. Por ejemplo, ante incrementos anómalos de temperatura, el sistema activa los mecanismos de enfriamiento correspondientes. Asimismo, cuando la humedad desciende por debajo del umbral configurado, el controlador puede activar automáticamente el humidificador.

- **Disponibilidad:** Las acciones locales, como la activación de la sirena, el enfriamiento y el control del humidificador, pueden ejecutarse incluso cuando la comunicación con el backend no está disponible. Los eventos registrados se sincronizan posteriormente cuando se restablece la conectividad.

- **Privacidad:** El procesamiento de imagen y sonido se realiza preferentemente en el dispositivo Edge, enviándose al backend únicamente los eventos y las evidencias necesarias para el funcionamiento del sistema.

- **Seguridad:** La comunicación entre los dispositivos IoT y el backend utiliza conexiones autenticadas y cifradas mediante protocolos como MQTT sobre TLS o HTTPS.

- **Interacción mínima:** Los dispositivos comunican sus estados mediante indicadores LED, señales sonoras o notificaciones desde la aplicación. Las funciones automáticas de monitoreo ambiental buscan reducir la intervención manual del propietario.

- **Prevención de falsos positivos:** Las alertas de seguridad se generan considerando la correlación de diferentes señales y ventanas de validación. En el caso de temperatura y humedad, se emplean lecturas consecutivas e histéresis para evitar activaciones innecesarias ante fluctuaciones momentáneas.

La arquitectura considera un **IoT Edge Service** como elemento central encargado de recibir la información generada por los sensores, aplicar reglas locales, controlar los actuadores y comunicarse con el backend de Sentrya.

Se propone utilizar una ESP32 para el procesamiento de imagen y sonido, mientras que los otros nodos se encargan de recopilar las mediciones de temperatura y humedad, así como de controlar los actuadores correspondientes.

El subsistema de humedad utiliza un sensor conectado a un ESP32 para registrar periódicamente la humedad relativa del ambiente. Cuando los valores se encuentran por debajo del límite inferior configurado, el controlador activa el humidificador mediante una interfaz de control adecuada. Una vez alcanzado el nivel de humedad establecido, el sistema desactiva el actuador para evitar un funcionamiento innecesario.

### Parámetros de referencia

Los umbrales son valores iniciales configurables desde la aplicación y deben calibrarse según la vivienda y el hardware instalado.

| Subsistema | Parámetro | Valor de referencia |
|---|---|---|
| Temperatura | T1 (Warning) | 45 °C |
| Temperatura | T2 (Critical) | 57 °C |
| Temperatura | Acción en T1 | Aviso al usuario + enfriamiento nivel 1 (ventilador al 50 %) |
| Temperatura | Acción en T2 | Aviso al usuario + enfriamiento máximo (ventilador al 100 % + A/C a 22 °C) + alerta crítica |
| Temperatura | Velocidad de aumento (opcional) | ≥ 8 °C/min → Critical |
| Temperatura | Histéresis para bajar de estado | 2 °C |
| Temperatura | Frecuencia de lectura | 30 s (Normal), 5 s (Warning), 1 s (Critical) |
| Temperatura | Confirmación de Critical | 3 lecturas consecutivas ≥ T2 |
| Temperatura | Rango y precisión del sensor | −40 a 125 °C, ±0.5 °C (referencia sujeta al sensor seleccionado) |
| Humedad | Rango objetivo | 40–60 % HR |
| Humedad | H1 (humedad baja) | < 40 % HR |
| Humedad | H2 (humedad alta) | > 60 % HR |
| Humedad | Acción en H1 | Notificar al usuario + activar humidificador |
| Humedad | Acción en H2 | Notificar al usuario + mantener humidificador apagado |
| Humedad | Umbral de desactivación automática | ≥ 50 % HR |
| Humedad | Histéresis | Activación por debajo de 40 % HR y desactivación al alcanzar 50 % HR |
| Humedad | Frecuencia de lectura | Cada 10 s |
| Humedad | Confirmación de condición anómala | 3 lecturas consecutivas fuera del rango configurado |
| Humedad | Envío de telemetría | Cada 60 s |
| Humedad | Unidad de medición | Porcentaje de humedad relativa (% HR) |
| Humedad | Precisión del sensor | Según especificaciones del modelo seleccionado |
| Seguridad | Detección de persona | Confianza ≥ 70 % |
| Seguridad | Reconocimiento de persona conocida | Coincidencia ≥ 80 % |
| Seguridad | Sonido anormal | Ver criterio en 5.6.3 |
| Seguridad | Ventana de correlación persona desconocida + sonido | ≤ 10 s |
| Seguridad | Video / audio | 1280 × 720 px a 15 fps / 16 kHz |
| Seguridad | Ventana de validación del usuario | 30 s; el evento se escala según el protocolo de seguridad configurado |



### 5.6.1 UML Deployment Diagram
Este diagrama representa físicamente dónde se encuentran los sensores y cómo se comunican con el Edge Service y la infraestructura cloud.

<img src="assets/IOTDD1.png" alt="IOT DD1">


Los tres dispositivos se encuentran dentro de la vivienda y se comunican con el IoT Edge Service. El controlador recibe imágenes y eventos de sonido, mediciones eléctricas (V, A, W) y lecturas de temperatura (°C). A su vez, comanda los actuadores locales: relé inteligente, sirena, cerradura de caja fuerte y sistema de enfriamiento (ventilador y A/C). Esto permite ejecutar decisiones críticas sin esperar respuesta del servidor. La comunicación con la nube se realiza mediante MQTT/TLS o HTTPS.


### 5.6.2 UML Component Diagram
Los módulos de cámara, sonido, humedad y temperatura envían sus datos al *Sensor Manager* del Edge Service, que los distribuye al *Person Detection Service*, al *Sound Analysis Service* y al *Rules Engine*. El *Rules Engine* genera eventos hacia el *IoT Communication Client* y emite órdenes al *Local Safety Controller*, que gobierna los actuadores (relé, sistema de enfriamiento, sirena y cerradura de caja fuerte). Los eventos relevantes se envían al backend, que se encarga del almacenamiento, las notificaciones y el escalamiento a autoridades.

<img src="assets/IOTCD1.png" alt="IOT CD1">


Las reglas principales del Rules Engine son:

Seguridad:
```
IF person_detected = true
AND person_recognized = false
AND suspicious_sound = true          // ventana de 10 s
THEN
    ACTIVATE_SIREN
    LOCK_DOORS
    CAPTURE_EVIDENCE
    CREATE SECURITY_ALERT (HIGH)
    NOTIFY_USER
    REQUEST_VALIDATION (30 s)
    IF user_confirms OR no_response_in_30s
        NOTIFY_AUTHORITIES (with evidence)
    ELSE IF user_rejects
        DEACTIVATE_SIREN, state = MONITORING
```

Temperatura:
```
IF temperature < T1 (45 °C)
    -> state = NORMAL
       COOLING_OFF (cuando baja de T1 − 2 °C)
ELSE IF temperature < T2 (57 °C)
    -> state = WARNING
    -> NOTIFY_USER
    -> START_COOLING (level 1: fan 50 %)
    -> INCREASE_SAMPLING_RATE
ELSE IF 3 consecutive readings >= T2
    -> state = CRITICAL
    -> NOTIFY_USER
    -> START_COOLING (level 2: fan 100 % + A/C 22 °C)
    -> ACTIVATE_BUZZER
    -> NOTIFY_AUTHORITIES
```

Humedad:
```
IF humidity < H1 (40 % HR)
    AND 3 consecutive readings confirm low humidity
    THEN
        -> state = LOW_HUMIDITY
        -> ACTIVATE_HUMIDIFIER
        -> NOTIFY_USER
        -> CREATE_HUMIDITY_EVENT

    ELSE IF humidity >= 50 % HR
        -> DEACTIVATE_HUMIDIFIER

        IF humidity <= H2 (60 % HR)
            -> state = NORMAL

    IF humidity > H2 (60 % HR)
    AND 3 consecutive readings confirm high humidity
    THEN
        -> state = HIGH_HUMIDITY
        -> DEACTIVATE_HUMIDIFIER
        -> NOTIFY_USER
        -> CREATE_HUMIDITY_WARNING

    IF humidity_sensor_disconnected = true
        -> DEACTIVATE_HUMIDIFIER
        -> CREATE_DEVICE_ERROR
        -> NOTIFY_USER
```



### 5.6.3 Camera + Sound Detector
El sistema analiza primero si hay una persona en el área supervisada y si puede ser reconocida. Si es desconocida, se analiza además el entorno sonoro. Cuando una persona desconocida y un sonido anormal ocurren dentro de una ventana de 10 s, se genera un evento de alta prioridad. El Edge Service ejecuta de inmediato las acciones locales: activa la sirena, bloquea las puertas y captura evidencia. En paralelo notifica al usuario y le pide validar el evento durante 30 s. Si el usuario lo confirma, o no responde en ese tiempo, se escala a las autoridades con la evidencia adjunta. Si lo rechaza, la sirena se apaga y el sistema vuelve a monitoreo. Las cajas fuertes solo se desbloquean con autenticación del usuario desde la aplicación.

<img src="assets/IOTCSD.png" alt="IOT CSD">

**Criterio para decidir que un sonido es anormal.** El sensor de audio no interpreta sonidos por sí mismo; el Sound Analysis Service del Edge Service combina dos condiciones:

1. **Nivel relativo al ruido de fondo (dB(A)).** El sistema calcula continuamente el ruido de fondo *L_bg* como la mediana móvil de los últimos 5 min. Un sonido es candidato si su nivel pico es ≥ *L_bg* + 20 dB y, además, ≥ 65 dB(A). Así se ignoran variaciones pequeñas en una casa silenciosa y se adapta a viviendas ruidosas.
2. **Clasificación del tipo de sonido.** Se analizan ventanas de 1 s (50 % de solape, 16 kHz) con un modelo de clasificación de audio sobre espectrograma log-mel, entrenado para las clases: rotura de vidrio, golpe o patada a puerta, grito, disparo y alarma. La clase debe tener confianza ≥ 0.75, o ≥ 0.65 entre 22:00 y 06:00, cuando la vivienda debería estar en silencio.

Un sonido es **sospechoso** si cumple ambas condiciones. Los sonidos impulsivos (vidrio, golpe, disparo) requieren una sola ventana. Los sostenidos (grito, alarma) requieren 2 ventanas consecutivas. Los sonidos cotidianos (TV, música, mascotas, electrodomésticos) pertenecen a clases normales y no disparan el evento. Cuando el usuario marca una alerta como falso positivo, esa muestra se usa para ajustar el umbral.



### 5.6.4 Humidity Sensor + Humidifier
El sistema considera como referencia un rango objetivo de humedad relativa entre 40 % y 60 %, cuyos valores podrán modificarse posteriormente desde la aplicación Sentrya. Cuando el sensor detecta que la humedad se encuentra por debajo del 40 % HR durante tres lecturas consecutivas, el controlador identifica una condición de humedad baja. Ante esta situación, el sistema activa automáticamente el humidificador, cuya función consiste en incrementar la humedad ambiental mediante la dispersión de vapor o partículas finas de agua. El actuador permanece encendido mientras se ejecuta la regla de humidificación y se desactiva cuando la humedad alcanza el umbral de apagado configurado, inicialmente establecido en 50 % HR. Este mecanismo utiliza histéresis para evitar que pequeñas variaciones alrededor del límite inferior provoquen ciclos constantes de encendido y apagado. En caso de que la humedad supere el 60 % HR, el controlador mantiene el humidificador apagado y genera una notificación para informar al propietario sobre la condición registrada.

<img src="assets/IOTPFS1.png" alt="IOT PFS1">



### 5.6.5 Temperature Sensor

El monitoreo usa dos umbrales configurables, T1 = 45 °C y T2 = 57 °C. Mientras la temperatura sea menor que T1, el sistema permanece en estado *Normal*, con lecturas cada 30 s. Al alcanzar T1 pasa a *Warning*: avisa al usuario, activa el enfriamiento nivel 1 (ventilador al 50 %) y lee cada 5 s. Al alcanzar T2, confirmada con 3 lecturas consecutivas, pasa a *Critical*: avisa al usuario, activa el enfriamiento máximo (ventilador al 100 % y A/C a 22 °C), activa el buzzer y notifica a las autoridades. Para evitar oscilaciones, el retorno a un estado inferior requiere que la temperatura baje 2 °C por debajo del umbral, y los actuadores se apagan al volver a *Normal*.

<img src="assets/IOTTS.png" alt="IOT TS">




### 5.6.6 Overall IoT Interaction

El diagrama integra los tres subsistemas de Sentrya, los cuales operan de manera concurrente para supervisar diferentes condiciones dentro de la vivienda. El subsistema de seguridad analiza la información capturada por la cámara y el sensor de sonido para identificar eventos que puedan representar situaciones de intrusión. El subsistema de temperatura registra continuamente las condiciones térmicas y activa los mecanismos de enfriamiento cuando se superan los umbrales configurados. Por su parte, el subsistema de humedad registra el porcentaje de humedad relativa y controla el humidificador cuando se detectan condiciones inferiores al límite establecido. Los tres subsistemas transmiten sus mediciones y eventos hacia el IoT Edge Service, que centraliza la información y ejecuta las reglas locales correspondientes.
Cuando se identifica una condición anómala, el controlador determina las acciones que deben ejecutarse según el tipo de evento:

- **Seguridad:** Activación de sirena, bloqueo de puertas, captura de evidencia y notificación al propietario.
- **Temperatura:** Activación de ventiladores, aire acondicionado y mecanismos de advertencia según el nivel de alerta.
- **Humedad:** Activación o desactivación del humidificador según los valores registrados y los límites establecidos.

Las acciones sobre los actuadores se realizan localmente, sin necesidad de esperar una respuesta del backend, lo que permite mantener las funciones de automatización ante interrupciones temporales de conectividad. Posteriormente, el IoT Edge Gateway transmite los eventos y las mediciones relevantes al backend de Sentrya. El backend almacena la telemetría recibida, administra los eventos generados y permite consultar las condiciones de los dispositivos desde la aplicación web o móvil. A través de la interfaz de Sentrya, el propietario puede visualizar el estado de sus sensores, revisar alertas, consultar mediciones históricas y ejecutar acciones sobre los dispositivos compatibles. En el caso del humidificador, la aplicación permite consultar la humedad actual, identificar si el dispositivo se encuentra encendido o apagado y conocer si está funcionando en modo automático o manual. El diagrama de secuencia representa el intercambio de mensajes entre los sensores, el IoT Edge Service, los actuadores, el backend, el servicio de notificaciones y la aplicación. Ante una condición de humedad baja, por ejemplo, el sensor transmite la medición al controlador, el Rules Engine verifica el cumplimiento de las condiciones y el Local Safety Controller ordena activar el humidificador. La confirmación de la acción y las mediciones posteriores son comunicadas al backend, permitiendo que el propietario visualice el estado actualizado del sistema.
De esta manera, la arquitectura propuesta integra la detección de eventos de seguridad, el monitoreo térmico y la automatización de humedad dentro de una misma plataforma, manteniendo una interacción coordinada entre sensores, actuadores y servicios digitales.

**Figura: Diagrama de interacción general del sistema IoT.**


<img src="assets/IOTALL1.png" alt="IOT ALL1">

**Figura: Diagrama de secuencia general del sistema IoT.**

<img src="assets/IOTECS1.png" alt="IOT ECS1">




