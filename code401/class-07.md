# [Reading-Notes](https://alsosteve.github.io/reading-notes/)
code fellows 401

# Read: 07 - Bearer Authorization

## Order of Events in Authentication

1. Register your application to get a client_id and client_secret
2. Ask the client if they want to sign in via a third party
3. Make a request to a third-party API endpoint
4. Receive access token
5. Receive authorization code
6. Make a request to the access token endpoint
7. Redirect to a third party authentication endpoint

## What can you do with an authorization code?
You exchange authorization codes for access tokens.

## What can you do with an access token?
It authorizes a user to access information in an api.

## What’s a benefit of using OAuth instead of your own basic authentication?
OAuth is more secure than making your own, unless you built OAuth.

## Vocab:

Client ID: a unique identifier for a browser–device pair that helps Google Analytics link user actions on a site.

Client Secret: a secret used by the OAuth Client to Authenticate to the Authorization Server.

Authentication Endpoint: a security mechanism designed to ensure that only authorized devices can connect to a given network, site or service.

Access Token Endpoint: where apps make a request to get an access token for a user.

API Endpoint: a point at which an API connects with the software program.

Authorization Code: a sequence of letters, numbers, or a combination of both, that validates a person's identity, approves a transaction or provides access to a secured area.

Access Token: an object encapsulating the security identity of a process or thread.