# create an instant cloud flow

- Go to make.powerapps.com
- choose flows
    - Instant flow
        - Manually Trigger a flow (create)


# inside the flow

- New step
    - type compose and select it (data operation)
        - In the inputs, select fx, type utcNow() and click ok

- New step
    - type compose and select it (data opeation)
        - In the inputs, select fx, type convertFromUtc(utcNow(), 'India Standard Time') and click ok


- save

# Test the flow

- Test manually.
