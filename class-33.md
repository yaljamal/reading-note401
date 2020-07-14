# ways to build and manage a Redux store

- Redux Toolkit :
  The makers of Redux have recognized that Redux is complicated and have introduced a “Batteries Included, Highly Opinionated” framework for making stores called the Redux Toolkit

  This toolkit specifies a few different means of building a reducer and action set that work well together and are easier to understand and integrate

- Ducks: Redux Reducer Bundles :

  You can still do:

  `````import { combineReducers } from 'redux';
  import \* as reducers from './ducks/index';

  const rootReducer = combineReducers(reducers);
  export default rootReducer;````
  You can still do:

  import \* as widgetActions from './ducks/widgets';
  `````

- `MobX` :

  `MobX` is a simple, scalable and battle tested state management solution.

  This tutorial will teach you all the important concepts of MobX in ten minutes.

  `MobX` is a standalone library, but most people are using it with React and this tutorial focuses on that combination.

  **The core idea**

  State is the heart of each application and there is no quicker way to create buggy, unmanageable applications than by producing an inconsistent state or state that is out-of-sync with local variables that linger around.

- `Hookstate`
  Is a modern alternative to Redux, Mobx, Formik without boilerplate ,it is simple but incredibly fast and flexible state management that is based on React state hook.
