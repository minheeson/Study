## AngularJS

#### JavaScript Framework 

​	ng-app 

#### 기본 개념

- __Scope__
  - AngularJS 내에서 작업이 이루어지는 공간
  - 모델의 데이터를 보관  
- __Model__
- __View__
- __Controller__
  - 비즈니스 로직을 담고 있는 컴포넌트 
    ~~~js
    var myApp = angular.module('myApp',[]);
    myApp.controller('GreetingController', ['$scope', function($scope) {
    $scope.greeting = 'Hola!';
    }]);
    ~~~
- __Directives__
  ~~~html
  <body ng-app>
  <span>Insert your name:</span>
  <input type="text" ng-model="user.name" />
  <h3>Echo: {{user.name}}</h3>
  </body>
  ~~~
  - 양방향 바인딩 (two-way binding)
  - ng-app : Angular에게 body 요소가 application에 포함되어 있다고 알려줌
  - ng-model / ng-bind / ng-init 













