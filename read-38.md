## Redux - Asynchronous Actions

How granular should your reducers be?
  * Reducers must stay pure. Never mutate arguments, perform side effects such as API calls, or call non-pure functions. For this reason, Reducers should stay simple and free of complexity if possible.
  * [resource](https://redux.js.org/basics/reducers
    )

Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched
  * This is probably a Pro as it simplifies things by enabling the use of combined reducers. 

Name a strategy for preventing the above...
  * I can't really find information on this. 

## Vocabulary

Store - A state container for JavaScript applications. Stores "store" the entire state of the app in an immutable object tree. State can only be changed by emitting an action. 
  * [resource](https://medium.com/the-web-tub/managing-your-react-state-with-redux-affab72de4b1)

Combined Reducers - A Redux helper function that turns an object whose values are different reducing functions into a single reducing function that can be passed to the store. 
  * [resource](https://redux.js.org/api/combinereducers)
