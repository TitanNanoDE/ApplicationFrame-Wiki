## Methods
### constructor(name: `string`) => `IndexedDB`
Instantiates a new indexed DB. All version definitions have to be made done synchronously. The actual database creation is immediately scheduled for the next event cycle. 

### define(version: `string`) => `IndexedDefinition`
Creates a new version definition for the DB. All stores and indexes for the current version have to be defined in this definition.

### read(storeName: `string`) => `IndexedQueryCompiler`
Creates a new query to the database. The store which should be queried from has to be specified.

### write(storeName: `string`, value: `object`) => `Promise`
Stores an object in the selected store. The promise resolves to the transaction result.