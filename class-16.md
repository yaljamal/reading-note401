# Event Driven Programming
is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision

## EventEmitter

allows us to get started incorporating Event-Driven Programming in our project right away.
`const EventEmitter = require('events').EventEmitter;` 
in fact there are several modules published on npm such as EventEmitter2 and EventEmitter3 which promise a faster performance than the native EventEmitter.

All objects that emit events are instances of the EventEmitter class. These objects expose an eventEmitter.on() function that allows one or more functions to be attached to named events emitted by the object. Typically, event names are camel-cased strings but any valid JavaScript property key can be used.

When the EventEmitter object emits an event, all of the functions attached to that specific event are called synchronously. Any values returned by the called listeners are ignored and will be discarded.
