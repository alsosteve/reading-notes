# [Reading-Notes](https://alsosteve.github.io/reading-notes/)
code fellows 401

# Read: 09 - Authorization/Authentication

## What header(s) are used in authentication and authorization?
The HTTP Authorization request header can be used to provide credentials that authenticate a user agent with a server, allowing access to a protected resource.

## What is safe to put into a JWT
A secret, a token, username, and password are safe to put into a JWT.

## How are JWTs validated?
JWT's are validated by decripting them.

## Vocab:

RBAC: Role-based access control (RBAC) is a policy-neutral access-control mechanism defined around roles and privileges.

User Roles: Gives permission to certain users to preform specific operations and requests to an api.

JWT Token: Internet standard for creating data with optional signature and/or optional encryption whose payload holds JSON that asserts some number of claims.