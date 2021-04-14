# ServiceWorker      
  
**exported:** default      
**kind:** object      
**declaration:** const      
  
The current service worker of the site      
## Properties      
  
### script        
  
**Type:** [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)        
**kind:** value        
  
  
  
  
### scope        
  
**Type:** (boolean&#124;string)        
**kind:** value        
  
- true: the scope is extracted from the mainfest file - false: the ServiceWorker is registered without a scope - string: the string is applied as scope  defaults to true        
  
  
### isSupported        
  
**kind:** value        
  
  
  
  
### PushManager        
  
**Type:** [PushManager](./Module:-ServiceWorker::PushManager#pushmanager)        
**kind:** value        
  
  
  
  
### NotificationManager        
  
**Type:** [NotificationManager](./Module:-ServiceWorker::NotificationManager#notificationmanager)        
**kind:** value        
  
  
  
  
### \_\_proto\_\_        
  
**Type:** [ServiceWorkerEventTarget](./Module:-ServiceWorker::lib::ServiceWorkerEventTarget#serviceworkereventtarget)        
**kind:** value        
  
  
  
  
## Methods      
  
### init() => {Promise<ServiceWorkerRegistration>}        
  
**kind:** function        
  
initialize the service worker. If no ServiceWorker is registered yet, it will be during the initialization.        
  
  
  
### checkUpdate() => {[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)}        
  
**kind:** function        
  
check if there is a pending service worker update that can be installed        
  
  
  
### remove() => {[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)}        
  
**kind:** function        
  
unregisters the service worker from the browser.        
  
  
  
### consume(object) => {[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**kind:** function        
  
consumes an application object. By consuming the application all events of both the service worker and the application are shared between the two. This allows independent applications (i.e. in seperated tabs) to operate as one.        
  
| Name | Type | Description |          
|------|------|-------------|          
| object | ApplicationTrait |   |\n        
  
  
