# IndexedStoreDefinition          
  
**kind:** object          
**declaration:** const          
  
  
## Properties          
  
### name            
  
**Type:** [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)            
**kind:** value            
  
  
  
  
### indexes            
  
**Type:** ?            
**kind:** value            
  
  
  
  
## Methods          
  
### _make(info) => {?}            
  
**kind:** function            
  
  
  
| Name | Type | Description |              
|------|------|-------------|              
| info | ? |   |            
  
  
  
# IndexedDefinition        
  
**kind:** object        
**declaration:** const        
  
  
## Properties        
  
### 🚫 _version          
  
**Type:** [number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)          
**kind:** value          
  
  
  
  
### 🚫 _currentStore          
  
**Type:** [IndexedStoreDefinition](./Module:-IndexedDB::index#indexedstoredefinition)          
**kind:** value          
  
  
  
  
### 🚫 _allStores          
  
**Type:** [Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array).&lt;[IndexedStoreDefinition](./Module:-IndexedDB::index#indexedstoredefinition)&gt;          
**kind:** value          
  
  
  
  
## Methods        
  
### _make(version) => {[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}          
  
**kind:** function          
  
Instantiates a new DB version.          
  
| Name | Type | Description |            
|------|------|-------------|            
| version | [number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number) |   |          
  
  
  
### store(info) => {[IndexedDefinition](./Module:-IndexedDB::index#indexeddefinition)}          
  
**kind:** function          
  
Creates a new store definition. Inside the store definition new indexes can be defined.          
  
| Name | Type | Description |            
|------|------|-------------|            
| info | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)&#124;{ name: [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String), keyPath: [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String), autoincrement: [boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean) } |   |          
  
  
  
### index(name, members, options) => {[IndexedDefinition](./Module:-IndexedDB::index#indexeddefinition)}          
  
**kind:** function          
  
Creates a new index in the last defined store. This has been chosen to be able to chain together all definition calls.          
  
| Name | Type | Description |            
|------|------|-------------|            
| name | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) |  name of the new index |          
| members | [Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array).&lt;[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)&gt; | [description] |          
| options | [Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object) | [description] |          
  
  
  
### 🚫 _execute(db, transaction) => {[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}          
  
**kind:** function          
  
executes the definition and creates the required stores and indexes          
  
| Name | Type | Description |            
|------|------|-------------|            
| db | [IDBDatabase](https://developer.mozilla.org/en-US/docs/Web/API/IDBDatabase) |          the db object to operate on |          
| transaction | [IDBTransaction](https://developer.mozilla.org/en-US/docs/Web/API/IDBTransaction) | the db transaction |          
  
  
  
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
  
  
  
### constructor(name) => {?}        
  
**kind:** function        
  
Instantiates a new indexed DB. All version definitions have to be made done synchronously. The actual database creation is immediately scheduled for the next event cycle.        
  
| Name | Type | Description |          
|------|------|-------------|          
| name | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | of the db to open |        
  
  
  
### ~~_make() => {?}~~        
  
**kind:** function        
  
  
  
  
  
### define(version) => {[IndexedDefinition](./Module:-IndexedDB::index#indexeddefinition)}        
  
**kind:** function        
  
Creates a new version definition for the DB. All stores and indexes for the current version have to be defined in this definition.        
  
| Name | Type | Description |          
|------|------|-------------|          
| version | [number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number) | the version to be defined, don't use floats |        
  
  
  
### read(storeName) => {[IndexedQueryCompiler](./Module:-IndexedDB::IndexedQueryCompiler#indexedquerycompiler)}        
  
**kind:** function        
  
Creates a new query to the database. The store which should be queried from has to be specified.        
  
| Name | Type | Description |          
|------|------|-------------|          
| storeName | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | to read from |        
  
  
  
### write(storeName, value) => {[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)}        
  
**kind:** function        
  
Stores an object in the selected store. The promise resolves to the transaction result.        
  
| Name | Type | Description |          
|------|------|-------------|          
| storeName | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | name of the targeted store |        
| value | [Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object) |     value to store |        
  
  
  
