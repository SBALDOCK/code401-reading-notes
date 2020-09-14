## Component Composition

- Can a parent component access the state of a child component?

  - By declaring a **ref** in the parent component and then pass it as a ref attribute to the child
  - [resource](https://stackoverflow.com/questions/27864951/how-to-access-childs-state-in-react#:~:text=In%20case%20that%20you%20really,you%20need%20to%20use%20React.)

- What can be passed along in a prop variable?

  - Props pass data from one component to another. This data is **read-only**, meaning that data coming from a parent is not changed by child components.
  - [resource](https://itnext.io/what-is-props-and-how-to-use-it-in-react-da307f500da0#:~:text=%E2%80%9CProps%E2%80%9D%20is%20a%20special%20keyword,from%20one%20component%20to%20another.&text=Furthermore%2C%20props%20data%20is%20read,be%20changed%20by%20child%20components.)

- How can a child component “know” the state of another component?
  - A child component can "know" the state of another component if a parent passed the same set of props to multiple child components?git

### Vocabulary

- **component props** - Props, short for **properties** is a key word that functions to pass data from one component to another. They are passed in a uni-directional flow, meaning one way from parent to child. This data is read-only and does not change when passed to a child component.

  - [resource](https://itnext.io/what-is-props-and-how-to-use-it-in-react-da307f500da0#:~:text=%E2%80%9CProps%E2%80%9D%20is%20a%20special%20keyword,from%20one%20component%20to%20another.&text=Furthermore%2C%20props%20data%20is%20read,be%20changed%20by%20child%20components.)

- **component state** - State is an object that determines now a component renders and behaves. It is what allows creation of components that are dynamic and interactive. An example of state would be water vs ice. They are the same thing, but have a different state depending upon the temperature.

  - [resource](https://thinkster.io/tutorials/understanding-react-state)

- **application state** - State is the interface between data from any kind of backend and the representation of the data with UI-elements in the frontend. State is able to keep the data of different components in sync because each state update with rerender all relevant components.
  - [resource](https://medium.com/dailyjs/comparison-of-state-management-solutions-for-react-2161a0b4af7b#:~:text=In%20an%20application%2C%20state%20is,will%20rerender%20all%20relevant%20components.)
