# Authentication

## What is OAuth

Source(https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)

SSO - Single sign-on

**What is OAuth?**

OAuth is an open-standard protocol for authorization.

It's a way to grant users access to unrelated third party websites/applications without the server/services sharing the initial password.

"In authentication parlance, this is known as secure, third-party, user-agent, delegated authorization."

Created in 2010 and used amongst the big mainstream corporations like Amazon, FB, Microsoft, etc.

**Give an example of what using OAuth would look like.**

When you go to a site and you are able to log into it with your credentials from another site.  
Recent example: Logging onto Netlify by using Github credentials.

OAuth can also be used "behind the scenes" of cloud storage files. For example, email systems for their use of attachments.

**How does OAuth work? What are the steps that it takes to authenticate the user?**

- User is signed into a site

- OAuth gives the user's identity to the second site

- The second site creates a single use token and a secret

- Initial site gives both to the client software

- Client software shows both to their authorization provider

- Client is asked to authenticate if they haven't already, then asked to approve authorization to the second site.

- User or software behind the scenes approves a transaction type at initial site

- Approved access token given to user

- User gives it to the initial site

- Initial site gives it to second site as "proof of authentication"

- Second site allows initial site access on behalf of user

**What is OpenID?**

"OpenID is about authentication: as a commenter on StackOverflow pithily put it:  
"OpenID is for humans logging into machines, OAuth is for machines logging into machines on behalf of humans.""

---

## Authorization and Authentication flows

Source(https://auth0.com/docs/flows)

**What is the difference between authorization and authentication?**

_Authentication_ - Verifying who a user is

_Authorization_ - verifying what the user has access to

The source for this question's answer also has a table of their differences.

(https://auth0.com/docs/get-started/authentication-and-authorization)

**What is Authorization Code Flow?**

Exchanges Authorization codes for tokens

**What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?**

Additional security for mobile and native applications during authentication

**What is Implicit Flow with Form Post?**

Access token requests used by public clients or applications that cannot securely store the client secret.

**What is Client Credentials Flow?**

The system will authenticate and authorize instead of the user. Used by machine-to-machine applications.

**What is Device Authorization Flow?**

Devices that connect to the internet ask the user to authorize the device by providing a link and asking user to go to it.  
For mobile/native applications.

**What is Resource Owner Password Flow?**

User provides credentials though an interactive form.  
Not recommended, but used by highly trusted applications.  
Best to only use when Authorization Code Flow can't be used.

---

## Additional Sources Provided by Reading Topic

[Auth0 for single page apps](https://auth0.com/docs/libraries/auth0-react)

---

### Things I want to know more about

<br>

[<<<Back](README.md)
