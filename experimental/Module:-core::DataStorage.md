# thenHandler(callback) => {?}                
  
**kind:** function                
**declaration:** const                
  
  
  
| Name | Type | Description |                  
|------|------|-------------|                  
| callback | ? |   |                
  
# catchHandler(callback) => {?}              
  
**kind:** function              
**declaration:** const              
  
  
  
| Name | Type | Description |                
|------|------|-------------|                
| callback | ? |   |              
  
# whenFilled(target) => {?}            
  
**kind:** function            
**declaration:** const            
  
  
  
| Name | Type | Description |              
|------|------|-------------|              
| target | ? |   |            
  
# whenNext(target) => {?}          
  
**kind:** function          
**declaration:** const          
  
  
  
| Name | Type | Description |            
|------|------|-------------|            
| target | ? |   |          
  
# once(target) => {?}        
  
**kind:** function        
**declaration:** const        
  
  
  
| Name | Type | Description |          
|------|------|-------------|          
| target | ? |   |        
  
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
  
[fill description]        
  
| Name | Type | Description |          
|------|------|-------------|          
| value | * | [description] |        
  
  
  
### when(callback) => {[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**Type:** ?        
**kind:** function        
  
Registers a callback which is executed everytime a value is filled into the DataStorage. If the DataStorage is already filled at the point of callback registration, the callback is invoced.        
  
| Name | Type | Description |          
|------|------|-------------|          
| callback | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) |   |        
  
  
  
### once(callback) => {[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**Type:** ?        
**kind:** function        
  
Registers a one time callback which is executed as soon as the DataStorage has been filled.        
  
| Name | Type | Description |          
|------|------|-------------|          
| callback | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) |   |        
  
  
  
### whenNext(callback) => {[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**Type:** ?        
**kind:** function        
  
Registers a one time callback for the next time the DataStorage is filled. This is usefull when waiting for an update.        
  
| Name | Type | Description |          
|------|------|-------------|          
| callback | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) |   |        
  
  
  
