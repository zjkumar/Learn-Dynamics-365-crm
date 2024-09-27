1. make.powerapps.com
2. create instant cloud flow -> choose "Manually trigger a flow"
3. new step -> initialize variable -> Name : Date, type : String, value : fx -> utcNow()
4. new step -> Data operation -> inputs -> fx -> formatDateTime(variables('Date'), 'd')
5. save
6. test the flow