# Become An Application Integration Professional (2023) - Parte 3

## Application Integration on Oracle Cloud

### Configuring Trigger Connections - Configuring Integration Triggers (Concepts & SaaS Adapters)

#### Integration Development (Review)

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_1.png" alt="oic" width="700">
</div>

#### Message Exchange Patterns

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_2.png" alt="oic" width="700">
</div>

Las integraciones de OIC acomodan múltiples paradigmas de mensajería y admiten los tipos de comunicación mostrados en la diapositiva.

En una interacción sincrónica, el cliente invoca una Integración de OIC y luego espera una respuesta a la solicitud. Mientras el cliente espera, el canal de comunicación entre las partes queda abierto hasta que se produce la respuesta. Esto puede ser indeseable si se dejan abiertos grandes números de canales durante largos períodos de tiempo. Puede que no sea necesario si el cliente no necesita una respuesta inmediata. En estos casos, una respuesta asincrónica puede ser más apropiada.

En una interacción asincrónica, el cliente invoca la Integración de OIC pero no espera una respuesta antes de continuar. Las operaciones asincrónicas abren un canal de comunicación entre las partes, realizan la solicitud y cierran el canal antes de que se produzca la respuesta. La respuesta puede llegar en un momento posterior a través de una operación de devolución de llamada o puede que no llegue en absoluto para interacciones unidireccionales.

#### Implementing the Message Exchange Pattern

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_3.png" alt="oic" width="700">
</div>

Cuando diseñas una integración, comienzas con una conexión de adaptador de disparador (fuente) para iniciar la integración. La información requerida para conectarse a la aplicación ya está definida en la conexión. Sin embargo, aún debes especificar cierta información, como el objeto de negocio, la operación u otros elementos para usar en la solicitud y respuesta, y cómo procesar los datos. Esto invoca al Asistente de Configuración de Extremo de Adaptador que te guía a través de la configuración de la conexión del adaptador.

#### Using the Adapter Endpoint Configuration Wizard

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_4.png" alt="oic" width="700">
</div>

- [documentación gen 2](https://docs.oracle.com/en/cloud/paas/integration-cloud/integrations-user/understand-trigger-and-invoke-connections.html#GUID-B5A3BAB4-3E10-4AF0-989E-52831F1AA1B4)
- [documentación gen 3](https://docs.oracle.com/en/cloud/paas/application-integration/integrations-user/understand-trigger-and-invoke-connections.html#GUID-B5A3BAB4-3E10-4AF0-989E-52831F1AA1B4)

#### Gettin Started — Trigger Connections (Review)

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_5.png" alt="oic" width="700">
</div>

#### Basic Info Page

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_6.png" alt="oic" width="700">
</div>

**¿Cómo te gustaría llamar a tu punto de conexión?**

Proporciona un nombre significativo para que otros puedan entender las responsabilidades de esta conexión. Puedes incluir letras del alfabeto inglés, números, guiones bajos y guiones en el nombre. No puedes incluir lo siguiente:

- Espacios en blanco (por ejemplo, Mi Conexión de Entrada)
- Caracteres especiales (por ejemplo, #;83& o righ(t)now4)
- Caracteres multibyte

**¿Qué hace este punto de conexión?**

Proporciona una descripción opcional de las responsabilidades de esta conexión. Por ejemplo: "Esta conexión recibe una solicitud entrante para sincronizar la información de la cuenta con la aplicación en la nube."

#### 1. Oracle Service Cloud (RightNow) Adapter

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_7.png" alt="oic" width="700">
</div>

Cuando arrastras el Adaptador de Oracle Service Cloud (RightNow) al disparador de una integración, aparece el Asistente de Configuración de Punto de Extremo del Adaptador. Este asistente te guía a través de la configuración de las propiedades del punto de extremo del Adaptador de Oracle Service Cloud (RightNow).

- **Objeto de negocio:** Representa un documento de negocio independiente que puede ser manipulado por la integración. Una integración puede enviar solicitudes para crear un nuevo registro para ese objeto de negocio. También pueden enviar una solicitud para actualizar o eliminar un registro existente para un objeto de negocio. Las integraciones también pueden enviar solicitudes para recuperar información sobre uno o más registros que representan ese objeto de negocio.

- **Suscripción a eventos:** Representa un documento de evento al que te suscribes cuando el Adaptador de Oracle Service Cloud (RightNow) está configurado en la dirección de disparador (fuente). La suscripción a eventos es generada por la aplicación Oracle Service Cloud (RightNow).

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_8.png" alt="oic" width="700">
</div>

Ingresa los valores de solicitud del disparador del Adaptador de Oracle Service Cloud (RightNow) para tu integración. Los valores que especifiques iniciarán la integración.

Selecciona para recibir un objeto de negocio como solicitud desde la aplicación Oracle Service Cloud (RightNow). Esta opción inicia el proceso de definición para definir y generar un WSDL para la operación SOAP que será invocada por la aplicación Oracle Service Cloud (RightNow).

Selecciona para recibir una suscripción a eventos como solicitud desde la aplicación Oracle Service Cloud (RightNow). Esta selección activa la integración. Las suscripciones a eventos solo son compatibles si la versión de la aplicación Oracle Service Cloud (RightNow) es igual o superior a la versión 15.5 (mayo de 2015). De lo contrario, solo se admiten objetos de negocio.

> [!NOTE] 
> La aplicación Oracle Service Cloud (RightNow) tiene un límite de `20 suscripciones` para cada suscripción de evento disponible. Por ejemplo, puedes construir un máximo de 20 integraciones, todas suscritas al evento de Creación de Cliente, y 20 integraciones suscritas al evento de Destrucción de Contacto. Si creas una 21a integración para la misma suscripción de evento, esto puede provocar errores durante la activación de la integración.

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_9.png" alt="oic" width="700">
</div>

#### 2. Oracle Engagement Cloud Adapter

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_10.png" alt="oic" width="700">
</div>

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_11.png" alt="oic" width="700">
</div>

Selecciona la suscripción a eventos desde la aplicación Oracle Engagement Cloud a la que deseas suscribirte. Este evento se recibe como una solicitud que inicia la integración. Solo se muestran los eventos a los que se puede suscribir.

Cualquier evento de negocio personalizado que hayas creado y publicado en la aplicación Application Composer también está disponible para la selección. Los eventos personalizados se identifican por su descripción.

Ingresa una expresión de filtro de condición de evento. Una expresión de filtro especifica que el contenido (carga útil o encabezados) de un mensaje debe ser analizado antes de que se envíe cualquier suscripción a eventos.

Por ejemplo, puedes aplicar una expresión de filtro que especifique que se envíe una suscripción a eventos solo si el mensaje incluye un ID de cliente. Cuando la lógica de la expresión se cumple, el evento se acepta para la entrega a la integración. Como otro ejemplo, supongamos que tienes la siguiente carga útil de evento y deseas procesar registros donde se proporcione el Nombre del Propietario.

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_12.png" alt="oic" width="700">
</div>

Selecciona `Retrasado/Delayed` para configurar una respuesta de devolución de llamada exitosa, una respuesta de devolución de llamada fallida, o ambas.

Esto te permite configurar la operación y los objetos de negocio que deseas que la aplicación Oracle Engagement Cloud procese como parte de una respuesta de devolución de llamada exitosa, una respuesta de devolución de llamada fallida, o ambas.

Selecciona el tipo de devolución de llamada para configurar. Después de configurar un tipo de devolución de llamada (por ejemplo, exitosa), puedes configurar el otro tipo (por ejemplo, fallida).

**Respuesta Exitosa:** Selecciona para configurar la operación y los objetos de negocio que deseas que la aplicación Oracle Engagement Cloud procese como parte de una respuesta de devolución de llamada exitosa enviada por la integración.

**Respuesta Fallida:** Selecciona para configurar la operación y los objetos de negocio que deseas que la aplicación Oracle Engagement Cloud procese como parte de una respuesta de devolución de llamada de error enviada por la integración.

Selecciona la operación a realizar en el objeto de negocio.

#### 3. Oracle ERP Cloud Adapter

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_13.png" alt="oic" width="700">
</div>

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_14.png" alt="oic" width="700">
</div>

**Página de solicitud: Recibir eventos empresariales generados dentro de ERP Cloud**

Selecciona la suscripción de eventos de la aplicación Oracle ERP Cloud. Este evento se recibe como una solicitud que inicia la integración. Solo se muestran los eventos a los que se puede suscribir.

Cualquier evento empresarial personalizado que hayas creado y publicado en la aplicación Application Composer también está disponible para su selección. Los eventos personalizados se identifican por su descripción.

Ingresa una expresión de filtro de condiciones de evento. Una expresión de filtro especifica que el contenido (carga útil o encabezados) de un mensaje debe ser analizado antes de que se envíe algún evento. Por ejemplo, puedes aplicar una expresión de filtro que especifique que se envíe un evento solo si el mensaje incluye un ID de cliente. Cuando la lógica de la expresión se cumple, se acepta el evento.

**Página de respuesta:**

Selecciona el tipo de respuesta apropiado para tus requisitos empresariales:

`Respuesta retrasada (asincrónica)/Delayed (asynchronous) response:` Se expone un servicio de devolución de llamada (para enrutar la devolución de llamada). Seleccionas `Retrasado/Delayed` como el tipo de respuesta en la página de Respuesta y seleccionas la operación y el objeto de negocio que conforman una respuesta de devolución de llamada exitosa, una respuesta de devolución de llamada fallida, o ambas.

`No se requiere respuesta:` Seleccionas `Ninguna/None` en la página de Respuesta porque no se requiere una respuesta.

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_15.png" alt="oic" width="700">
</div>

**Recibir Mensaje de Devolución de Llamada al Finalizar el Trabajo de Importación Masiva FBDI enviado a través de otra Integración**

Especifica cuándo descargar los archivos de registro que describen el estado general del trabajo de importación de Oracle ERP Cloud.

`Siempre/Always:` Descargar siempre los registros, independientemente del éxito o fracaso del trabajo de importación.

`En caso de Fracaso/On Failure:` Solo descargar los registros si el trabajo de importación falla.

`En caso de Éxito/On Success:` Solo descargar los registros si el trabajo de importación es exitoso.

`Nunca/Never:` Nunca descargar los registros.

Selecciona el proceso de importación de datos masivos para recibirlo como una solicitud que inicia la integración. También puedes escribir las letras iniciales del nombre para filtrar la visualización de los procesos de importación de datos masivos.

### Configuring Trigger Connections - Configuring Integration Triggers (Technology Adapters)

#### Request and Response Pages: Business Objects

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_16.png" alt="oic" width="700">
</div>

**Página de Solicitud: Recibir Solicitudes de Aplicaciones de ERP Cloud (enviadas explícitamente desde Script Groovy o Lógica de Negocios)**

Selecciona el objeto de negocio de la aplicación Oracle ERP Cloud para recibirlo como una solicitud que inicia la integración. Se muestra una descripción del objeto de negocio en la parte inferior de la página.

**Página de Respuesta:**

Selecciona el tipo de respuesta apropiado para los requisitos de tu negocio:

- **Respuesta Inmediata (sincrónica):** Se devuelve un objeto de negocio de respuesta de inmediato. Seleccionas Inmediata como el tipo de respuesta en la página de Respuesta y seleccionas el objeto de negocio como parte de la respuesta al cliente.

- **Respuesta Retardada (asincrónica):** Se expone un servicio de devolución de llamada (para enrutamiento de la devolución de llamada). Seleccionas Retardada como el tipo de respuesta en la página de Respuesta y seleccionas la operación y el objeto de negocio que conforman una respuesta de devolución de llamada exitosa, una respuesta de devolución de llamada fallida o ambas.

- **No se requiere respuesta:** Seleccionas Ninguna en la página de Respuesta porque no se requiere una respuesta.

#### 4. (Generic) SOAP Adapter

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_17.png" alt="oic" width="700">
</div>

**Capacidades del Adaptador SOAP cuando se configura como disparador:**

- Asegura que un payload estructurado (XML) entrante de un cliente no exceda los 10 MB de tamaño.
- Asegura que un payload no estructurado (MTOM) entrante de un cliente no exceda 1 GB de tamaño. Si el tamaño del payload excede 1 GB, se devuelve un mensaje de código de error HTTP al cliente: 413 Solicitud demasiado grande.
- Permite configurar solo puntos finales SOAP basados en el protocolo HTTPS para aceptar solicitudes SOAP entrantes.
- Admite la configuración de los puntos finales SOAP de entrada utilizando las siguientes políticas de seguridad: Autenticación básica de HTTP, autenticación basada en token de WS-Username y compatibilidad con Security Assertion Markup Language (SAML) para acceder a propiedades estándar y personalizadas de encabezado SOAP/HTTP presentes en la solicitud SOAP entrante y hacerlas disponibles como parte de un mensaje de Oracle Autonomous Integration Cloud para cualquier procesamiento en acciones posteriores.
- Permite implementar los siguientes patrones de intercambio de mensajes en el punto final SOAP de entrada: solicitud/respuesta síncrona, solicitud unidireccional y solicitud asincrónica con soporte de devolución de llamada.

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_18.png" alt="oic" width="700">
</div>

**Página de Operación de Disparador**

Ingrese el tipo de puerto y la operación para el Adaptador SOAP. Si su WSDL incluye solo un servicio, tipo de puerto y operación, estos se seleccionan automáticamente. Si el WSDL incluye varios servicios y tipos de puerto, seleccione los que desee utilizar en su integración. Según los valores seleccionados, otros objetos como el objeto de solicitud, objeto de respuesta y objeto de fallo también pueden mostrarse automáticamente.
Seleccione Sí para desactivar la validación de acción SOAP para las solicitudes entrantes. Esto es útil en entornos en los que su WSDL incluye código personalizado y desea omitir la validación. Cuando se establece en No (el valor predeterminado), Oracle Integration valida la acción SOAP para garantizar que coincida con el WSDL.

**Página de Encabezado**

Ingrese los detalles del encabezado para el Adaptador SOAP. Los encabezados que especifique se aplican al objeto de solicitud y/o respuesta de la operación seleccionada. Los elementos seleccionados se incluyen bajo elementos de envoltura respectivos en el WSDL de integración y se muestran en el mapeador como una solicitud y/o respuesta.

#### 5. (Generic) REST Adapter

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_19.png" alt="oic" width="700">
</div>

**Capacidades del Adaptador REST al Exponer una Integración como una API REST al Configurar la Conexión como un Disparador**

Soporta la configuración de lo siguiente:

- URI de recursos relativos
- Soporte para los métodos HTTP GET, PUT, POST, DELETE y PATCH
- Parámetros de plantilla y consulta
- Soporte para un payload de solicitud/respuesta
   - Soporte para payloads JSON, XML, binarios (en línea y no estructurados) y codificados en formulario de URL
   - Soporte para matrices JSON homogéneas, incluidas las matrices de nivel superior
   - Soporte para matrices JSON multidimensionales

Las APIs REST expuestas utilizando el Adaptador REST están aseguradas mediante Autenticación Básica, autenticación basada en token OAuth y autenticación basada en JWT. Las APIs REST implementan el protocolo HTTPS, lo que obliga a que todas las solicitudes entrantes tengan seguridad a nivel de transporte. Las APIs REST expuestas utilizando el Adaptador REST están protegidas utilizando Autenticación Básica y autenticación basada en token OAuth.

Impone limitaciones de tamaño para mensajes y adjuntos entrantes.

Soporte para encabezados HTTP estándar y personalizados para modelar una integración y exponer propiedades de encabezado HTTP estándar y personalizadas a Oracle Integration para acciones posteriores.

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_20.png" alt="oic" width="700">
</div>

Puedes exponer múltiples puntos de entrada a una única integración orquestada que utiliza el Adaptador REST como la conexión de disparador. Cada punto de entrada puede configurarse con una URI de recurso y una acción/verbo HTTP diferentes, según sea necesario. Esta característica elimina la necesidad de crear múltiples integraciones (cada una con una URI de recurso y verbo separados) para realizar diferentes operaciones.

Esta función es útil en los siguientes escenarios:

- Admite múltiples URIs de recurso y acciones/verbos en una integración específica a través del Adaptador REST.
- Admite múltiples patrones de integración (por ejemplo, síncrono y asíncrono). La combinación de un recurso y un verbo se llama operación. Cada operación puede configurarse como un servicio síncrono o unidireccional asíncrono. Los servicios asíncronos aceptan la solicitud y devuelven inmediatamente un estado HTTP 202.

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_21.png" alt="oic" width="700">
</div>

Especifica la ruta relativa asociada con el recurso. La ruta puede contener parámetros de plantilla especificados entre llaves (por ejemplo, {id-orden}). Un recurso es cualquier fuente de información específica que puede ser abordada. La ruta del recurso sigue una URL fija y prefijada, seguida de la ruta relativa especificada.

Por defecto, la URL tiene el siguiente prefijo de ruta:

```
https://URL-de-instancia/ic/api/integration/v1/flows/rest/NOMBRE_DE_LA_INTEGRACIÓN/VERSIÓN
```

Por ejemplo, si el nombre de la integración es ExposeFlowAsRESTResource, la URL será:

```
https://URL-de-instancia/ic/api/integration/v1/flows/rest/EXPOSEFLOWASRESTRESOURCE
```

Selecciona una sola acción HTTP (método) para que el punto de acceso realice:

- GET: Recupera (lee) información (por ejemplo, realiza consultas). Si seleccionas esta opción, no puedes configurar un cuerpo de solicitud para este punto de acceso.
- PUT: Actualiza información.
- POST: Crea información.
- DELETE: Elimina información. Si seleccionas esta opción, no puedes configurar un cuerpo de solicitud para este punto de acceso.
- PATCH: Actualiza parcialmente recursos existentes (por ejemplo, cuando solo necesitas actualizar un atributo del recurso).

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_22.png" alt="oic" width="700">
</div>

**Desde la página de Configuración de Recursos:**

- **Agregar y revisar parámetros para este endpoint:** Haz clic para especificar los parámetros de consulta y ver los parámetros de solicitud de plantilla creados como parte de la URI del recurso para este endpoint. Si seleccionas esta opción y haces clic en Siguiente, se mostrará la página de Parámetros de Solicitud.
- **Configurar un carga útil de solicitud para este endpoint:** Haz clic para configurar la carga útil de solicitud para este endpoint, incluida la especificación de la ubicación del esquema y el tipo de carga útil con el que deseas que el endpoint responda. También puedes seleccionar esta opción si deseas incluir un adjunto con la solicitud de entrada. Si seleccionas esta opción y haces clic en Siguiente, se mostrará la página de Solicitud.
- **Seleccionar el tipo de encabezado de solicitud para configurar:**
    - **Estándar:** Selecciona para configurar encabezados HTTP estándar para el mensaje de solicitud.
    - **Personalizado:** Selecciona para configurar encabezados HTTP personalizados para el mensaje de solicitud.
    - **Seleccionar las opciones de procesamiento de adjuntos:** Selecciona el tipo de adjunto multipartes para incluir. Esta opción solo está disponible si seleccionaste la acción POST en la página de Información Básica.
    - **Aceptar adjuntos de la solicitud:** Selecciona para que el punto final REST procese los adjuntos de la solicitud multipartes entrante. Esta selección actualiza la página para mostrar el campo Seleccionar el tipo de carga útil que deseas que el endpoint reciba en la parte inferior de la página.
    - **La solicitud es un formulario HTML:** Selecciona para que el punto final REST acepte para configurar un formulario HTML. Debes seleccionar primero la opción Aceptar adjuntos de la solicitud antes de poder seleccionar esta opción. Esta selección asume que el tipo de medio es multipart/form-data.

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_23.png" alt="oic" width="700">
</div>

Selecciona las opciones de procesamiento de adjuntos: Selecciona el tipo de adjunto multipartes para incluir.

**Aceptar adjuntos de la respuesta:** Selecciona para recibir la respuesta desde la carga útil. Esta selección actualiza la página para mostrar el campo **Seleccionar el tipo de carga útil con la que deseas que el punto de acceso responda** en la parte inferior de la página.

**La respuesta es un formulario HTML:** Selecciona para que el punto final REST acepte configurar un formulario HTML. Debes seleccionar primero la opción **Aceptar adjuntos de la respuesta** antes de poder seleccionar esta opción. Esta selección asume que el tipo de medio es multipart/form-data.

Selecciona el formato de carga útil de respuesta a utilizar. El cuerpo de carga útil de respuesta debe estar definido por el elemento XSD que define la estructura de esta repesentation.XML Schema

**Muestra JSON:** Selecciona esta opción para usar archivos Swagger y RAML. Se admiten archivos de muestra JSON de hasta 100 KB de tamaño.

No se admiten matrices vacías en archivos de muestra JSON. Es posible que necesites procesar archivos de muestra JSON grandes con caracteres especiales antes de utilizar el Asistente de Configuración de Puntos de Acceso del Adaptador.

**Documento XML de Muestra (Con un Solo Espacio de Nombres o Ninguno):** Selecciona esta opción para usar un documento XML para generar el esquema.

**Documento JSON de Muestra:** Selecciona esta opción para usar un documento JSON para generar el esquema.

**Binario:** Úsalo con cargas útiles que son no estructuradas y en línea, por ejemplo. Preserva el contenido del archivo, pero requiere que el receptor determine el tipo de archivo, por ejemplo, a partir de la extensión del nombre del archivo. El tipo de medio de Internet para una secuencia de bytes arbitraria es application/octet-stream.

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_24.png" alt="oic" width="700">
</div>

**Página de Operaciones de Disparo del Adaptador REST**

Revise o edite operaciones existentes o agregue una nueva operación. Cada operación representa una rama de acción de selección diferente en una sola integración. El número máximo de operaciones (ramas) que puede crear en una integración es seis. Cada punto de entrada se puede configurar con una URI de recurso y una acción/verbo HTTP diferentes, según sea necesario. Esta función elimina la necesidad de crear múltiples integraciones (cada una con una URI de recurso y un verbo separados) para realizar diferentes operaciones. Puede exponer múltiples puntos de entrada a una sola integración orquestada con una acción de selección que utiliza el Adaptador REST como la conexión de disparo.

#### 6. File Adapter

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_25.png" alt="oic" width="700">
</div>

**El Adaptador de Archivos proporciona los siguientes beneficios:**

- Transfiere (lectura/escritura) archivos a cualquier servidor accesible públicamente en formato binario o ASCII.
- Admite un patrón de intercambio de mensajes unidireccional síncrono. No hay respuesta del servidor.
- Permite la creación de archivos binarios (opacos) y archivos basados en esquemas como esquemas XML y valores separados por comas (CSV).

> [!NOTE]
> El Adaptador de Archivos admite archivos de Microsoft Excel. Puede enviar el archivo como opaco (sin procesar) o primero guardarlo como un archivo CSV antes de usarlo con Oracle Integration. 
> 
> Admite el procesamiento de archivos de menos de 10 MB de tamaño. Tenga en cuenta que el tamaño de los archivos CSV aumenta al traducirse en un mensaje. Por lo tanto, el tamaño del archivo debe ser inferior a 10 MB para que, después de la traducción, el tamaño del mensaje no supere los 10 MB. 
> 
> Admite la carga de un archivo XSD sin un espacio de nombres objetivo. En estos casos, se agrega un espacio de nombres sustituto al archivo XSD que luego utilizan todos los mensajes: http://xmlns.oracle.com/cloud/adapter/nxsd/surrogate 
> 
> Admite XSD complejos que pueden importar e incluir otros XSD. Los XSD incluidos en el archivo ZIP pueden importar el XSD desde una ubicación HTTP. Todos los archivos XSD deben agregarse a un archivo ZIP y cargarse al configurar el Adaptador de Archivos para operaciones de lectura y escritura en el Asistente de Configuración de Extremos del Adaptador.

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_26.png" alt="oic" width="700">
</div>

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_27.png" alt="oic" width="700">
</div>

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_28.png" alt="oic" width="700">
</div>

### Configuring Invoke Connections - Using the Configuration Wizard (SaaS & DB Adapters)

#### Message Exchange Patterns (Revisited)

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_2.png" alt="oic" width="700">
</div>

Las integraciones de OIC pueden invocar servicios externos o internos de OIC utilizando cualquiera de los tres patrones básicos de interacción de servicios web.

En una interacción síncrona, la integración de OIC invoca el servicio externo y luego espera una respuesta a la solicitud. Mientras OIC espera, el canal de comunicación entre las partes queda abierto hasta que se recibe la respuesta. Esto puede ser poco deseable si se dejan abiertos un gran número de canales durante largos períodos de tiempo. Puede que no sea necesario si la integración no necesita una respuesta inmediata.

En una interacción asíncrona, la integración de OIC invoca el servicio externo pero no espera una respuesta antes de continuar. Las operaciones asíncronas abren un canal de comunicación entre las partes, realizan la solicitud y cierran el canal antes de que se reciba la respuesta. La respuesta puede llegar en un momento posterior a través de una operación de devolución de llamada o puede que no llegue en absoluto para interacciones unidireccionales.

#### Getting Started—lnvoke Connections (Review)

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_29.png" alt="oic" width="700">
</div>

#### Basic Info Page (Review)

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_30.png" alt="oic" width="700">
</div>

**¿Cómo quieres llamar a tu punto de conexión?**

Proporciona un nombre significativo para que otros puedan entender las responsabilidades de esta conexión. Puedes incluir caracteres alfabéticos en inglés, números, guiones bajos y guiones en el nombre. No puedes incluir lo siguiente:

- Espacios en blanco (por ejemplo, Mi Conexión de Entrada)
- Caracteres especiales (por ejemplo, #;83& o ahor(a)ra4)
- Caracteres multibyte

**¿Qué hace este punto de conexión?**

Ingresa una descripción opcional de las responsabilidades de la conexión.

#### 1. Oracle Service Cloud (RightNow)

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_31.png" alt="oic" width="700">
</div>

Admite el lenguaje de consulta de objetos RightNow (ROQL) para consultar información de metadatos cuando el Adaptador de Oracle Service Cloud (RightNow) está configurado en la dirección de invocación.

Admite atributos personalizados (nuevo concepto de atributos personalizados de Oracle Service Cloud (RightNow) y campos personalizados con el paquete C predeterminado) en objetos de negocio para aprovechar el soporte de Oracle Service Cloud (RightNow) para atributos personalizados.

Maneja automáticamente los detalles de la política de seguridad necesarios para conectarse a la aplicación Oracle Service Cloud (RightNow).

Proporciona capacidades estándar de manejo de errores.

Permite realizar operaciones CRUD (crear, obtener, actualizar y eliminar) contra objetos de negocio en la aplicación Oracle Service Cloud (RightNow). Te permite cargar un archivo como un adjunto a Oracle Service Cloud (RightNow) o puedes mapear los datos en la solicitud del cuerpo SOAP.

Te permite descargar un archivo como un adjunto de Oracle Service Cloud (RightNow) a Oracle Integration. Después de que se descarga el archivo, el Adaptador de Oracle Service Cloud (RightNow) expone la referencia del archivo en el mapeador para su uso por Otros adaptadores para su procesamiento adicional. La siguiente funcionalidad es compatible:

- Puedes descargar un solo archivo a la vez.
- Puedes descargar cualquier archivo de Oracle Service Cloud (RightNow).
- El archivo descargado se expone como una referencia de archivo del sistema de archivos virtual (VFS).

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_32.png" alt="oic" width="700">
</div>

**CRUD:** Representa las operaciones de crear, leer, actualizar, eliminar o destruir que se deben realizar en los objetos de negocio de Oracle Service Cloud (RightNow). Cada letra se asigna a una declaración SQL estándar, método HTTP u operación de DOS. Selecciona la operación CRUD para realizar en el objeto de negocio: Crear, Destruir, Obtener o Actualizar.

Si seleccionas **Crear** o **Actualizar**, puedes seleccionar un objeto de negocio que admita adjuntos de archivos. Esto te permite cargar archivos en Oracle Service Cloud (RightNow).

Selecciona para habilitar aspectos del procesamiento en el servidor. De forma predeterminada, no se selecciona ninguna opción. Cuando hayas terminado, haz clic en Aceptar.

- **Suprimir Eventos Externos:** Selecciona para evitar que la aplicación Oracle Service Cloud (RightNow) procese cualquier evento externo generado después de la finalización de las operaciones de creación, actualización o eliminación.
- **Suprimir Reglas:** Selecciona para evitar que se ejecuten reglas de negocio después de la finalización de las operaciones de creación, actualización o eliminación. Las reglas de negocio son herramientas para simplificar y automatizar tareas comerciales comunes. Consulta la documentación de Oracle Service Cloud (RightNow) para obtener más información.
- **Suprimir Respuesta:** Selecciona para evitar que la operación CRUD de Crear devuelva un ID de respuesta. Si esta casilla de verificación está desactivada, la operación de Crear devuelve un ID del objeto creado.

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_33.png" alt="oic" width="700">
</div>

**Adjunto de Archivo/File Attachment:** Selecciona para descargar un archivo como un adjunto desde Oracle Service Cloud (RightNow) a Oracle Integration. Después de seleccionar **Adjunto de Archivo**, se te pedirá seleccionar el objeto de negocio desde el cual descargar el adjunto de archivo en la tabla **Seleccionar un Objeto de Negocio del cual te gustaría descargar el adjunto/Select a Bussines Object you would like to download the attachment**. Después de descargar el archivo, el Adaptador de Oracle Service Cloud (RightNow) expone la referencia del archivo en el mapeador para su uso por otros adaptadores para un procesamiento adicional.

**ROQL:** (RightNow Object Query Language) te permite definir una consulta basada en ROQL para enviarla como una solicitud para ejecutar en la aplicación Oracle Service Cloud (RightNow). Si seleccionas esta opción, la página se actualiza para mostrar un campo para ingresar una consulta.

**Probar Mi Consulta/Test My Query:** Haz clic para validar completamente la consulta contra la aplicación Oracle Service Cloud (RightNow). Los resultados de la consulta se muestran. Si ocurren errores, recibirás resultados sobre cómo corregir la consulta. Si no validas completamente tu consulta presionando este botón, todavía se valida cuando presionas *Siguiente/Next*, pero con limitaciones potenciales basadas en cómo se escribió la consulta.

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_34.png" alt="oic" width="700">
</div>

**Operación por Lote/Batch Operation:** Selecciona para configurar múltiples operaciones en un lote. Esto te permite ejecutar múltiples operaciones en una secuencia definida.

Al seleccionar esta opción, la página se actualiza para mostrar una opción para lo siguiente:

**Hacer clic para agregar una operación a la lista:** Haz clic para crear una lista de operaciones por lotes y sus objetos de negocio. Las operaciones se realizan en el orden en que aparecen en la lista (de arriba hacia abajo). Cuando completes, haz clic en **Aceptar/OK**.

Cuando completes la configuración del Adaptador de Oracle Service Cloud (RightNow) y hagas clic en Siguiente para acceder a la página de Resumen, puedes realizar las siguientes tareas de operaciones por lotes:

- Icono de Edición: Haz clic para editar una fila de operaciones en la tabla o cambiar el orden de las operaciones por lotes.
- Icono de Eliminación: Haz clic para eliminar una fila de operación seleccionada en la tabla.

#### 2. Oracle Engagement Cloud

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_35.png" alt="oic" width="700">
</div>

El Adaptador de Oracle Engagement Cloud proporciona las siguientes capacidades:

Genera un mapeo automático al objeto de negocio, servicio o recurso de API REST de Oracle Fusion Applications expuesto que seleccionas durante la configuración del adaptador:

- **Objeto de negocio:** Representa un documento de negocio autónomo que puede ser actuado por la integración. Una integración puede enviar solicitudes para crear un nuevo registro para ese objeto de negocio. También pueden enviar una solicitud para actualizar o eliminar un registro existente para un objeto de negocio. Las integraciones también pueden enviar solicitudes para recuperar información sobre uno o más registros que representan ese objeto de negocio.
- **API de negocio (REST):** Representa un recurso de API REST de Oracle Fusion Applications. Puedes seleccionar recursos de negocio principales y sus recursos de negocio secundarios correspondientes. El soporte se proporciona en la dirección de invocación (saliente).

Te permite ver anotaciones en los elementos del Adaptador de Oracle Engagement Cloud en el mapeador.

Invoca dinámicamente un punto final/URL REST en tiempo de ejecución sin requerir que configures ninguna conexión de invocación adicional o detalles de salida REST.

Maneja automáticamente los detalles de la política de seguridad requeridos para conectarse a la aplicación Oracle Engagement Cloud.

Proporciona capacidades estándar de manejo de errores.

Te permite mapear objetos de negocio que tienen estructuras de datos polimórficas.

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_36.png" alt="oic" width="700">
</div>

**Objetos de Negocio:** Selecciona para navegar por objeto de negocio.

Selecciona para filtrar la visualización de objetos de negocio y luego selecciona el objeto de negocio a utilizar.

- **Todos**
- **Activos**
- **Personalizados**
- **Obsoletos**
- **Estándar**

Selecciona la operación a realizar en el objeto de negocio seleccionado. Las operaciones disponibles para selección se basan en el objeto de negocio que seleccionaste.

El Ciclo de Vida muestra el estado del objeto de negocio seleccionado. Obsoleto indica que el documento de negocio está cerca del final de su uso y debe utilizarse con precaución.

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_37.png" alt="oic" width="700">
</div>

**Servicios:** Selecciona para navegar por servicio. Hay una correspondencia uno a uno entre el objeto de negocio y el servicio. El servicio actúa sobre el documento de negocio.
Selecciona para filtrar la visualización de servicios y luego selecciona el servicio a utilizar.

- **Activos**
- **Obsoletos**
- **Estándar**

Selecciona la operación a realizar en el servicio seleccionado. Las operaciones disponibles para selección se basan en el servicio que seleccionaste.

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_38.png" alt="oic" width="700">
</div>

Recurso de Negocio (REST): Selecciona para navegar por una lista de los recursos de API REST de Oracle Fusion Applications disponibles.

> [!NOTE]
> El Adaptador de Oracle Engagement Cloud actualmente extrae todos los recursos expuestos por el catálogo de interfaces y los muestra para su selección.

Selecciona la aplicación de servicio para ver los recursos de negocio definidos en la aplicación.

Selecciona para filtrar la visualización de recursos de negocio y luego selecciona el recurso de negocio a utilizar.

- Todos
- Estándar

Selecciona la operación a realizar en el recurso de negocio (REST) seleccionado. Las operaciones disponibles para selección se basan en el recurso de negocio que seleccionaste.

También puedes hacer clic en **Examinar y configurar un recurso secundario/Browse and configure child resource** para seleccionar los recursos de negocio secundarios correspondientes a ese padre para utilizar. Haz clic para acceder a una página para seleccionar lo siguiente:

- Los recursos de negocio secundarios del recurso de negocio principal seleccionado.
- La operación a realizar en los recursos de negocio secundarios.

Después de hacer clic en **Ok**, el nombre del enlace cambia a **Ver y editar la configuración de un recurso secundario/View and edit the configuration of a child resource**. Tanto el recurso de negocio principal como los secundarios se muestran en la página de Resumen.

#### 3. Oracle ERP Cloud

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_39.png" alt="oic" width="700">
</div>

El Adaptador de Oracle ERP Cloud proporciona los siguientes beneficios:

Genera mapeo automático a los objetos de negocio expuestos, la suscripción a eventos o la API de negocio (REST) que selecciones durante la configuración del adaptador:

- **Objeto de negocio:** Representa un documento de negocio autocontenido en el que se puede actuar mediante la integración. Una integración puede enviar solicitudes para crear un nuevo registro para ese objeto de negocio. También pueden enviar una solicitud para actualizar o eliminar un registro existente de un objeto de negocio. Las integraciones también pueden enviar solicitudes para recuperar información sobre uno o más registros que representan ese objeto de negocio.

- **API de negocio (REST):** Representa un recurso de API REST de Oracle Fusion Applications. Puedes seleccionar recursos de negocio principales y sus correspondientes recursos de negocio secundarios. El soporte se proporciona en la dirección de invocación (salida).

Invoca dinámicamente un punto final/URL REST en tiempo de ejecución sin requerir que configures ninguna conexión de invocación adicional o detalles de salida REST.

Maneja automáticamente los detalles de la política de seguridad requeridos para conectarse a la aplicación de Oracle ERP Cloud.

Proporciona capacidades estándar de manejo de errores.
Expone eventos y servicios web de Supply Chain Management (SCM) Cloud.

Te permite cargar un archivo en una ubicación FTP segura. El archivo es identificado y proporcionado a Oracle ERP Cloud para que los datos puedan ser cargados en las tablas de negocio de Oracle ERP Cloud.

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_40.png" alt="oic" width="700">
</div>

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_41.png" alt="oic" width="700">
</div>

Realizar operaciones masivas compatibles con FBDI, como la importación de arrendamientos de activos, entradas de diario, extractos bancarios, facturas por pagar, tareas de proyecto, pedidos de ventas y transacciones de envío. También puedes configurar notificaciones de eventos y devoluciones de llamada en estas operaciones.

Selecciona el nombre del trabajo a importar. Los trabajos de importación son los trabajos en segundo plano que se ejecutan en Oracle ERP Cloud para realizar operaciones de carga de datos. El nombre del trabajo que selecciones se utiliza para importar datos. La lista de trabajos de importación se obtiene invocando ErplcsIntegrationService en el WSDL del servicio de catálogo de servicios.

La siguiente información se obtiene con cada trabajo:

- **Nombre de visualización del trabajo:** Para ser mostrado en la interfaz de usuario.
- **ID de interfaz:** La clave del trabajo de importación.
- **Cuenta de UCM:** La cuenta con la que cargar el archivo.

Selecciona el tipo de datos de registro para que Oracle ERP Cloud extraiga mientras procesa el archivo de datos:

- **Todos:** Todos los registros fallidos con archivos de proceso de carga e importación de soporte.
- **Error:** Registros que no se pudieron cargar e importar.
- **Registro:** Archivos de registro para procesos de carga e importación.
- **Salida:** Archivos de salida para procesos de carga e importación.
- **Ninguno:** Ninguno.

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_42.png" alt="oic" width="700">
</div>

Selecciona para cargar archivos en Oracle WebCenter Content (Universal Content Manager) en formato cifrado o no cifrado. Ten en cuenta que una vez que los archivos se carguen, necesitarás agregar una acción separada en tu flujo de integración para invocar el proceso programado o la API apropiada en ERP Cloud para procesar el archivo. Utiliza esta opción solo cuando no puedas utilizar la opción de Importar Datos Masivos, que se encarga automáticamente de todo esto.

Selecciona el grupo de seguridad en el que cargar el archivo. Un grupo de seguridad es un conjunto de archivos agrupados bajo un nombre único. Cada archivo en el repositorio del servidor de contenido pertenece a un grupo de seguridad. El acceso a los grupos de seguridad está controlado por permisos asignados a roles en el servidor de contenido. Los roles se asignan a usuarios donde se mantienen en Oracle Fusion Applications. El grupo de seguridad predeterminado en Fusion Applications es FAFusionImportExport.

Selecciona la cuenta de documento para asignar al archivo. En Fusion Applications, cada elemento de contenido tiene una cuenta asignada. Debes tener los permisos apropiados para la cuenta, como leer y/o escribir. El acceso al documento es la intersección entre los permisos de la cuenta y los permisos del grupo de seguridad. Hay varias cuentas de Fusion Applications.

Selecciona la casilla de verificación para cifrar el archivo antes de cargarlo en UCM. Para seleccionar esta casilla de verificación, debes haber seleccionado cifrar el archivo al configurar la conexión del Adaptador de Oracle ERP Cloud en la página de Conexiones.

#### 4. Oracle HCM Cloud

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_43.png" alt="oic" width="700">
</div>

El Adaptador de Oracle HCM Cloud proporciona los siguientes beneficios:

- Una integración puede enviar solicitudes para crear un nuevo registro para ese objeto de negocio. También pueden enviar una solicitud para actualizar o eliminar un registro existente para un objeto de negocio. Las integraciones también pueden enviar solicitudes para recuperar información sobre uno o más registros que representan ese objeto de negocio.
- Expone la API de Recursos Empresariales (REST), que representa un recurso de la API de Oracle Fusion Applications REST. Puedes seleccionar recursos empresariales principales y sus recursos empresariales secundarios correspondientes. Se proporciona soporte en la dirección de invocación (salida).
- Admite el consumo de la API REST de Oracle HCM Cloud. Esto permite que el Adaptador de Oracle HCM Cloud consuma servicios REST bajo Oracle HCM Cloud cuando está configurado como una conexión de invocación.
- Maneja automáticamente los detalles de la política de seguridad requeridos para conectarse a la aplicación Oracle HCM Cloud.
- Te permite mapear objetos de negocio que tienen estructuras de datos polimórficas.
- Admite la suscripción al feed Atom de HCM. Los feeds Atom te permiten realizar un seguimiento de los cambios realizados en los recursos habilitados para feed en Oracle Global Human Resources Cloud. Para cualquier actualización de interés para las aplicaciones descendentes, como nuevas contrataciones, terminaciones, transferencias de empleados y promociones, Oracle Global Human Resources Cloud publica feeds Atom.
- Te permite cargar archivos en Oracle WebCenter Content (Universal Content Manager) en formato cifrado o no cifrado.

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_44.png" alt="oic" width="700">
</div>

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_45.png" alt="oic" width="700">
</div>

Este recurso proporciona una herramienta flexible para generar archivos de datos e informes. El Adaptador de Oracle HCM Cloud funciona como una herramienta de extracción de descubrimiento en Oracle HCM Cloud. El proceso de extracción de datos se automatiza de acuerdo con los siguientes pasos:

- Invocación del extracto de datos HCM dado por el cliente fuera del Adaptador de Oracle HCM Cloud
- Descubrimiento del extracto tal como se entrega en Oracle WebCenter Content
- Recuperación de la salida del extracto en su formato tal como se entrega a Oracle WebCenter Content y persistencia del extracto en el almacenamiento provisional de Oracle Integration
- Definición del esquema XML por parte del usuario para la salida del extracto para la transformación usando una Acción de Archivo de Etapa que está disponible en una integración orquestada

Selecciona las acciones a realizar en el extracto:

- **Descifrar el extracto:** El extracto se descifra si está en forma cifrada y la información PGP está presente en la configuración de la conexión.
- **Descomprimir el extracto:** El extracto se descomprime si está en formato comprimido.

Las acciones seleccionadas se realizan en el extracto después de que se descarga en Oracle Integration.
Más información sobre la gestión de Extractos HCM está disponible aquí: [enlace](https://docs.oracle.com/en/cloud/saas/human-resources/24a/faihm/index.html#COPYRIGHT_0000)

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_46.png" alt="oic" width="700">
</div>

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_47.png" alt="oic" width="700">
</div>

Selecciona el grupo de seguridad en el que deseas cargar el archivo. Un grupo de seguridad es un conjunto de archivos agrupados bajo un nombre único. Cada archivo en el repositorio del servidor de contenido pertenece a un grupo de seguridad. El acceso a los grupos de seguridad está controlado por los permisos asignados a roles en el servidor de contenido. Los roles se asignan a usuarios donde se mantienen en las aplicaciones de Fusion de Oracle. El grupo de seguridad predeterminado en las aplicaciones de Fusion es...

Selecciona la cuenta de documento para asignar al archivo. En las aplicaciones de Fusion, cada elemento de contenido tiene una cuenta asignada. Debes tener los permisos adecuados para la cuenta, como leer y/o escribir. El acceso al documento es la intersección entre los permisos de la cuenta y los permisos del grupo de seguridad. Hay varias cuentas de aplicaciones de Fusion.

Selecciona la casilla de verificación para cifrar el archivo antes de cargarlo en UCM. Para seleccionar esta casilla de verificación, debes haber seleccionado cifrar el archivo al configurar la conexión del Adaptador de Oracle HCM Cloud en la página de Conexiones.

#### 5. Oracle ATP/ADW Databases

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_48.png" alt="oic" width="700">
</div>

Los adaptadores de Oracle ATP/ADW ofrecen las siguientes capacidades:

- **Conectividad Directa:** Soporte para conectarse directamente a las bases de datos Oracle ATP y ADW sin necesidad de utilizar un agente de conectividad local. Este tipo de conexión es adecuado únicamente para conexiones de invocación y no se puede configurar como una conexión de activación. Los escenarios de sondeo entrante deben implementarse utilizando patrones de integración de orquestación programada.

- **Integración con Bases de Datos Alojadas en Privado:** Capacidad para integrar bases de datos Oracle ATP o ADW alojadas en privado con Oracle Integration utilizando el agente de conectividad local.

- **Invocación de Procedimientos Almacenados:** Soporte para invocar procedimientos almacenados en la base de datos Oracle.

- **Tipos de Datos No-JDBC:** Soporte para tipos de datos no-JDBC como registros PL/SQL y tablas PL/SQL en invocaciones salientes de procedimientos almacenados.

- **Ejecución de Sentencias DML y Consultas SQL:** Soporte para ejecutar sentencias de Lenguaje de Manipulación de Datos (DML) y consultas SQL, incluidas operaciones Select, Insert, Update y Delete.

- **Operaciones en Lote:** Soporte para actualizar o insertar múltiples registros en una sola solicitud, mejorando el rendimiento y la eficiencia.

- **Operaciones SELECT:** Soporte para realizar operaciones SELECT contra tablas de bases de datos para recuperar datos.

- **Funcionalidad de Operaciones en una Tabla:** Esta función permite modelar sentencias SQL utilizando el Asistente de Configuración de Puntos de Extremo del Adaptador. También admite el manejo de múltiples registros en una sola solicitud, proporcionando flexibilidad y optimización en las interacciones con la base de datos.

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_49.png" alt="oic" width="700">
</div>

Selecciona un esquema de base de datos de la lista. Esta acción refresca la página para mostrar campos para seleccionar un paquete o procedimiento a invocar. Los caracteres especiales (por ejemplo, #) no son compatibles en los nombres de esquema.

Selecciona el paquete de base de datos. Esta acción refresca la página para mostrar los procedimientos disponibles para el paquete. Cuando se importa un paquete de integración predefinido que contiene procedimientos almacenados PLS o SQL, el paquete envolvente no se recrea en la base de datos de destino. Para agregar el paquete envolvente, confirma que JPublisher está instalado en la base de datos de destino y define el procedimiento almacenado original. Después de confirmar que JPublisher está instalado y que se ha definido el procedimiento almacenado, abre la utilidad PL/SQL Wrapper y ejecuta el comando add scripts para agregar los scripts incluidos en los archivos de inventario exportados (IAR).

Seleccionar Procedimiento muestra los parámetros de entrada (in), salida (out) y entrada/salida (in/out) para el procedimiento seleccionado.

**Nota**

- Los procedimientos almacenados devuelven objetos binarios grandes (por ejemplo, tipos de datos de base de datos BLOB) como tipos base64Binary en XML. Dependiendo de los casos de uso, estos pueden ser decodificados durante la transformación usando funciones incorporadas como decodeBase64 o pueden ser pasados tal cual para el procesamiento posterior.
- Los parámetros de entrada/salida del adaptador están definidos en función de los parámetros IN/OUT del procedimiento almacenado. El parámetro IN corresponde a la solicitud y el parámetro OUT se traduce como la respuesta.

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_50.png" alt="oic" width="700">
</div>

La página Ejecutar una Declaración SQL aparece cuando se selecciona Ejecutar una Declaración SQL como la acción a realizar en la página Información Básica.

No utilice nombres de esquema/base de datos en las consultas SQL. Configure los detalles en la conexión. Por ejemplo:

```sql
Update HR.employee set HR. employee. first_name = 'Name' 
where HR . employee .employee_id = '1'
```

puede cambiarse a una consulta simple, como:

```sql
Update employee set first name  = 'Name' where employee_id = '1'
```

donde HR se utiliza en los detalles de conexión. Esto restringe a un usuario con privilegios específicos a un esquema/base de datos particular.

Asegúrese de proporcionar espacios adecuados entre las palabras clave para una declaración SQL pura. Por ejemplo, la siguiente declaración falla durante la activación de la integración porque no hay un espacio en blanco entre VALUES y (#.

```sql
INSERT INTO table_name VALUES (#EMPNO,  #EMPNAME)
```

Agregue un espacio en blanco entre VALUES y (#, y la declaración se procesa correctamente.

```sql
INSERT INTO table_name VALUES (#EMPNO, #EMPNAME)
```

Defina todos los parámetros de enlace en el mismo orden y defina los parámetros que toman valores absolutos al final. Por ejemplo:

```sql
INSERT INTO table_nane (EMPNO, EMPNAME, EMPUUID, EMPPHONE, EMPHIREDATE) 
VALUES (#EMPNO, #EMPNAME, Sys_guid( ), NULL, SYSDATE)
```

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_51.png" alt="oic" width="700">
</div>

**Página de Importación de Tablas**

Filtre y seleccione las tablas a importar basadas en el esquema seleccionado. Estas tablas se utilizan para generar una declaración SQL basada en la operación seleccionada.

Puede importar el siguiente número de tablas:

- Un máximo de tres tablas para acciones de inserción, actualización e inserción o actualización
- Un máximo de cinco tablas para la función de operación en tabla de selección

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_52.png" alt="oic" width="700">
</div>

**Página de Relaciones**
Revise las relaciones entre las tablas seleccionadas y opcionalmente cree, elimine o cambie el nombre de las relaciones. Estas relaciones se utilizan en las declaraciones SQL de inserción o actualización.

**Página de Crear Relación**
Especifique las relaciones padre e hijo a utilizar en la declaración SQL.

Seleccione el tipo de asignación (uno a muchos, uno a uno o uno a uno con la clave externa en la tabla secundaria). Por ejemplo, si seleccionó Empleados como la tabla principal y Departamentos como la tabla secundaria, se muestran las siguientes opciones:

- Empleados tiene una relación 1:1 con Departamentos
- Empleados tiene una relación 1:1 con Departamentos (Clave externa en la tabla secundaria)
- Empleados tiene una relación 1:M con Departamentos

**Página de Filtrado de Atributos**

Filtre los atributos a excluir.

**Página de Opciones Avanzadas**

Proporcione opciones avanzadas adicionales comosecuenciación. Esto solo es válido para las operaciones de inserción y combinación.

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_3/pic_53.png" alt="oic" width="700">
</div>

**Opción de Revisión y Edición de Consulta SQL**

Haga clic para editar la consulta en el Generador de Expresiones.

- **Agregar Nuevo:** Haga clic para agregar nuevos criterios a la consulta SQL.
- Haga clic en **Agregar Nuevo**.
- En el campo **Primer Argumento/First Argument**, haga clic en **Editar** y seleccione el argumento a agregar (por ejemplo, **deptno**).
- En el campo **Operador/Operator**, seleccione el operador a utilizar para la comparación desde la lista desplegable (por ejemplo, =).
- En el campo **Segundo Argumento/Second Argument**, seleccione la opción a utilizar:
    - **Literal:** Haga clic para especificar un valor. Si se selecciona, se le solicitará que seleccione el tipo de datos (por ejemplo, entero) y especifique el valor.
    - **Parámetro:** Haga clic para especificar un parámetro de enlace.
    - **Clave de Consulta/Query Key:** Haga clic para ejecutar la comparación contra otra columna en la tabla. 
    
        Los nuevos criterios se agregan a la consulta SQL con una cláusula WHERE. Si agrega consultas SQL subsiguientes, se agregan a la consulta SQL con una cláusula AND.

- **Agregar Anidado/Add Nested:** Haga clic para agregar criterios anidados a la consulta SQL.
- **Editar:** Haga clic para editar los criterios SQL que especificó.
- **Eliminar:** Haga clic para eliminar los criterios SQL que especificó.

# [Parte 4](./Notas_4.md)