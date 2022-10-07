[Home](../README.md)

# Class 15

## OAuth

1. What is OAuth?
  "OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential." Essentially, it allows a single sign on without sites actually being able to see your password.

2. Give an example of what using OAuth would look like.
  An example is the login popup that allows you to create or sign in to an account using an existing external account such as Google, Apple, Facebook, Github, etc.

3. How does OAuth work? What are the steps that it takes to authenticate the user?

    **i.**    The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.

    **ii.**   The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.

    **iii.**  The first site gives this token and secret to the initiating user’s client software.

    **iv.**   The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
  
    **v.**    If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
  
    **vi.**   The user approves (or their software silently approves) a particular transaction type at the first website.
  
    **vii.**  The user is given an approved access token (notice it’s no longer a request token).
  
    **viii.** The user gives the approved access token to the first website.
  
    **ix.**   The first website gives the access token to the second website as proof of authentication on behalf of the user.
  
    **x.**    The second website lets the first website access their site on behalf of the user.
  
    **xi.**   The user sees a successfully completed transaction occurring.
  
    **xii.**  OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. In fact, many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons).

4. What is OpenID?
    
    OpenID is to authentication as OAuth is to authorization. It basically would serve he same function as a google or facebook sign-on, except that it's use as a single sign on is its sole purpose. It could be used as one of the sign in options for OAuth.

## Authorization and Authentication Flows

1. What is the difference between authorization and authentication?
  
    Authentication is the process of a user proving their identity, whereas authorization is the process of granting a user access to a system based on their authentication.

2. What is Authorization Code Flow?
  
    Auth Code Flow is the defined process of exchanging an Authorization Code for a token.
    ![Auth-Code-Flow](../images/auth-sequence-auth-code.png)

3. What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

    Provides compatibility with mobile, native apps, and SPAs.

4. What is Implicit Flow with Form Post?

    Implicit Flow is an alternative to Authorization Code Flow that is intended for Public Clients, or applications which are unable to securely store Client Secrets

5. What is Client Credentials Flow?

    Client credentials flow is for machine to machine applications, where the system authenticates and authorizes the application instead of a user.

6. What is Device Authorization Flow?

    For devices with limited input options, they can provide a link that the user can go to to do auth.

7. What is Resource Owner Password Flow?

    Users authenticate with username and password, which can be stored for future exchange for a token. It should only be used when the app is highly trusted and redirect-based auth is unavailable.
