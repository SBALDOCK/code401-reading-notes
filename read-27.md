## Props and State

- Does a deployed React application require a server?

  - No. React applications build a virtual DOM and performs operations on the client's browser
  - [resource](https://stackoverflow.com/questions/26696204/does-react-js-require-server-side)

- Why do we prefer to test a React application at the behavior rather than the unit level?

  - BDD is preferred because the system itself does not evolve due to the framework, so the end goal of the test is always to confirm that a certain behavior takes place. The output must be correct under a given condition, but it does not matter how the output is generated.
  - [source](https://blog.testlodge.com/tdd-vs-bdd/#:~:text=In%20TDD%20(Test%20Driven%20Development,from%20the%20end%20users%20perspective.)

- What does `npm run build` do?

  - npm run build creates a **build** directory with a production build of the application.
  - This creates Javascript and CSS files inside a build/static directory
  - [resource](https://create-react-app.dev/docs/deployment/)

- Describe the actual composition / architecture of a React application
  - React is a view that caters to the user interface. It doesn't enforce an architecture. React comprises of components that may or may not hold state, or data needed to track for making an application work
  - [resource](https://www.simform.com/react-architecture-best-practices/)

### Vocabulary

- **BDD** - Behavior Driven Development. Different than Test Driven Development (Unit Testing) in that it tests the actual behavior of the system the end users perspective rather than checking the implementation of functionality.
- BDD is also a test-first approach
- [resource](https://blog.testlodge.com/tdd-vs-bdd/#:~:text=In%20TDD%20(Test%20Driven%20Development,from%20the%20end%20users%20perspective.)

- **Acceptance Tests** - Testing to determine whether the software system has met the requirement specifications. Evaluating the system's compliance with business requirements.
- [resource](https://www.tutorialspoint.com/software_testing_dictionary/acceptance_testing.htm#:~:text=Acceptance%20testing%2C%20a%20testing%20technique,for%20delivery%20to%20end%20users.)

- **mounting** - Process of outputting a virtual representation of a component to the final UI representation. For instance, outputting a React Element into the DOM element or DOM tree. This is important because one can only be sure a component is output/rendered when it is mounted.

* [resource](https://stackoverflow.com/questions/31556450/what-is-mounting-in-react-js#:~:text=Mounting%20is%20the%20process%20of,element)%20in%20the%20DOM%20tree.)

- **build** - Creating a build directory with a production build of an application

* [resource](https://create-react-app.dev/docs/production-build/)
