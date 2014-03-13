# Controllers

## ...

* Manage the page
* Use the `ng-controller` attribute
* `ng-controller="whatever"` defines a controller called "whatever"
* Manage `$scope`!!
  * `$` typically means a builtin angular service
  * Controllers attach things to `$scope`

Controllers can:

* Add models
  * Models = POJSO's (Plain-Old Javascript Objects"
* Response to UI Actions
* *Note*: Should be thin-ish
* THE CONTROLLER DOES NOT **DIRECTLY** MANIPULATE THE DOM
* If the above happens, maybe refactor (??). Solutions include:
  * Establish a binding and let Angular handle
  * Use a builtin directive to do what we want
  * Build your own directive
* Either way, it's not NG-ish to manipulate dom in controller


## Example

HTML:

```html
<body ng-controller="GreeterCtrl">
  Hello, {{greetee.name}}?
</body>
```

Javascript:

```js
function GreeterCtrl ($scope) {
  $scope.greetee = { name : 'whoever' };
}
```

`ng-controller=GreeterCtrl` invokes the function `GreeterCtrl`, which
manipulates the variable `greetee` in the scope.



# View

Angular uses HTML, Attributes, and Custom Element.

* Extend HTML attributes with Plain-Old-Html-*
* Example: <vvhatever*>

# Directives

* Custom Attributes: `<div thing="whatever"></div>`
* Custom Element: `<vvhatever></vvhatever>`
* `CSS Class: `<div class="vvhatever">`

Directives include:

* `ng-app`
* `ng-controller`
* `ng-repeat`

## `ng-repeat`

Syntax:

* `ng-repeat="item in items"`
* `ng-repeat="(key, val) in object"`



# ng-model

* Data-binding!

# ng-click

# Builtin directives

* `input`, `textarea`, `select`
* `ng-app`
* `ng-blur`
* `ng-change`
* `ng-checked`
* `ng-class`
* `ng-click`
* `ng-cloak`
* `ng-controller`
* `ng-show`, `ng-hide`
* `ng-model`
* `ng-repeat`
