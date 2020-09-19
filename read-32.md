## Custom Hooks

What does a component’s lifecycle refer to?

Why do you sometimes need to “wrap” functions in useCallback when called from within useEffect
  * This prevents the re-creation of a function by defining an inline function to use as an event handler
  * [resource](https://stackoverflow.com/questions/54371244/what-is-the-intention-of-using-reacts-usecallback-hook-in-place-of-useeffect)
  
Why are functional components preferred over class components?
  * Readability, resuability, less code, testability, more efficicient, references state directy rather than referencing with "this" in front of it.

What is wrong with the following code?
  * I believe the issue is that you cannot call a Hook from inside a loop (useEffect)

### Vocabulary

* **state hook** - The way to access state using functional components. Instead of state only being locally available within a class, a state hook is called inside of a functional component. The results is a cleaner, more readable, more efficient code block.

* **effect hook** - A hook used to cause change (side effect) that needs to happen along with each state change. an example might be updating a database or update a document title.

* **reducer hook** - A hook that returns the accumulation of something, such as React state. A clear way to think about it would be a set of ingredients(state) that are combined and accumulated to form a sauce. They are reduced down to a finished product which will always be the same if the same ingredints, amounts, stove and temperatures are used. 
  * [resource](https://www.telerik.com/kendo-react-ui/react-hooks-guide/#toc-custom-react-hooks)