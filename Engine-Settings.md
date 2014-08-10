**coreLock:** The coreLock option locks the settings and prevents from overwriting the coreLock is disabled by default.

**masterApplication:** The masterApplication option defines the name of the app which should get master privileges. For default there is no app name set.	

**renderMode:** The render mode defines how to handle the different threads. Default means all applications are running in the main thread.

**preProcessing:** turn on preprocessing, to use Application Frame specific syntax.

**singleApplicationMode:** if turned on, only one application can be created.	

**support:** When enabled the engine checks if the runtime environment supports all required APIs. If any dependencies couldn't be found, the user will be forwarded to crashPage.

**crashPage:** defines the page to which the engine forwards if there is a unsolved dependency.

**grantRoot:** gives the main application the possibility to access the engine object (only available in node)


[< back](https://github.com/TitanNano/ApplicationFrame/wiki)