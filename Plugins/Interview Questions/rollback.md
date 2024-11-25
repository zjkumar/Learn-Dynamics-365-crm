# If Async(or Async Workflow) and Sync both plugins are registered on the same entity and event. And Sync Plugin gets failed. What would happen with Async Plugin?

- Sync plugins execute within the database transaction.
- If any sync plugin fails, then the transaction is rolled back.
- Changes made by the sync plugin is not committed to the database.
- Async plugins are registered with async services only after successful transaction.
- Since the transaction is rolled back, async plugin is not registered with the async queues.
- So they wont get triggered.