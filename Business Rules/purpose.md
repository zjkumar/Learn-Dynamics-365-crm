### Business Rules :

Business rules are used to define logic on forms without writing scripts.

With conditions and actions, we can achieve the following on the forms using Business Rules :

- Set Column values
- Clear column values
- Set column requirement levels
- Show/hide columns
- Enable/Disable columns
- Validate data and show error messages
- Show business recommendations based on business intelligence.


## Scope of Business Rules :

- ### Form:
    - The logic defined applies only to the selected form.

- ### All Forms:
    - The logic applies to all the forms of the entity.

- ### Entity:
    - If the scope is entity, then the logic runs on the server side.
    - Many other users updates data not using forms, like they update the fields through web api, through other integration tools, etc
    - In these scenarios forms will not run.
    - So logic scope is set to entity, which means if any change is made to entity from any source, the logic applies.
