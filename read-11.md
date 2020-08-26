## Authentication

### User Modeling
* It is the duty of the developer to store sensitive user information responsibly
* Users trust that their information will not be leaked
* Some forms of sensitive data can be stored in plain text as long as the database is password protected
* More sensitive information such as a user password should be encrypted using a hashing algorithm
* User models that have sensitive data should never be sent to client applications
  * Instead create a second user profile model to hold the data and strictly limit access

### Cryptography
* Science that studes methods for encoding messages so that they can only be read by a person with access to the secret information required for decoding

### Hash Algorithms
* **Cryptographic Hash Algorithm** - Takes data and produces a has that is deliberately difficult to reverse
* Often used for checking the integrity of data
* Hash password can be stored when a user signs up

### Cypher Algorithms
* **Cryptographic Cypher Algorithm** - Takes data and a key and produces encrypted data. Later, the data can be reversed into the origin data through decryption
* User tokens are created by associating a random unique string (tokendSeed) with a user account, and then in turn encrypting the tokenSeed with a secrety key that only the server knows

### Basic Authorization
* Common method used to send a username and password in an HTTP request
* Joined with a `:` then "base64 encoded"
* `Authorization: Basic <credentials>`
* Simplest techique for enforcing access controls
* Does not require cookies, session identifiers, or login pages
* Server decodes Basic Authorization header to retrieve username and password. 
* If validated, server responds back to client with a validation response

### JWT (JSON Web Token)
* Method for securely transmitting information between parties as a JSON object
* Verified and trusted due to digital signature
* Can be signed using a secret key or a public/private key pair

[home](README.md)


