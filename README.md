# Angular JS Toggle Demo

Project demonstrates creating and updating a toggle variable in controller and also shows the usage of ng-click and ng-show or ng-hide.

### Setup

For this project I am using Angular 1.6.4

```html
<script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.6.4/angular.min.js"></script>
```

### Code

```html
<button ng-show="!controller.toggle" ng-click="controller.toggle = !controller.toggle"> SHOW </button>
<button ng-show="controller.toggle" ng-click="controller.toggle = !controller.toggle"> HIDE </button>
<div ng-class="controller.toggle ? 'shown' : 'hidden'">
    Hello world
</div>
```

### Explanation

**ng-show** is a class that will make an element visible in the DOM. So if toggle variable is true HIDE button will be visible else SHOW button will be visible.

**ng-click** will actually change the boolean value of the toggle variable.
