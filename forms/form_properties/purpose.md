***It has 4 tabs.***
***events, display,  parameters, non-event dependencies.***

### 1. Events : 
**You can manage whether javascript libraries should be available for the current form and choose if you want to run them when form loads or saves.**

### 2. Display : 
**You can choose the name for your current form to distinguish identify the form and describe how the current form, and how it is different from other forms**

### 3. Parameters :
**Forms can be opened with code using URL. These URLs may contain query parameters. And for security reasons, you don't want to accept all the parameters. So you can add which query parameters are acceptable.**

### Prerequisite Understanding :-
> You can create ribbon buttons for your business specific needs, like a custom action that updates the status of a record when a ribbon button is clicked, etc. Understand that when these are clicked, it runs some scripts which do not have access to form context or execution context because these are buttons on command bar. Understand that these buttons requires access to some fields from an entity.

> Also you may have some scripts running in the background, for example : A script that runs every night to update the “Last Contacted” date for all leads. From this example, understand that it requires access to specific fields in the Leads entity.

> From above, understand that there can be scripts that are not configured with form related event handlers.

### 4. Non-Event Dependencies : 
**When non form related scripts run, they depend on some fields. From the above example, the script that run every night, might depend on fields like, lead title, lead email, etc. These are dependent fields. Now you don't want to accidentally remove these fields, or customize it because these scripts depends on them. So you register these fields as dependent fields(script depends on these fields) in the Non-Event Dependencies tab.**