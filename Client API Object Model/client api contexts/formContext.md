# Form Context :

- Form Context provides reference to the form or item on the form, such as, quick view control or a row in editable grid.

- Form context has two components, Data object and UI object.
- 

    - ## Data object :
        _Provides properties and methods to work with data on a form, including table data and data in bpf control._

        - ### atributes :
            - Collection of non-table data on the form.

        - ### entity :
            - Collection of all columns included(only those represented) on the form.
        
        - ### process :
            - Provides objects and methods to interact with bpf data on a form



    - ## UI object :
        _Provides methods to retrieve info about user interface, in addition to collections for several sub components of the form or grid._

        - ### formSelector :
            - Helps to determine the forms available for the current user.

            - Navigate method is used to close the current form and open a different one.

        - ### navigation :
            - Provides access to navigation items.

        - ### process :
            - Provides methods to interact with bpf control on a form.  