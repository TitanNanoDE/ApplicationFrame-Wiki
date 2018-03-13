# thenHandler(callback) => {?}                
  
**kind:** function                
**declaration:** const                
  
| Name | Type |                  
|------|------|                  
| callback | ? |                
  
fake then if this should be handed to something that expects a promise                
# catchHandler(callback) => {?}              
  
**kind:** function              
**declaration:** const              
  
| Name | Type |                
|------|------|                
| callback | ? |              
  
dummy catch in case someone tries to use it              
# whenFilled(target) => {?}            
  
**kind:** function            
**declaration:** const            
  
| Name | Type |              
|------|------|              
| target | ? |            
  
  
# whenNext(target) => {?}          
  
**kind:** function          
**declaration:** const          
  
| Name | Type |            
|------|------|            
| target | ? |          
  
  
# once(target) => {?}        
  
**kind:** function        
**declaration:** const        
  
| Name | Type |          
|------|------|          
| target | ? |        
  
  
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
  
  
  
### when        
  
**Type:** ?        
**kind:** value        
  
| Name | Type |          
|------|------|          
| callback | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) |        
  
Registers a callback which is executed everytime a value is filled into the DataStorage. If the DataStorage is already filled at the point of callback registration, the callback is invoced.        
  
### once        
  
**Type:** ?        
**kind:** value        
  
| Name | Type |          
|------|------|          
| callback | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) |        
  
Registers a one time callback which is executed as soon as the DataStorage has been filled.        
  
### whenNext        
  
**Type:** ?        
**kind:** value        
  
| Name | Type |          
|------|------|          
| callback | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) |        
  
Registers a one time callback for the next time the DataStorage is filled. This is usefull when waiting for an update.        
  
### \_\_proto\_\_        
  
**Type:** [EventTarget](./Module:-core::EventTarget#eventtarget)        
**kind:** value        
  
  
  
## Methods      
  
### value() => {?}        
  
**Type:** *        
**kind:** function        
  
  
  
  
### constructor() => {[DataStorage](./Module:-core::DataStorage#datastorage)}        
  
**kind:** function        
  
  
  
  
### fill(value) => {[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**kind:** function        
  
| Name | Type |          
|------|------|          
| value | * |        
  
[fill description]        
  
  
  
