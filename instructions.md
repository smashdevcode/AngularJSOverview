
# Instructions

## Directives, Data Binding, and Filtering

1. Add "ng-app" directive to the &lt;html&gt; element.

 ```
 <html ng-app>
 ```

1. Add "ng-model" directive to the "search" input element.

 ```
 <input name="search" type="text" ng-model="searchText" />
 ```

1. Add a data binding expression to the page.

 ```
 {{ searchText }}
 ```

1. Add "ng-init" directive to the &lt;body&gt; element.

 ```
 <body ng-init="customers=['James','Ken','Jason','Dave','Brian']">
 ```

1. Add "ng-repeat" directive to the &lt;tr&gt; element and a data binding expression to the first &lt;td&gt; element.

 ```
 <tr ng-repeat="customer in customers">
     <td>{{ customer }}</td>
     <td></td>
 </tr>
 ```

1. Add "filter" to the "ng-repeat" directive.

 ```
 <tr ng-repeat="customer in customers | filter:searchText">
 ```

## Modules and Controllers

1. Define a module.

 ```
 var app = angular.module('customersApp', []);
 ```

1. Add a controller.

 ```
 app.controller('CustomersController', function ($scope) {

 });
 ```

1. Add "customers" property to the controller's scope object.

 ```
 app.controller('CustomersController', function ($scope) {
   $scope.customers = [
     { id: 1, name: 'James', total: 4.555 },
     { id: 2, name: 'Ken', total: 3.223 },
     { id: 3, name: 'Jason', total: 5.667 },
     { id: 4, name: 'Dave', total: 7.887 },
     { id: 5, name: 'Brian', total: 10.112 }
   ];
 });
 ```

1. Update the "ng-app" directive with the module name.

 ```
 <html ng-app="customersApp">
 ```

1. Add a new &lt;div&gt; element with a "ng-controller" directive around our main content.

 ```
 <div ng-controller="CustomersController">
 ```

1. Update the table template to take advantage of the customer object properties.

 ```
 <tr ng-repeat="customer in customers | filter:searchText">
    <td>{{ customer.name }}</td>
    <td>{{ customer.total | currency }}</td>
 </tr>
 ```

## Routing

1. Define routes using the "$routeProvider" provider.

 ```
 app.config(function ($routeProvider) {
   $routeProvider.when('/orders',
   {
     controller: 'OrdersController',
     templateUrl: '/views/orders.html'
   })
   .when('/',
   {
     controller: 'CustomersController',
     templateUrl: '/views/customers.html'
   })
 });
 ```

1. Add an "OrdersController" controller.

 ```
 app.controller('OrdersController', function ($scope) {

 });
 ```

1. Add "ngRoute" as a dependency to the main module.

 ```
 var app = angular.module('customersApp', ['ngRoute']);
 ```

1. Replace the main content with a &lt;div&gt; element containing the "ng-view" directive.

 ```
 <div ng-view></div>
 ```

1. Add a "views" folder.

1. Add a "customers.html" view.

 ```
 <h2>Customers</h2>

 <div>
   <label for="search">Search:</label>
   <input name="search" type="text" ng-model="searchText"/>
 </div>

 <div>{{ searchText }}</div>

 <div>
   <table>
     <thead>
       <tr>
         <th>Name</th>
         <th>Total</th>
       </tr>
     </thead>
     <tbody>
       <tr ng-repeat="customer in customers | filter:searchText">
          <td><a href="#/orders">{{ customer.name }}</a></td>
          <td>{{ customer.total | currency }}</td>
       </tr>
     </tbody>
   </table>
 </div>
 ```

1. Add an "orders.html" view.

 ```
 <h2>Customer Orders</h2>

 <p><a href="#/">Back to Customers</a></p>
 ```
