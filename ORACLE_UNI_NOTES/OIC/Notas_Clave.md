# Notas Clave

Serie de notas que considero importantes a resaltar de toda la información dada en el curso. Ya sean ideas muy puntuales o conceptos que si o si debemos tener memorizados o prensetes en todo momento a la hora de aprender y trabajar con Oracle OIC

---

- Oracle Integration se ejecuta en la infraestructura, en la nube Gen2 (actualmente la versión 3 en Gen3)

- `Bussines Accelerators:` Soluciones empresariales que son configurables y completamente gestionadas por Oracle
- `Technical Accelerators`: Entregan patrones técnicos listos para usar que también son configurables
- `Recipes`: Son integraciones de muestra que sirven como un inicio rapido o ejemplo
- Extención de integración al importar/exportar `.iar`
- Extención de paquete al importar/exportar `.par`
- La mejor practica es organizar integraciones similares en paquetes, los cuales podrán ser exportados/importados facilmente
- No se pueden crear paquetes vacios
- Identificadores de Integración deben ser unicos
- No existen fronteras (boundaries) administrativas no de seguridad
- Todas las integraciones son visibles entre si, independientemente de su paquete asignado
- Exportaciones de integraciones (o un paquete de integraciones) incluyen todos sus recursos de conexión dependientes.
- Los recursos de conexión están definidos por un tipo de adaptador y un identificador único.
- La información de URL y las credenciales **NO** se exportan.
- Las integraciones importadas **NO** incluirán la importación de sus recursos de conexión dependientes si ya existen en el entorno objetivo de OIC.
- Si todos los recursos de conexión ya existen, la integración puede ser activada inmediatamente.
- De lo contrario, cuando se importa un recurso de conexión, las propiedades de conexión apropiadas y las credenciales deben configurarse antes de activar la integración.
  - Alternativamente, las integraciones importadas se pueden reconfigurar fácilmente para utilizar un recurso de conexión existente diferente a través de la API REST de OIC.
- Si tienes una cuenta de API Platform Cloud Service, puedes optar por publicar información del punto de conexión para integraciones que estén configuradas con una conexión de activador de interfaz REST.
- El numero de version de una integración es de esta forma `xx.yy.zzzz`:
  - xx es la versión mayor
  - yy & zzzz son la versión menor
- Podemos crear integraciones con el mismo identificador pero con un nuevo numero de version mayor o menor
- El Estilo de Integración de `Enrutamiento Básico/Basic Routing` ha sido descontinuado.
- `Cuatro patrones de integración:` Interfaz síncrona [solicitud-respuesta], interfaz asíncrona [unidireccional], interfaz asíncrona con devolución de llamada, basado en eventos (polling)
- `Orquestación Programada/Scheduled Orchestation` = `Transferencia de Archivos/File Transfer`
- `Publish to OIC`: Crea una integración en la que defines un adaptador de disparador para publicar mensajes a OIC a través de una interfaz o evento asincrónico. Esta integración está desacoplada de todos los suscriptores, ya que todas las integraciones participantes pueden activarse y desactivarse independientemente entre sí.
- `Subscribe to OIC`: Crea una integración en la que te suscribes a una integración publicadora existente. Luego defines un adaptador invocable para procesar mensajes que han sido publicados a OIC por esa integración.
- `Oracle BPEL Process Manager:` Te permite definir cómo se ejecuta un proceso empresarial que involucra servicios web. Los mensajes `BPEL` invocan servicios remotos y orquestan la ejecución del proceso.
- `Campo de seguimiento/Tracking Field:` Debemos asignar al menos uno (maximo 3). Uno de estos campos debe seleccionarse como el campo de identificación empresarial principal. El identificador empresarial principal te permite realizar un seguimiento de los campos a lo largo de los flujos de integración durante el tiempo de ejecución y siempre está disponible. Durante el tiempo de ejecución, el estado de los identificadores empresariales es visible en la página de Seguimiento y (si han ocurrido errores de integración) en la página de Errores.
- [WSDL](./Extras.md/#¿qué-son-los-archivos-wsdl)
- Crear una conexión solo requiere información básica y políticas de conexión y seguridad definidas.
- Los casos de uso específicos se facilitan más tarde al configurar una conexión para ser utilizada dentro de un flujo de integración.
- Normalmente, se crea solo una conexión por cada sistema externo o aplicación.
- OIC administra múltiples conexiones en tiempo de ejecución para cada flujo de integración según sea necesario.
- [Oracle Service Cloud (RightNow)](./Extras.md/#oracle-service-cloud-rightnow)
- [Clave CSF](./Extras.md/#clave-csf-en-oracle-engagement-cloud)
- [Oracle ERP Cloud Adapter](./Extras.md/#adaptador-oracle-erp-cloud)
- El algoritmo compatible para la Clave Pública es RSA para encriptación y el tamaño de la clave debe ser de 1024 bits de longitud
- [Oracle HCM Cloud Adapter](./Extras.md/#oracle-hcm-cloud)
- [DVM](./Extras.md/#dvm)
- [DMZ](./Extras.md/#dmz)
- [MTOM](./Extras.md/#mtom)
- La conexión REST (invoke) soporta los tipos de conexión: _Swagger, RAML, Metadata Catalog o Base URL_
- [Conexiones/Certificados SSL](./Extras.md/#conexionescertificados-ssl)
- Si realizas una conexión SSL en la que el certificado raíz no existe en Oracle Integration, se producirá una excepción. En ese caso, debes cargar el certificado adecuado. Un certificado permite que Oracle Integration se conecte con servicios externos
- [Agente de Conectividad](./Extras.md/#agente-de-conectividad-en-oic)
- Después de crear el grupo de agentes, NO podrás editar el identificador del grupo de agentes. En su lugar, debes eliminar y volver a crear otro grupo de agentes para asociarlo con un identificador de grupo de agentes diferente.
- El agente de conectividad se utiliza con un proxy SSL.
- El agente de conectividad se utiliza para invocar puntos finales locales seguros (SSL).
- 