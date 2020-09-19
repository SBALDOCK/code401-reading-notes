## Context API

Describe use cases for useMemo() and useReducer()
  * **useMemo()** - Implement useMemo in a React application that renders a list of users and allows the end-user to filter users by their name. This filter only happens when a user explicitly clicks a button, not when input is typed into an input field. With large data sets, leverage **useMemo** to **memoize** return values and run a function only if its dependencies have change
    *[resource](https://www.robinwieruch.de/react-usememo-hook)
  * **useReducer()** - When you need to manage state transitions for a list of items
    *[resource](https://www.robinwieruch.de/react-usereducer-hook)

Why do custom hooks need the use prefix?
  * Using a prefix is necessary in order to avoid conflicts with other plugins. For example, use a unique prefix that will be unlikely that another developer might use to name their custom hook, so that in the scenario when a user installs both plugins, potential bugs may occur. 
    *[resource](https://developer.wordpress.org/plugins/hooks/custom-hooks/)

What do custom hooks usually do?
  * Custom hooks usually allows the extraction and reuse of functions. This is an alternative to **rendering props** and using **high-order components** and one that solves the problem wihouth needing to add additional components to the tree. 
    *[resource](https://reactjs.org/docs/hooks-custom.html)

Using any list of custom hooks, research and name one that you think will be useful in your applications
  * useArray Hook - I can see this custom hook coming in handy when needing to manipulate lists
  *[resource](https://blog.bitsrc.io/10-react-custom-hooks-you-should-have-in-your-toolbox-aa27d3f5564d)

Describe how a hook that fetches API data might work
  * A fetch hook fetches data with axios or a similar fetching library from the API, sets the data in the local state of the component wih an update function, but might run into problems with constantly updating and fetching. It is important to include an empty array along with a new hook to avoid activating the hook on component updates and only for the mounting of the component. 
    * [resource](https://www.robinwieruch.de/react-hooks-fetch-data)

### Vocabulary

* **reducer** - A reducer function takes two arguments, the current state and an action, and returns based on both arguments a new state. 
  *[resource](https://www.robinwieruch.de/javascript-reducer)