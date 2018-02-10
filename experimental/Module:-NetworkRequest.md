# EventTarget              
  
**Type:** default              
**kind:** import              
  
  
#             
  
  
@module core/NetworkRequest            
# stripHashKey(object) => {Object}          
  
**kind:** function          
**declaration:** const          
  
| Name | Type |            
|------|------|            
| object | Object |          
  
removes angulars hashKey property from an object          
# NetworkRequest        
  
**exported:** default        
**kind:** object        
**declaration:** const        
## Properties        
  
### _body          
  
**Type:** Object          
**kind:** object          
  
@private          
  
### _headers          
  
**Type:** Object          
**kind:** value          
  
@private          
  
### type          
  
**Type:** [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)          
**kind:** value          
  
  
  
### method          
  
**Type:** [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)          
**kind:** value          
  
  
  
### url          
  
**Type:** [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)          
**kind:** value          
  
  
  
### _listeners          
  
**Type:** function[]          
**kind:** value          
  
@private          
  
### completed          
  
**Type:** Boolean          
**kind:** value          
  
[completed description]          
  
### \_\_proto\_\_          
  
**Type:** [EventTarget](./Module:-EventTarget.md#EventTarget)          
**kind:** value          
  
undefined          
  
## Methods        
  
### constructor(url, config) => {[NetworkRequest](./Module:-NetworkRequest.md#NetworkRequest)}          
  
**kind:** function          
  
| Name | Type |            
|------|------|            
| url | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) |          
| config | Object |          
  
The constructor for the NetworkRequest. It simply sets up the properties.          
  
  
### _make(args) => {[void](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}          
  
**kind:** function          
  
| Name | Type |            
|------|------|            
| args | array |          
  
[_make description]  @deprecated use the constructor          
  
  
### body(data) => {[NetworkRequest](./Module:-NetworkRequest.md#NetworkRequest)}          
  
**kind:** function          
  
| Name | Type |            
|------|------|            
| data | Object |          
  
this method will set the given object as the request body.          
  
  
### headers(headers) => {[NetworkRequest](./Module:-NetworkRequest.md#NetworkRequest)}          
  
**kind:** function          
  
| Name | Type |            
|------|------|            
| headers | Object |          
  
This method will set the request headers, in case custom headers are required.          
  
  
### setHeader(key, value) => {[NetworkRequest](./Module:-NetworkRequest.md#NetworkRequest)}          
  
**kind:** function          
  
| Name | Type |            
|------|------|            
| key | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) |          
| value | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) |          
  
Sets a single header for this request.          
  
  
### onReady(fn) => {[void](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}          
  
**kind:** function          
  
| Name | Type |            
|------|------|            
| fn | [function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) |          
  
sets a callback for when the request is ready          
  
  
### send() => {[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)}          
  
**kind:** function          
  
This will actually create the network connection and initiate the request.          
  
  
A network request @extends EventTarget        
#       
  
  
the default export      
