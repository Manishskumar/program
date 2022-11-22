<html>
<Script scr="https://ajax googleapis.com//ajax/libs/angularjs/1.6.9/angular.min.js"></script>
<Script scr="https://ajax googleapis.com//ajax/libs/angularjs/1.6.9/angular-route.js"></script>
<body ng-app="myApp">
<p><a href="#/!">main</a></p>
<a href="#!red">red</a>
<a href="#!blue">blue</a>
<a href="#!green">green</a>
<div ng-view></div>
<script>
var app=angular.module("myApp",["ngRoute"]);
app.config(function($routeProvider){
$routeProvider
.when("/",{
          templateUrl: "main.htm"
          })
          .when("/red",{
          templateUrl: "red.htm"
          })
          .when("/blue",{
          templateUrl: "main.htm"
          })
          .when("/green",{
          templateUrl: "green.htm"
          });
          });
          </script>
          <p.click on the link to nivgate to "red.htm", "blue.htm" , "green.htm" or back to the "main.htm"></p>
          </body>
          </html>
