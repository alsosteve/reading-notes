# [Reading-Notes](https://alsosteve.github.io/reading-notes/)
Code Fellows Python 401

# Read: 33 - Authentication & Production Server

## [JSON Web Tokens](https://jwt.io/introduction/)
- JSON Web Token (JWT) defines a compact and self-contained way for securely transmitting JSON information

### when to use:
1. Authorization
2. Info Exchange

### JWT Structure
- Header
- Payload
- Signature

### Header
two parts: the type of the token, and the signing algorithm

``` json
{
  "alg": "HS256",
  "typ": "JWT"
}
```

### Payload
- contains the claims
  - statements about an entity and additional data
#### claims:
- Registered claims: predefined claims which are not mandatory but recommended
- Public claims: can be defined at will by those using JWTs but should be defined as a URI that contains a collision resistant namespace
- Private claims: custom claims created to share information

#### ex.
``` json
{
  "sub": "1234567890",
  "name": "John Doe",
  "admin": true
}
```

### Signature
To create the signature part you have to take the encoded header, the encoded payload, a secret, the algorithm specified in the header, and sign that.

#### ex
``` json
HMACSHA256(
  base64UrlEncode(header) + "." +
  base64UrlEncode(payload),
  secret)
```

## Use diagram
![use diagram](https://cdn2.auth0.com/docs/media/articles/api-auth/client-credentials-grant.png)

## Why use them
- less verbose 
- compact

## [DRF JWT Authentication](https://simpleisbetterthancomplex.com/tutorial/2018/12/19/how-to-use-jwt-authentication-with-django-rest-framework.html)

## [https://build.vsupalov.com/django-runserver-in-production/](https://build.vsupalov.com/django-runserver-in-production/)
- server started with runserver is not guaranteed to be performant
- only use tech in production
- DJANGO provides a uwsgi.py
- use a production-ready web server like Nginx
- let your app be handled by a WSGI application server like Gunicorn.
- with Heroku, a web server is provided implicitly

## [Optional Video:  JWT with DRF](https://www.youtube.com/watch?v=Fhcn2qx-4VQ)

## Bookmark and Review
- [Gunicorn](https://gunicorn.org/)
- [Django Migrations Primer](https://realpython.com/django-migrations-a-primer/)