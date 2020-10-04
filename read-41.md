## React Native

Compare and Contrast Redux Toolkit with Redux “Ducks”
  * **Ducks** is a file structure that proposes putting all Redux-related logic for a given slice into a single file. In theory, this simplifies things and removes redundancies surrounding action type imports. 
  * With regards to Slices, the traditional method of defining a slice and exporting its action creators and reducers is very similar to the Redux Ducks pattern proposal. However, this has some downsides to be aware of. 
  * Redux action types are not meanto to be exclusive to a single slice. 
  * JS Modules can have **circular reference** problems if two modules try to import each other. 
  * [resource](https://redux-toolkit.js.org/usage/usage-guide#exporting-and-using-slices)

What is the principle advantage of Redux Toolkit
  * It is unopinionated
  * Lets you decide how to handle everything
  * Simplifies commond Redux use cases
  * Exports individual functions for use in an app
  * Simplified Store setup with **configureStore**
  * Simplified reducers with **createReducer**
  * Simplifying Slices with **createSlice**
  * [resource](https://redux-toolkit.js.org/usage/usage-guide)

### Vocabulary

**redux toolkit slices** - Functions that accept an initial state, an object full of reducer functions, and a "slice name", and generates action creators and action types that correspond to the reducers and state
  * [resource](https://redux-toolkit.js.org/api/createSlice)

**namespace** - A context component for identifiers. An example of a namespace is a directory, where each name uniquely identifies one file or subdirectory. They are heirarchies to allow for the reuse of names in different contexts. Some additional examples are file systems. In computer programming, they are employed for the purpose of grouping symbols and identifiers around a particular functionality to avoid name collisions.
  * [resource](https://en.wikipedia.org/wiki/Namespace)