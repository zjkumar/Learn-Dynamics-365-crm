# What happens when we set the execution order of Plugin to '0'?

- By default the execution order of plugin is 1.
- If we set it to 0, for that particular message, this plugin runs before any other plugins and workflows.
- We can set it when registering a step in the setting "Execution order"
- If the plugin is async, then this plugin is the first among other plugins (not among all async operations) to get executed for that particular message.   