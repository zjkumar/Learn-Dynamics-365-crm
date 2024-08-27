# Plugin :

A plug-in is custom business logic (code) that you can integrate with Dynamics 365 customer engagement/dataverse to modify or enhance the behavior of the platform.

**Scenarios :**
- Data manipulation before record is being saved.

- Validation before commiting the changes.

- Cancel an operation based on the validation.

- Immediate response to the user, if needed.

- Retrieve values/ take actions after operations, that has been completed.

- Triggers not available within workflow/Power Automate. 


**How to plugin business logic in the Dataverse?**

- Identify Primary Table (Target)

- Identify Trigger (Message)

- Identify Execution Order (Pre/Post)

- Identify data needed for the business logic/operation 


**Tools needed for plugin development :**

- Microsoft .Net Framework 4.6.2

- Microsoft Visual Studio

- Microsoft Dataverse/Dynamics 365 SDK (Plugin Registration Tool)


**How to write plugin ?**

Following are the high-level steps to write a plugin:

- Create a C# .Net Framework Class Library Project

- Install Microsoft.CrmSdk.CoreAssemblies nu-get package.

- Implement IPlugin interface of Microsoft.Xrm.Sdk

- Implement Execute method 

- Write Code to implement business logic

- Sign the project and build

- Register Plugin using PluginRegistrationTool (CRM SDK)