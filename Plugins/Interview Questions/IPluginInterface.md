# What interface we use a plugin to inherit CRM Services?

- To inherit CRM services, we use IPlugin Interface.
- It is available from Microsoft.Xrm.Sdk namespace.
- We need to install Microsoft.CrmSdk.CoreAssemblies to use this namespace
- IPlugin interface has a single method Execute which accepts a single parameter of data type IServiceProvider
- It contains different services like ITracingService which is used to trace the logs to the CRM, IPluginExecutionContext which contains the business data, entity name, message name, Input Output parameters, shared variables, pre image, post image, depth, target, etc. IPluginExecutionContext defines the execution context of the plugin with which we can perform operations on the business data.
- IPlugin interface contains IOrganizationServiceFactory where we can get IOrganizationService which is used to perform CRUD operations on the database.
- 