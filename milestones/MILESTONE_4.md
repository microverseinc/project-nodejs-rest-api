# Milestone 4

## Introduction
So far we have been storing the data in memory, but Emvents Inc. wants to store the data in a persistent way. We will do that using a MongoDB database and the Mongoose ODM (Object Data Modeling).

## Get ready

- **Install MongoDB**:
MongoDB will be the document-oriented database that you will use to store the data of your API. Install it in your computer. [https://www.mongodb.com/download-center#community](https://www.mongodb.com/download-center#community)

- **Familiarize with mongo concepts**:
You might be used to relational databases (e.g. MySQL). Get yourself some time to learn about new concepts that are specific of document-oriented databases such as documents and collections. [https://docs.mongodb.com/getting-started/shell/introduction/](https://docs.mongodb.com/getting-started/shell/introduction/)

- **Play around with the Mongo shell**:
Use the Mongo Shell to create a new database and selecting it with the use command. Then, create a new collection to store Events by inserting one document in it. Use findOne to get the event you just inserted. [https://docs.mongodb.com/manual/reference/mongo-shell/](https://docs.mongodb.com/manual/reference/mongo-shell/)

- **Master the Mongo shell**:
Learn how to create, read, update, and delete MongoDB documents using its shell. [https://docs.mongodb.com/manual/crud/](https://docs.mongodb.com/manual/crud/)

- **Introduction to indexes**:
Learn what a MongoDB index is and how they can help you improve the performance of your mongoDB queries. [https://docs.mongodb.com/v3.0/core/indexes-introduction/](https://docs.mongodb.com/v3.0/core/indexes-introduction/)

- **Install mongoose**:
Mongoose provides a straight-forward, schema-based solution to model your application data and simplifies the process of working with MongoDB. Create a sample project and understand how you can use it in your Node.js app [http://mongoosejs.com/docs/guide.html](http://mongoosejs.com/docs/guide.html)

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

**NOTE**: Do you want to become a remote software developer? [Join our online training program](http://www.microverse.org/) where students from all around the world learn together doing remote pair programming, all while working on open source and freelance projects.
