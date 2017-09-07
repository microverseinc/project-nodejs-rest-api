# Milestone 4

## Introduction
So far we have been storing the data in memory, but Emvents Inc. wants to store the data in a persistent way. We will do that using a MongoDB database and the Mongoose ODM (Object Data Modeling).

## Requirements

1. Create a variable that references a MongoDB collection that will be used to store “events”

2. Calling POST /event should save the new event document to the MongoDB collection
   - Criteria: For now, make sure you use the Node.js native driver and not Mongoose. Link: [http://mongodb.github.io/node-mongodb-native/2.2/quick-start/quick-start/](http://mongodb.github.io/node-mongodb-native/2.2/quick-start/quick-start/)
   - Criteria: You should not generate an id anymore. MongoDB will do it for you.
   
3. Refactor the GET /events endpoint so it gets the events from the MongoDB collection

4. Refactor the GET /events/{id} endpoint so it gets the event from the MongoDB collection

5. Updating an existing event (i.e. POST /events/{id}) should save the changes to the MongoDB database.

6. Deleting an event should delete the event from the database.

7. Refactor your code using Mongoose

8. Create a dedicated folder and files to organize your routes.

9. Create a dedicated folder and files to organize your models.

10. Make sure all your tests still pass.

11. Add a new search endpoint (and a test) to allow the user to search events.
   - It should accept a query parameter called “title”
   - It should search events by title
   - It should use the following path: /events/search?title={text_to_search}

12. Requirement: Create an index in the database to improve the performance of this last query. 
   - Use the mongo shell command “explain” to check the performance improvement.
   - Link: [https://docs.mongodb.com/v3.2/tutorial/analyze-query-plan/](https://docs.mongodb.com/v3.2/tutorial/analyze-query-plan/)

---

**NOTE**: Do you need help or some extra motivation to complete the project? [Fill in this form](https://microverse.typeform.com/to/Lh3CKF) and we will help you find a coding partner (like a gym buddy for pair programming) and give you access to curated lists of readings, videos and documentation to get ready for each requirement.