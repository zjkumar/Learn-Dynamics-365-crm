# Can we pass data between two Plugins? or what is shared variables ?

- We can pass data between two plugins using shared variables.
- Shared variables are a collection of key value pairs, available in the IPluginExecutionContext.
- Developers can share variables between different steps if the message and entity are same.

**Advantages :**
- It allows us to pass values from pre event to post event of a plugin of same message and entity.
- It is possible to read/write into shared variables.
- Certain data validations required in post event can be achieved by passing them from pre event.

**Disadvantages :**
- Cannot share variable of different steps with different message or entity.
- Need to use ParentContext.SharedVariables collection if data is passed from stage 10 and needed to access in stage 20 or stage 40 of message type create or update or delete.
