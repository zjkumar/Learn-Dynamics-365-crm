# What is early binding and late binding ?
- These are two approaches to access and manipulate CRM data.

**Early binding :**
- It involves generating strongly typed classes based on CRM entity schema.

**Late binding :**
- It makes use of the generic _Entity_ class.


## Advantages :
- **Early Binding :**
    - It provides compile time checking
    - It provides intellisense support and provides code auto completion.
    - It makes development easier.

- **Late Binding :**
    - It doesn't require pre-generated classes.
    - It is more dynamic and flexible if the entity schema is unknown 


## Disadvantages :
- **Early Binding :**
    - Requires tools like CrmSvcUtil.exe
    - Requires generating classes every time the entity schema is updated.
    - less flexible than late binding

- **Late Binding :**
    - doesn't provide intellisense support.
    - Developers need to know the attribute names in before hand.
    - slows down the development process.
    - more error prone.


# When should we go for early binding and late binding ?

- If we have stable schema or predictable entity schema then we go for early binding.
- If data type is criticial then we go for early binding.
- If the schema changes frequently, then we go for late binding.

