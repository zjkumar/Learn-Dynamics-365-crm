# What interface we use a plugin to inherit CRM Services?

- To inherit CRM services, we use IPlugin Interface.
- It is available from Microsoft.Xrm.Sdk namespace.
- We need to install Microsoft.CrmSdk.CoreAssemblies to use this namespace
- IPlugin interface has a single method Execute which accepts a single parameter of data type IServiceProvider