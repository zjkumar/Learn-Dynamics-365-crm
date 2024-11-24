# Can we configure our own connection string and credential inside the plugins?

**Connection String :**
- It is a string containing key info to connect to a data source.
- It contains info like username, password, data source url, connection type, etc.
- It allows you to establish a connection with the CRM.

**_Yes, it is possible to configure our own connection string._**
**_But it is not recommended to directly hardcode in our plugins_**
**_We use secure configuration from the plugin registration tool to pass the connection string for more security_**