# Catalog      
  
**exported:** default      
**kind:** object      
**declaration:** let      
  
  
## Properties      
  
### 🚫 _listeners        
  
**Type:** [Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array).&lt;[Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype)&gt;        
**kind:** value        
  
  
  
  
## Methods      
  
### _make() => {[void](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**kind:** function        
  
Stores key value pairs and emits events when ever a pair is assigned        
  
  
  
### on(event, listener) => {[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)}        
  
**kind:** function        
  
gives the ability to register an callback as soon as a event is fired        
  
| Name | Type | Description |          
|------|------|-------------|          
| event | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) |    the event to wait for |        
| listener | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) | the callback function |        
  
  
  
### add(key, value) => {[void](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**kind:** function        
  
assigns a new pair        
  
| Name | Type | Description |          
|------|------|-------------|          
| key | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) |   the key for the assignment |        
| value | * | any value can be stored |        
  
  
  
