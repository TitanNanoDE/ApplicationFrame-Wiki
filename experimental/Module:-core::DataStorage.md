# DataStorage      
  
**exported:** default      
**kind:** object      
**declaration:** const      
  
  
## Properties      
  
### 🚫 _value        
  
**Type:** *        
**kind:** value        
  
  
  
  
### 🚫 _filledCallbacks        
  
**Type:** [Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array).&lt;[Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype)&gt;        
**kind:** value        
  
  
  
  
### value        
  
**Type:** *        
**kind:** value        
  
  
  
  
### \_\_proto\_\_        
  
**Type:** [EventTarget](./Module:-core::EventTarget#eventtarget)        
**kind:** value        
  
  
  
  
## Methods      
  
### constructor() => {[DataStorage](./Module:-core::DataStorage#datastorage)}        
  
**kind:** function        
  
  
  
  
  
### fill(value) => {[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**kind:** function        
  
stores a value inside the DataStorage and triggers callbacks.        
  
| Name | Type | Description |          
|------|------|-------------|          
| value | * | any value can be stored |\n        
  
  
### when(callback) => {[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**Type:** ?        
**kind:** function        
  
Registers a callback which is executed everytime a value is filled into the DataStorage. If the DataStorage is already filled at the point of callback registration, the callback is invoced.        
  
| Name | Type | Description |          
|------|------|-------------|          
| callback | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) |   |\n        
  
  
### once(callback) => {[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**Type:** ?        
**kind:** function        
  
Registers a one time callback which is executed as soon as the DataStorage has been filled.        
  
| Name | Type | Description |          
|------|------|-------------|          
| callback | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) |   |\n        
  
  
### whenNext(callback) => {[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**Type:** ?        
**kind:** function        
  
Registers a one time callback for the next time the DataStorage is filled. This is usefull when waiting for an update.        
  
| Name | Type | Description |          
|------|------|-------------|          
| callback | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) |   |\n        
  
  
