# Power Automate :

- Microsoft Power Automate is an online workflow service that helps you create automated workflows between apps and services to synchronize data, files, get notifications, etc.

- Power Automate primarily operates asynchronously, meaning it runs tasks in the background without requiring immediate completion before moving on to the next task.


**_Major categories of Power Automate_**

- **`Cloud Flows :`** 

    - **Automated :** 
        - Allows us to create an automation that is triggered by an event such as arrival of an email from a specific person, or a mention of your company in social media.

    - **Instant Flows :**
        - Allows us to start an automation with a click of a button. You can automate for repetitive tasks from your Desktop or Mobile devices. For example, instantly send a reminder to the team with a push of a button from your device.

    - **Scheduled Flows :**
        - Allows us to schedule an automation such as daily data upload to a database.

- **`Desktop Flows :`**
    - Desktop flows broaden the existing automation capabilities in Power Automate and enable you to automate all repretitive desktop processes.




## Understanding the scope when creating a flow :

_`Note that you are the owner of the flow when you create a flow`_

**Business Unit :** Actions are taken on rows owned by anyone in your business unit.

**Organization :** Actions are taken on rows owned by anyone withtin the current environment.

**Parent-Child Business Unit :** Actions are taken on rows owned by anyone in your business unit or your child business unit.

**User :** Actions are taken on rows owned by you.


**_Run as :_** Determines the permission and access rights the flow has when it runs.




# Notes/Tips :

- **Run as**:

    - if i set scope as organization, the flow will consider all the rows of an entity.

    - if i set run as to flow owner, the flow, when accessing the row, will check if i(flow owner) has permission to access or not and proceed as if he is running the flow.

    - if i set run as to modifying user, the flow, when accessing the row, will check if the user who caused the trigger due to hitting save button (he is modifying user because he caused the trigger) has permission to access or not and proceed as if he is running the flow.

    - if i set run as to row owner, the flow, when accessing the row, will check if owner of the row has permission to access or not and proceed as if he is running the flow.



- **Regarding :**

    - The “Regarding” option allows you to specify the context or subject of a record by linking it to another record.

    - This helps in understanding the relationship and relevance between different records.

    - Ippudu oka task (phone call) ni create chestunnav, so oka new task row create chestunnav. Ee task dheniki sambandhinchi create chestunnav ? Case ki sambandhincha, or lead ki sambandhincha or dheniki sambandhinchi (regarding which row you are creating the task)

    - regarding which row you are creating the current row is represent by "Regarding" 


## Advantages of Power Automate over Classic Workflows

- Power Automate supports Looping, workflow doesn't

- Power Automate supports Parallel branch, OOB connectors to external systems(trigger and perform actions in external services) whereas workflow doesn't.

- You can group steps to run in a transaction.

- Supports Run on a schedule whereas in workflow you need to write custom workflow (not possible in classic workflow)

- You can run analytics, provides Modern Designer and supports AI-assisted authoring, which are not available in classic workflows.



## Disadvantages of Power Automate over Classic workflow

- There is no access to pre-image of event data, it is possible in workflow.

- There is no wait conditions available on Power Automate, whereas it is available on workflows.

- 