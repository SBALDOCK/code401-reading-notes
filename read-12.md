## OAuth

### OAUTH2.0
* "Open standard for access delegation"
* Gives users the ability to gran application access to services without giving the application their password
* When you "login with ..." you have given an application the keys to some personal information and access levels at Google.
* Used as a simplified way of logging in through one system
* When you grant access, the application acts as "you" and can perform certain tasks that you grant access to

### How Does OAuth Work?
* Can be thought of as a series of handshakes, where one application asks the user if it's ok to login as them for a specific purpose
* User agrees to allow to happen
* Remote Service contacts application with one-time use code for a token
* Once token is granted, the application is able to contact the remote service, using the token to access information as if it is the user
* **Token** is the user

### Access Code
* `<a>` - Provided to take a client to a service authorization page
* Tag passes information through a query string to the authorization server
  * response_type=code - Server wants a code
  * client_id=<your client id> - Tells server which app the user grants access to
  * redirect_uri=<your redirect uri> - Tells server which server endpoint to redirect to
  * scope=<list of scopes> - tells server what you want users to give access to
  * state=<anything you want>  - Place where information can be stored that is passed to server

### Access Token
* If user grants access to application, auth server redirects to provided URI callback with "code". Once in possession of code, exchange it for an access token by make a **POST** request to the auth server and providing:
  * grant_type=authorization_code
  * code=<the code your received
  * redirect_uri=REDIRECT_URI must be same as the redirect URI your client provided
  * client_id=<your client id> tells the authorization server which application is making the requests
  * client_secret=<your client secret> authenticates that the application making the request is the application registered with the client_id


### What is OAuth really all about
* Authorization, not authenication
* Originally meant for a service to authorize another service
  * Photo printing service - Photo printing business lets users upload photos digitally, but most people store their photos in the cloud. So the authorization was between the printing business and the cloud - example
  * Ask user for their username and password, but users won't do this
  * Only want to give access to certain photos
* Limited Access authorization
* Services can authorize against each other on your behalf once you've given them permission
* Called **access delegation**
* OAuth Flow 
  * Service needs to access google drive
  * User logged into service and google
  * Each service trusts the user but don't trust each other
  * If both services have OAuth implementation, one service checks with the user before allowing access to another service


[home](README.md)