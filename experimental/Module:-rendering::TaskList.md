# TaskList      
  
**exported:** default      
**kind:** object      
**declaration:** let      
  
  
## Properties      
  
### tasks        
  
**Type:**  id: *, work: Function         
**kind:** value        
  
  
  
  
### registeredIds        
  
**Type:** [Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)        
**kind:** value        
  
  
  
  
### last        
  
**Type:**  id: string, work: Function         
**kind:** value        
  
  
  
  
### length        
  
**Type:** [number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)        
**kind:** value        
  
  
  
  
## Methods      
  
### constructor() => {[TaskList](./Module:-rendering::TaskList#tasklist)}        
  
**kind:** function        
  
Render TaskList to manage rendertaks and optionally track duplicates by ids.        
  
  
  
### push(task, [id]) => {[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**kind:** function        
  
adds a new item to the task list.        
  
| Name | Type | Description |          
|------|------|-------------|          
| task | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) | the task to add to the list |        
| [id] | * | the id of this tasks. If provided no task with the same id can be added again. |        
  
  
  
### unshift(task, [id=null]) => {[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**kind:** function        
  
adds a new task to the beginning of the list        
  
| Name | Type | Description |          
|------|------|-------------|          
| task | Function} |      [description] |        
| [id=null] | * | [description] |        
  
  
  
### flush() => {[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**kind:** function        
  
clears the task list        
  
  
  
### filter(callback) => {[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**kind:** function        
  
Filters out tasks that do not satisfy the condition.        
  
| Name | Type | Description |          
|------|------|-------------|          
| callback | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) |   |        
  
  
  
### run(args) => {[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**kind:** function        
  
Runs all tasks but keeps tasks, which didn't complete, in the list.        
  
| Name | Type | Description |          
|------|------|-------------|          
| args | ...* | arguments for the task execution |        
  
  
  
### getAll() => {?}        
  
**kind:** function        
  
  
  
  
  
