# TaskList      
  
**exported:** default      
**kind:** object      
**declaration:** let      
## Properties      
  
### tasks        
  
**Type:** [Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)        
**kind:** value        
  
  
  
### registeredIds        
  
**Type:** [Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)        
**kind:** value        
  
  
  
## Methods      
  
### last() => {?}        
  
**Type:**  id: string, work: Function         
**kind:** function        
  
  
  
  
### length() => {?}        
  
**Type:** number        
**kind:** function        
  
  
  
  
### constructor() => {[TaskList](./Module:-rendering::TaskList#tasklist)}        
  
**kind:** function        
  
Render TaskList to manage rendertaks and optionally track duplicates by ids.        
  
  
### push(task, [id]) => {[void](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**kind:** function        
  
| Name | Type |          
|------|------|          
| task | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) |        
| [id] | string|number|null |        
  
adds a new item to the task list.        
  
  
### unshift(task, ) => {?}        
  
**kind:** function        
  
| Name | Type |          
|------|------|          
| task | undefined |        
| undefined | undefined |        
  
undefined        
  
  
### flush() => {?}        
  
**kind:** function        
  
undefined        
  
  
### filter(callback) => {?}        
  
**kind:** function        
  
| Name | Type |          
|------|------|          
| callback | undefined |        
  
undefined        
  
  
### run() => {?}        
  
**kind:** function        
  
| Name | Type |          
|------|------|          
| undefined | undefined |        
  
undefined        
  
  
### getAll() => {?}        
  
**kind:** function        
  
undefined        
  
  
@lends module:RenderEngine.TaskList.prototype      
