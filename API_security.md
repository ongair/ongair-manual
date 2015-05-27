# Security

###URL

Depending on the environment where you account has been set up, use the correct prefix.

- https://app.ongair.im
- https://beta.ongair.im

All requests must have the authentication token in the header or within the URL parameters. The first option is preferred.

###Option 1

|Header        | Values        |
|-------------|-------------|
|Accept|application/json|
|Authorization| Token token=<enter_token_here>|

###Option 2

    https://app.ongair.im/api/v1/base/status?token=<enter_token_here>

###Authentication Error
In the event of an authentication error .e.g. no token is provided or an invalid token is provided then the result is a 401 error code with the response:

    {"error":"Invalid API Token"}
