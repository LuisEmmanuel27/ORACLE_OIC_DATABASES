# Become An Application Integration Professional (2023) - Parte 2

## Application Integration on Oracle Cloud

### Fundamentals of Creating Integrations - Integration Design Fundamentals

#### What Is an OIC Integration?

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_1.png" alt="oic" width="700">
</div>

Las Integraciones son el ingrediente principal de Oracle Integration. Una integración incluye al menos una conexión (para las solicitudes enviadas a Oracle Integration) de `disparador/trigger` (origen) y una conexión (para las solicitudes enviadas desde Oracle Integration al destino) de `invocación/invoke` (destino)  y el `mapeo/mapping` de campos entre esas dos conexiones.

Cuando creas tus integraciones, construyes sobre las conexiones que ya has creado al definir cómo procesar los datos para las conexiones de disparador (origen) e invocación (destino). Esto puede incluir la definición del tipo de operaciones a realizar en los datos, los objetos y campos empresariales contra los cuales realizar esas operaciones, los esquemas requeridos, y así sucesivamente. Para hacer esto más fácil, las tareas de configuración más complejas son manejadas por Oracle Integration.

Una vez que tus conexiones de disparador (origen) e invocación (destino) están configuradas, las acciones de mapeo entre ambas se muestran para que puedas definir cómo se transfiere la información entre las estructuras de datos de disparador (origen) e invocación (destino) tanto para los mensajes de solicitud como para los de respuesta.

#### OIC Integration Styles

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_2.png" alt="oic" width="700">
</div>

- El Estilo de Integración de `Enrutamiento Básico/Basic Routing` ha sido descontinuado. Oracle recomienda que utilices el Estilo de Orquestación Dirigida por Aplicación, que proporciona más flexibilidad.

- Los patrones de integración de disparar y olvidar son manejados por los Estilos `Publicar en OIC/Publish to OIC` y `Suscribirse a OIC/Subscribe to OIC`. Por lo tanto, existe una dependencia en la que un Publicador debe ser configurado antes de crear el Suscriptor. Sin embargo, puedes tener más de una integración suscrita al mismo Publicador.

- La mayoría de las integraciones utilizarán el Estilo de `Orquestación Dirigida por Aplicación/App Driven Orchestration` ya que permite los cuatro patrones de interacción (interfaz síncrona [solicitud-respuesta], interfaz asíncrona [unidireccional], interfaz asíncrona con devolución de llamada, basado en eventos).

- El Estilo de `Orquestación Programada/Scheduled Orchestation` es útil para casos de uso que necesitan ser activados en un horario recurrente y/o bajo demanda.

- El Estilo de `Transferencia de Archivos/File Transfer` es actualmente **`idéntico`** al Estilo de Orquestación Programada.

#### Integration Style Patterns Described

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_3.png" alt="oic" width="700">
</div>

| Patrón | Descripción |
| --- | --- |
| Enrutamiento Básico | Este estilo de diseño de lienzo de integración ha sido descontinuado. |
| Publicar en OIC | Crea una integración en la que defines un adaptador de disparador para publicar mensajes a OIC a través de una interfaz o evento asincrónico. Esta integración está desacoplada de todos los suscriptores, ya que todas las integraciones participantes pueden activarse y desactivarse independientemente entre sí. |
| Suscribirse a OIC | Crea una integración en la que te suscribes a una integración publicadora existente. Luego defines un adaptador invocable para procesar mensajes que han sido publicados a OIC por esa integración. |
| Orquestación Impulsada por Aplicaciones | Crea una integración que utiliza capacidades básicas del Administrador de Procesos BPEL. Puedes incluir expresiones Switch y construcciones loop, así como estrategias para el manejo de fallas. Los cuatro patrones de intercambio de mensajes son compatibles. |
| Orquestación Programada | Crea una integración con las mismas opciones de actividad de orquestación que el estilo impulsado por aplicaciones. La diferencia es un horario, o se utiliza una solicitud bajo demanda para activar la integración en lugar del patrón basado en interfaces para el intercambio |
| Transferencia de Archivos | Este estilo es actualmente idéntico al estilo Orquestacion Programada |

#### App Driven Orchestration Style

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_4.png" alt="oic" width="700">
</div>

Puedes crear integraciones orquestadas basadas en objetos empresariales o eventos. Las integraciones orquestadas pueden ser de tipo síncrono, asíncrono o de disparar y olvidar. Las integraciones orquestadas utilizan las capacidades de Oracle BPEL Process Manager. Oracle BPEL Process Manager te permite definir cómo se ejecuta un proceso empresarial que involucra servicios web. Los mensajes BPEL invocan servicios remotos y orquestan la ejecución del proceso. Al diseñar integraciones, puedes crear múltiples expresiones de enrutamiento.

> [!NOTE]
> Asegúrate de optimizar el diseño de la integración. Si una integración orquestada contiene demasiadas acciones (por ejemplo, hay 25 o más acciones de escritura de etapa), puede producirse un fallo en la activación. Si es necesario, divide una integración con muchas acciones en varias integraciones.

#### Scheduled Orchestration Style

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_5.png" alt="oic" width="700">
</div>

Puedes programar la ejecución de integraciones. Por ejemplo, puedes crear una `integración orquestada` que se activa mediante un `horario/schedule`. Puedes programar esta ejecución de la integración para copiar archivos en una fecha y hora de tu elección. También puedes definir la frecuencia de la integración. Cuando creas este tipo de integraciones, se muestra un icono de horario junto a la entrada de la integración en la página de Integraciones.

#### Integration Development and Management Workflow

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_6.png" alt="oic" width="700">
</div>

#### Basic Integration Development Workflow Steps

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_7.png" alt="oic" width="700">
</div>

#### 1. Basic Integration Development Workflow Steps

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_8.png" alt="oic" width="700">
</div>

Selecciona un adaptador de la ventana emergente. También puedes buscar el adaptador que deseas utilizar ingresando un nombre parcial o completo en el campo de búsqueda y haciendo clic en Buscar.

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_8_2.png" alt="oic" width="700">
</div>

Ingresa la información para describir la conexión.

Ingresa un nombre significativo para ayudar a otros a encontrar tu conexión cuando comiencen a crear sus propias integraciones. El nombre que ingreses se agregará automáticamente en mayúsculas al campo de Identificador. Si utilizas el nombre del identificador, no incluyas un espacio en blanco (por ejemplo, Oportunidad de Venta).

Selecciona el rol (dirección) en el que se puede usar esta conexión (desencadenar, invocar o ambos). Solo se muestran los roles admitidos por este adaptador para la selección. Cuando seleccionas un rol, solo se muestran en la página de Conexiones las propiedades de conexión y las políticas de seguridad apropiadas para ese rol. Si seleccionas un adaptador que admite tanto la invocación como el desencadenamiento, pero seleccionas solo uno de esos roles, y luego intentas arrastrar el adaptador a la sección que no seleccionaste, recibirás un error (por ejemplo, configura un Adaptador de Nube de Oracle Service (RightNow) solo como invocar, pero arrastra el adaptador a la sección de desencadenador).

Ingresa una descripción opcional de la conexión.

Haz clic en Crear. Tu conexión se crea y ahora estás listo para configurar los detalles de la conexión, como el contacto de correo electrónico, las propiedades de la conexión, las políticas de seguridad, las credenciales de inicio de sesión de la conexión y (para ciertas conexiones) el grupo de agentes.

#### 2. Creating Integration

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_9.png" alt="oic" width="700">
</div>

#### 3. Add and Configure the Trigger (Source) Connection

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_10.png" alt="oic" width="700">
</div>

#### 4. Add and Configure an Invoke (Target) Connection

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_11.png" alt="oic" width="700">
</div>

#### 5. & 6. Request and Response Data Mapping

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_12.png" alt="oic" width="700">
</div>

Una de las tareas clave en cualquier integración es definir cómo se transfiere, o se mapea, los datos entre dos aplicaciones.

En la mayoría de los casos, los mensajes que deseas transferir entre las aplicaciones en una integración tienen estructuras de datos diferentes. Un mapeador visual te permite mapear campos entre aplicaciones arrastrando campos de origen sobre campos de destino. Cuando abres el mapeador para una solicitud o mensaje en una integración, las estructuras de datos se completan automáticamente con la información extraída de las conexiones de origen y destino. Puedes expandir y cargar niveles de estructura de datos a pedido para mostrar niveles adicionales. No hay límite en los niveles de visualización.

Los mapas que creas se llaman mapas de transformación y utilizan el `Lenguaje de Hojas de Estilo Extensible (XSL)` para describir los mapeos de datos, lo que te permite realizar manipulaciones y transformaciones de datos complejas. Se proporciona un conjunto estándar de funciones `XPath` para que definas cómo se modifica los datos al moverse de una aplicación a otra. También se proporciona una función especializada para que hagas referencia a búsquedas directamente desde el mapeador.

El mapeador admite tanto esquemas calificados como no calificados (es decir, esquemas sin elementFormDefault = "qualified"). También se admiten elementos y atributos con y sin prefijos de espacio de nombres.

Se admiten grupos de sustitución en esquemas. Puedes ver todos los elementos sustituibles en un elemento base en el mapeador y seleccionar el que deseas usar.

Los elementos y atributos para los cuales se requiere mapeo se identifican con un asterisco azul (*) a la izquierda de sus nombres. Para mostrar solo los campos requeridos, haz clic en el ícono de `Filtro/Filter`, selecciona `Campos Requeridos/Required Fields` y haz clic en `Aplicar/Apply`.

#### 7. Assigning Business Identifiers

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_13.png" alt="oic" width="700">
</div>

Los identificadores empresariales te permiten realizar un seguimiento de los campos de carga útil en los mensajes durante el tiempo de ejecución. Puedes especificar hasta tres campos de identificación empresarial para realizar un seguimiento durante el tiempo de diseño. Uno de estos campos debe seleccionarse como el campo de identificación empresarial principal. El identificador empresarial principal te permite realizar un seguimiento de los campos a lo largo de los flujos de integración durante el tiempo de ejecución y siempre está disponible. Durante el tiempo de ejecución, el estado de los identificadores empresariales es visible en la página de Seguimiento y (si han ocurrido errores de integración) en la página de Errores.

Para asignar identificadores empresariales:

Desde el menú, selecciona Seguimiento. Se muestra el cuadro de diálogo Identificadores Empresariales para Seguimiento. La carga útil de origen para la integración seleccionada se muestra en el lado izquierdo. Solo puedes asignar identificadores empresariales a campos de las `cargas útiles/payloads` de origen. No puedes asignar identificadores empresariales a campos de las `cargas útiles/payloads` de destino.

Desde la sección de Origen, arrastra el campo de carga útil que deseas rastrear hasta la sección de Arrastra un campo de desencadenador aquí. Puedes filtrar la visualización de las estructuras de origen haciendo clic en el enlace de Filtro. Esto te permite filtrar si se utilizan o no los campos y el tipo de campo (campos requeridos, campos personalizados o todos los campos).

Selecciona la casilla de verificación si deseas que este sea el identificador empresarial principal. Se requiere al menos un identificador. Si solo agregas uno, se seleccionará automáticamente como la clave principal.

En el campo de Nombre de Seguimiento, opcionalmente ingresa un nombre descriptivo para rastrear durante el tiempo de ejecución (por ejemplo, `Orgld`). El nombre se muestra cuando este campo se utiliza para filtrar mensajes en la página de Seguimiento o (si hay un error de integración) en la página de Errores durante el tiempo de ejecución.

#### 8. Activation Options (Review)

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_14.png" alt="oic" width="700">
</div>

#### Testing a SOAP Interface Trigger Connection

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_15.png" alt="oic" width="700">
</div>

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_15_2.png" alt="oic" width="700">
</div>

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_15_3.png" alt="oic" width="700">
</div>

### Creating OIC Adapter Connections - Defining OIC Adapter Connections

#### Oracle Adapters: Benefits

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_16.png" alt="oic" width="700">
</div>

**Beneficios de los Adaptadores de OIC**

Mejoran la productividad del desarrollador al permitir una interfaz, impulsada por el usuario, para descubrir metadatos y objetos empresariales de los servicios en la nube. Esto contrasta con la forma en que los desarrolladores trabajaban en el pasado al examinar archivos `WSDL`.

> [!NOTE]
> [Saber más sobre archivos WSDL](./Extras.md/#¿qué-son-los-archivos-wsdl)

Proporcionan beneficios en tiempo de ejecución con la gestión de sesiones y seguridad. La gestión de sesiones es un gran dolor de cabeza para la integración, como el manejo del tiempo de espera de sesión y la abstracción, entre otros. Por lo general, requiere codificación manual. Con los adaptadores, todo está empaquetado, cubierto y transparente para los usuarios finales.

Mejoran el aspecto transformador general de la integración al proporcionar servicios web normalizados. Típicamente, al realizar integraciones, se pasa mucho tiempo mapeando datos desde la fuente al servicio de destino. Los adaptadores te permiten generar servicios web normalizados y amigables para la integración, lo que hace que el mapeo sea mucho más rápido.

#### Oracle Cloud Adapters: Supported Features

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_17.png" alt="oic" width="700">
</div>

#### Aviable OIC Adapters

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_18.png" alt="oic" width="700">
</div>

#### OIC Connections Review

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_19.png" alt="oic" width="700">
</div>

Antes de integrar aplicaciones, debes ser capaz de conectarte a estas aplicaciones. Puede llevar mucho tiempo y esfuerzo crear el código para conectarse a otras aplicaciones. Las conexiones de OIC te permiten conectarte con aplicaciones locales y en la nube para compartir datos. Estas conexiones se basan en adaptadores e incluyen información adicional, como la `URL del WSDL` y `credenciales de seguridad`, según lo requerido por el adaptador para comunicarse con una instancia específica de una aplicación. Creas una conexión para cada instancia de aplicación que participe en las integraciones de OIC.

#### Whats Is a Connection?

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_20.png" alt="oic" width="700">
</div>

Las conexiones definen información sobre las instancias de cada configuración que estás integrando. OIC incluye un conjunto de adaptadores predefinidos, que son los tipos de aplicaciones en los que puedes basar tus conexiones, como Oracle Engagement Cloud, Oracle ERP Cloud, Oracle Cloud, Oracle Service Cloud (RightNow) y otros.

Una conexión se basa en un adaptador. Por ejemplo, para crear una conexión a una instancia específica de la aplicación Oracle ERP Cloud, debes seleccionar el adaptador Oracle ERP Cloud y luego especificar la URL del host, la política de seguridad y las credenciales de seguridad para conectarte a ella.

#### Creating a Connection

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_21.png" alt="oic" width="700">
</div>

#### Getting Started (Review)

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_22.png" alt="oic" width="700">
</div>

#### Providing Basic Connection Information (Review)

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_22_2.png" alt="oic" width="700">
</div>

Selecciona un adaptador de la ventana de diálogo. También puedes buscar el tipo de adaptador que deseas utilizar ingresando un nombre parcial o completo en el campo de búsqueda y haciendo clic en Buscar. 

Se mostrará el cuadro de diálogo Crear Nueva Conexión.

Ingresa la información para describir la conexión.

Ingresa un nombre significativo para ayudar a otros a encontrar tu conexión cuando comiencen a crear sus propias integraciones. El nombre que ingreses se agregará automáticamente en mayúsculas al campo de Identificador. Si utilizas el nombre del identificador, no incluyas un espacio en blanco (por ejemplo, Oportunidad de Venta).

Selecciona el rol (dirección) en el que se utilizará esta conexión (`desencadenar/trigger`, `invocar/invoke` o ambos). Solo se muestran los roles admitidos por este adaptador para la selección. Cuando seleccionas un rol, solo se muestran las propiedades de conexión y las políticas de seguridad apropiadas para ese rol en la página de Conexiones. Si seleccionas un adaptador que admite invocación y desencadenamiento, pero seleccionas solo uno de esos roles, y luego intentas arrastrar el adaptador a la sección que no seleccionaste, recibirás un error (por ejemplo, configura un Adaptador de Oracle RightNow Cloud solo como invocar, pero arrastra el adaptador a la sección de desencadenador).

Ingresa una descripción opcional de la conexión.

Haz clic en Crear.

Tu conexión se ha creado y ahora estás listo para configurar los detalles de la conexión, como el contacto de correo electrónico, las propiedades de la conexión, las políticas de seguridad, las credenciales de inicio de sesión de la conexión y (para ciertas conexiones) el grupo de agentes.

#### Defining Connection and Security Properties

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_23.png" alt="oic" width="700">
</div>

- [Documentacion de adaptadores OIC Gen 3](https://docs.oracle.com/en/cloud/paas/application-integration/find-adapters.html)
- [Documentacion de adaptadores OIC Gen 2](https://docs.oracle.com/en/cloud/paas/integration-cloud/find-adapters.html)

#### 1. Oracle Service Cloud Adapter Connection

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_24.png" alt="oic" width="700">
</div>

#### 2. Oracle Engagement Cloud Adapter Connection

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_25.png" alt="oic" width="700">
</div>

#### 3. Oracle ERP Cloud Adapter Connection

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_26.png" alt="oic" width="700">
</div>

#### 4. Oracle HCM Cloud Adapter Connection

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_27.png" alt="oic" width="700">
</div>

#### 5. Salesforce Adapter Connection

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_28.png" alt="oic" width="700">
</div>

### Creating OIC Adapter Connections - Exploring Additional Adapter Connections

#### 6. Oracle ATP/ADW Adapter Connection

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_29.png" alt="oic" width="700">
</div>

#### 7. Oracle Siebel Adapter Connection

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_30.png" alt="oic" width="700">
</div>

#### 8. Oracle E-Business Suite Adapter Connection

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_31.png" alt="oic" width="700">
</div>

#### FTP Adapter Connection

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_32.png" alt="oic" width="700">
</div>

#### SOAP Adapter Connection (Trigger) & (Invoke)

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_33.png" alt="oic" width="700">
</div>

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_33_2.png" alt="oic" width="700">
</div>

#### REST Adapter Connection (Trigger) & (Invoke)

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_34.png" alt="oic" width="700">
</div>

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_34_2.png" alt="oic" width="700">
</div>

#### Testing the Connection

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_35.png" alt="oic" width="700">
</div>

#### Uploading SSL Certificates

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_36.png" alt="oic" width="700">
</div>

### Creating OIC Adapter Connections - Using the On-Premises Connectivity Agent

#### On.Premises Connectivity Agent Framework

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_37.png" alt="oic" width="700">
</div>

#### Agent Runetime Behavior

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_38.png" alt="oic" width="700">
</div>

#### Available Ada ters for On-Premises Use Cases

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_39.png" alt="oic" width="700">
</div>

#### Deployment Topology

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_40.png" alt="oic" width="700">
</div>

#### Workflow For Using the Connectivity Agent

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_41.png" alt="oic" width="700">
</div>

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_41_2.png" alt="oic" width="700">
</div>

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_41_3.png" alt="oic" width="700">
</div>

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_41_4.png" alt="oic" width="700">
</div>

#### Preparing to Run the Connectivity Agent Installer

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_42.png" alt="oic" width="700">
</div>

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_42_2.png" alt="oic" width="700">
</div>

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_42_3.png" alt="oic" width="700">
</div>

#### Executing the Connectivity Agent Installer

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_43.png" alt="oic" width="700">
</div>

#### Post-lnstallation: Examining the Files

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_44.png" alt="oic" width="700">
</div>

# [Parte 3](./Notas_3.md)