
## Examen de Prueba YT

1. **You are configuring an ERP Cloud adapter connection invoke action within an Oracle Integration Cloud (OIC) integration. How many child resources can you select?**
   1. 01
   2. 05
   3. 10
   4. Unlimited
2. **Which is NOT an available option while configuring an ERP Cloud adapter to use in an Oracle Integration Cloud (OIC) integration?**
   1. Extract bulk data from ERP Cloud
   2. Upload files to UCM
   3. Invoke CRUD operation on ERP Cloud REST API
   4. Enabte catlback
3. **Which metadata formats are supported by the adapter when configuring Oracle Integration Cloud (OIC) connections?**
   1. Open API, RAML, Swagger
   2. Swagger, WADL, RAML
   3. Open API, WADL, RAML
   4. Swagger, RAML, WADL
4. **Which is NOT an advantage of using Oracle Integration Cloud (OIC) for creating application integrations?**
   1. Public/Private Cloud portability
   2. Auto-association of Oracle SaaS applications
   3. Data mapping recommendations
   4. User choice of IDE for development
   5. Prebuilt integrations
5. **Oracle Integration Cloud (OIC) service is available in two editions, Standard and Enterprise. Which two OIC Enterprise Edition capabilities are ALSO available in OIC Standard Edition?**
   1. Integration Insight
   2. Visual Builder
   3. Process Applications
   4. File Server
   5. Enterprise application adapters (such as EBS, 3DE, SAP, and Siebel)
   6. B2B Trading Partner agreements
6. **Your team is responsible for an OIC package that contains five integrations. Currently, three of these integrations are active while the other two are inactive. Which statement is valid if you were to replace a connection used in this package?**
   1. You can only replace the connections used by the three active integrations.
   2. You cannot replace connections unless atl integrations in the package are in an active state.
   3. You can only replace the connections used by the two inactive integrations.
   4. You cannot replace connections unless all integrations in the package are in an inactive state.
7. **Your organization has a number of active integrations in Oracle Integration Cloud (OIC). Your advice is sought on the consequences of deactivating integration instances. Which statement concerning integration deactivation is NOT valid?**
   1. All existing history, monitoring, and runtime data will be lost.
   2. You can choose to retain the event subscription, where events are resent if the integration is reactivated again within six hours.
   3. Processing of any new messages will be immediately stopped.
   4. You will not be able to observe any failed instances occurring after the deactivation request.
8. **You have a use case that requires a large data extract, which is more than 10 MB, to be processed within an Oracle Integration Cloud (OIC) integration. Which are three valid options?**
   1. Retrieve the file by invoking a SOAP API, which sends base64 encoded data within the SOAP body, and then decode the data and make it available for processing using a Stage File action.
   2. Retrieve the file by invoking a SOAP API, which sends the document as an MTOM attachment, and make it available for processing using a Stage File action.
   3. Retrieve the file from an external endpoint using APIS that support application/blob as content type, and make it available for processing using a Stage File action.
   4. Send the file as a multipart attachment to an OIC integration using a REST trigger, and make it available for processing using a Stage File action.
   5. Upload the file to the OIC File Server, and then use an FTP Adapter Download File operation, which makes it available for processing using a Stage File action.
9. **One of your downstream applications is becoming overwhelmed with too many individual synchronous invocations from your current Oracle Integration Cloud (OIC) integration. It is recommended that you redesign the integration to take advantage of the batch processing capabilities of the application. Which approach is a valid OIC design best practice that Will provide the best solution to mitigate this issue?**
   1.  Create a custom batch call function, register the function as a library in your OIC environment, then use the Javascript action to invoke the application.
   2.  Throttle the individual synchronous calls by adding a wait activity prior to each invocation to the application within the loop.
   3.  Use the Append option in the Write File operation of the stage File action within a loop to create a single batch file to be sent to the application.
   4.  Reactivate the integration and use the disable tracing and message tracking option which will optimize performance for each invocation to the application.
10. **You are implementing a synchronous Oracle Integration Cloud (OIC) integration flow that processes file records within a while loop action. At the end of each loop, you want to delay processing of the next record for a certain period of time. Which is a valid consideration when using the wait action?**
    1.  The wait action cannot be used in a synchronous flow.
    2.  The Wait action can only be positioned as the last action in the loop.
    3.  The minimum wait time cannot be less than five seconds when configuring a wait action in any integration flow. 
    4.  The maximum wait time cannot exceed two minutes when configuring a wait action in a synchronous flow.
11. **Which operation is NOT supported by an Oracle Integration Cloud (OIC) Connection resource configured with the FTP Adapter in the Invoke role?**
    1.  WriteFi1e
    2.  Delete File
    3.  Download File
    4.  Last File
    5.  Read File
    6.  Read File in Segments
12. **Which set of operations are supported by the Oracle Integration Cloud (OIC) File Adapter?**
    1.  read, write, list, download
    2.  read, write, list, move
    3.  read, write, list
    4.  read, write
    5.  read, write, list, download, move, delete
13. **You need to create an Oracle Integration Cloud (OIC) integration that processes many records individually that are contained within a large file. You have been advised to use an implementation approach that uses the Download File operation of an FTP adapter in conjunction with the Stage File action Read File in Segments operation to mitigate issues with memory consumption. </br> When using this approach, which is a valid consideration regarding the use ofthe Read File in Segments operation?**
    1.  The Read File in Segments operation allows you to process the segments sequentially or in parallel.
    2.  Segment sizes default to 50 records but can be configured to any other segment size.
    3.  You must provide the actual filename because file references cannot be processed by the Read File in Segments operation.
    4.  You need to explicitly configure a Scope action for this operation if you want to add additional actions during the processing of each segment.
14. **When defining the frequency for scheduled orchestration Style integration runs, you can choose either Basic or the Advanced option. Which expression format is used for defining advanced scheduled runs?**
    1.  iCal
    2.  Groovy
    3.  cron
    4.  YAML
15. **As an Oracle Integration Cloud (OIC) specialist, you are tasked with implementing a scheduled integration between two enterprise applications. The client requires that the integration be run every weekday at 3:00 PM to synchronize data between the systems. </br> Which advanced scheduling configuration expression Will you use?**
    1.  "FREQ=WEEKLY;BYDAY=MO-FR;BYHOUR=15"
    2.  "FREQ=DAILY;BYDAY!=SA,SU;BYHOUR=15"
    3.  "FREQ=DAILY;BYDAY=MO-FR;BYHOUR=15"
    4.  "FREQ=WEEKLY;BYDAY=MO,TU,WE,TH,FR;BYHOUR=15"
16. **The Oracle Integration Cloud (OIC) integration design editor provides a data mapper UI tool that is available for Map actions. Which statements are TRUE regarding the use ofthe Mapper tool? Select TWO**
    1.  You cannot drag and drop an XPath fitnction activity directly to a target node element.
    2.  You can drag and drop a source data element to multiple target node elements.
    3.  You cannot drag and drop a source data element to a target node element that is already mapped.
    4.  You cannot drag and drop an XSLT flow control statement directly to a target node element.
17. **There are use cases in which you need to perform an advanced XSLT task that you cannot perform in the Oracle Integration Cloud (OIC) data mapper. To perform the advanced mapping tasks, you decide to use an external XSLT mapper and then import the .XSI file back to your integration. Which is NOT a valid consideration when handling this use case?**
    1.  The exported archive must be imported into an Oracle Service Bus project in JDeveloper.
    2.  The exprted archive file can include a map file that is largely complete in content or a map file that is empty of content.
    3.  Once the advanced mapping is complete, you must import the entire integration that contains the updated.xsl files.
    4.  You must export the entire integration that contains one or more .xsl files.
18. **CSV-formatted data has been extracted from ERP Cloud by invoking a web service using the SOAP Adapter, and the data extract has been returned as an MTOM attachment. You now need to send this CSV file to an external REST API that supports accepting this content as a Base64 encoded string. Which XPath mapper function should be used to map the SOAP MTOM attachment to the Base64 element present in the target REST API payload?**
    1.  decodeBase64ToReference
    2.  encodeReferenceToBase64
    3.  decodeBase64
    4.  encodeBase64
19. **Which action CANNOT be performed from the Oracle Integration Cloud (OIC) Monitoring Dashboard?**
    1.  View Connectivity Agent Group Status
    2.  Download Design-time Audit Records
    3.  View Design-time Metrics
    4.  Download OIC Lookups
    5.  View Current Email Count
20. **You are tasked with creating an Oracle Integration Cloud (OIC) integration flow that supports a B2B exchange. When configuring the B2B action there are several capabilities as well as limitations. Which statement is NOT valid concerning OIC B2B capabilities?**
    1.  You can customize standard Electronic Data Interchange (EDI) documents by adding new schema constructs or by editing existing constructs.
    2.  It is mandatory to preform validations on EDI documents for inbound translations; however, for outbound translations it is optional.
    3.  A previously created Trading Partner Agrement is optional when configuring the inbound or outbound translation.
21. **Which statement about Oracle Integration Cloud (OIC) is NOT valid?**
    1.  OIC Lookups are based on a static definition, meaning you create and populate them during design time, and cannot be changed by runtime activities.
    2.  An application-driven integration can contain one or more trigger (source) connections for requests sent to OIC and one or more invoke (target) connections for requests sent from OIC.
    3.  Using the connectivity agent, you can create hybrid integrations and exchange messages between applications in private or on-premises networks and OIC.
    4.  When you open the mapper for a request or response message in an integration, the data structures are automatically populated with the information pulled from the source and target connections.
22. **Which are types of certificates in Oracle Infrastructure Cloud (OIC) that can be imported from the Certificates page under Settings? Select THREE**
    1.  Trust Certificate
    2.  Identity Certificate
    3.  Multi Domain SSL Certificate
    4.  Message Protection Certificate
    5.  Unified Communications Certificate
23. **You have an Oracle Integration Cloud (OIC) synchronous integration flow that updates external systems with several invocations. However, several ofyour OIC integration clients are reporting that they are experiencing timeouts waiting for the response confirmation from this processing. Which is a legitimate stratey to mitigate this issue?**
    1.  Change the implementation logic to invoke multiple fine-grained external API calls within a single loop.
    2.  Change the design implementation strategy to an asynchronous flow that provides a separate notification to clients when the processing is complete.
    3.  Increase the blocking timeout within the OIC integration settings to allow for extended time.

## Respuestas Examen de Prueba YT

1. `10` - Al configurar una acción de invocación de conexión del adaptador ERP Cloud en una integración de Oracle Integration Cloud (OIC), puedes seleccionar un máximo de diez recursos secundarios.
2. `Invoke CRUD operation on ERP Cloud REST API` -  Esta opción no está disponible al configurar un adaptador ERP Cloud para usar en una integración de Oracle Integration Cloud (OIC). Las opciones disponibles incluyen la extracción de datos a granel de ERP Cloud, la carga de archivos en UCM, y la habilitación de callback.
3. `Open API, RAML, Swagger`
4. `User choice of IDE for development`
5. `Visual Builder & File Server`
6. `You can only replace the connections used by the two inactive integrations.`
7. `You will not be able to observe any failed instances occurring after the deactivation request.`
8. `i, ii & v`
9. `Use the Append option in the Write File operation of the stage File action within a loop to create a single batch file to be sent to the application.`
10. `The wait action cannot be used in a synchronous flow.`
11. `Last File`
12. `read, write, list, download, move, delete`
13. `The Read File in Segments operation allows you to process the segments sequentially or in parallel.`
14. `iCal`
15. `"FREQ=WEEKLY;BYDAY=MO,TU,WE,TH,FR;BYHOUR=15"`
16. `ii & iii`
17. `The exported archive must be imported into an Oracle Service Bus project in JDeveloper.`
18. `encodeBase64`
19. `Download OIC Lookups`
20. `A previously created Trading Partner Agrement is optional when configuring the inbound or outbound translation.`
21. `An application-driven integration can contain one or more trigger (source) connections for requests sent to OIC and one or more invoke (target) connections for requests sent from OIC.`
22. `i, ii, iv`
23. `Change the design implementation strategy to an asynchronous flow that provides a separate notification to clients when the processing is complete.`