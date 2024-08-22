# Workflows :
-  Workflow in Dynamics 365 CRM is a series of automated steps or actions that are executed sequentially to perform a specific business process.

- Workflows automate business processes without user interface.

- Automated workflows reduces manual tasks, saving you time and money

_Each workflow process is associated with a single entity._ 

### Considerations when configuring workflows:

- When to start a workflow (when to trigger) ?

- Should they run as real-time or background ?

- What actions should they perform ?

- Under what conditions should actions be performed ?


The decision of using a background or real-time workflow depends mainly on:

- Urgency of the action.
- Impact on user experience.
- Need for immediate feedback vs. allowing the system to handle the task asynchronously.

_Even if both workflows appear similar because they are based on time conditions, the difference in urgency and system interaction determines which one to use._


### Workflow Job Retention :

- It defines if you want to save the job or delete the job after succuessful execution of a workflow.

- Note that, if any error arise, it will keep the logs and the job session in the process session



### Considerations to use Workflows :

- They do not trigger in offline mode.

- They do not trigger on Pre-operation, always trigger in Post-operation.

- The triggering events are limited to create/update/delete/assign/state change, which is a disadvantage when you have custom message-based actions.

- OOB workflows cannot retrieve child records and perform any operation. You need custom workflow plugins to achieve it.

- Only 4 nested if conditions are allowed.


## Converting between real-time and background workflows :

- You can change a real-time workflow into a background workflow by choosing Convert to a background workflow on the toolbar.

- You can change a background workflow into a real-time workflow by choosing Convert to a real-time workflow on the toolbar. If the background workflow uses a wait conditions it will become invalid and you won’t be able to activate it until you remove the wait condition.