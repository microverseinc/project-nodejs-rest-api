# Milestone 2

## Introduction
Like we often do in product development, we will start by building an MVP (Minimum Viable Product). During this milestone, you will build a simple RESTful API to manage events using, for now, an in-memory data structure (e.g. array) to store the data.

## Get ready

- **Express.js routing**:
Learn how you can use routing to process different requests through your API. [http://expressjs.com/en/starter/basic-routing.html](http://expressjs.com/en/starter/basic-routing.html)

- **Express Route Paths**:
During the development of your API, you will use route paths to define handlers for different requests. [http://expressjs.com/en/guide/routing.html](http://expressjs.com/en/guide/routing.html)

- **RESTful APIs**:
Learn what makes an API a RESTful API and why REST is so important [http://www.andrewhavens.com/posts/20/beginners-guide-to-creating-a-rest-api/](http://www.andrewhavens.com/posts/20/beginners-guide-to-creating-a-rest-api/)

- **Express.js route parameters**:
Learn how to manage parameters in a route to collect data from a request [http://expressjs.com/en/4x/api.html#req](http://expressjs.com/en/4x/api.html#req)

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

**NOTE**: Do you want to become a remote software developer? [Join our online training program](http://www.microverse.org/) where students from all around the world learn together doing remote pair programming, all while working on open source and freelance projects.
