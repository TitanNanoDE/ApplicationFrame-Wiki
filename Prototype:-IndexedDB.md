## Methods
### constructor(name: `string`) => [`IndexedDB`](https://github.com/TitanNanoDE/ApplicationFrame/wiki/Prototype%3A-IndexedDB)
Instantiates a new indexed DB. All version definitions have to be made done synchronously. The actual database creation is immediately scheduled for the next event cycle. 

### define(version: `number`) => [`IndexedDefinition`](https://github.com/TitanNanoDE/ApplicationFrame/wiki/Prototype:-IndexedDefinition)
Creates a new version definition for the DB. All stores and indexes for the current version have to be defined in this definition.

### read(storeName: `string`) => `IndexedQueryCompiler`
Creates a new query to the database. The store which should be queried from has to be specified.

### write(storeName: `string`, value: `object`) => [`Promise`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)
Stores an object in the selected store. The promise resolves to the transaction result.

## Examples

### Creating a new DB
 
```JavaScript
import IndexedDB from 'application-frame/IndexedDB';
const { create } = Object;

const DB = create(IndexedDB).constructor('myTestDB')
    .define(1)
        .store('testStore')
            .index('id', ['id'], null)
            .index('idAndDate', ['id', 'date'], null)
        .store('secondStore')
            .index('nameAndPassword', ['name', 'password']);

DB.define(2)
    .store('newV2Store')
        .index('id', 'id', { unique: true });
```

