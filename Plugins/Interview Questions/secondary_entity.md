# What is secondary entity ?

- Secondary Entity is used in relationship based operations.
- It provides additional context about the related entity to the plugin.
- It is used in Associate/Disassociate/merge based messages. or SetRelated/RemoveRelated messages.
- It can be accessed from (Entity)IPluginExecutionContext.InputParameters["RelatedEntities"].
- When we want to associate or relate a primary entity record with another entity record, or remove relation btw the same, then we use Secondary Entity.