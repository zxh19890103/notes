### getDerivedStateFromProps

getDerivedStateFromProps exists for only one purpose. 

It enables a component to update its internal state as the result of changes in props.

Derived state should be used sparingly

### All problems with it were caused by 
1. unconditionally updating state from props
2. updating state whenever props and state don't match.
