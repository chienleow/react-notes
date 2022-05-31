# React Notes
Notes from:
- Youtube tutorial: [React JS Crash Course 2021](https://youtu.be/w7ejDZ8SWv8)
- Udemy: [The Complete 2022 Web Development Bootcamp](https://www.udemy.com/course/the-complete-web-development-bootcamp/)

## What is [React](https://reactjs.org/)?
- JavaScript library for building user interfaces
- strictly front-end, runs in the browser
- create reusable components for repetitive elements
- runs on the client as a SPA (Single Page App)
  - where you have a single html page >> routing is done through React >> compiles to a JS bundle that is lodaded by the browser
- React doesn't have a built-in routing system, unlike [Angular](https://angular.io/), so we have to install an extra package [react router dom](https://reactrouter.com/web/guides/quick-start)

## Why use React?
- Structure the "view" (MVC) layer of your application
- Reusable components (hold their own state, data)
- JSX (Dynamic markup)
- Interactive UIs with virtual DOM (allows you to update parts of the page that need to be updated without reloading the entire page)
- Performance & Testing
- Data management (one-way data binding, all the data in your state is immutable, you can't mutate it directly)

## Main Concepts
1. Lists and Keys
  - Keys help React identify which items have changed, are added, or are removed. 
  - Keys should be given to the elements inside the array to give the elements a stable identity.

## Components
- [Docs: Thinking in React](https://reactjs.org/docs/thinking-in-react.html): Process of building a React app
- [Functional VS Class Components](https://github.com/chienleow/react-notes/blob/main/functional-vs-class-components.md)

## State
- Components can have "state" - an object that determines how a component renders and behaves
  - E.g. collapsible menu, state: "open", "close"

## Hooks
### What is a Hook? [Docs](https://reactjs.org/docs/hooks-state.html#whats-a-hook)
A Hook is a special function that lets you "hook into" React features.
  - `useState` 🎥[15 mins video](https://youtu.be/O6P86uwfdR0)
    - a Hook that lets you add React state to function components
    - returns a stateful value and a function to update it
