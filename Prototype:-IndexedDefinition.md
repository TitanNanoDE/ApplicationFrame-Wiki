## Methods

### constructor(version: `number`) => [`IndexedDefinition`](https://github.com/TitanNanoDE/ApplicationFrame/wiki/Prototype%3A-IndexedDefinition)
Instantiates a new DB version.

### store(info: `string|StoreOptions`) => [`IndexedDefinition`](https://github.com/TitanNanoDE/ApplicationFrame/wiki/Prototype%3A-IndexedDefinition)
Creates a new store definition. Inside the store definition new indexes can be defined.

### index([name: `string`, members: `string[]`, options: object](https://developer.mozilla.org/en-US/docs/Web/API/IDBObjectStore/createIndex#Parameters)) => [`IndexedDefinition`](https://github.com/TitanNanoDE/ApplicationFrame/wiki/Prototype%3A-IndexedDefinition)
Creates a new index in the last defined store. This has been chosen to be able to chain together all definition calls.

## StoreOptions
| Name          | Type    |
| ------------- | ------- |
| name          | string  | 
| keyPath       | string  | 
| autoIncrement | boolean |