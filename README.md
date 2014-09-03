angular-options-disabled
========================

Angular directive for disabling specific options in ng-options directive.


Installation
============

```bower install angular-options-disabled```

How to use
==========

Include ```ngOptionsDisabled``` module to your app, for example: ```angular.module('myApp', ['ngOptionsDisabled'])```.

Add ```ng-options-disabled``` attribute to your ```select``` element with following syntax ```condition for item in collection```.

Example
=======

```html
<select ng-model="country" ng-options="country.id as country.name for country in countries" ng-options-disabled="country.disabled == true for country in countries">
```

Credits
=======
Originally based on stackoverflow answer by Vikas Gulati. Fixed and improved by Dima Knivets.