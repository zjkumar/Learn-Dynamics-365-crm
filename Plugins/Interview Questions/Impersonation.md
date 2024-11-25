# Does Impersonation work for Offline Plugins?

- **Impersonation :**
    - It means elevating the users permissions to perform business logic
    - It is useful when the current user doesn't have required permissions to execute a business logic.
    - In such scenario, we elevate the current user's permission and execute the business logic.
    - It can be done in two ways:
    - ***At plugin registration: ***
        - When registering a step on plugin registration tool, we can select a user with higher permission from the "Run in User's Context" option
    - ***During plugin execution: ***
        - We can override the user specified at "Run in User's Context" by setting the IOrganizationServiceFactory.CreateOrganizationService method with the userId parameter.
        - We must know the userId in before hand or we can retrieve the userId from the Users record in the code.
    
    - ***_Note that the user who has higher powers to execute the business logic must have the privilige 'prvActOnBehalfOfAnotherUser'_***
