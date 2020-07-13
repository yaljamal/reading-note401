# Redux - Asynchronous Actions

- Using Redux actions to connect to remote APIs via Thunk Middleware Normally, action generators return a function

- you may need to get something from a remote api, you’ll need your actions to do some asynchronous action before you dispatch it to the reducer. we want to set it up like this, where the action you dispatch from your React App returns a function, not an actual action object, which is what Redux `expects` and `requires`

# Actions

- When you call an asynchronous API, there are two crucial moments in time: the moment you start the call, and the moment when you receive an answer (or a timeout).

- An action informing the reducers that the request began.

- The reducers may handle this action by toggling an isFetching flag in the state. This way the UI knows it's time to show a spinner.

- An action informing the reducers that the request finished successfully.

- An action informing the reducers that the request failed.
