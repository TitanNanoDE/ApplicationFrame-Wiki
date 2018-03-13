# IndexedQuery        
  
**kind:** object        
**declaration:** const        
## Properties        
  
### name          
  
**Type:** [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)          
**kind:** value          
  
  
  
### rangeStart          
  
**Type:** *          
**kind:** value          
  
  
  
### rangeEnd          
  
**Type:** *          
**kind:** value          
  
  
  
## Methods        
  
  
  
A query object for an indexedDB request.        
# IndexedQueryCompiler      
  
**exported:** default      
**kind:** object      
**declaration:** const      
## Properties      
  
### 🚫 _currentQuery        
  
**Type:** [IndexedQuery](./Module:-IndexedDB::IndexedQueryCompiler#indexedquery)        
**kind:** value        
  
  
  
### 🚫 _allQueries        
  
**Type:** [Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array).&lt;[IndexedQuery](./Module:-IndexedDB::IndexedQueryCompiler#indexedquery)&gt;        
**kind:** value        
  
  
  
### 🚫 _store        
  
**Type:** [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)        
**kind:** value        
  
  
  
### 🚫 _db        
  
**Type:** [Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise).&lt;[IDBDatabase](https://developer.mozilla.org/en-US/docs/Web/API/IDBDatabase)&gt;        
**kind:** value        
  
  
  
### sortOrder        
  
**Type:** [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)        
**kind:** value        
  
  
  
## Methods      
  
### _make(storeName, db) => {[undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)}        
  
**kind:** function        
  
| Name | Type |          
|------|------|          
| storeName | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) |        
| db | [IDBDatabase](https://developer.mozilla.org/en-US/docs/Web/API/IDBDatabase) |        
  
creates a new indexed query        
  
  
### 🚫 _transformExclude(value, exclude) => {[type]}        
  
**kind:** function        
  
| Name | Type |          
|------|------|          
| value | * |        
| exclude | [boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean) |        
  
  
  
  
### where(indexName) => {[IndexedQueryCompiler](./Module:-IndexedDB::IndexedQueryCompiler#indexedquerycompiler)}        
  
**kind:** function        
  
| Name | Type |          
|------|------|          
| indexName | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) |        
  
adds a where clause to the query.        
  
  
### equals(value) => {[IndexedQueryCompiler](./Module:-IndexedDB::IndexedQueryCompiler#indexedquerycompiler)}        
  
**kind:** function        
  
| Name | Type |          
|------|------|          
| value | * |        
  
filters items from the result if the index doesn't match the given value.        
  
  
### from(value, [exclude=false]) => {[IndexedQueryCompiler](./Module:-IndexedDB::IndexedQueryCompiler#indexedquerycompiler)}        
  
**kind:** function        
  
| Name | Type |          
|------|------|          
| value | * |        
| [exclude=false] | Boolean |        
  
starts a new value range        
  
  
### to(value, [exclude=false]) => {[IndexedQueryCompiler](./Module:-IndexedDB::IndexedQueryCompiler#indexedquerycompiler)}        
  
**kind:** function        
  
| Name | Type |          
|------|------|          
| value | * |        
| [exclude=false] | Boolean |        
  
ends a value range        
  
  
### lowerThan(value) => {[IndexedQueryCompiler](./Module:-IndexedDB::IndexedQueryCompiler#indexedquerycompiler)}        
  
**kind:** function        
  
| Name | Type |          
|------|------|          
| value | * |        
  
filters items from the result where the index is lower than the given value        
  
  
### higherThan(value) => {[IndexedQueryCompiler](./Module:-IndexedDB::IndexedQueryCompiler#indexedquerycompiler)}        
  
**kind:** function        
  
| Name | Type |          
|------|------|          
| value | * |        
  
filters items from the result where the index is higher than the given value        
  
  
### or(indexName) => {[IndexedQueryCompiler](./Module:-IndexedDB::IndexedQueryCompiler#indexedquerycompiler)}        
  
**kind:** function        
  
| Name | Type |          
|------|------|          
| indexName | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) |        
  
starts an or clause to query an additional index        
  
  
### sort(direction) => {IndexedDefinition}        
  
**kind:** function        
  
| Name | Type |          
|------|------|          
| direction | 'ASC'&#124;'DESC' |        
  
applies a sort order to the query results        
  
  
### get(limit) => {[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise).&lt;[Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)&gt;}        
  
**kind:** function        
  
| Name | Type |          
|------|------|          
| limit | ...number |        
  
assembles the results based on the composed query        
  
  
### 🚫 _execute(start, end) => {[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise).&lt;[Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)&gt;}        
  
**kind:** function        
  
| Name | Type |          
|------|------|          
| start | [number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number) |        
| end | [number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number) |        
  
  
  
  
the query compiler for indexedDB requests.      
