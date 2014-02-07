###Basic How To
To get started, you have to fork this repo at first. After that create a new branch and make your changes. At the end you can create  a pull request to merge your changes.

###Important
If you want to contribute to Application Frame there are some points you have to notice:
* all AF scripts uses only three globals:
  1. `self` - the global object, in a web like environment this is the same as `window` 
  2. `$` - the selector function to select a API of a module or the core AF
  3. `$` - the scope selector function to select a created scope
* if you create a new module, always wrap the code in a closure scope or if possible use the AF wrapper
* if you create a new module, the first line in your closure scope is alway`this.self= this, 'use strict';`
* if you create a new lib, make sure that your first line is `self.lib= lib || {};`
* every file starts with a header comment line

###Additional Infos
All functions of AF that aren't really related to AF are placed in extra script files / modules, which are contained in the modules folder. Files in the libs folder are JS objects which does not need to run initial code and only provide useful functions.



