1. make.powerapps.com
2. go to flows
3. create instant cloud flows
4. choose manually trigger a flow.
5. initialize variable 
    - Name : Uri
    - type : String
    - value : https://venkatasubbaraopolisetty.com/

6. New step -> Compose Action choose data operation
7. Inputs -> choose fx -> encodeUriComponent(variables('Uri')) -> this will encode the value in Uri variable.
8. save