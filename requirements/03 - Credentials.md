# Credentials

You've implemented authentication! There are some things we need to improve but you've completed the core of it. The first improvement we should make is to actually provide and verify credentials before we create a token for the user.

1. Modify the `/login` controller function to accept a `username` and `password` in the request body.
2. Perform a check to make sure the username and password provided matches the values on the mock user;
    1. If the credentials match, create the token and send it in the response.
    2. If they don't match, send an error message.