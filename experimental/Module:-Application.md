# EventTarget        
  
**Type:** default        
**kind:** import        
  
  
# Application      
  
**exported:** default      
**kind:** object      
**declaration:** const      
## Properties      
  
### name        
  
**Type:** [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)        
**kind:** value        
  
Name of this application so other components can identify the application.        
  
### version        
  
**Type:** [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)        
**kind:** value        
  
Some components may need to know the version of this applicaion.        
  
### author        
  
**Type:** [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)        
**kind:** value        
  
  
  
### \_\_proto\_\_        
  
**Type:** [EventTarget](Module:-EventTarget.md#EventTarget)        
**kind:** value        
  
[\_\_proto\_\_ description]        
  
## Methods      
  
### constructor() => {[Application](Module:-Application.md#Application)}        
  
**kind:** function        
  
Constructs the Application prototype.        
  
  
### _make(args) => {[Application](Module:-Application.md#Application)}        
  
**kind:** function        
  
| Name | Type |          
|------|------|          
| args | any[] |        
  
@deprecated Do not use any more. @see module:core/Application~Application.constructor        
  
  
### init() => {[void](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**kind:** function        
  
Initializes this application, default interface for components and modules.        
  
  
### terminate(reason) => {[void](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**kind:** function        
  
| Name | Type |          
|------|------|          
| reason | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) |        
  
This function will try to terminate the application by emitting the termination event.        
  
  
This prototype provides a base construct for the core of an ECMAScript applicaion      
