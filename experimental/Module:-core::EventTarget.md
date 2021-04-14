# EventTarget      
  
**exported:** default      
**kind:** object      
**declaration:** const      
  
  
## Properties      
  
### 🚫 _listeners        
  
**Type:** [object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)        
**kind:** value        
  
  
  
  
## Methods      
  
### constructor() => {[EventTarget](./Module:-core::EventTarget#eventtarget)}        
  
**kind:** function        
  
  
  
  
  
### ~~_make(args) => {this}~~        
  
**kind:** function        
  
Do not use the make constructors        
  
| Name | Type | Description |          
|------|------|-------------|          
| args | ...* |   |\n        
  
  
### on(type, listener) => {[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**kind:** function        
  
registers a new listener for the given event        
  
| Name | Type | Description |          
|------|------|-------------|          
| type | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | the type / name of event |          
| listener | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) | callback to execute when the event fires |\n        
  
  
### emit(type, data) => {[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**kind:** function        
  
emmits a new event on this object        
  
| Name | Type | Description |          
|------|------|-------------|          
| type | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | the type of event |          
| data | * | data to send to the callbacks |\n        
  
  
### removeListener(type, listener) => {[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**kind:** function        
  
removes a previously attached listener function.        
  
| Name | Type | Description |          
|------|------|-------------|          
| type | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) |     the listener type |          
| listener | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) | the listener function to remove |\n        
  
  
