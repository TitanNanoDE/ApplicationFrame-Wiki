# IndexedQueryCompiler      
  
**exported:** default      
**kind:** object      
**declaration:** const      
  
the query compiler for indexedDB requests.      
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
  
creates a new indexed query        
  
| Name | Type | Description |          
|------|------|-------------|          
| storeName | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | the store to query |          
| db | [Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise).&lt;[IDBDatabase](https://developer.mozilla.org/en-US/docs/Web/API/IDBDatabase)&gt; |   the db to query |\n        
  
  
### 🚫 _transformExclude(value, exclude) => {?}        
  
**kind:** function        
  
  
  
| Name | Type | Description |          
|------|------|-------------|          
| value | * |   [description] |          
| exclude | [boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean) | [description] |\n        
  
  
### where(indexName) => {[IndexedQueryCompiler](./Module:-IndexedDB::IndexedQueryCompiler#indexedquerycompiler)}        
  
**kind:** function        
  
adds a where clause to the query.        
  
| Name | Type | Description |          
|------|------|-------------|          
| indexName | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | the index to operate on |\n        
  
  
### equals(value) => {[IndexedQueryCompiler](./Module:-IndexedDB::IndexedQueryCompiler#indexedquerycompiler)}        
  
**kind:** function        
  
filters items from the result if the index doesn't match the given value.        
  
| Name | Type | Description |          
|------|------|-------------|          
| value | * | value to compare |\n        
  
  
### from(value, [exclude=false]) => {[IndexedQueryCompiler](./Module:-IndexedDB::IndexedQueryCompiler#indexedquerycompiler)}        
  
**kind:** function        
  
starts a new value range        
  
| Name | Type | Description |          
|------|------|-------------|          
| value | * |                 range start value |          
| [exclude=false] | Boolean | determines if the start value will be included in the range |\n        
  
  
### to(value, [exclude=false]) => {[IndexedQueryCompiler](./Module:-IndexedDB::IndexedQueryCompiler#indexedquerycompiler)}        
  
**kind:** function        
  
ends a value range        
  
| Name | Type | Description |          
|------|------|-------------|          
| value | * |                 end value of the range |          
| [exclude=false] | Boolean | determines if the end value will be included in the range |\n        
  
  
### lowerThan(value) => {[IndexedQueryCompiler](./Module:-IndexedDB::IndexedQueryCompiler#indexedquerycompiler)}        
  
**kind:** function        
  
filters items from the result where the index is lower than the given value        
  
| Name | Type | Description |          
|------|------|-------------|          
| value | * |   |\n        
  
  
### higherThan(value) => {[IndexedQueryCompiler](./Module:-IndexedDB::IndexedQueryCompiler#indexedquerycompiler)}        
  
**kind:** function        
  
filters items from the result where the index is higher than the given value        
  
| Name | Type | Description |          
|------|------|-------------|          
| value | * |   |\n        
  
  
### or(indexName) => {[IndexedQueryCompiler](./Module:-IndexedDB::IndexedQueryCompiler#indexedquerycompiler)}        
  
**kind:** function        
  
starts an or clause to query an additional index        
  
| Name | Type | Description |          
|------|------|-------------|          
| indexName | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | [description] |\n        
  
  
### sort(direction) => {[IndexedQueryCompiler](./Module:-IndexedDB::IndexedQueryCompiler#indexedquerycompiler)}        
  
**kind:** function        
  
applies a sort order to the query results        
  
| Name | Type | Description |          
|------|------|-------------|          
| direction | 'ASC'&#124;'DESC' | sort direction |\n        
  
  
### get(limit) => {[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise).&lt;[Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)&gt;}        
  
**kind:** function        
  
assembles the results based on the composed query        
  
| Name | Type | Description |          
|------|------|-------------|          
| limit | ...number | one or two arguments which represent the start and end of the result range |\n        
  
  
### 🚫 _execute(start, end) => {[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise).&lt;[Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)&gt;}        
  
**kind:** function        
  
  
  
| Name | Type | Description |          
|------|------|-------------|          
| start | [number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number) | start index |          
| end | [number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number) |   end index |\n        
  
  
