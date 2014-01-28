If you want to contribute to Application Frame here are some points you have to notice:

* all AF scripts uses only three globals:

* 1. `self` - the global object, in a web like environment this is the same as `window` 
  2. `$` - the selector function to select a API of a module or the core AF
  3. `$` - the scope selector function to select a created scope

* if you create a new module, always wrap the code in a closure scope or if possible use the AF wrapper.
* if you create a new module, the first line in your closure scope is alway`'use strict', this.self= self || this;`
