## Access Control (ACL)

* When is Basic Authorization used vs. Bearer Authorization?
  * Use basic when a username and password are sufficient security for accessing an application. If the information accessed is highly sensitive, user bearer authorization. Bearer authorization is better for the exchange of sensitive information, 
* What does the JSON Web Token package do?
  * A JSON Web Token is returned when a user logs in using credentials, which is saved locally. 
  * Example - A server could generate a token that has the claim "logged in as admin" and provide to a client. The client could then use that token to provide that it is logged in as admin
  *[wikipedia page](https://en.wikipedia.org/wiki/JSON_Web_Token)
* What considerations should we make when creating and storing a SECRET?
  * Do not store unencrypted secrets in .git repositories
  * Dont share unencrypted secrets in messaging systems
  * Store secrets safely
  * Restrict API access and permissions
  * Avoid git add * comments on git
  * Add sensitive files to .gitignore
  * Use encryption to store secrets within .git repositories

### Vocabulary
* Encryption - A method of turning information into secret code to hide it's true meaning 
* Token - A generated code provided to a user/application in order to gain access to something. Tokens in and of themselves are meaningless/useless, but only have meaning in the context of a system that interprets the token
* Bearer - The predominant type of access token which basically means, give the bearer of this token access to something
* Secret - A piece of information that is used to encrypt or decrypt messages. Also may be known as a private key.
* JSON Web Token - A way of creating data with signature and/or encryption which holds JSON. These tokens are signed using a SECRET

### Preview
* What 3 things had you heard about previously and now have better clarity?
* Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
* What are you most excited about trying to implement or see how it works?


