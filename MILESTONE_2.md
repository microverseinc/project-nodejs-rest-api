# Milestone 2

## Introduction
Like we often do in product development, we will start by building an MVP (Minimum Viable Product). During this milestone, you will build a simple RESTful API to manage events using, for now, an in-memory data structure (e.g. array) to store the data.

## Requirements

1. Define a Javascript object that represents an "Event". 
   - It should contain an id, title, a description, and a date.
    
2. Create a Javascript object that will be used to store all your events. 
   - Use it as a dictionary where they id of the event will be the key used to store each event. 
   - Add multiple event objects to your data structure.

3. There should be an endpoint to get a list of all the events (GET /events)

4. There should be an endpoint to get one event and all its fields by its id (GET /events/{id})
   - It should return a 404 error code if the event can’t be found

5. There should be an endpoint that allows to create a new event (POST /events)
   - It should add the event to the events object
   - It should receive as a parameter an object with a title, description and date
   - It should automatically generate a new ID
   - It should return the event generated
   - It should use body-parser and accept json

6. There should be an endpoint that allows to update an existing event (PATCH /events/{id})
   - It should validate that an existing event ID is passed as parameter
   - It should return the modified event

7. There should be an endpoint that allows to delete an existing event (DELETE /events/{id})
   - It should return an empty response

8. Test your API using Postman

---

**NOTE**: Do you need help or some extra motivation to complete the project? [Fill in this form](https://microverse.typeform.com/to/Lh3CKF) and we will help you find a coding partner (like a gym buddy for pair programming), give you access to curated links for each section.