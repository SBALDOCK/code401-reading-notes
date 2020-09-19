## Hooks API

Why do we not need more .html pages in a multi-page React app?
  * One of React's main selling points is the resuability of components. With this reusability, you can run everything through a single html element and render everything on the page with very little html. 

If we wanted a component to show up on every page, where would we put it and why?
* Outside the <BrowserRouter/>
* Inside the <BrowserRouter />, outside a <Route />
  * We would place it inside the browser router, outside a route. 
* Inside a <Route />

What does props.children contain?
  * Props.children contains whatever is included betwee opening and closing tags when invoking a component
  * [resource](https://codeburst.io/a-quick-intro-to-reacts-props-children-cb3d2fce4891)

### Vocabulary

* Composition - Passing children prop directly into component output

* Children/Child Components - A prop that allows the transfer passage of components as data to other components. 

* Hash Routing - Hash routing uses a URL hash to keep UI in sync with the URL. 
  *[resource](https://reactrouter.com/web/api/HashRouter)

* Link Routing - A routing protocol that assumes that each node has a public/private key pair and has the capabiilty of signing and verifying digital signatures. Each node broadcasts its IP address and a Medium Access Code. 
  * [resource](https://www.sciencedirect.com/topics/computer-science/link-state-routing-protocol)

