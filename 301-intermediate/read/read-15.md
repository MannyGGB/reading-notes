# Reading 15

(https://www.csoonline.com/article/562635/what-is-oauth-how-the-open-authorization-framework-works.html)

- What is OAuth? It is an authorisation protocol that allows authenticated access between servers and services without sharing the initial logon credentials.
- Give an example of what using OAuth would look like. For example, when you sign up for a website using Google or Facebook, you are using your authenticated access to Google or Facebook to sign up for the website without sharing your Google or Facebook logon credentials with said website.
- How does OAuth work? What are the steps that it takes to authenticate the user? As shown on the website,
  1. The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
  2. The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
  3. The first site gives this token and secret to the initiating user’s client software.
  4. The client’s software presents the request token and secret to their authorization provider.
  5. If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
  6. The user approves a particular transaction type at the first website.
  7. The user is given an approved access token.
  8. The user gives the approved access token to the first website.
  9. The first website gives the access token to the second website as proof of authentication on behalf of the user.
  10. The second website lets the first website access their site on behalf of the user.
  11. The user sees a successfully completed transaction occurring.
- What is OpenID? OpenID is similar to OAuth, but instead of focusing on authorisation, it is focused on authentication. Currently, it has become a complement to OAuth as an authentication layer.

  (https://auth0.com/docs/get-started/authentication-and-authorization-flow)

- What is the difference between authorization and authentication? Authorisation is related to what access the user has, whereas authentication is concerned with who the user is.
- What is Authorization Code Flow? This process involves exchanging an authorisation code for a token in confidential applications.
- What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)? This process introduces a Code Verifier or secret that can be verified by the authorization server. We need this extra layer of security when clients cannot hold credentials securely.
- What is Implicit Flow with Form Post? This process requests and gets tokens through the frontend without secrets going on in the back end. There is no need to maintain and protect secrets, so it was more common for traditional web apps, and now discouraged because it can expose token bits.
- What is Client Credentials Flow? This involves the exchange of application credentials for an access token. It is best suited for Machine-to-Machine apps.
- What is Device Authorization Flow? In this case, the user is prompted to go to a link to authorise their device. Apps pass along their Client ID to get a token.
- What is Resource Owner Password Flow? The user provides their credentials in the form of a username and password. These credentials can be stored in the backend for future use. It must not be used by third-party clients, only for highly-trusted apps.
