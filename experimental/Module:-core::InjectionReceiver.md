# InjectionReceiver      
  
**exported:** default      
**kind:** object      
**declaration:** const      
  
Manages the injection of module dependencies.      
## Properties      
  
### 🚫 _injectedObjects        
  
**Type:** WeakMap<*, *>        
**kind:** value        
  
  
  
  
## Methods      
  
### constructor() => {[InjectionReceiver](./Module:-core::InjectionReceiver#injectionreceiver)}        
  
**kind:** function        
  
  
  
  
  
### inject(original, injected) => {[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**kind:** function        
  
Injects a replacement dependency into the module that owns this InjectionReceiver.        
  
| Name | Type | Description |          
|------|------|-------------|          
| original | * | the original value |          
| injected | * | the replacement value |\n        
  
  
### injected(object) => {*}        
  
**kind:** function        
  
returns the injected value for an original value        
  
| Name | Type | Description |          
|------|------|-------------|          
| object | * | the original value |\n        
  
  
