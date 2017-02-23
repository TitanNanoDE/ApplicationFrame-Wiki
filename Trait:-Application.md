**Required Traits: `EventTarget`**

## Properties
| Name    | Value Trait | Visibility | Description                                               |
| ------- | ----------- | ---------- | --------------------------------------------------------- |
| name    | string      | public     | Name of the application, other components can identify it.|
| version | string      | public     | The current version of the application.                   |
| author  | string      | public     | Author meta data.                                         |

## Methods
### init(): `void`
Initializes the application when bootstrapping.

### terminate(reason: `string`): `void`
Emits a termination notice on the object. 
This is intended to notify sub components about the termination of the application.