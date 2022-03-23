# Authentication & Production Server

## Reading

### JSON Web Tokens

[Source](https://jwt.io/introduction/)

JWT securely transmits information between parties as a JSON object. Since they are signed with a public/private key pair, information can be trusted and verifed.

When to use JWTs:

- For authorization (Most common scenario). After log in, requests include the token so the user can access the resources permitted with that token.

- For securely exchanging information between parties, making sure the senders are who they say.

JWT structure:

Each part is separated by a dot.

> JWT Ex:  `xxxxx.yyyyy.zzzzz`

- Header

  - Token type (JWT)

  - Signing algorithm

- Payload

  - Registered Claims

  - Public Claims

  - Private Claims

- Signature

How JWTs work:

User logs in, JWT is returned.  
User wants access to a protected route or resource, user agent sends JWT.  
Server's protected routes check if the JWT is valid.  
If valid, user gets access to those protected resources.

- Tokens should not be kept longer than required

- Prevent JWT from getting too big when sending them through HTTP headers. Too much information in a single token can cause some servers to not accept them

Why use JWTs:

"As JSON is less verbose than XML, when it is encoded its size is also smaller, making JWT more compact than SAML. This makes JWT a good choice to be passed in HTML and HTTP environments."

</br>

### DRF JWT Authentication

[Source](https://simpleisbetterthancomplex.com/tutorial/2018/12/19/how-to-use-jwt-authentication-with-django-rest-framework.html)

JWT is acquired by exchanging a username and password, gets an access token and a refresh token

- access tokens are short-term and expire within 5 minutes. They are sent via HTTP header.

- refresh tokens are somewhat longer-term and expire in 24 hours. They are necessary for making sure the user still has correct permissions. They travel in the POST data.

JWT information is encoded with Base64

This article gives the installation and setup using the `djangorestframework_simplejwt` library

</br>

### Django Runserver Is Not Your Production Server

[Source](https://build.vsupalov.com/django-runserver-in-production/)

App is run locally with `python manage.py runserver` while in development, but should not be used for production setup because of bad security and performance.

A production stack is used because it is made up of components that are designed for their own specific tasks, making the process fast and reliable.

Django does not wait for or react to requests.

Requests need to go through a `web server`

`Application server` will take the requests and create Python objects that are usable by Django.

`uwsgi.py` file has a function to get a Python object that represents an incoming request, the application server calls this function.

- The function calls your code, makes the response object, then passes that object to the WSGI server.

- That response is translated into an HTTP response then passed back to the web server.

- Web server then delivers to the user

---

## Videos

### JWT with DRF

[Source](https://www.youtube.com/watch?v=Fhcn2qx-4VQ)

---

## Bookmark/Skim

### Gunicorn

[Source](https://gunicorn.org/)

### Django Migrations Primer

[Source](https://realpython.com/django-migrations-a-primer/)

---

</br>

[<<<Back](README.md)