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
  
| Name | Type |          
|------|------|          
| type | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) |        
| listener | [function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) |        
  
registers a new listener for the given event.        
  
  
### emit(type, data) => {[void](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**kind:** function        
  
| Name | Type |          
|------|------|          
| type | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) |        
| data | * |        
  
emmits a new event on this object        
  
  
### removeListener(type, listener) => {[void](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**kind:** function        
  
| Name | Type |          
|------|------|          
| type | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) |        
| listener | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) |        
  
removes a previously attached listener function.        
  
  
  
