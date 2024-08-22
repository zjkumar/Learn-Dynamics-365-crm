# Actions :

1. In Dynamics 365, many operations are tied to entities such as CRUD operations. For example, when you create a new Contact, the operation is directly tied to Contact Entity.

2. Actions allow you to define operations based on business requirements rather than being limited to entity operations.

3. For example, if you need to approve an Order, it involves multiple steps like :
    - Checking availability of inventory
    - Updating order status to "Approved"
    - Sending notification email to customer
    - Logging approval in a custom entity

4. Since workflows are tied to single entity, and when creating a workflow, you must choose only one entity, the workflow scope is restricted to single entity, which means you can either check availability of inventory (if you choose inventory entity when creating a workflow) or you can update order status (if you choose order entity when creating a workflow). 

5. Whereas with Actions, you can perform all the above steps to approve an order.

6. Actions allow you to create business logic that can be triggered by code or workflows.



**_Actions can be either:_**

- `Global (un-bound)` : Actions can be generic, they can apply to all the entites

- `Entity / Table (bound)` : Actions are applied to a particular entity.


**_Actions can be triggered from:_**

- Plugin
- workflow
- js
- web api
- power automate
- tooling connection (3rd party)
