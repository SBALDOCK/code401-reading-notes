## Application State with Redux

What are the advantages of storing tokens in "cookies" vs "local storage"?

  * Cookies provide a higher protection from malicious JavaScript attacks. Using cookies also means less work for a client, as it shifts the burden to the server. 
  * [resource](https://edward-huang.com/authentication/tech/2019/09/10/all-you-need-to-know-about-authentication-is-here/#:~:text=Advantages%20of%20using%20Cookie%2Dbased%20Authentication&text=Implementing%20or%20storing%20your%20token,script%20to%20the%20victims'%20website.)

Explain 3rd party cookies

  * Created by domains other than the one a user is visiting directly. Used for cross-site tracking, regtargeting and adserving. They allow website owners to provide certain services such as live chats. The reason for a third-oarty cookie is because a URL does not match a domain. 
  *[resource](https://clearcode.cc/blog/difference-between-first-party-third-party-cookies/)

How do pixel tags work?

* A tracking (pixel) tag is added by using a code in a site's HTML code or email, containing an external link to the pixel server. When someone visits a website, the HTML code is processed by the user's browser, which follows the link and opens the hidden graphic. Tracking pixels can provide information about users such as the type of device they are using or their location. 
* [resource](https://whatagraph.com/blog/articles/tracking-pixel#:~:text=their%20digital%20ad.-,How%20Do%20Tracking%20Pixels%20Work%3F,and%20opens%20the%20hidden%20graphic.)

### Vocabulary

**cookies** - A small text file that is created when a user used their browser to visit a website that uses cookies to keep track of user movements within the site, helping resume use where the user left off, remembering login registration, theme selection, preferences, and other customization functions
  * [resource](https://www.allaboutcookies.org/cookies/)

**authorization** - Authorization is the definition of access for users based upon what access they need to a certain application. For instanced, an admin might need a level of authorization with much greater access than that of a user. 

**access control** - Access control is the process of building authorization levels based on user role, so that different individuals within an organization can view and edit the application in different ways depending upon need. 

**conditional rendering** - Conditional rendering is the output of authorization, so that certain elements of an application will be presented only to those who are appropriately authorized. An example might be the option to "edit" a profile for one user, but the option to both "edit" and "delete" a profile by another users. Those options will either present themselves or not based on authoriztation and access control. 

