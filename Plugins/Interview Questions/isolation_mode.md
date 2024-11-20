# What are the different isolation modes of a plugin ?

**1. Sandbox (Isolated) Mode or Partial Trust Mode.**
- In Sandbox mode, the plug-in runs in a restricted environment with limited permissions. 
- This mode is designed to enhance security and stability by isolating the plug-in from the main Dynamics 365 environment. 
- It is controlled by Microsoft system and users don't have access to the resources.
- If any error, it is isolated from the dynamics 365, preventing the error from affecting other parts of D365.
- Online D365 must use this mode.

**2. None (Full Trust) Mode**
- In None mode, the plug-in runs with full trust and has unrestricted access to the system resources. 
- This mode is less secure but allows the plug-in to perform more complex operations. 
- Errors encountered in None mode can potentially affect the main system, as there is no isolation between the plug-in and the Dynamics 365 environment.
- Online d 365 cannot use none mode. Only on-premise can use none mode.