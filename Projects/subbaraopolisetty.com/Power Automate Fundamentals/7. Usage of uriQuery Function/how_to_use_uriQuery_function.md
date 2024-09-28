1. Create Instant cloud flow -> choose -> Manually trigger a flow
2. new step -> compose data operation (name the step as 'Weburl with params') -> inputs -> youtube url containing params
3. new step -> compose data operation -> inputs -> fx -> uriQuery(outputs('Weburl_with_params'))
4. save
5. test the flow