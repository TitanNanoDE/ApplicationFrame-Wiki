A routable is a object that can be passed into the Router directly. Mostly this should be some kind of view component / controller.

## Properties
| Name                 | Trait   | Description                                                                  |
|----------------------|---------|------------------------------------------------------------------------------|
| isRoutedPersistently | boolean | indicates where ever the router should route this route persistently or not. |

## Methods
### onRouteEnter(path: `string`) => `void` 
This method will be called by a router once a transition into the route was triggered.

### onRouteLeave(path: `string`) => `void`
This method will be called by a router once a transition out of the route was triggered.

