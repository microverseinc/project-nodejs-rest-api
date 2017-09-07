# Milestone 5

## Introduction
Emvents Inc. wants users to be able to sign up to events with their accounts and they want organizers to be able to manage their events. In order to do that, we need to know who is who. In this milestone we will add users and authentication to our RESTful API.

## Requirements

1. Requirement: The application should have a User schema.
   - Each User document should have the following properties: username, password, email address and full name.

2. The Mongo database should have a new collection for Users.

3. A new endpoint to create a User should be available.
   - The endpoint should be POST /users
   - It should have tests to make sure it works as expected.
   - It should not be possible to create a new user with an email that already exists.
   - It should not be possible to create a new user with a username that already exists.
   - If should return a 409 (Conflict) error if the username or email already exists.
   - Optional: The password should be hashed before it’s stored in the database.

4. Passport and passport-http should be used to authenticate users using username and password.
   - Passport-http should be used to implement Basic HTTP authentication
   - Session support should be disabled

5. All the endpoints created until this point should require the user to provide authentication credentials (username and password). 
   - Otherwise, they must return a 401 HTTP error.
   - The POST /users endpoint should not require authentication

6. Requirement: Use the "Basic Auth" functionality of Postman to test the authentication flow works correctly. 
   - Link: [https://www.getpostman.com/docs/postman/sending_api_requests/authorization](https://www.getpostman.com/docs/postman/sending_api_requests/authorization)

7. Your application should have tests to make sure the authentication logic is working as expected.
   - Make sure to modify the existing tests since they now require credentials to be sent with 
each request.

8. Optional: Your application should use auth tokens or any other similar mechanism (e.g. OAuth) so that clients don't need to send username and password with every request.
