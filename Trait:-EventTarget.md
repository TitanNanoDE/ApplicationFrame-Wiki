## Properties

| Name  | Trait | Description |
| ----- | ----- | ----------- |
| none  |       |             |

## Methods

### on(name: `string`, listener: `(eventData: Object) => void`) => `void` 
This method registers a new listener for the given event. 
The listener is called every time the event is emitted on the object.

### emit(name: `string`, eventData: `Object`) => `void`
Emits an event with the given name on the object. Every registered listener for the event will be called.