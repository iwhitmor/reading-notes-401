# React: Hooks, Events, Forms, State, & Components

## [Making Sense of Hooks](https://medium.com/@dan_abramov/making-sense-of-react-hooks-fdbde8803889)

* Why Hooks?

  * Hooks let us organize the logic inside a component into reusable isolated units

  * Hooks apply the React philosophy (explicit data flow and composition) inside a component, rather than just between the components

  * Unlike patterns like render props or higher-order components, Hooks don’t introduce unnecessary nesting into your component tree. They also don’t suffer from the drawbacks of mixins

  * Hooks will reduce the number of concepts you need to juggle when writing React applications

  * Hooks are fully encapsulated — each time you call a Hook, it gets isolated local state within the currently executing component

## [Hooks API](https://reactjs.org/docs/hooks-overview.html)

* Hooks are a new addition in React 16.8. They let you use state and other React features without writing a class

* Hooks are functions that let you “hook into” React state and lifecycle features from function components. Hooks don’t work inside classes — they let you use React without classes

* React provides a few built-in Hooks like useState. You can also create your own Hooks to reuse stateful behavior between different components

* Effect Hook

  * You’ve likely performed data fetching, subscriptions, or manually changing the DOM from React components before. We call these operations “side effects” (or “effects” for short) because they can affect other components and can’t be done during rendering

* Rules of Hooks:

  * Only call Hooks at the top level. Don’t call Hooks inside loops, conditions, or nested functions

  * Only call Hooks from React function components. Don’t call Hooks from regular JavaScript functions. (There is just one other valid place to call Hooks — your own custom Hooks. We’ll learn about them in a moment.)

## [Effects Hooks](https://reactjs.org/docs/hooks-effect.html)

* Effects without cleanup

  * Sometimes, we want to run some additional code after React has updated the DOM. Network requests, manual DOM mutations, and logging are common examples of effects that don’t require a cleanup. We say that because we can run them and immediately forget about them. Let’s compare how classes and Hooks let us express such side effects

* Effects with cleanup

  * Some effects need cleanup. For example, we might want to set up a subscription to some external data source. In that case, it is important to clean up so that we don’t introduce a memory leak! Let’s compare how we can do it with classes and with Hooks

## [Handling Events](https://reactjs.org/docs/handling-events.html)

* Handling events with React elements is very similar to handling events on DOM elements. There are some syntax differences:

  * React events are named using camelCase, rather than lowercase

  * With JSX you pass a function as the event handler, rather than a string

## [Forms](https://reactjs.org/docs/forms.html)

* HTML form elements work a bit differently from other DOM elements in React, because form elements naturally keep some internal state

* Controlled Components

  * In HTML, form elements such as <input>, <textarea>, and <select> typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with setState()

  * We can combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React in this way is called a “controlled component”

  * With a controlled component, the input’s value is always driven by the React state. While this means you have to type a bit more code, you can now pass the value to other UI elements too, or reset it from other event handlers

## [Components and Props](https://reactjs.org/docs/components-and-props.html)

* Composing Components

  * Components can refer to other components in their output. This lets us use the same component abstraction for any level of detail. A button, a form, a dialog, a screen: in React apps, all those are commonly expressed as components

  * Typically, new React apps have a single App component at the very top. However, if you integrate React into an existing app, you might start bottom-up with a small component like Button and gradually work your way to the top of the view hierarchy

* All React components must act like pure functions with respect to their props

### Additional Resources

* [The State Hook](https://reactjs.org/docs/hooks-state.html)

* [Hooks API Reference](https://reactjs.org/docs/hooks-reference.html)

* [State and Lifecycle](https://reactjs.org/docs/state-and-lifecycle.html)
