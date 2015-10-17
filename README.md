<!doctype html>
<html>

 <head>
  <script src = "https://ajax.googleapis.com/ajax/libs/angularjs/1.3.0-beta.17/angular.min.js"></script>
 </head>

 <body ng-app = "Helloworldapp">
    
   <div ng-controller = "HelloWorldctrl"> 
     <h2> Welcome. {{helloto.title}} </h2>
     <div>
       <input type = "text" ng-model = "title" placeholder = "Enter your title">
     </div>         
   </div>
   
   <script>
     angular.module("Helloworldapp", []) 
     .controller("HelloWorldctrl", function($scope) 
     {
      $scope.helloTo = {};
      $scope.helloTo.title = "This is my title";
     }
     );
   </script>
 
 </body>

</html>
