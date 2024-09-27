1. create instant cloud flow -> Manually trigger a flow
2. initialize variable -> Name : plan, type : object, value : { "name": "kumar","plantype": null, "connection": "landline" }
3. new step -> compose (data operation)
4. inputs -> fx -> coalesce(variables('plan')?['plantype'], false)
5. new step -> compose (data operation)
6. inputs -> fx -> coalesce(variables('plan')?['plantype'], 'standard')
7. save