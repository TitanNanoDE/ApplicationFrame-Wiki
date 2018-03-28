# preRenderHooks                        
  
**Type:** [Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array).&lt;[Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype)&gt;                        
**kind:** value                        
**declaration:** let                        
  
  
  
# postRenderHooks                      
  
**Type:** [Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array).&lt;[Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype)&gt;                      
**kind:** value                      
**declaration:** let                      
  
  
  
# currentFrameInterface                    
  
**Type:** [CurrentFrameInterface](./Module:-rendering::CurrentFrameInterface#currentframeinterface)                    
**kind:** value                    
**declaration:** let                    
  
  
  
# frameBuffer                  
  
**Type:** [Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array).&lt;[Frame](./Module:-rendering::Frame#frame)&gt;                  
**kind:** value                  
**declaration:** const                  
  
  
  
# active                
  
**Type:** [boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)                
**kind:** value                
**declaration:** let                
  
  
  
# getNow() => {?}              
  
**kind:** function              
**declaration:** const              
  
  
  
# renderConfig            
  
**kind:** object            
**declaration:** const            
  
  
## Properties            
  
### lightray              
  
**Type:** [boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)              
**kind:** value              
  
  
  
  
## Methods            
  
  
  
# renderCycle(startTime) => {[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}          
  
**kind:** function          
**declaration:** let          
  
performs all render tasks from one frame. This is one render cycle.          
  
| Name | Type | Description |            
|------|------|-------------|            
| startTime | [number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number) | the time the render cycle started |          
  
# scheduleNextFrame() => {[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**kind:** function        
**declaration:** let        
  
Schedules a new render cycle in the browsers rendering engine. The cycle is performed as soon as the browser is ready to render a new frame.        
  
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
| f | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) | a hook function to execute before each render cycle |        
  
  
  
### addPostRenderHook(f) => {[Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype)}        
  
**kind:** function        
  
  
  
| Name | Type | Description |          
|------|------|-------------|          
| f | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) | a hook function to execute after each render cycle |        
  
  
  
### removePreRenderHook(f) => {*}        
  
**kind:** function        
  
Removes a previously added pre render hook        
  
| Name | Type | Description |          
|------|------|-------------|          
| f | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) | the function which was previously added |        
  
  
  
### removePostRenderHook(f) => {*}        
  
**kind:** function        
  
Removes a previously added post render hook        
  
| Name | Type | Description |          
|------|------|-------------|          
| f | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) | the function which was previously added |        
  
  
  
### schedulePreRenderTask(f, [id]) => {[Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype)}        
  
**kind:** function        
  
  
  
| Name | Type | Description |          
|------|------|-------------|          
| f | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) | the task to preform in the next render cycle. |        
| [id] | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | optional task id |        
  
  
  
### scheduleRenderTask(f, [id]) => {[Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype)}        
  
**kind:** function        
  
  
  
| Name | Type | Description |          
|------|------|-------------|          
| f | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) | the task to preform in the next render cycle. |        
| [id] | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | optional task id |        
  
  
  
### schedulePostRenderTask(f) => {[Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype)}        
  
**kind:** function        
  
  
  
| Name | Type | Description |          
|------|------|-------------|          
| f | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) | the task to preform after the next render cycle. |        
  
  
  
### renderFrame() => {[void](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**kind:** function        
  
Forces the engine to render a new frame even if there are no tasks        
  
  
  
### skipFrame() => {[RenderEngine](./Module:-rendering::index#renderengine)}        
  
**kind:** function        
  
skips the current frame and provices scheduling methods for the next frame.        
  
  
  
