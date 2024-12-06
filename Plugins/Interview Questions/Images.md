# What is pre image and post image ?

- Images are snapshots of entity's attributes before or after the database changes.
- It is used :
    - If we need a column value that isn't modified (unmodified column values are not carried by the message request)
    - If we need to know the column value before it is modified on the UI.

**Pre Image :**
    - It contains the snapshot of the existing attributes before committing changes to the database
    - It is not available in the pre operation of the create message type because, as we know it is a snapshot of existing attributes but the record is not yet created.
    - In all Update and delete message types and in pre operation and post operation, pre image is available.

**Post Image :**
    - It contains the snapshot of the attributes after committing changes to the database.
    - It is available in the post operation stage of message type create and update.
    - In all other message types of pre and post stages, it is not available. 
    - pre stage -> create, update, delete -> post image is not available because, as the definition says, it is snapshot of attributes after database changes, but pre stage means the database operation is not yet completed
    - post stage -> create, update -> (available)
    - post stage -> delete -> not available -> because delete message removes the record, and post image means snapshot of attributes after the database changes. After the modification of db, the record is deleted, so there is no post image.


**Accessing in the plugin code :**
    - We can access using Entity preLead = (Entity)context.PreEntityImages["PreImage1"]; if we defined multiple images
    - If we defined only a single image, then we can use context.GetPreImage()

**Considerations :**
    - If more attributes are defined, it may consume more resources.