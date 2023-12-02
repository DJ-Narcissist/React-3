### Conceptual Exercise

Answer the following questions below:

- What is Redux? Why might you use it?
    A. A library for state management, used for mananging large applications with quite a bit of state, solves the issue of prop-drilling.

- What are three features of the Redux developer tool in Chrome?
    A. Time-traveling debugging, action logging and state inspection

- What is a store?
    A. The centralized place where state is stored.

- What is a reducer?
    A. A functions that accept 2 objects a state and an action, use the action to produce and return a new state object.

- What is an action?
    A. Objects with key of type. THat dexcribe a change in the application's state

- What is an action creator?
    A. A function that returns an action object

- How does data flow in a React/Redux application?
    A. Dispatch(current state, action) -> reducer -> new state (store)

- What is the purpose of the `<Provider>` component?
    A. To make the Redux store available to tall componenets in a React application without passing it explicitly through each level of componenet tree.

- What is the purpose of the `useSelector` hook? What does it return?
    A. To access and extract specific places of state form the Redux store, and ensures that the UI reflects the most up-to-date state from the Rexdux store. The return the currently selected part of the Redux store's state.

- Describe the `useDispatch` hook. What do you use it for?
    A. Part of the React-Redux library and is used in functional React componenets to gain access to the dispatch function from th eRedux store.
- What is redux-thunk and why would you use it?
    A. A middleware for Redux, a predictable state container for Javascript applications. It allows you to write action creatord that return functionc instead of plain action objects. You use it for Async actions, side effects and conditional dispatch.

- What are propTypes?
    A.  property avaiable in REact that allows  you to specfiy the type of data expected for pops in a React compoonent.

- Describe the `useCallback` hook.  What is it used for?
    A. A built in hook that accepts  afunction and an array of dependencies. Allows you to add function sas dependencies to useEffect without hitting infinite render issues
    
- Compare and contrast the `useReducer` hook with Redux (including react-redux).  Why would you choose one over the other?

    A. Both are state management solutions in React. useReducer is already built into React, is more simple due to this but because it is a local state there is no global store. While Redux is a global state, has an external library for management and  requires more to setup. I would use useReducer when the components are simpler and for more complex components Redux is used.