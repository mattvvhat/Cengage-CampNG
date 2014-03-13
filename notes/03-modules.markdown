# Modules

This is similar to an app or package. That is, it's self-contained and has
everything it needs to run (except dependencies). It is best-practice to keep
yourapp in a module.

Contains:

* Controllers
* Services
* Filters
* Directives
* Configuration


Create:

```js
/**
 * @param moduleName string name of module
 * @param deps array list of dependencies as string"
 */
angular.module('moduleName', [ deps ]);
```


**NOTE**: To use a module in your code, you must have: `ng-app="module"` on the container.


