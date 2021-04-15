# IndexedDeleteRangeCompiler      
  
**exported:** default      
**kind:** object      
**declaration:** const      
  
the range compiler for indexedDB delete operations.      
## Properties      
  
### 🚫 \[Private.db\]        
  
**Type:** [Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise).&lt;[IDBDatabase](https://developer.mozilla.org/en-US/docs/Web/API/IDBDatabase)&gt;        
**kind:** value        
  
  
  
  
### 🚫 \[Private.query\]        
  
**Type:** [IndexedQuery](./Module:-IndexedDB::IndexedQueryCompiler#indexedquery)        
**kind:** value        
  
  
  
  
### 🚫 \[Private.store\]        
  
**Type:** [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)        
**kind:** value        
  
  
  
  
## Methods      
  
### 🚫 \[Private.buildKeyRange\]() => {[IDBKeyRange](https://developer.mozilla.org/en-US/docs/Web/API/IDBKeyRange)}        
  
**kind:** function        
  
Builds a IDBKeyRange from an {IndexedQuery}        
  
  
  
### constructor(storeName, db) => {[IndexedDeleteRangeCompiler](./Module:-IndexedDB::IndexedDeleteRangeCompiler#indexeddeleterangecompiler)}        
  
**kind:** function        
  
creates a new indexed query        
  
| Name | Type | Description |          
|------|------|-------------|          
| storeName | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | the store to query |          
| db | [Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise).&lt;[IDBDatabase](https://developer.mozilla.org/en-US/docs/Web/API/IDBDatabase)&gt; |   the db to query |\n        
  
  
### equals(value) => {[IndexedDeleteRangeCompiler](./Module:-IndexedDB::IndexedDeleteRangeCompiler#indexeddeleterangecompiler)}        
  
**kind:** function        
  
filters items from the result if the index doesn't match the given value.        
  
| Name | Type | Description |          
|------|------|-------------|          
| value | * | value to compare |\n        
  
  
### from(value, [exclude=false]) => {[IndexedDeleteRangeCompiler](./Module:-IndexedDB::IndexedDeleteRangeCompiler#indexeddeleterangecompiler)}        
  
**kind:** function        
  
starts a new value range        
  
| Name | Type | Description |          
|------|------|-------------|          
| value | * |                 range start value |          
| [exclude=false] | [boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean) | determines if the start value will be included in the range |\n        
  
  
### to(value, [exclude=false]) => {[IndexedDeleteRangeCompiler](./Module:-IndexedDB::IndexedDeleteRangeCompiler#indexeddeleterangecompiler)}        
  
**kind:** function        
  
ends a value range        
  
| Name | Type | Description |          
|------|------|-------------|          
| value | * |                 end value of the range |          
| [exclude=false] | [boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean) | determines if the end value will be included in the range |\n        
  
  
### lowerThan(value) => {[IndexedDeleteRangeCompiler](./Module:-IndexedDB::IndexedDeleteRangeCompiler#indexeddeleterangecompiler)}        
  
**kind:** function        
  
filters items from the result where the index is lower than the given value        
  
| Name | Type | Description |          
|------|------|-------------|          
| value | * |   |\n        
  
  
### higherThan(value) => {[IndexedDeleteRangeCompiler](./Module:-IndexedDB::IndexedDeleteRangeCompiler#indexeddeleterangecompiler)}        
  
**kind:** function        
  
filters items from the result where the index is higher than the given value        
  
| Name | Type | Description |          
|------|------|-------------|          
| value | * |   |\n        
  
  
### commit() => {[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)}        
  
**kind:** function        
  
applies the delete operation based on the specified range        
  
  
  
