# NetworkRequest      
  
**exported:** default      
**kind:** object      
**declaration:** const      
  
A network request      
## Properties      
  
### 🚫 _body        
  
**Type:** [Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)        
**kind:** object        
  
  
  
  
### 🚫 _headers        
  
**Type:** [Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)        
**kind:** value        
  
  
  
  
### type        
  
**Type:** [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)        
**kind:** value        
  
  
  
  
### method        
  
**Type:** [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)        
**kind:** value        
  
  
  
  
### url        
  
**Type:** [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)        
**kind:** value        
  
  
  
  
### 🚫 _listeners        
  
**Type:** [Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array).&lt;[function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype)&gt;        
**kind:** value        
  
  
  
  
### completed        
  
**Type:** Boolean        
**kind:** value        
  
[completed description]        
  
  
### \_\_proto\_\_        
  
**Type:** [EventTarget](./Module:-core::EventTarget#eventtarget)        
**kind:** value        
  
  
  
  
## Methods      
  
### constructor(url, config) => {[NetworkRequest](./Module:-core::NetworkRequest#networkrequest)}        
  
**kind:** function        
  
The constructor for the NetworkRequest. It simply sets up the properties.        
  
| Name | Type | Description |          
|------|------|-------------|          
| url | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | the url this request should be made to |        
| config | [Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object) | addintional configuartion for the request |        
  
  
  
### ~~_make(args) => {[void](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}~~        
  
**kind:** function        
  
use the constructor        
[_make description]        
  
| Name | Type | Description |          
|------|------|-------------|          
| args | array | [description] |        
  
  
  
### body(data) => {[NetworkRequest](./Module:-core::NetworkRequest#networkrequest)}        
  
**kind:** function        
  
this method will set the given object as the request body.        
  
| Name | Type | Description |          
|------|------|-------------|          
| data | [Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object) | body data for this request |        
  
  
  
### headers(headers) => {[NetworkRequest](./Module:-core::NetworkRequest#networkrequest)}        
  
**kind:** function        
  
This method will set the request headers, in case custom headers are required.        
  
| Name | Type | Description |          
|------|------|-------------|          
| headers | [Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object) | a object with all header properties for this request |        
  
  
  
### setHeader(key, value) => {[NetworkRequest](./Module:-core::NetworkRequest#networkrequest)}        
  
**kind:** function        
  
Sets a single header for this request.        
  
| Name | Type | Description |          
|------|------|-------------|          
| key | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | the header key |        
| value | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | the header value |        
  
  
  
### onReady(fn) => {[void](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**kind:** function        
  
sets a callback for when the request is ready        
  
| Name | Type | Description |          
|------|------|-------------|          
| fn | [function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype) | a callback function as soon as the data is ready |        
  
  
  
### send() => {[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)}        
  
**kind:** function        
  
This will actually create the network connection and initiate the request.        
  
  
  
