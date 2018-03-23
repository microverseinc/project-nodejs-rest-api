# Milestone 3

## Introduction
Since we are building this project for a "real" client, we want to make sure we are shipping a high-quality product. In this milestone use testing to make sure the API works properly, even after a big refactoring (coming in milestone 4).

## Get ready

- **Learn the basics of unit testing**:
You will use unit testing to check that your API works as expected in a systematic way. This is very helpful when you are changing big parts of your code (refactoring) and you want to make sure you haven’t broken anything. [https://martinfowler.com/bliki/UnitTest.html](https://martinfowler.com/bliki/UnitTest.html)

- **Learn the basics of ES6**:
ES6 is a significant update to the Javascript language. Complete some of the “katas” in this website so you can master ES6. Try at least the “Promise”, “Block scope”, and “Arrow functions” sections. [http://es6katas.org/](http://es6katas.org/)

- **Install the unit testing libraries**:
Using npm, install the necessary libraries for unit testing in JavaScript: mocha (test runner, https://mochajs.org/) and chai (test assertion library, http://chaijs.com/). [https://mochajs.org/](https://mochajs.org/)

- **Learn how to use chai-http**:
You will use chai-http in order to be able to test your API by sending fake HTTP requests to your server. [https://github.com/chaijs/chai-http](https://github.com/chaijs/chai-http)

- **Familiarize yourself with the BDD syntax**:
You will use expect and should in your unit tests to check that your API is returning the right data in the right format. Get use to this way of asserting the data returned by your API. [http://chaijs.com/api/bdd/](http://chaijs.com/api/bdd/)

- **Learn the basics of how to test your Node API**:
Setting up your test suite can sometimes be challenging. Read this guide that will show you an example that you can use for your own project. [https://scotch.io/tutorials/test-a-node-restful-api-with-mocha-and-chai](https://scotch.io/tutorials/test-a-node-restful-api-with-mocha-and-chai)

## Requirements

1. Your package.json should be configured to run the tests from `npm run test`

2. Add mocha, chai and chai-http to your package.json as development dependencies

3. You should implement a test for the endpoint that returns all the events
   - Use chai-http to start and make requests to your server

4. You should implement a test for the endpoint that creates an event

5. You should implement a test for the endpoint that returns one event by its id

6. You should implement a test for the endpoint that updates an existing event

7. You should implement a test for the endpoint that deletes an existing event

---

**NOTE**: Do you want to become a remote software developer? [Join our online training program](http://www.microverse.org/) where students from all around the world learn together doing remote pair programming, all while working on open source and freelance projects.
