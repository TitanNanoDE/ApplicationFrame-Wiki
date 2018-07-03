# RenderEngine      
  
**exported:** RenderEngine      
**kind:** object      
**declaration:** const      
  
RenderEngine Singleton      
## Properties      
  
### 🚫 _currentFrame        
  
**Type:** [number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)        
**kind:** value        
  
  
  
  
### lightray        
  
**Type:** [boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)        
**kind:** value        
  
  
  
  
### lightray        
  
**kind:** setter        
  
  
  
  
### performance        
  
**kind:** object        
  
  
#### Properties        
  
##### fps          
  
**Type:** [number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)          
**kind:** value          
  
  
  
  
##### lastFrameDuration          
  
**Type:** [number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)          
**kind:** value          
  
  
  
  
##### renderedFrames          
  
**Type:** [number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)          
**kind:** value          
  
  
  
  
#### Methods        
  
  
  
  
## Methods      
  
### addPreRenderHook(f) => {[Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype)}        
  
**kind:** function        
  
  
  
| Name | Type | Description |          
|------|------|-------------|          
| f | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) | a hook function to execute before each render cycle |\n        
  
  
### addPostRenderHook(f) => {[Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype)}        
  
**kind:** function        
  
  
  
| Name | Type | Description |          
|------|------|-------------|          
| f | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) | a hook function to execute after each render cycle |\n        
  
  
### removePreRenderHook(f) => {*}        
  
**kind:** function        
  
Removes a previously added pre render hook        
  
| Name | Type | Description |          
|------|------|-------------|          
| f | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) | the function which was previously added |\n        
  
  
### removePostRenderHook(f) => {*}        
  
**kind:** function        
  
Removes a previously added post render hook        
  
| Name | Type | Description |          
|------|------|-------------|          
| f | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) | the function which was previously added |\n        
  
  
### schedulePreRenderTask(f, [id]) => {[Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype)}        
  
**kind:** function        
  
  
  
| Name | Type | Description |          
|------|------|-------------|          
| f | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) | the task to preform in the next render cycle. |          
| [id] | * | optional task id |\n        
  
  
### scheduleRenderTask(f, [id]) => {[Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype)}        
  
**kind:** function        
  
  
  
| Name | Type | Description |          
|------|------|-------------|          
| f | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) | the task to preform in the next render cycle. |          
| [id] | * | optional task id |\n        
  
  
### schedulePostRenderTask(f) => {[Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype)}        
  
**kind:** function        
  
  
  
| Name | Type | Description |          
|------|------|-------------|          
| f | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) | the task to preform after the next render cycle. |\n        
  
  
### renderFrame() => {[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**kind:** function        
  
Forces the engine to render a new frame even if there are no tasks        
  
  
  
### skipFrame() => {[RenderEngine](./Module:-rendering::index#renderengine)}        
  
**kind:** function        
  
skips the current frame and provices scheduling methods for the next frame.        
  
  
  
