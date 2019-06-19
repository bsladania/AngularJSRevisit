AngularJS - version 1.0 was released in 2012; JavaScript framework;
====================================================================================================================================
Properties: AngularJS is easy to learn; It is perfect for Single Page Applications (SPAs); It extends HTML with new attributes.
Script: <script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.6.9/angular.min.js"></script>

AngularJS extends HTML with ng-directives.
The ng-app directive defines an AngularJS application.
The ng-model directive binds the value of HTML controls (input, select, textarea) to application data.
The ng-bind directive binds application data to the HTML view.

Example:

<div ng-app="" ng-init="firstName='John'">
<p>The name is <span ng-bind="firstName"></span></p>
</div>

Alternative

<div ng-app="" ng-init="firstName='John'">
  <p>The name is {{firstName}}</p>
</div>

//Example with module and controller

<div ng-app="myApp" ng-controller="myCtrl">
  First Name: <input type="text" ng-model="firstName">
<br>
  Full Name: {{firstName}}
</div>

<script>
  var app = angular.module('myApp', []);
  app.controller('myCtrl', function($scope) {
    $scope.firstName= "Tony";
  });
</script>


