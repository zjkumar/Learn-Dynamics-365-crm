# Difference between Secure & Unsecured Config?

- Secure and Unsecure config is used to pass the configuration data to the plugins without hardcoding them.
- We can pass the config data when registering a step.
- We can access the data from the constructor method of the plugin.

- **Unsecure Config :**
    - It is suitable to pass non sensitive data where confidentiality doesn't matter.
    - It can be viewed by any user who have access to the plugin registration tool.
    - It is migrated from one env to other as part of the solution.

- **Secure Config :**
    - It is suitable to pass sensitive data.
    - It can be viewed only by CRM admins
    - It cannot be migrated.