## Bearer Authorization

### Bearer Authorization

* Write the following steps in correct order:
  * Register your application to get a client_id and client_secret
  * Make a request to a third-party API endpoint
  * Ask the client if they want to sign in via a third party
  * Redirect to a third party authentication endpoint
  * Receive Authorization Code
  * Make a request to the access token enpoint
  * Receive Access Token
  
* What can you do with an authorization code?
  * Leverage an authorization code to be granted an access token

* What can you do with an access token?
  * Access tokens allow applications to make API requests on behalf of a user. It represents authorization to specific parts of a user's data.

* What's a benefit of using OAuth instead of basic authentication?
  * User login information is never stored in a database. 

### Vocabulary

* **Client ID** - Client IDs are public identifiers for apps, typically implemented as a hex string. Although public, it is best kept secure to avoid any phishing attacks
* **Client Secret** - A secret only know to the application and authorization server. Must not be guessable
* **Authentication Endpoint** - Used to request access tokens or authorization codes
  - [github](https://identityserver.github.io/Documentation/docsv2/endpoints/authorization.html)
* **Access Token Endpoint** - Where applications make a request to get an access token on behalf of a user
  - [oauth.com](https://www.oauth.com/oauth2-servers/access-tokens/)
* **API Endpoint** - Unique URL that acts as a touchpoint with another system it interacts with
* **Authorization Code** - Temporary code that client exchanges for access token. Obtained from authorization server.
* **Access Token** -  Credential provided by authorization server in exchange for authorization code, granted client access to an API on behalf of a user

* Service makes a boolean decision regarding the success of a login attempt
* This applies to both Basic Authentication (username and password) or OAuth (server to server handshaking)
* **Bearer Token** - Secondary authentication as a workaround to repeatedly obtaining username and password or proceeding through cumbersome OAuth process
* **Bearer Tokens** - encoded JSON objects that contain sufficient information for the server to confirm that any client request with a valid token must have come from a previously authenticated client with either Basic or OAuth. 
* Sent to client after initial signin process
* Client must make every additional request with bearer token
* Example header - `Authorization: Bearer encoded.jsonwebtoken.here`
* Server opens token, re-authenticates and then grants/denies access
* Can be performed in middleware with Express servers



[home](README.md)