#                               
  
  
@module RenderEngine                              
# preRenderHooks                            
  
**Type:** Function[]                            
**kind:** value                            
**declaration:** let                            
  
  
# postRenderHooks                          
  
**Type:** Function[]                          
**kind:** value                          
**declaration:** let                          
  
  
# currentFrameInterface                        
  
**Type:** [CurrentFrameInterface](./Module:-rendering::CurrentFrameInterface#currentframeinterface)                        
**kind:** value                        
**declaration:** let                        
  
  
# frameBuffer                      
  
**Type:** [Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)                      
**kind:** value                      
**declaration:** const                      
  
undefined                      
# active                    
  
**Type:** [boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)                    
**kind:** value                    
**declaration:** let                    
  
  
# getNow() => {?}                  
  
**kind:** function                  
**declaration:** const                  
  
undefined                  
# renderConfig                
  
**kind:** object                
**declaration:** const                
## Properties                
  
### lightray                  
  
**Type:** [boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)                  
**kind:** value                  
  
undefined                  
  
## Methods                
  
  
  
undefined                
# renderCycle(startTime) => {[void](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}              
  
**kind:** function              
**declaration:** let              
  
| Name | Type |                
|------|------|                
| startTime | number |              
  
performs all render tasks from one frame. This is one render cycle.              
# scheduleNextFrame() => {[void](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}            
  
**kind:** function            
**declaration:** let            
  
Schedules a new render cycle in the browsers rendering engine. The cycle is performed as soon as the browser is ready to render a new frame.            
# RenderEngine          
  
**exported:** true          
**kind:** object          
**declaration:** const          
## Properties          
  
### _currentFrame            
  
**Type:** number            
**kind:** value            
  
undefined            
  
### performance            
  
**kind:** object            
#### Properties            
  
##### fps              
  
**Type:** number              
**kind:** value              
  
undefined              
  
##### lastFrameDuration              
  
**Type:** number              
**kind:** value              
  
undefined              
  
##### renderedFrames              
  
**Type:** number              
**kind:** value              
  
undefined              
  
#### Methods            
  
  
  
undefined            
  
## Methods          
  
### lightray() => {?}            
  
**kind:** function            
  
undefined            
  
  
### lightray(value) => {?}            
  
**kind:** function            
  
| Name | Type |              
|------|------|              
| value | undefined |            
  
undefined            
  
  
### addPreRenderHook(f) => {[Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype)}            
  
**kind:** function            
  
| Name | Type |              
|------|------|              
| f | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) |            
  
  
  
  
### addPostRenderHook(f) => {[Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype)}            
  
**kind:** function            
  
| Name | Type |              
|------|------|              
| f | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) |            
  
  
  
  
### removePreRenderHook(f) => {*}            
  
**kind:** function            
  
| Name | Type |              
|------|------|              
| f | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) |            
  
Removes a previously added pre render hook            
  
  
### removePostRenderHook(f) => {*}            
  
**kind:** function            
  
| Name | Type |              
|------|------|              
| f | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) |            
  
Removes a previously added post render hook            
  
  
### schedulePreRenderTask(f, [id]) => {[Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype)}            
  
**kind:** function            
  
| Name | Type |              
|------|------|              
| f | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) |            
| [id] | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) |            
  
  
  
  
### scheduleRenderTask(f, [id]) => {[Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype)}            
  
**kind:** function            
  
| Name | Type |              
|------|------|              
| f | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) |            
| [id] | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) |            
  
  
  
  
### schedulePostRenderTask(f) => {[Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype)}            
  
**kind:** function            
  
| Name | Type |              
|------|------|              
| f | [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) |            
  
  
  
  
### renderFrame() => {[void](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}            
  
**kind:** function            
  
Forces the engine to render a new frame even if there are no tasks            
  
  
### skipFrame() => {?}            
  
**kind:** function            
  
undefined            
  
  
RenderEngine Singleton          
#         
  
  
init zero frame        
#       
  
  
@member {module:RenderEngine~RenderEngine} RenderEngine @static      
