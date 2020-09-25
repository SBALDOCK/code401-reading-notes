## <Login /> and <Auth />

Why is the Context API useful?
  - Context allows any component to make use of state without the hassle of props drilling and involving components that have no need for state

Can a component outside of a provider get its context?
  - No, only components within a provider can access context. 

What are some common use cases for using the Context API?
  - A common use case is within an application that has many components that have use for the same state. 

Describe “Context Hell”
  - Way too many nested components
    * [resource](https://www.polidea.com/blog/react-hooks-vs-wrapper-hell-writing-state-in-a-function-with-ease/)
    


## Vocabulary

Global State - How React manages state from the top down, either passing props down to child components, or managing state through hooks and context. 

Global Context - Passing state through a context provider to components rather than passing state by props drilling. Any component that needs to access state may.

Provider - A React component that allows consuming components to subscribe to context changes. 
  * [resource](https://reactjs.org/docs/context.html#contextprovider)

Consumer - A component that subscribes to context changes. Allows you to subscribe to a context within a function component. 
  *[resource](https://reactjs.org/docs/context.html#:~:text=Context.Consumer&text=A%20React%20component%20that%20subscribes,a%20function%20as%20a%20child.&text=For%20more%20information%20about%20the,'%20pattern%2C%20see%20render%20props.)