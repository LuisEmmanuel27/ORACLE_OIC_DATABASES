
## Examen de Prueba YT

1. **You are configuring an ERP Cloud adapter connection invoke action within an Oracle Integration Cloud (OIC) integration. How many child resources can you select?**
   1. 01
   2. 05
   3. 10
   4. Unlimited<br><br>
2. **Which is NOT an available option while configuring an ERP Cloud adapter to use in an Oracle Integration Cloud (OIC) integration?**
   1. Extract bulk data from ERP Cloud
   2. Upload files to UCM
   3. Invoke CRUD operation on ERP Cloud REST API
   4. Enabte catlback<br><br>
3. **Which metadata formats are supported by the adapter when configuring Oracle Integration Cloud (OIC) connections?**
   1. Open API, RAML, Swagger
   2. Swagger, WADL, RAML
   3. Open API, WADL, RAML
   4. Swagger, RAML, WADL<br><br>
4. **Which is NOT an advantage of using Oracle Integration Cloud (OIC) for creating application integrations?**
   1. Public/Private Cloud portability
   2. Auto-association of Oracle SaaS applications
   3. Data mapping recommendations
   4. User choice of IDE for development
   5. Prebuilt integrations<br><br>
5. **Oracle Integration Cloud (OIC) service is available in two editions, Standard and Enterprise. Which two OIC Enterprise Edition capabilities are ALSO available in OIC Standard Edition?**
   1. Integration Insight
   2. Visual Builder
   3. Process Applications
   4. File Server
   5. Enterprise application adapters (such as EBS, 3DE, SAP, and Siebel)
   6. B2B Trading Partner agreements<br><br>
6. **Your team is responsible for an OIC package that contains five integrations. Currently, three of these integrations are active while the other two are inactive. Which statement is valid if you were to replace a connection used in this package?**
   1. You can only replace the connections used by the three active integrations.
   2. You cannot replace connections unless atl integrations in the package are in an active state.
   3. You can only replace the connections used by the two inactive integrations.
   4. You cannot replace connections unless all integrations in the package are in an inactive state.<br><br>
7. **Your organization has a number of active integrations in Oracle Integration Cloud (OIC). Your advice is sought on the consequences of deactivating integration instances. Which statement concerning integration deactivation is NOT valid?**
   1. All existing history, monitoring, and runtime data will be lost.
   2. You can choose to retain the event subscription, where events are resent if the integration is reactivated again within six hours.
   3. Processing of any new messages will be immediately stopped.
   4. You will not be able to observe any failed instances occurring after the deactivation request.<br><br>
8. **You have a use case that requires a large data extract, which is more than 10 MB, to be processed within an Oracle Integration Cloud (OIC) integration. Which are three valid options?**
   1. Retrieve the file by invoking a SOAP API, which sends base64 encoded data within the SOAP body, and then decode the data and make it available for processing using a Stage File action.
   2. Retrieve the file by invoking a SOAP API, which sends the document as an MTOM attachment, and make it available for processing using a Stage File action.
   3. Retrieve the file from an external endpoint using APIS that support application/blob as content type, and make it available for processing using a Stage File action.
   4. Send the file as a multipart attachment to an OIC integration using a REST trigger, and make it available for processing using a Stage File action.
   5. Upload the file to the OIC File Server, and then use an FTP Adapter Download File operation, which makes it available for processing using a Stage File action.<br><br>
9. **One of your downstream applications is becoming overwhelmed with too many individual synchronous invocations from your current Oracle Integration Cloud (OIC) integration. It is recommended that you redesign the integration to take advantage of the batch processing capabilities of the application. Which approach is a valid OIC design best practice that Will provide the best solution to mitigate this issue?**
   1.  Create a custom batch call function, register the function as a library in your OIC environment, then use the Javascript action to invoke the application.
   2.  Throttle the individual synchronous calls by adding a wait activity prior to each invocation to the application within the loop.
   3.  Use the Append option in the Write File operation of the stage File action within a loop to create a single batch file to be sent to the application.
   4.  Reactivate the integration and use the disable tracing and message tracking option which will optimize performance for each invocation to the application.<br><br>
10. **You are implementing a synchronous Oracle Integration Cloud (OIC) integration flow that processes file records within a while loop action. At the end of each loop, you want to delay processing of the next record for a certain period of time. Which is a valid consideration when using the wait action?**
    1.  The wait action cannot be used in a synchronous flow.
    2.  The Wait action can only be positioned as the last action in the loop.
    3.  The minimum wait time cannot be less than five seconds when configuring a wait action in any integration flow. 
    4.  The maximum wait time cannot exceed two minutes when configuring a wait action in a synchronous flow.<br><br>
11. **Which operation is NOT supported by an Oracle Integration Cloud (OIC) Connection resource configured with the FTP Adapter in the Invoke role?**
    1.  WriteFi1e
    2.  Delete File
    3.  Download File
    4.  Last File
    5.  Read File
    6.  Read File in Segments<br><br>
12. **Which set of operations are supported by the Oracle Integration Cloud (OIC) File Adapter?**
    1.  read, write, list, download
    2.  read, write, list, move
    3.  read, write, list
    4.  read, write
    5.  read, write, list, download, move, delete<br><br>
13. **You need to create an Oracle Integration Cloud (OIC) integration that processes many records individually that are contained within a large file. You have been advised to use an implementation approach that uses the Download File operation of an FTP adapter in conjunction with the Stage File action Read File in Segments operation to mitigate issues with memory consumption. </br> When using this approach, which is a valid consideration regarding the use ofthe Read File in Segments operation?**
    1.  The Read File in Segments operation allows you to process the segments sequentially or in parallel.
    2.  Segment sizes default to 50 records but can be configured to any other segment size.
    3.  You must provide the actual filename because file references cannot be processed by the Read File in Segments operation.
    4.  You need to explicitly configure a Scope action for this operation if you want to add additional actions during the processing of each segment.<br><br>
14. **When defining the frequency for scheduled orchestration Style integration runs, you can choose either Basic or the Advanced option. Which expression format is used for defining advanced scheduled runs?**
    1.  iCal
    2.  Groovy
    3.  cron
    4.  YAML<br><br>
15. **As an Oracle Integration Cloud (OIC) specialist, you are tasked with implementing a scheduled integration between two enterprise applications. The client requires that the integration be run every weekday at 3:00 PM to synchronize data between the systems. </br> Which advanced scheduling configuration expression Will you use?**
    1.  "FREQ=WEEKLY;BYDAY=MO-FR;BYHOUR=15"
    2.  "FREQ=DAILY;BYDAY!=SA,SU;BYHOUR=15"
    3.  "FREQ=DAILY;BYDAY=MO-FR;BYHOUR=15"
    4.  "FREQ=WEEKLY;BYDAY=MO,TU,WE,TH,FR;BYHOUR=15"<br><br>
16. **The Oracle Integration Cloud (OIC) integration design editor provides a data mapper UI tool that is available for Map actions. Which statements are TRUE regarding the use ofthe Mapper tool? Select TWO**
    1.  You cannot drag and drop an XPath fitnction activity directly to a target node element.
    2.  You can drag and drop a source data element to multiple target node elements.
    3.  You cannot drag and drop a source data element to a target node element that is already mapped.
    4.  You cannot drag and drop an XSLT flow control statement directly to a target node element.<br><br>
17. **There are use cases in which you need to perform an advanced XSLT task that you cannot perform in the Oracle Integration Cloud (OIC) data mapper. To perform the advanced mapping tasks, you decide to use an external XSLT mapper and then import the .XSI file back to your integration. Which is NOT a valid consideration when handling this use case?**
    1.  The exported archive must be imported into an Oracle Service Bus project in JDeveloper.
    2.  The exprted archive file can include a map file that is largely complete in content or a map file that is empty of content.
    3.  Once the advanced mapping is complete, you must import the entire integration that contains the updated.xsl files.
    4.  You must export the entire integration that contains one or more .xsl files.<br><br>
18. **CSV-formatted data has been extracted from ERP Cloud by invoking a web service using the SOAP Adapter, and the data extract has been returned as an MTOM attachment. You now need to send this CSV file to an external REST API that supports accepting this content as a Base64 encoded string. Which XPath mapper function should be used to map the SOAP MTOM attachment to the Base64 element present in the target REST API payload?**
    1.  decodeBase64ToReference
    2.  encodeReferenceToBase64
    3.  decodeBase64
    4.  encodeBase64<br><br>
19. **Which action CANNOT be performed from the Oracle Integration Cloud (OIC) Monitoring Dashboard?**
    1.  View Connectivity Agent Group Status
    2.  Download Design-time Audit Records
    3.  View Design-time Metrics
    4.  Download OIC Lookups
    5.  View Current Email Count<br><br>
20. **You are tasked with creating an Oracle Integration Cloud (OIC) integration flow that supports a B2B exchange. When configuring the B2B action there are several capabilities as well as limitations. Which statement is NOT valid concerning OIC B2B capabilities?**
    1.  You can customize standard Electronic Data Interchange (EDI) documents by adding new schema constructs or by editing existing constructs.
    2.  It is mandatory to preform validations on EDI documents for inbound translations; however, for outbound translations it is optional.
    3.  A previously created Trading Partner Agrement is optional when configuring the inbound or outbound translation.<br><br>
21. **Which statement about Oracle Integration Cloud (OIC) is NOT valid?**
    1.  OIC Lookups are based on a static definition, meaning you create and populate them during design time, and cannot be changed by runtime activities.
    2.  An application-driven integration can contain one or more trigger (source) connections for requests sent to OIC and one or more invoke (target) connections for requests sent from OIC.
    3.  Using the connectivity agent, you can create hybrid integrations and exchange messages between applications in private or on-premises networks and OIC.
    4.  When you open the mapper for a request or response message in an integration, the data structures are automatically populated with the information pulled from the source and target connections.<br><br>
22. **Which are types of certificates in Oracle Infrastructure Cloud (OIC) that can be imported from the Certificates page under Settings? Select THREE**
    1.  Trust Certificate
    2.  Identity Certificate
    3.  Multi Domain SSL Certificate
    4.  Message Protection Certificate
    5.  Unified Communications Certificate<br><br>
23. **You have an Oracle Integration Cloud (OIC) synchronous integration flow that updates external systems with several invocations. However, several ofyour OIC integration clients are reporting that they are experiencing timeouts waiting for the response confirmation from this processing. Which is a legitimate stratey to mitigate this issue?**
    1.  Change the implementation logic to invoke multiple fine-grained external API calls within a single loop.
    2.  Change the design implementation strategy to an asynchronous flow that provides a separate notification to clients when the processing is complete.
    3.  Increase the blocking timeout within the OIC integration settings to allow for extended time.<br><br>
24. **Which are valid considerations when leveraging the Oracle Integration Cloud (OIC) connectivity agent for high availability on-premise environments? SelectTWO.**
    1.  Each host on which the agent is installed must be configured on separate subnets and assigned to the same OIC Agent group.
    2.  You cannot have more than two Agent instances per Agent group. Attempting to include a third Agent instance in the same group during installation results in an error.
    3.  You should install the connectivity agents on the same host as the target application, and then specify different Agent group identifiers for each Agent during its installation.
    4.  File Adapter is not supported in high availability environments. When using File Adapter and if some groups have multiple instances, use a dedicated Agent group (with one agent only).
    5.  You need to have the OIC Service Deployer role permissions to download and install the OIC on- premise connectivity agent.<br><br>
25. **You are designing an OIC integration that files in a shared file system located within your on-premises data center. You have decided to leverage various Stage File Action operations within the integration flow in conjunction with an on-premises OIC connectivity agent. </br> Which statement is not valid concerning file operation capabilities with regard to restrictions on using Stage File Action operations with the file and attachment features ofthe Connectivity agent?**
    1.  Files uploaded through the Connectivity agent are not available with the zip File operation.
    2.  Files uploaded through the Connectivity agent can only be read with a file reference, with regard to both the Read Entire File and Read File in Segments operations.
    3.  Files uploaded through the Connectivity agent are not available with the List File operation.
    4.  Files uploaded through the Connectivity agent cannot be unzipped using a file reference.<br><br>
26. **Which are TRUE about WSDL? </br> SelectTWO.**
    1.  It stands for "Web Service Description Language" and is a document written in Object Notation.
    2.  It uses XML to define the service layer document which consists of origin of the web service, headers, port types, request and response data.
    3.  It uses XML or JSON to define the service layer document which consists oforigin ofthe web service, headers, port types, request and response
    4.  It is a wrapper for a SOAP message.
    5.  It stands for 'Web Service Description Language" and is a document written in XML.<br><br>
27. **Which statements are TRUE concerning the implementation ofan API-first stratew? </br> Select TWO.**
    1.  You define the API definition/contract first any work on its implementation or any applications that use it, allowing teams to work in parallel.
    2.  The general assumption is that SOAP/WSDL are key specifications for defining the API.
    3.  The code to execute business logic needs to exist and be exposed as an API first before you build a strategy around it.
    4.  The API needs to be developed before any UI or new business logic is created.<br><br>
28. **You are working on an integration within Oracle Integration Cloud (OIC), which includes several connections to external systems. As part of your development work, you need to implement global fault handling to ensure that any unexpected errors are caught and handled correctly. Which approach should you use to add global fault handling within your integration?**
    1.  Create a separate integration solely for the purpose of handling faults and configure your main integration to call it when necessary.
    2.  Use the Raise Fault action within your integration flow to generate custom faults and handle them accordingly.
    3.  Add a Try-Catch action to your integration flow and configure it to catch and handle any faults.
    4.  Open the Global Fault Handler page on the integration canvas and add actions as needed to handle unexpected faults.<br><br>
29. **In Oracle Integration Cloud (OIC), you are designing an integration flow that processes customer orders. You need to enforce a specific validation rule that if an order contains more than 10 items, it must be rejected with an appropriate error message. </br> Which is the most appropriate approach for leveraging the Throw New Fault action in your integration to achieve this requirement?**
    1.  Implement the validation rule using a Switch action, and then use the Throw New Fault action within the default branch ifthe validation rule is not met.
    2.  Use the Throw New Fault action directly in the main flow, checking the order item count, and throwing the fault if the validation rule is not met.
    3.  Create a scope within the main flow, add the Throw New Fault action, and use an if-then branch to check the order item count, and throw the fault if the validation rule is not met.
    4.  Create a separate integration flow to handle the validation, and then call it using the Throw New Fault action if the order item count exceeds the limit.<br><br>
30. **You are designing a new integration in OIC that needs to expose a RESTful interface trigger for client applications. Which is a valid consideration when choosing request and response options using the REST Adapter Endpoint Configuration Wizard?**
    1.  If you select a PUT or POST action (HTTP method), you must define a JSON response payload format.
    2.  File attachments can be accepted as a request option for the Trigger interface, but you cannot include attachments as a response to the client.
    3.  Both standard and custom HTTP headers can be defined for both the request and the response.
    4.  Although you can define both query and template parameters, only template parameters are available for mapping in the mapper because query parameters are considered optional.<br><br>
31. **You are tasked with creating a new integration in Oracle Integration Cloud (OIC) that will be exposed to clients as a SOAP web service. This integration will also invoke an external SOAP web service as part of the orchestration flow logic. Therefore, you will need to define two Connection resources (one for the Trigger and one for an Invoke action). Which is statement is VALID regarding the creation of these SOAP adapter connections?**
    1.  You must explicitly specify the target server TLS version for the external web service outbound Invoke connection configuration.
    2.  The SAML and OAuth security policies are available options for creating the inbound Trigger connection.
    3.  The WSDL URL property value can be defined by uploading a file for either the inbound Trigger connection or the outbound Invoke connection configuration.<br><br>
32. **A company has using Oracle Integration Cloud (OIC) to integrate its business applications, such as Oracle HCM Cloud, Oracle ERP Cloud, and Salesforce. However, they are planning to migrate some oftheir integration workloads from their current OIC instance to a new instance in a different region to comply with data sovereignty regulations. Which statement is true regarding the exporting and importing of integrations?**
    1.  You can import a package containing activated integrations.
    2.  You can export an integration either as a separate file (IAR) or bundled in a package (PAR) and it will still contain the connection resources.
    3.  You cannot import an integration if it already exists with the same identifier and version.
    4.  To change an integration identifier or version,you can manually edit the exported integration (IAR) file before importing it into another instance.<br><br>
33. **Oracle Integration Cloud (OIC) integrations can be exported so that later they can be imported into another OIC instance environment. Which statement is NOT true about the import and export of OIC integrations?**
    1.  Imported integrations cannot be immediately activated if their dependent connection resources are not already present in the target OIC environment.
    2.  Imported integrations can be reconfigured to use different connection resources by using the OIC REST API.
    3.  Exported integrations include all their dependent connection resource information except URLS and credentials.
    4.  Integrations must be exported as a package if you want to import them into another OIC environment.<br><br>
34. **You are an Oracle Integration Cloud (OIC) specialist working on a project to integrate two systems using OIC. During testing, you notice that the integration instance fails to execute and returns an error message. Which step would you take first to troubleshoot the issue?**
    1.  Check the instancelogs for specific error messages and details.
    2.  Contact Oracle Support and wait for a respnse.
    3.  Immediately restart the integration instance.
    4.  Increase the number of instances to handle the error.<br><br>
35. **You need to create a scheduled orchestration integration that is based on an existing app-driven orchestration using the same display name. Which statement is valid for this use case?**
    1.  You can clone the existing integration and specify it to use the scheduled orchestration pattern.
    2.  You can create the new integration as a different major version ofthe existing one.
    3.  You cannot create another integration that uses the same name.
    4.  You can create the new integration by using the same display name but with a different identifier.<br><br>
36. **GlobalTech Corporation uses Oracle Integration Cloud (OIC) to synchronize data between their CRM and ERP systems. They currently have a scheduled integration that runs nightly at 3 AM. With the implementation of a new CRM system that supports real-time data synchronization, GlobalTech wants to update their ERP system immediately after any data changes in the CRM. To achieve this, they need to convert their scheduled integration to an app-driven integration, allowing the CRM system to trigger the integration upon data changes. <br> When implementing this conversion, which of these considerations is NOT valid?**
    1.  Any existing scheduled parameters will be automatically converted to integration properties.
    2.  You cannot convert a scheduled integration with assignments that have the fault data type.
    3.  You must choose an existing REST Adapter trigger connection resource.
    4.  You cannot convert a scheduled integration to a REST Adapter-triggered integration with multiple verbs.<br><br>
37. **Which adapter should be used for a configured connection from an orchestrated integration to the enabled File Server associated within the same OIC environment?**
    1.  Local Adapter
    2.  FTP Adapter
    3.  File Adapter
    4.  REST Adapter<br><br>
38. **Which type of certificate requires the uploading of a keystore (.jks) file in Oracle Integration Cloud to facilitate two- way SSL communication with external services?**
    1.  Message Protection Certificate
    2.  Identity Certificate
    3.  Unified Communications Certificate
    4.  Multi Certificate<br><br>
39. **When creating a new Oracle Integration Cloud (OIC) Connection resource, there are several steps that must be done before it is fully configured and can be used in an integration flow. Which task is NOT required in order to transition a new Connection resource from the Draft to the Configured state?**
    1.  Configure the Security properties
    2.  Specify the corresponding Lookup
    3.  Execute a successful test ofthe Connection
    4.  SFcify an adapter type
    5.  SFcify the Connection role
    6.  Configure the Connection properties<br><br>
40. **In an Oracle Integration Cloud (OIC) project, you are asked to leverage a custom JavaScript library function to be used within an application-driven orchestration integration flow. Which set ofsteps should you follow to correctly use the JavaScript librarywithin your OIC integration?**
    1.  Copy and paste the entire JavaScript function code into a new JavaScript stage within the integration flow, and then map the inbound and outbound data elements in the corresponding map action.
    2.  Import the JavaScript library file into your OIC instance's database schema, and then use a Local Invoke action to call the library function.
    3.  Import the JavaScript library file to the OIC Console, and then use the JavaScript action within the integration flow to reference the library function.
    4.  Use the Function Call action within the integration flow to reference an external URL that is hosting the JavaScript library function.<br><br>
41. **Your team is using a JavaScript library function within an Oracle Integration Cloud (OIC) integration flow. Because of business requirements, one ofthe functions needs to be updated with additional code to incorporate new logic. <br> Which consideration regarding JavaScript library functions is NOT valid?**
    1.  Active integrations using a function that has been updated must be reactivated.
    2.  The JavaScript action has a timeout threshold of 60 seconds.
    3.  JavaScript frnctions are not allowed to make outbound calls to external sewices.
    4.  Network, disk, or thread access is not supported from within a JavaScript function.<br><br>
42. **You can recover unsaved changes in an Oracle Integration Cloud (OIC) integration that crashes during design time because of a browser crash, loss of network connectivity, or a server going down. <br> Which statement is NOT true about the unsaved changes feature in OIC?**
    1.  A backup copy is created after each completed task, therefore there is no time limit to logging back in and recovering your changes.
    2.  Changes made while working inside Data Mapper cannot be recovered.
    3.  A user with the serviceAdministrator role can recover all unsaved changes.
    4.  A user with the serviceAdministrator role can unlock an integration that has unsaved changes.
    5.  Changes made while editing a Connections page cannot be recovered.<br><br>
43. **Which Oracle Integration Cloud (OIC) setvice role does NOT have permission to run an OIC integration flow?**
    1.  Servicelnvoker
    2.  ServiceAdministrator
    3.  ServiceDeveloper
    4.  ServiceUser<br><br>
44. **You can group one or more Oracle Integration Cloud (OIC) integrations into a single structure called a package. <br> Which statement is NOT true about OIC packages?**
    1.  New packages can created by clicking the Create button on the Packages page in the OIC console.
    2.  You can import packages directly from the Oracle Marketplace.
    3.  Integrations do not need to part of a package.
    4.  Packages enable you to easily import and export a group of integrations to and from OIC.
    5.  All packages must include at least one integration.
    6.  Packages cannot be locked to deny Other users access to your integrations.<br><br>
45. **Which Oracle Integration Cloud (OIC) XPath function can be used to retrieve data from an OIC Lookup within the Data Mapper tool?**
    1.  get-content-as-string
    2.  lookupValue
    3.  get-value-from-lookup
    4.  getLookup<br><br>
46. **You are developing an integration in Oracle Integration Cloud (OIC) to integrate two systems and wish to use an OIC Lookup. The goal is to transform customer status codes between the two systems. Which set ofsteps are essential for correctly utilizing the Lookup?**
    1.  Define a Lookup table containing the customer status code mappings, and then use the Invoke action to call a web service for the transformation.
    2.  Design a custom script to perform the transformation, and then use the Lookup function within a Map action to reference the script and transform the customer status codes.
    3.  Create a connection between the two systems, then use a SQL query to access the Lookup table directly. and map the customer Status codes.
    4.  Create a Lookup table with the mappings of customer status codes, and then use the Lookup function within a Map action to reference the table and perform the transformation.<br><br>
47. **You have created a Scheduled integration in Oracle Integration Cloud (OIC), which uses schedule parameters named startDate and endDate to determine the date range for a data synchronization process. The default values for these parameters are set to the previous and current dates. However, you now want to schedule a run of the instance with different start and end dates. </br> What should you do to achieve this?**
    1.  Modify the parameter value in the instance's integration proFrties and the instance.
    2.  Modify the parameter value in the integration code and redeploy the integration.
    3.  Override the parameter value when scheduling the integration instance.
    4.  Create a new version of the integration by modifing the parameter value, and then deploy the new scheduled integration version.<br><br>
48. **Which statement is NOT true Schedule Parameters in Oracle Integration Cloud (OIC) integration flows?**
    1.  Wates to Schedule Parameter values can be made manually when starting a schedule.
    2.  Updates to Schedule Parameter values can be made manually submitting an ad hoc request.
    3.  Schedule Parameters are always visible as an additional data source in the Sources section of the mappers and expression editors within the integration.
    4.  Updates to Schedule Parameter values made dynamically in an Assign action will not persist on to the next instance run of the integration.
49. **You are tasked with testing an integration that uses a REST trigger in Oracle Integration Cloud (OIC). You have successfully configured the REST Adapter, and now you want to verify that the integration frnctions correctly. <br> What should you do to test the integration?**
    1.  Manually trigger the integration by sending an email to a specified email address with the required REST parameters.
    2.  Export the integration as a .jar file and run it in a local development environment.
    3.  Perform a SQL query on the associated database to ensure that the expected data is present.
    4.  Use the "Test" button in the integration designer to create a request, validate the response, and review the execution logs.<br><br>
50. **In Oracle Integration Cloud (OIC), you are working on an integration that uses a REST trigger, which Will require authentication. You need to ensure that only authorized clients can access the integration. <br> Which configuration should you apply**
    1.  Encryrpt the payload using a custom encryption algorithm and provide the decryption key to authorized clients.
    2.  Enable Cross-Origin Resource Sharing (CORS) and set an API key in the REST Adapter configuration.
    3.  Set up an IP whitelist in the OIC instance, allowing only specific IP addresses to access the integration.
    4.  Configure the REST Adapter with a Basic Authentication or OAuth 2.0 security policy and provide the required credentials.<br><br>
51. **Your design of an asynchronous Oracle Integration Cloud (OIC) integration flow includes the requirement for additional processing logic that is conditionally based on the results returned to the integration instance from earlier external service invocations. You decide to leverage the switch action to facilitate this implementation. <br> Which is a valid consideration concerning the configuration and capabilities of the switch action?**
    1.  Data objects returned from actions within a branch of a Switch action are not visible in the main flow of the integration after the switch action.
    2.  The Switch action must include an otherwise branch.
    3.  Nested Switch actions are not supported and, therefore, you may need to create more complex conditional expressions, if necessary.<br><br>
52. **Once they have been configured, which actions are allowed to be repositioned to another location within the design canvas ofan orchestration Style integration flow? Select THREE.**
    1.  Stage File Action using a Write File operation
    2.  For Each Loop Action
    3.  Switch Action
    4.  JavaScript Call Action
    5.  Stage File Action using a Read File operation
    6.  Stage File Action using a Read File in Segments operation<br><br>
53. **As an integration developer, you are creating an integration in Oracle Integration Cloud (OIC) to transform a payload with multiple orders. You need to configure the for-each action to loop through each order and process them individually. How do you correctly configure for the for-each action to support this scenario?**
    1.  Select the Group By option and group the orders by the order number.
    2.  Select the Sequential Processing option and set the batch size to the number of orders.
    3.  Select the Parallel Processing option and set the number of threads to the number of orders.
    4.  Select the Repeating Element field and map the source element that contains the orders.
54. **Which is NOT a valid consideration when leveraging the Throw New Fault action in an integration flow?**
    1.  If the conditional expression for the skip condition is empty, the fault will never be thrown.
    2.  You are required to define a fault code when configuring the Throw New Fault action.
    3.  You can place the Throw New Fault action inside the Global Fault hander.
    4.  You can place the Throw New Fault action directly on the main flow path.
55. **You have a use case that requires the design of a synchronous Oracle Integration Cloud (OIC) integration flow that returns a custom business fault message to the client if processing fails due to an external runtime fault encountered during the integration instance execution. Which implementation strategy best satisfies this requirement?**
    1.  Implement a Scope fault handler to catch the runtime fault, and then use the Fault Return action providing mapped data for the custom fault.
    2.  Implement a Scope fault handler to catch the runtime fault, then allow the Global fault handler to automatically send the runtime fault to the Error Hospital.
    3.  Create a custom Scope fault handler to catch the runtime fault, and then use the Re-throw Fault action to send the fault to the Error Hospital.
    4.  Implement the Global fault handler to catch the runtime fault, and then use the Re-throw Fault action to send the custom fault to the client.

## Respuestas Examen de Prueba YT

1. `10`
2. `Invoke CRUD operation on ERP Cloud REST API`
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
24. `ii & iv`
25. `Files uploaded through the Connectivity agent cannot be unzipped using a file reference.`
26. `ii & v`
27. `i & iv`
28. `Open the Global Fault Handler page on the integration canvas and add actions as needed to handle unexpected faults.`
29. `Create a scope within the main flow, add the Throw New Fault action, and use an if-then branch to check the order item count, and throw the fault if the validation rule is not met.`
30. `Both standard and custom HTTP headers can be defined for both the request and the response.`
31. `The SAML and OAuth security policies are available options for creating the inbound Trigger connection.`
32. `You can export an integration either as a separate file (IAR) or bundled in a package (PAR) and it will still contain the connection resources.`
33. `Integrations must be exported as a package if you want to import them into another OIC environment.`
34. `Check the instancelogs for specific error messages and details.`
35. `You can create the new integration by using the same display name but with a different identifier.`
36. `Any existing scheduled parameters will be automatically converted to integration properties.`
37. `FTP Adapter`
38. `Identity Certificate`
39. `Specify the corresponding Lookup`
40. `Import the JavaScript library file to the OIC Console, and then use the JavaScript action within the integration flow to reference the library function.`
41. `The JavaScript action has a timeout threshold of 60 seconds.`
42. `A user with the serviceAdministrator role can recover all unsaved changes.`
43. `Servicelnvoker`
44. `New packages can created by clicking the Create button on the Packages page in the OIC console.`
45. `lookupValue`
46. `Create a Lookup table with the mappings of customer status codes, and then use the Lookup function within a Map action to reference the table and perform the transformation.`
47. `Override the parameter value when scheduling the integration instance.`
48. `Updates to Schedule Parameter values made dynamically in an Assign action will not persist on to the next instance run of the integration.`
49. `Use the "Test" button in the integration designer to create a request, validate the response, and review the execution logs.`
50. `Configure the REST Adapter with a Basic Authentication or OAuth 2.0 security policy and provide the required credentials.`
51. `Data objects returned from actions within a branch of a Switch action are not visible in the main flow of the integration after the switch action.`
52. `i, iv, v`
53. `Select the Repeating Element field and map the source element that contains the orders.`
54. `If the conditional expression for the skip condition is empty, the fault will never be thrown.`
55. `Implement a Scope fault handler to catch the runtime fault, and then use the Fault Return action providing mapped data for the custom fault.`

---

# [Parte 3](./Preguntas3.md)