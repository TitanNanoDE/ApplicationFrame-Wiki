## Basic Setup
To create a Application Frame app, you usually need at least two files.

The first file will be your core application:

````JavaScript
// App.js

import Application from 'application-frame/core/Application';

const App = {
    name: 'Demo App',
    version: '1.0.0',

    init() {
        this.constructor();
    },

    __proto__: Application,
};

export default Application;

```

What does this do?

with `const App` we create a new application. The properties `name` and `version` are meta information, they are not required, but are good to have.
The next property is where it gets interesting `init()` is a method on our application. This method will launch our application. Here you should place any start up code. At the moment it only contains `this.constructor()` which will setup all the default functionality of an Application Frame app.

```
// bootstrap.js

import App from './App';

const ready = function() {
    App.init();
}

if (document.readyState === 'complete') {
    ready();
} else {
    window.addEventListener('DOMContentLoaded', ready);
}
```

This little bootstrap script will call your init function as soon as the page is ready. If you have to wait for other libraries, this is a good place to do so.

For instructions on how to build a UI check out [How To: Getting Started with DataBinding](https://github.com/TitanNanoDE/af-DataBinding/wiki/How-To:-Getting-Started-with-DataBinding)