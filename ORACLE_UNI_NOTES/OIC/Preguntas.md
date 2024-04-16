# Preguntas de Práctica para Certificación

## Preguntas curso OIC

`1 - 5: Skill Check: Module 2 - OIC Architectural Overview`

`6 - 10: Skill Check: Module 3 - Integrations Life Cycle & Packages`

`11 - 15: Skill Check: Module 4 - Fundamentals of Creating Integrations`

`16 - 20: Skill Check: Module 5 - Creating OIC Adapter Connections`

`21 - 25: Skill Check: Module 6 - Configuring Trigger Connections`

`26 - 30: Skill Check: Module 7 - Configuring Invoke Connections`

`31 - 35: Skill Check: Module 8 - Data Mapping`

`36 - 40: Skill Check: Module 9 - Orchestration Integration Actions`

`41 - 45: Skill Check: Module 10 - Additional OIC Capabilities`

`46 - 50: Skill Check: Module 11 - File Handling Concepts and Options`

`51 - 55: Skill Check: Module 12 - Orchestration Scopes and Fault Handling`

`56 - 60: Skill Check: Module 13 - OIC Feature Updates and Enhancements`

1. **Which icon associated with an integration shown on the Integrations page must you click to access the Test link for testing an integration based on a REST trigger?**
   1. Run
   2. Test
   3. Activate
   4. Menu <br><br>
2. **An integration must first be activated before testing.**
   1. True
   2. False <br><br>
3. **Which is NOT a capability of the OIC Integrations feature?**
   1. Simplifies connectivity between applications both in the cloud and deployed on-premises
   2. Reduces time to decision with human-in-the-loop approvals and exception handling
   3. Uses a configuration approach versus coding
   4. Provides an intelligent drag-and-drop data mapping tool <br><br>
4. **Which feature is NOT bundled with Oracle Integration Cloud (OIC)?**
   1. Process Builder
   2. Integrations
   3. Visual Builder
   4. SOA Suite <br><br>
5. **Which file extension can you use to save integrations as a binary file?**
   1. .iar
   2. .jar
   3. .zip
   4. .int <br><br>
6. **When creating a new integration, the Create Version option requires that you use a unique identifier.**
   1. True
   2. False <br><br>
7. **Which statement is TRUE about integration packages in OIC?**
   1. Packages provide a unique namespace for integrations.
   2. You must first create an empty package prior to adding new integrations.
   3. Integrations in a package can be directly accessed by integrations in other packages.
   4. An integration can belong to one or more packages. <br><br>
8. **To view details in the activity stream of the integration instance that you have tested, you can click the Instance ID link on the integration test page.**
   1. True
   2. False <br><br>
9. **Which statement is NOT true about importing integrations into an OIC environment?**
   1.  Imported integrations will not include dependent connections if they already exist in the target OIC.
   2.  If dependent connection resources already exist in the target OIC, the imported integration can be immediately activated.
   3.  Imported integrations can be reconfigured using the OIC REST API.
   4.  Imported connection resources will contain all connection properties and credentials. <br><br>
10. **Which scenario is NOT true about to OIC integrations being in an active state at the same time?**
    1.  Same identifier, different minor version numbers.
    2.  Different identifiers, same minor version numbers.
    3.  Same identifier, different major version number.
    4.  Different identifiers, same major version number. <br><br>
11. **When activating a completed integration, you have the option to enable integration instance tracking with or without the complete payload for all flow activities.**
    1.  True
    2.  False <br><br>
12. **When testing an integration that uses a SOAP-trigger connection, you can use either an external SOAP client or the integration testing page that is available in the OIC console.**
    1.  True
    2.  False <br><br>
13. **Which statement is TRUE about the [Oracle Asserter testing framework](./Extras.md/#marco-de-pruebas-oracle-asserter) in OIC?**
    1.  You can enable Oracle Asserter only when activating the integration.
    2.  When exporting an integration, you can include asserter recordings.
    3.  Asserter recordings can be run only in the environment in which they were recorded.
    4.  The Oracle Asserter option is not available in OIC production environments. <br><br>
14. **When configuring business identifiers for an integration configuration, what is the maximum number of tracking fields that can be defined?**
    1.  2
    2.  3
    3.  5
    4.  10 <br><br>
15. **What are the requirements for authentication credentials when testing a SOAP-trigger integration by using the SoapUI client?**
    1.  OIC credentials can be passed as an WSS Username Token in the HTTP header.
    2.  Authentication is not required when testing integrations.
    3.  OIC credentials can be passed as a WSS Username Token in the SOAP body.
    4.  OIC credentials can be passed as a WSS Username Token in the SOAP header. <br><br>
16. **Which feature is NOT available with most Oracle Cloud Adapters?**
    1.  Session management during runtime interactions
    2.  Native support via object query languages for integration use cases
    3.  The automatic discovery of application assets at design time
    4.  Ability to connect directly from OIC without requiring security credentials at design time <br><br>
17. **When defining a Connection resource, you can select either the Invoke or Trigger role, but not both.**
    1.  True
    2.  False <br><br>
18. **When defining a Connection resource based on the Service Cloud (RightNow) adapter, which is required while configuring connectivity properties?**
    1.  The Wallet that was downloaded from the service instance
    2.  The Fusion URL for the service instance
    3.  The REST API Base URL for the service instance
    4.  The WSDL URL for the service instance <br><br>
19. **The service catalog is a Fusion Application service that returns a list of external services available for integration when configuring connections. To which two Oracle Cloud applications does the service catalog return the external services?**
    1.  SOA Cloud
    2.  Service Cloud (RightNow)
    3.  HCM Cloud
    4.  Eloqua Cloud
    5.  ERP Cloud <br><br>
20. **The Integrated SOA Gateway (ISG) is required to provide bi-directional connectivity to an E-Business Suite application and OIC.**
    1.  True
    2.  False <br><br>
21. **A Connection resource configured as an inbound trigger for an integration using the File Adapter will require an OIC Connectivity Agent to be deployed.**
    1.  True
    2.  False <br><br>
22. **Which statement is FALSE about configuring a connection as an inbound trigger for an integration based on the generic REST adapter?**
    1.  When using the POST or PUT method, you must select JSON for the request payload format.
    2.  You can configure the response payload format to be binary (for example, a .zip file).
    3.  You must associate just one HTTP method for each request operation.
    4.  You can configure Cross Origin Resource Sharing (CORS) for any request operation. <br><br>
23. **After you have completed the configuration for a Trigger connection that defines a synchronous message exchange pattern for your integration, what should you do to handle the response message back to the client of the integration?**
    1.  A Map action is automatically added at the end of the integration flow with a default response. Optionally, you can configure data for the response.
    2.  You need to add a Map action to the end of the flow, which will provide a default response. Optionally, you can configure data for the response.
    3.  An empty Map action is automatically added at the end of the integration flow. You must then configure data for the response.
    4.  You need to add a Map action to the end of the flow. Then you must configure data for the response. <br><br>
24. **Which statement is TRUE about configuring connections within an integration based on the generic SOAP adapter?**
    1.  SoapAction validations are required for all inbound (Trigger) connections to OIC.
    2.  Configuring custom SOAP headers is only available for outbound (Invoke) adapter configurations.
    3.  You can configure both standard and custom HTTP headers for the inbound (Trigger) connection.
    4.  You can select one or more operations for the inbound (Trigger) connection based on the available operations in the abstract WSDL. <br><br>
25. **Which is NOT an available option for Response Type when configuring a Trigger role connection using Fusion application adapters?**
    1.  None
    2.  Immediate
    3.  Delayed
    4.  Callback <br><br>
26. **OIC Integrations can invoke external or internal OIC services using any of the three basic web service interaction patterns. Which is NOT an interaction pattern used by SOAP web services?**
    1.  One-Way
    2.  Publish/Subscribe
    3.  Asynchronous Request/Callback
    4.  Synchronous Request/Reply <br><br>
27. **When using an Oracle ATP or ADW adapter, which operation is NOT available while configuring an invoke connection?**
    1.  Invoke a Stored Procedure
    2.  Perform an Operation On a Table
    3.  Import XML Schema
    4.  Run a SQL Statement <br><br>
28. **Which two operations enable you to specify the file schema when configuring an FTP adapter for an invoke connection?**
    1.  Write File
    2.  Read a File
    3.  List Files
    4.  Move a File
    5.  Download File <br><br>
29. **The OIC Adapter Endpoint Configuration Wizard is limited to integrations invoking only Oracle or third-party application adapters.**
    1.  True
    2.  False <br><br>
30. **Which syntax is used when configuring a connection to query data using an Oracle Service Cloud (RightNow) adapter?**
    1.  YAML
    2.  ROQL
    3.  SQL
    4.  Groovy <br><br>
31. **Which statement is NOT true about testing mappings in the Data Mapper tool?**
    1.  Custom JavaScript functions will be tested as long as they are registered as a library.
    2.  In the input panel, you can manually enter a real payload or automatically generate a test payload.
    3.  If your mapping includes two source data structures, payloads for both sources can be generated.
    4.  Payloads for scalar parameters are not automatically created. <br><br>
32. **When using the Data Mapper Recommendations engine, automatic mapping recommendations are categorized by three strength levels: Low, Medium, High.**
    1.  True
    2.  False <br><br>
33. **Which statement is true about OIC Data Mapper?**
    1.  All Source and Target data objects are represented internally as XML structures.
    2.  Required fields identified by a blue asterisk must be mapped to avoid a validation error.
    3.  Substitution groups in schemas are not supported.
    4.  Mapping supports only qualified schemas. <br><br>
34. **Which is NOT a Data Mapper feature for facilitating transformations in a Map action?**
    1.  Access to both standard and custom XPath functions
    2.  Using one or more XSLT templates
    3.  An expression builder for more complex XSLT expressions
    4.  Using domain-value maps with OIC Lookups <br><br>
35. **Which statement is NOT true about lookups in OIC?**
    1.  SaaS adapter connections are needed to define a Lookup.
    2.  Lookups can be cloned or exported to a CSV file for easy reuse.
    3.  Referencing a Lookup in the Data Mapper requires the use of the lookupValue function.
    4.  Lookups are not deployed as part of integration activations, but are loaded when referenced at run time. <br><br>
36. **Which statement is NOT valid about the Wait action?**
    1.  The Wait action is not available in App Driven integrations that are configured with a synchronous trigger.
    2.  The Wait action can be configured only for a static period of time up to 6 hours.
    3.  After configuration, you can move the Wait action to another location within the integration flow by using the Reposition button.
    4.  The Wait action can be used only within a looping construct, such as a For-Each or Wait action. <br><br>
37. **The For-Each action uses a repeating element to indicate the number of iterations that can be processed sequentially or in parallel.**
    1.  True
    2.  False <br><br>
38. **Which is NOT a feature or capability associated with using the Integration Call action?**
    1.  It optimizes the call in-memory before traversing the network stack.
    2.  It allows for invoking another integration running locally in the same OIC instance.
    3.  It eliminates the need to create an explicit REST or SOAP adapter connection for that endpoint.
    4.  It can also invoke a scheduled orchestration integration that has no explicit interface. <br><br>
39. **Which action is used in an OIC integration flow to create variables or to assign new values to existing variables?**
    1.  Logger
    2.  Assign
    3.  EDI Translate
    4.  Map <br><br>
40. **When configuring the Write File operation of the Stage File action, which location would you designate for the newly created file?**
    1.  A defined location in the integration's runtime memory referenced by a variable
    2.  A specified directory on a remote file system accessible by a File or FTP adapter connection
    3.  A specified directory in the integration's virtual file system (VFS) <br><br>
41. **You can pause an integration schedule from the Monitoring console even if a run is already in progress.**
    1.  True 
    2.  False <br><br>
42. **What is the primary purpose of using business identifiers in Oracle Integration Cloud (OIC) integrations?**
    1.  To provide a unique reference for tracking and monitoring integrations
    2.  To enhance the security of integrations by encrypting data
    3.  To improve the performance of integrations by reducing processing time
    4.  To automate the deployment of integrations across multiple environments <br><br>
43. **Which statement is NOT true about the OIC REST API?**
    1.  All REST API calls must be executed over secure sockets layer (SSL).
    2.  For Connection resources, you can update both the connection URL as well as security credentials.
    3.  You can deactivate an integration to stop it from processing any new messages to include pending requests.
    4.  All REST API calls require valid credentials of an OIC user with the ServiceAdministrator role. <br><br>
44. **Which statement is NOT true about defining an advanced schedule for a Scheduled Orchestration?**
    1.  You can choose both a basic and advanced schedule if needed.
    2.  You must use iCal syntax to create the expression statement.
    3.  You cannot define a frequency repetition of less than one minute.
    4.  You can define multiple schedule frequencies within one expression. <br><br>
45. **Which statement is true about Scheduled Orchestration style integrations?**
    1.  The design canvas is identical as when creating an App Driven style orchestration to include options for configuring a Trigger connection.
    2.  You can resubmit failed runs only for scheduled orchestrations by using the REST API.
    3.  You must define a basic or advanced schedule before activation.
    4.  You can initiate an integration run by creating an ad hoc request or in sequence with a scheduled run. <br><br>
46. **Which scenario is a valid use case for utilizing schedule parameters in a Scheduled Orchestration style integration in Oracle Integration Cloud (OIC)?**
    1.  To monitor the file transfer progress between two integration instances
    2.  To define which file was last processed in a batch when limiting the number of files in each scheduled run
    3.  To trigger an integration for processing a file when it is uploaded to an FTP server
    4.  To enable real-time file transfer between two different cloud applications <br><br>
47. **Which can be leveraged to create a native schema (NXSD) file for complex files containing records whose fields have multiple delimiter types?**
    1.  Stage File Action
    2.  Native Format Builder
    3.  Data Mapper
    4.  File Adapter Expression Builder <br><br>
48. **The configuration and usage of a trigger or invoke connection based on a File adapter requires the deployment of an OIC Connectivity Agent.**
    1.  True
    2.  False <br><br>
49. **Which is NOT a configuration option when defining the Download File operation of an invoke connection based on an FTP adapter?**
    1.  Specifying a schema for structured files less than 10 MB
    2.  Specifying the VFS directory to use for the downloaded file
    3.  Performing unzip on a compressed file
    4.  Performing PGP decryption on an encrypted file <br><br>
50. **Which OIC adapter enables you to decrypt a file being read or downloaded using PGP cryptography?**
    1.  File
    2.  FTP
    3.  Both File and FTP
    4.  Neither File nor FTP <br><br>
51. **Which End action CANNOT be used to return errors back to a client of a synchronous integration flow?**
    1.  Re-Throw Fault
    2.  Return
    3.  Callback
    4.  Fault Return <br><br>
52. **The Global fault handler has a default implementation that rethrows the fault to the OIC error hospital.**
    1.  True
    2.  False <br><br>
53. **What is the Parking Lot design pattern in the context of handling errors in OIC integrations?**
    1.  A pattern used for retrying failed messages
    2.  A pattern used for temporarily storing failed messages for later processing
    3.  A pattern used for propagating errors back to the calling application
    4.  A pattern used for routing messages based on message content <br><br>
54. **Which statement is NOT true about the Scope action in an OIC integration?**
    1.  A scope action can be added in the integration's Global fault handler.
    2.  Up to three nested scopes can be added to a basic scope action.
    3.  Scope actions provide for adding scope-level fault handling logic.
    4.  A scope action can be repositioned to another location in the integration if it is collapsed. <br><br>
55. **Which is NOT true about leveraging the Throw New Fault action in an integration flow?**
    1.  You can place the Throw New Fault action directly on the main flow path.
    2.  You can place the Throw New Fault action inside the Global Fault handler.
    3.  If the conditional expression for the skip condition is empty, the fault will never be thrown.
    4.  You are required to define a fault code when configuring the Throw New Fault action. <br><br>
56. **What is Oracle's recommended alternative for the deprecated Read Multiple Files operation that was previously available for the FTP adapter?**
    1.  Use the Read File in Segments operation of a Stage File action within the integration. 
    2.  Use a File adapter with a Connectivity Agent installed to achieve the same functionality.
    3.  Use the FTP adapter's Read File operation within a looping construct.
    4.  Use the FTP adapter's List File operation to retrieve all files within a directory instead. <br><br>
57. **What is the name of the log file that will be stored for up to 30 days in OCI Logging when you enable logging for the OIC instance?**
    1.  activity-stream-json.log
    2.  oic-integration.log
    3.  ics-flow.log
    4.  integration-flow-json.log <br><br>
58. **Which is NOT available as a new OIC built-in adapter?**
    1.  Jira
    2.  Zendesk
    3.  LinkedIn
    4.  PeopleSoft <br><br>
59. **Considering that the Publish and Subscribe integration patterns have been deprecated, what is Oracle's recommended alternative for achieving a similar integration solution?**
    1.  Use other integration styles in conjunction with FTP adapters to distribute messages as files in the OIC File Server.
    2.  Deploy one or more JMS topics to SOA Cloud and leverage the WebLogic JMS adapters within new integrations.
    3.  Use App-Driven or Scheduled orchestrations leveraging OCI Streaming Adapter connections.
    4.  Use the new B2B feature to create "internal" trading partner agreements between two integrations. <br><br>
60. **Support for consuming platform events is now available as an enhancement to the SAP SuccessFactors adapter.**
    1.  True
    2.  False <br><br>
61. **You can use either an Append or an Assign operation in a Data Stitch action.**
    1.  True
    2.  False <br><br>
62. **In the scenario involving the synchronization of Opportunities in Salesforce to new Orders in Oracle NetSuite, what happens at the end of a successful opportunity-to-order integration flow instance?**
    1.  The new NetSuite sales order number is returned to Salesforce.
    2.  The Opportunity is updated with the new NetSuite order ID.
    3.  The new NetSuite Order object is sent to Salesforce as a callback.
    4.  A Boolean result is returned to Salesforce with a value of TRUE.

## Respuestas curso OIC

1. `Run`
2. `True` - Testing requires the integration to be active and able to be invoked.
3. `Reduces time to decision with human-in-the-loop approvals and exception handling` - This is a capability of the Process feature, not the Integrations feature.
4. `SOA Suite`
5. `.iar` - The .iar file extension is used which means: "integration archive".
6. `False` - This statement is false because the identifier must remain the same. Only the version number must be changed.
7. `Integrations in a package can be directly accessed by integrations in other packages.` - Integrations are visible to one another regardless of package.
8. `True` - The link is available after the instance has been executed.
9. `Imported connection resources will contain all connection properties and credentials.` - This statement is not true because credential information for connections is not included when integrations are exported; therefore, they are not available when imported.
10. `Same identifier, different minor version numbers.` - Two integrations with the same identifier must have a different major version number to be active at the same time.
11. `True`
12. `False` - This statement is FALSE because there is no SOAP client tester in the OIC console. The testing page is available only for REST-trigger integrations.
13. `When exporting an integration, you can include asserter recordings.` - You can include asserter recordings with the integration, which can then be imported and run in another OIC environment.
14. `3` - Although one is required, up to three can be defined.
15. `OIC credentials can be passed as a WSS Username Token in the SOAP header.`
16. `Ability to connect directly from OIC without requiring security credentials at design time` - Although there is a simple interface for security properties, any external resource requiring credentials will still require you to configure security for that adapter connection.
17. `False` - This statement is FALSE because you can choose both roles and later use the connection for either a Trigger or an Invoke use case within an integration.
18. `The WSDL URL for the service instance`
19. `HCM Cloud & ERP Cloud` - Oracle Fusion applications include: ERP Cloud, HCM Cloud, and Engagement Cloud (now called the CX Sales and B2B Service).
20. `True` -  Although a connectivity agent can be used instead of the ISG for access REST services, an ISG is required for bi-directional connectivity.
21. `True` - The Connectivity Agent must be deployed and made accessible to the file system, then once connected to OIC, it serves as a polling agent for serving files to the integration.
22. `When using the POST or PUT method, you must select JSON for the request payload format.` - This is FALSE because other payload formats (such as XML) can be used. In addition, you can choose to require an attachment type instead.
23. `An empty Map action is automatically added at the end of the integration flow. You must then configure data for the response.` - After a synchronous pattern trigger has been configured, the design canvas will automatically show an empty Map action. It must then be implemented to configure the data mappings for your desired response. This is typically handled after most other integration logic has been completed in the flow.
24. `You can configure both standard and custom HTTP headers for the inbound (Trigger) connection.` - This is also true for outbound (Invoke) connections.
25. `Callback` - Although the Delayed type will effectively provide the framework to allow an integration flow to send a callback to the service, there is no Callback type.
26. `Publish/Subscribe` - Publish/Subscribe is not a web service interaction pattern.
27. `Import XML Schema` - This operation is not available for the ATP/ADW adapter.
28. `Write File & Read a File` - Read a File and Write File adapter operations enable you to specify the file schema.
29. `False` - Many other technology adapters (such as FTP, REST, SOAP, and so on) can also leverage the Adapter Endpoint Configuration Wizard.
30. `ROQL` - This application uses the proprietary RightNow Object Query Language (ROQL) for queries.
31. `Custom JavaScript functions will be tested as long as they are registered as a library.` - This statement is FALSE because custom JavaScript functions cannot be tested under any circumstances in the Data Mapper test tool.
32. `True`
33. `All Source and Target data objects are represented internally as XML structures.` - Regardless of the actual data structure, XML structures are used internally to facilitate XSLT mapping.
34. `Using one or more XSLT templates` - XSLT templates are not supported in the Data Mapper tool.
35. `SaaS adapter connections are needed to define a Lookup.` - This statement is FALSE because alternatively, you could use any generic string value for a Domain Name when creating the Lookup.
36. `The Wait action can be used only within a looping construct, such as a For-Each or Wait action.` - This is FALSE because it can be used anywhere in a non-synchronous integration flow.
37. `True`
38. `It optimizes the call in-memory before traversing the network stack.` - The optimized call does NOT traverse the network stack.
39. `Assign`
40. `A specified directory in the integration's virtual file system (VFS)` - All newly created files will be stored in the VFS. You can later send that file to an external file system.
41. `True` - If a run is already in progress, pausing a schedule will also pause that instance as well.
42. `To provide a unique reference for tracking and monitoring integrations` - Business identifiers are used to uniquely identify instances of a specific integration. This helps in tracking and monitoring the progress of these instances, enabling users to search, filter, and correlate instances based on specific business identifiers.
43. `All REST API calls require valid credentials of an OIC user with the ServiceAdministrator role.` - This is FALSE because the ServiceAdministrator role is not required for "view-only" APIs.
44. `You can choose both a basic and advanced schedule if needed.` - This is FALSE because you must choose either the basic or advanced option when defining a schedule.
45. `You can initiate an integration run by creating an ad hoc request or in sequence with a scheduled run.` - If a schedule is already defined, it can be done in sequence with a scheduled run.
46. `To define which file was last processed in a batch when limiting the number of files in each scheduled run` - This specific example was used in the lecture.
47. `Native Format Builder` - The Native Format Builder Wizard (available in JDeveloper or OEPE) is the recommended tool for creating more complex NXSD files.
48. `True` - The Connectivity Agent is required when configuring a File adapter for either role.
49. `Specifying a schema for structured files less than 10 MB` - Specifying the schema for structured files is available only when you attempt to read the file into memory using the Read File operation.
50. `FTP`
51. `Callback` - This action cannot be used at all in synchronous integration orchestrations.
52. `True`
53. `A pattern used for retrying failed messages`
54. `Up to three nested scopes can be added to a basic scope action.` - This statement is FALSE because there is no limit to the number of nested scopes that can be added.
55. `If the conditional expression for the skip condition is empty, the fault will never be thrown.` - This statement is FALSE because the fault will ALWAYS be thrown if the skip condition is empty.
56. `Use the FTP adapter's Read File operation within a looping construct.` - This allows for all files to be read in sequence or in parallel (using For-Each or While actions).
57. `activity-stream-json.log`
58. `PeopleSoft`
59. `Use App-Driven or Scheduled orchestrations leveraging OCI Streaming Adapter connections.`
60. 
61. `False` - This is FALSE because that feature was added to the Salesforce adapter (not SAP SuccessFactors).
62. `True`
63. `The Opportunity is updated with the new NetSuite order ID.`

---

# [Parte 2](./Preguntas2.md)