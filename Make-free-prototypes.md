With the release of v0.3, ApplicationFrame will start to use Make free prototypes for all new prototypes. Make free prototypes are slightly different instantiated then the old Make prototypes.

## Instantiation of Make Prototypes
```JavaScript
import Prototype from '../lib/Prototype.js';

let instance = Make(Prototype)();
```

## Instantiation of Make free Prototypes
```JavaScript
import Prototype from '../lib/Prototype.js';

let instance = Object.create(Prototype).constructor();
```
