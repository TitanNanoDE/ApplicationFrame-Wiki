## Properties
| Name  | Trait | Description                                       |
| ----- | ----- | ------------------------------------------------- |
| value | any   | Holds the current value in the storage. Readonly. |

## Methods
### constructor() => `DataStorage`
Instantiates a new data storage.

### fill(value: `any`) => `void`
fills the data storage with the given value.

### when(callback: `(value: any) => void`) => `void`
Registers a callback for when ever a new value is filled into the data storage.
This also fires if there is already a value inside the storage.

### whenNext(callback: `(value: any) => void`) => `void`
Same as `when()` but only fires when the data storage is filled the next time. The callback is not invoked for the current value.

### once(callback: `(value: any) => void`) => `void`
Registers a callback which is invoked once the data storage has been filled. If the storage is already filled, it is invoked immediately.


## Specialties
Every method has two properties. `then()` and `catch()`. This means they can always be passed into something that expects a promise. While `catch()`'s callback never will be called, the `then()` callbacks will be registered just like they would have been in the actual function.
