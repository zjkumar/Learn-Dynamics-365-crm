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

## Example Code
_Here’s an example of how to create an alternate key programmatically:_

csharp
EntityKeyMetadata keyMetadata = new EntityKeyMetadata
{
    LogicalName = "account",
    DisplayName = new Label("Account Key", 1033),
    KeyAttributes = new string[] { "accountnumber" }
};

CreateEntityKeyRequest createKeyRequest = new CreateEntityKeyRequest
{
    EntityKeyMetadata = keyMetadata
};

service.Execute(createKeyRequest);


**Use Cases :**
- Data Integration: When integrating Dynamics 365 with external systems that use natural keys.

- Data Migration: During data migration projects to ensure records are uniquely identified.

- Data Quality: To enforce data quality by preventing duplicate records.

**Constraints :**
- Valid Attribute Types: Only certain attribute types can be used in alternate keys, such as string, integer, and decimal.

- Field-Level Security: Attributes with field-level security cannot be used in alternate keys.

- Logical and Inherited Attributes: Most logical and inherited attributes cannot be used in alternate keys.

**Summary :**
Alternate keys in Dynamics 365 CRM provide a powerful way to uniquely identify records using attributes other than the primary key. They are particularly useful for data integration, migration, and ensuring data quality. By understanding how to create and use alternate keys, you can enhance the performance and integrity of your CRM data.

