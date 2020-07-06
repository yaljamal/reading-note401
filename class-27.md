# Context API
* Context provides a means of passing state down the component tree through a Provider/Consumer relationship.
* At as high a level as makes sense, a “provider” can make it’s state available, along with means of altering it (methods).
* At the lower levels any component can “opt-in” and become a “consumer” and receive this.state from context.

## When to Use Context ?
Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language. For example, in the code below we manually thread through a “theme” prop in order to style the Button component:

# API
```{REACT.CREATECONTEXT
const MyContext = React.createContext(defaultValue);

CONTEXT.PROVIDER
< MyContext.Provider value={/* some value */}>}```