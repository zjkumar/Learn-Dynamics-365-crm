# What is alternate keys in CRM ?
- Generally, a record of an entity is identified by its primary key.
- External applications may not be able to identify the record based on the guid.
- In these scenarios, it is ideal to create alternate keys.
- Alternate keys makes use of the natural attributes of the entity like email address, account number, etc and uniquely identifies the record.

_There are 2 ways to define the alternate keys:_
- **Customization tools :**
    - Navigate to the customizations
    - Navigate to the entity
    - select keys
    - New -> select attributes (which are deemed to be unique)
    - save.
    - This will create alternate keys for the entity based on the attributes to identify the record.

- **Programmatically :** 
    - Use the EntityKeyMetadata class to define the key attributes.
    - Use the CreateEntityKeyRequest message to create the key.

