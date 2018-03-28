# heapObjects                  
  
**declaration:** const                  
  
  
  
# heapObjectsReleased                
  
**kind:** object                
**declaration:** const                
  
  
  
# heapArrays              
  
**declaration:** const              
  
  
  
# heapArraysReleased            
  
**Type:** [Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)            
**kind:** value            
**declaration:** const            
  
  
  
# allocate(typeOrLength, [prototype={}]) => {*}          
  
**exported:** allocate          
**kind:** function          
**declaration:** const          
  
Allocates objects and arrays in memory. The allocated structures are excluded from garbage collection.          
  
| Name | Type | Description |            
|------|------|-------------|            
| typeOrLength | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)&#124;[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number) | either the length of an array, or a string identifying an object type. |          
| [prototype={}] | [Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object) | the structures prototype |          
  
# release(object) => {[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**exported:** release        
**kind:** function        
**declaration:** const        
  
Marks he given structure as unused and therefore available for usage. If a new array or object is to be allocated the released items will be reused, before an actual new object is created.        
  
| Name | Type | Description |          
|------|------|-------------|          
| object | * | data to be released |        
  
# flushHeap() => {[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}      
  
**exported:** flushHeap      
**kind:** function      
**declaration:** const      
  
Makes all released object available for garbage collection.      
  
