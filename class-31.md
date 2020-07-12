# Combined Reducers

`combineReducers` is simply a utility function to simplify the most common use case when writing Redux reducers. `CombineReducers` enforces several rules to help users avoid common errors. `CombineReducers` will call each slice reducer with its current slice of state and the current action, giving the slice reducer a chance to respond and update its slice of state if needed.

## Arguments

`reducers` (Object): An object whose values correspond to different reducing functions that need to be combined into one. See the notes below for some rules every passed reducer must follow.
`Returns`
(Function): A reducer that invokes every reducer inside the reducers object, and constructs a state object with the same shape.
