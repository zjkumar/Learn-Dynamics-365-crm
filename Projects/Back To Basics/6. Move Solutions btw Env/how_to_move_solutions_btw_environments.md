# First step is to create a solution

**_Lets create a new solution_**

- make.powerapps.com
- solutions
    - create new solution named "Contact Customizations"


**_add a column to the existing contact entity_**
- make.powerapps.com
- solutions
    - Navigate to Default Solution
        - Tables
            - Contact (create new column named "Vaccination Completed" with Yes/No data type with No as default)
            - Select Information form of the contact entity and add the above created field to the form.
        - Publish all customizations


**_add existing component to Contact Customizations solution_**
- Solutions
    - Contact Customizations
        - Add existing
            - Select Table 
                - Contact (include all objects)
                - Add
        - Publish All Customizations


# Export the solution
- Solutions
    - Contact Customizations
        - Export Solution _(Displays list of solutions on which "Contact Customizations" solution is dependent on, and warns that "import will fail if target env. doesn't have these list of solutions")_
        - Choose the unmanaged type
        - It will download a zip file.

- make.powerapps.com
- Choose the environment in which you want to import the solution
- Navigate to solutions
    - Import Solution
    - choose the zip file.
