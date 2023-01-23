# Authenticating HTTP Requests

## Learning Objectives

- Use bearer token authentication to protect an API resource

## Introduction

In this exercise, you're going to build a small but complete bearer token authentication system. Here's a reminder for the flow:

1. The client sends a request containing login credentials to the server.
2. The server checks the credentials are correct and sends back a token.
3. The client sends a request to a secure resource, putting the token in the `authorization` header of the request.
4. The server verifies that the token is valid and sends back the requested resource, or an error message if the token wasn't valid.

Here's the diagram again to help you visualise this flow:

![](./assets/Auth_Flow.png)

## Instructions

1. Fork this repository and clone the fork.
2. Run `npm ci` to install dependencies.
3. Run `npm start` to run the application.
4. Complete each requirement in the `requirements` directory in numerical order.
   1. As part of this, you will need to create an environment variable to store your secret!
   2. Copy the `.env.example` file and name your file `.env`
   3. Assign the `JWT_SECRET` variable some string value for your secret (e.g. `JWT_TOKEN="my_super_secure_secret"`) 
   4. You can then reference this secret by using the node process env object (e.g. `const secret = process.env.JWT_SECRET`)
