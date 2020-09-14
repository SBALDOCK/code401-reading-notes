## Routing

- Do child components have direct access to props/state from the parent?

  - No, props passed down from parents to child components are one-way and only "readable". They cannot be changed or accessed by the child component.

- When a component “wraps” another component, how does the child component’s output get rendered?
  - The child component is provided a structure for how it will be displayed based upon the wrapper component. This is useful for creating a UI that uses elements repeatedly throughout a design.
  - [resource](https://www.digitalocean.com/community/tutorials/how-to-create-wrapper-components-in-react-with-props)

`<Main>`
`<Content />`
`</Main>`

- Can a component, such as <Content />, which is a child also be used as a standalone component elsewhere in the application?

  - Yes. Child components can be reused elsewhere in an application by using **props.children**.

- What trick can a parent use to share all props with it’s children
  - A parent can use a **spread** operator to share all props
  - This is an ES6 option rather than a React feature. It allows for expansion of an iterable like a string, object or array.
  - `const IntermediateComponent = (props) => {`
    `return (<ChildComponent {...props} />)}`
  - [resource](https://flaviocopes.com/react-pass-props-to-children/)

### Vocabulary

- **props.children** - Properties passed to children components from parents that are used to display the contents of opening and closing tags when invoking the component. A component includes a reference to whatever the child component contents are and renders that.

  - [resource](https://codeburst.io/a-quick-intro-to-reacts-props-children-cb3d2fce4891)

- **composition** - A method for reusing code between components that is an alternative option to inheritance and recommended for use in React. It is useful if a parent component does not know their children ahead of time. This is when a component should use **children** to pass children elements directly to the output. \*[resource](https://reactjs.org/docs/composition-vs-inheritance.html)
