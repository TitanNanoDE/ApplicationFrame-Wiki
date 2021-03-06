# IndexedDB      
  
**exported:** default      
**kind:** object      
**declaration:** const      
  
  
## Properties      
  
### 🚫 _name        
  
**Type:** [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)        
**kind:** value        
  
the name of the current db        
  
  
### 🚫 _definitions        
  
**Type:** [Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array).&lt;[Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/prototype)&gt;        
**kind:** value        
  
  
  
  
## Methods      
  
### 🚫 _setup() => {[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise).&lt;[IDBDatabase](https://developer.mozilla.org/en-US/docs/Web/API/IDBDatabase)&gt;}        
  
**kind:** function        
  
runs all db setup tasks        
  
  
  
### constructor(name) => {[IndexedDB](./Module:-IndexedDB::index#indexeddb)}        
  
**kind:** function        
  
Instantiates a new indexed DB. All version definitions have to be made done synchronously. The actual database creation is immediately scheduled for the next event cycle.        
  
| Name | Type | Description |          
|------|------|-------------|          
| name | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | of the db to open |\n        
  
  
### ~~_make(args) => {[IndexedDB](./Module:-IndexedDB::index#indexeddb)}~~        
  
**kind:** function        
  
  
  
| Name | Type | Description |          
|------|------|-------------|          
| args | ...any |   |\n        
  
  
### define(version) => {[IndexedDefinition](./Module:-IndexedDB::index#indexeddefinition)}        
  
**kind:** function        
  
Creates a new version definition for the DB. All stores and indexes for the current version have to be defined in this definition.        
  
| Name | Type | Description |          
|------|------|-------------|          
| version | [number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number) | the version to be defined, don't use floats |\n        
  
  
### read(storeName) => {[IndexedQueryCompiler](./Module:-IndexedDB::IndexedQueryCompiler#indexedquerycompiler)}        
  
**kind:** function        
  
Creates a new query to the database. The store which should be queried from has to be specified.        
  
| Name | Type | Description |          
|------|------|-------------|          
| storeName | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | to read from |\n        
  
  
### write(storeName, value) => {[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)}        
  
**kind:** function        
  
Stores an object in the selected store. The promise resolves to the transaction result.        
  
| Name | Type | Description |          
|------|------|-------------|          
| storeName | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | name of the targeted store |          
| value | [object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object) |     value to store |\n        
  
  
### delete(storeName) => {[IndexedDeleteRangeCompiler](./Module:-IndexedDB::IndexedDeleteRangeCompiler#indexeddeleterangecompiler)}        
  
**kind:** function        
  
Removes objects which match the specified key range from the selected store. The key range is always matched against the stores primary key.        
  
| Name | Type | Description |          
|------|------|-------------|          
| storeName | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) |   |\n        
  
  
### clear(storeName) => {[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)}        
  
**kind:** function        
  
Removes all entries from the selected store.        
  
| Name | Type | Description |          
|------|------|-------------|          
| storeName | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) |   |\n        
  
  
### close() => {?}        
  
**kind:** function        
  
  
  
  
  
### upgrade(version) => {?}        
  
**kind:** function        
  
  
  
| Name | Type | Description |          
|------|------|-------------|          
| version | ? |   |\n        
  
  
