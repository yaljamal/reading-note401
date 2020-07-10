# State with Redux

Redux is available as a package on NPM for use with a module bundler or in a Node application
`npm install redux`

## Managing state with Redux requires the combination of 3 distinct aspects into a “Store” :

1. State
2. Reducers (strategies to alter state)
3. Actions (methods that get “dispatched” or “run”, which trigger associated reducers)

## Redux Store

- Ultimately, the “store” is where your application state is, well, stored. The store’s job is to identify the various reducers and middleware that need to be made available and used globally.

- React uses “reducers” to hold and manage state. Reducers typically manage just one part of the larger application state. For example, in a storefront application, you would likely have a separate reducer for Products, Categories, and Carts
