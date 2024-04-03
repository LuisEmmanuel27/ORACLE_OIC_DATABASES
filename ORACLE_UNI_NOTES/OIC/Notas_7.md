# Become An Application Integration Professional (2023) - Parte 7

## Application Integration on Oracle Cloud

### File Handling Concepts and Options - Leveraging Options for Handling Files

#### Integration Style Options

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_7/pic_1.png" alt="oic" width="700">
</div>

#### OIC Toolls and Options for File Handling

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_7/pic_2.png" alt="oic" width="700">
</div>

#### File Adapter Options Summary

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_7/pic_3.png" alt="oic" width="700">
</div>

#### FTO Adapter Options Summary

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_7/pic_4.png" alt="oic" width="700">
</div>

#### Differences Between File and FTP Adapters

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_7/pic_5.png" alt="oic" width="700">
</div>

#### SOAP and REST Adapter Options

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_7/pic_6.png" alt="oic" width="700">
</div>

**Adaptador SOAP:**

- Asegura que una carga estructurada entrante (XML) de un cliente no exceda los 10 MB de tamaño.
- Asegura que una carga no estructurada entrante (MTOM) de un cliente no exceda los 512 MB de tamaño.
- Admite el envío y recepción de contenido binario y no binario como un archivo adjunto MTOM (hasta 1 GB) como parte de un mensaje de solicitud al invocar API SOAP externas.

**Adaptador REST:**

- Asegura que las solicitudes de mensajes entrantes (desencadenadores) sin adjuntos no excedan los 10 MB de tamaño. Los mensajes con adjuntos (por ejemplo, multipart/mixed y multipart/form-data) no están sujetos a esta restricción.
- Asegura que las solicitudes de carga de mensajes estructurados entrantes (cualquier encabezado de tipo de contenido que contenga JSON, XML, HTML, YAML o YML) de un cliente no excedan los 10 MB de tamaño.
- Asegura que los adjuntos JSON entrantes no excedan los 1 GB de tamaño.
- Asegura que las respuestas que contienen adjuntos para solicitudes REST salientes no excedan 1 GB. Estos archivos adjuntos pueden ser multipart/mixed, multipart/form-data o application/octet-stream.
- Asegura que los mensajes salientes (invocar) que devuelven una carga no estructurada (multipart-formdata y binary/octed-stream) de un cliente no excedan 1 GB de tamaño.
- Asegura que los mensajes salientes (invocar) que devuelven cargas de mensajes estructurados (cualquier encabezado de tipo de contenido que contenga JSON, XML, HTML, YAML o YML) de un cliente no excedan los 10 MB de tamaño.

#### Stage File Action Operations Summary

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_7/pic_7.png" alt="oic" width="700">
</div>

#### Stage File Action

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_7/pic_8.png" alt="oic" width="700">
</div>

#### Fil-Based Mapper Functions

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_7/pic_9.png" alt="oic" width="700">
</div>

El sistema de archivos virtual (VFS, por sus siglas en inglés) te permite almacenar archivos y utilizar referencias internas a estos archivos en la carga del mensaje. También puedes mapear el contenido del archivo VFS a un elemento de cadena.

Por ejemplo, puedes almacenar archivos y utilizar referencias en el VFS de la siguiente manera:

El Adaptador REST admite la característica de adjunto multipart y application/octet-stream. El adjunto se almacena en un área de preparación y se genera una attachmentReference (clave de cadena). La clave de attachmentReference se envía como parte de la carga del mensaje y más tarde recupera la instancia del adjunto desde el área de preparación.

El Adaptador FTP utiliza fileReference para leer/escribir un archivo sin un esquema. fileReference también es una referencia a un archivo almacenado en el VFS.

Se proporcionan dos funciones XPath para realizar estas tareas. Estas funciones funcionan con cualquier adaptador.

- **encodeReferenceToBase64(String referencia):** Acepta la referencia de archivo del VFS como entrada y devuelve el contenido codificado en base64 del archivo como valor de retorno. Esta función tiene un límite de tamaño de archivo de 10 MB. Esto es muy útil al enviar contenido de archivo como adjunto en línea a puntos finales SOAP. También puede ser útil al enviar contenido de la acción de archivo de etapa a un servidor FTP remoto.
- **decodeBase64ToReference(String base64String):** Acepta el contenido codificado en base64 como entrada, lo decodifica, almacena el valor decodificado en base64 en un archivo en el VFS y devuelve la referencia a este archivo. No hay límite de tamaño porque el contenido ya está en memoria. Esta función se utiliza ampliamente para leer adjuntos de archivos de puntos finales basados en SOAP y luego enviarlos a servidores FTP remotos.

#### Scheduled Orchestration Parameters

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_7/pic_10.png" alt="oic" width="700">
</div>

A veces es necesario obtener la fecha y hora de la última ejecución de la integración programada para evitar el procesamiento duplicado de datos. O tal vez necesitas saber qué archivo dentro de un lote es el siguiente que debe procesarse al limitar el número de archivos a procesar en una ejecución programada.

Esto es posible en el tipo de integración programada y se puede lograr utilizando parámetros de programación.

Puedes crear y actualizar parámetros de tipo escalar en integraciones programadas que determinen cómo agrupar y leer los datos recibidos de una ubicación de origen. Luego, utilizas estos valores de parámetros aguas abajo en la integración. Puedes crear y asignar valores a estos parámetros en la página de Parámetros de Programación que está disponible en integraciones orquestadas programadas. También puedes asignar valores a estos parámetros en acciones de asignación. Se admiten hasta cinco parámetros en la página de Parámetros de Programación.

#### File Sizes Support Summary

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_7/pic_11.png" alt="oic" width="700">
</div>

### File Handling Concepts and Options - Reviewing Example Solutions for Files

#### How to Read a Structured File?

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_7/pic_12.png" alt="oic" width="700">
</div>

Los archivos del servidor FTP de origen o del servidor de archivos se pueden leer en Integration Cloud como un archivo estructurado o como un archivo opaco. Los archivos estructurados pueden ser XML, JSON o un archivo simple separado por comas (CSV).

Por ejemplo, estos podrían ser una lista de facturas, registros de empleados en formato XML o JSON, que tienen una estructura definida. La operación de lectura de archivos de FTP (y de archivos) puede leer registros de tales archivos. El esquema (o estructura) se puede especificar proporcionando un archivo de esquema (XSD). Integration Cloud también puede generar un archivo de esquema utilizando un archivo de muestra XML, JSON o CSV, cuando el desarrollador no tiene el archivo de esquema.

La operación de lectura de archivos lee los registros del archivo de origen en la memoria. Las actividades de mapeador subsiguientes presentarán la estructura del esquema permitiendo al desarrollador mapear los valores requeridos según lo requiera el flujo de integración.

#### How to Process Large Files? (up to 1 GB)

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_7/pic_13.png" alt="oic" width="700">
</div>

La operación 'Leer archivo' es adecuada para archivos de hasta 10 MB de tamaño. Sin embargo, OIC no permite cargar archivos más grandes que 10 MB en la memoria por razones de rendimiento. Para leer archivos más grandes, los desarrolladores deben utilizar la opción "Descargar archivo" de una conexión FTP. Esto permite que los archivos se descarguen directamente en el sistema de archivos local de OIC sin leerse en la memoria. La descarga FTP se puede utilizar para archivos de hasta 1 GB de tamaño.

Una vez que el archivo esté disponible dentro de OIC, se puede utilizar la acción 'Stage File' con la operación 'Leer archivo en segmentos' para realizar un procesamiento segmentado del contenido del archivo. Esta operación le permite especificar el tamaño del segmento en número de registros, para procesar, por ejemplo, 20 o 50 registros por ciclo de lectura. Este enfoque, junto con la opción de procesamiento paralelo, proporciona un rendimiento mejorado adicional.

> [!IMPORTANT]
> Grado de paralelismo - La operación 'Leer archivo en segmentos' utiliza lecturas paralelas internamente para mejorar el rendimiento de la lectura. Ocasionalmente, puede haber casos de uso donde se necesite mantener la secuencia ordenada de registros. En tales casos, seleccione 'Procesar secuencialmente' para deshabilitar el procesamiento paralelo.

#### How to Decrypt and Encrypt Files?

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_7/pic_14.png" alt="oic" width="700">
</div>

La desencriptación puede realizarse utilizando la operación "Descargar archivo" de la conexión FTP. Debido a que "Descargar archivo" no lee el contenido en la memoria, la lectura del archivo es efectivamente un archivo opaco. (No se puede suministrar ningún esquema). Pero una vez que se descarga y desencripta el archivo, se puede utilizar la acción "Leer archivo" o "Leer archivo en segmentos" de la acción 'Stage File' para leer los datos estructurados dentro del archivo.

La encriptación se puede realizar durante la operación "Escribir archivo" de la conexión FTP. Tenga en cuenta que tanto archivos estructurados como opacos pueden ser encriptados. Elija "Habilitar seguridad PGP" como se muestra en la diapositiva.

> [!NOTE]
> La encriptación y la desencriptación actualmente solo están disponibles en las conexiones del adaptador FTP. Las claves de encriptación y desencriptación deben ser proporcionadas al configurar la conexión FTP.

#### How to Read/Write Native File Formats?

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_7/pic_15.png" alt="oic" width="700">
</div>

La traducción desde el formato de datos nativo a XML y viceversa se realiza utilizando un archivo de definición (definición de esquema no XML), que a su vez está definido en formato de esquema XML. El Asistente de Creación de Formato Nativo te permite muestrear datos nativos y crear la gramática XSD nativa (NXSD) para la traducción de datos nativos.

El Asistente de Creación de Formato Nativo está disponible en:

- Oracle JDeveloper con la extensión Oracle SOA Composite Editor
- Oracle Enterprise Pack for Eclipse (OEPE)

El asistente te guía en la creación de un archivo de esquema nativo a partir de los siguientes formatos de archivo:

- Delimitado (contiene registros cuyos campos están delimitados por un carácter especial)
- Longitud Fija (contiene registros cuyos campos tienen una longitud fija)
- Tipo Complejo (contiene registros cuyos campos pueden ser registros que tienen múltiples tipos de delimitadores)

Debes tener un archivo de datos de muestra para el tipo seleccionado para crear un esquema nativo.

#### Using the Native Format Builder Wizard

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_7/pic_16.png" alt="oic" width="700">
</div>

El asistente NXSD proporciona atributos de búsqueda anticipada que te permiten especificar patrones de expresión regular para filtrar tanto registros de longitud fija como registros de longitud variable. Puedes utilizar el soporte de procesamiento condicional, utilizando atributos de búsqueda anticipada con tipos de archivo de Longitud Fija, Delimitado y Complejo.

Usando este procesamiento condicional, puedes obtener resultados donde solo los registros que satisfacen la expresión regular se publican en XML. También puedes especificar la opción de generar una excepción cuando un registro no cumple con la expresión regular. Esto ayuda en el procesamiento condicional al proporcionar una condición de elección.

Para el soporte de expresiones regulares, puedes especificar la secuencia de caracteres contra la cual se puede hacer coincidir la expresión regular. Ten en cuenta que la secuencia de caracteres no debe exceder el límite del registro.

Para los registros de Longitud Fija, la longitud del registro y los diversos campos del registro se conocen de antemano. Esto te ayuda a especificar la posición de inicio y la longitud del flujo contra el cual se debe hacer coincidir la expresión regular.

Además, los datos de longitud fija en el formato nativo pueden definirse en el esquema nativo utilizando el estilo de longitud fija. Hay tres tipos de longitud fija:

- Con _relleno/padding_
- Sin _relleno/padding_
- Con la longitud real también leída de los datos nativos

#### Inventory Source File to SOAP Web Service

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_7/pic_17.png" alt="oic" width="700">
</div>

#### PDF File to SOAP Service as MTOM Attachment

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_7/pic_18.png" alt="oic" width="700">
</div>

#### HDL File to Oracle HCM as Inline Attachment

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_7/pic_19.png" alt="oic" width="700">
</div>

#### Images From Zip File Uploaded to a REST Service

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_7/pic_20.png" alt="oic" width="700">
</div>

#### Read Large File & Process All Records to ERP

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_7/pic_21.png" alt="oic" width="700">
</div>

#### Aggregate Records Into Local File & Transfer to FTP

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_7/pic_22.png" alt="oic" width="700">
</div>

#### OIC Design/Modeling Considerations for Fusion Apps

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_7/pic_23.png" alt="oic" width="700">
</div>

Todas las integraciones que involucran ERP FBDI, HCM HDL y CRM requieren un archivo de datos generado en base a la plantilla de objeto respectiva en formato de valores separados por comas (CSV). Este archivo puede ser creado por un sistema local o otras aplicaciones en la nube, y luego cargado en un servidor SFTP para ser consumido por Oracle Integration Cloud (OIC). Opcionalmente, el archivo también puede ser cargado en el Servidor de Contenido de Fusion Applications (UCM).

Dentro de OIC, un flujo de integración consumirá el archivo y, si es necesario, lo procesará utilizando acciones como enriquecimiento y transformación para generar un archivo de datos para el objeto respectivo de Fusion Applications. Si el archivo de datos es generado en un sistema local de acuerdo con la plantilla de objeto respectiva, OIC puede pasar este archivo a ERP o HCM Cloud para iniciar el proceso de importación.

De manera similar, los archivos pueden ser extraídos de Fusion Applications y entregados a OIC a través del servidor UCM. El servidor UCM, ubicado dentro de Fusion Applications, recibe y almacena los archivos extraídos para su procesamiento posterior.

#### Inbound FTP <= 1 MB / Outbound <= 10 MB

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_7/pic_24.png" alt="oic" width="700">
</div>

#### Inbound FTP <= 10 MB / Outbound <= 10 MB

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_7/pic_25.png" alt="oic" width="700">
</div>

#### Inbound FTP > 10 MB / Outbound > 10 MB

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_7/pic_26.png" alt="oic" width="700">
</div>

#### Inbound REST <= 10 MB / Outbound <= 10 MB

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_7/pic_27.png" alt="oic" width="700">
</div>

#### Inbound REST > 10 MB / Outbound <= 10 MB

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_7/pic_28.png" alt="oic" width="700">
</div>

#### Response file > 10 MB / Outbound > 10 MB

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_7/pic_29.png" alt="oic" width="700">
</div>

# [Parte 8](./Notas_8.md)