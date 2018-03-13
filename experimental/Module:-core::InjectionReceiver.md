# InjectionReceiver      
  
**exported:** default      
**kind:** object      
**declaration:** const      
## Properties      
  
### 🚫 _injectedObjects        
  
**Type:** [Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)        
**kind:** value        
  
  
  
## Methods      
  
### constructor() => {[InjectionReceiver](./Module:-core::InjectionReceiver#injectionreceiver)}        
  
**kind:** function        
  
  
  
  
### inject(original, injected) => {[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**kind:** function        
  
| Name | Type |          
|------|------|          
| original | * |        
| injected | * |        
  
Injects a replacement dependency into the module that owns this InjectionReceiver.        
  
  
### injected(object) => {*}        
  
**kind:** function        
  
| Name | Type |          
|------|------|          
| object | * |        
  
returns the injected value for an original value        
  
  
Manages the injection of module dependencies.      
