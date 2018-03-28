# EventTarget      
  
**exported:** default      
**kind:** object      
**declaration:** const      
  
  
## Properties      
  
### 🚫 _listeners        
  
**Type:** [Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)        
**kind:** value        
  
  
  
  
## Methods      
  
### constructor() => {[EventTarget](./Module:-core::EventTarget#eventtarget)}        
  
**kind:** function        
  
  
  
  
  
### ~~_make() => {this}~~        
  
**kind:** function        
  
Do not use the make constructors        
  
  
  
### on(type, listener) => {[void](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**kind:** function        
  
registers a new listener for the given event.        
  
| Name | Type | Description |          
|------|------|-------------|          
| type | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | the type of event |        
| listener | [function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) | callback to execute when the event fires |        
  
  
  
### emit(type, data) => {[void](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**kind:** function        
  
emmits a new event on this object        
  
| Name | Type | Description |          
|------|------|-------------|          
| type | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | the type of event |        
| data | * | data to send to the callbacks |        
  
  
  
### removeListener(type, listener) => {[void](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**kind:** function        
  
removes a previously attached listener function.        
  
| Name | Type | Description |          
|------|------|-------------|          
| type | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) |     the listener type |        
| listener | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) | the listener function to remove |        
  
  
  
