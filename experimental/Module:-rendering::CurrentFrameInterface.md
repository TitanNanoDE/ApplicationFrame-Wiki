# CurrentFrameInterface      
  
**exported:** default      
**kind:** object      
**declaration:** const      
  
An abstract representation of the currently rendering frame      
## Properties      
  
### 🚫 _startTime        
  
**Type:** [number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)        
**kind:** value        
  
  
  
  
### 🚫 _maxFrameDuration        
  
**Type:** [number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)        
**kind:** value        
  
  
  
  
### INTERUPT_CURRENT_TASK        
  
  
  
  
  
## Methods      
  
### constructor(startTime, maxFrameDuration) => {[CurrentFrameInterface](./Module:-rendering::CurrentFrameInterface#currentframeinterface)}        
  
**kind:** function        
  
  
  
| Name | Type | Description |          
|------|------|-------------|          
| startTime | [number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number) |    the time the current frame has started rendering |          
| maxFrameDuration | [number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number) | the maximum duration |\n        
  
  
### ttl() => {[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)}        
  
**kind:** function        
  
the remaining available render time of the frame        
  
  
  
