# Application      
  
**exported:** default      
**kind:** object      
**declaration:** const      
## Properties      
  
### name        
  
**Type:** [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)        
**kind:** value        
  
Name of the application, other components can identify it.        
  
### version        
  
**Type:** [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)        
**kind:** value        
  
The current version of the application.        
  
### author        
  
**Type:** [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)        
**kind:** value        
  
Author meta data.        
  
### \_\_proto\_\_        
  
**Type:** [EventTarget](./Module:-core::EventTarget#eventtarget)        
**kind:** value        
  
  
  
## Methods      
  
### constructor() => {[Application](./Module:-core::Application#application)}        
  
**kind:** function        
  
Constructs the Application prototype.        
  
  
### ~~_make(args) => {[Application](./Module:-core::Application#application)}~~        
  
**kind:** function        
  
| Name | Type |          
|------|------|          
| args | [Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array).&lt;any&gt; |        
  
Do not use any more.        
@see module:core/Application~Application.constructor        
  
  
### init() => {[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**kind:** function        
  
Initializes the application when bootstrapping.        
  
  
### terminate(reason) => {[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**kind:** function        
  
| Name | Type |          
|------|------|          
| reason | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) |        
  
Emits a termination notice on the object. This is intended to notify sub components about the termination of the application.        
  
  
This prototype provides a base construct for the core of an ECMAScript application      
