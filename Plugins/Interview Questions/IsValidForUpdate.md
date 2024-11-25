# Why the field IsValidForUpdate used for from plugin perspective?

- **Validation :**
    - IsValidForUpdate is used to check if a particular field is eligible to modify.
    - It reduces errors and ensures that only permissible fields are modified.

- **Avoid Exceptions :**
    - It avoids any run time exceptions that occur when trying to update read only or restricted fields.