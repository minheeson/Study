## AngularJS

#### JavaScript Framework 

#### 기본 개념

- __Scope__
  - AngularJS 내에서 작업이 이루어지는 공간
  - 모델의 데이터를 보관  
- __Model__ __View__
  ~~~html
  <body ng-app>
  <span>Insert your name:</span>
  <input type="text" ng-model="user.name" />
  <h3>Echo: {{user.name}}</h3>
  </body>
  ~~~
  - 양방향 바인딩 (two-way binding)
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
  <div ng-app="" ng-init="firstName='John'">
    <p>Name: <input type="text" ng-model="firstName"></p>
    <p>You wrote: {{ firstName }}</p>
  </div>
  ~~~
  - ng-app : Angular에게 body 요소가 application에 포함되어 있다고 알려줌
  - ng-model / ng-repeat / ng-init   
- __Filters__
  - 모델 정보를 뷰에 뿌리기 전에 실행하는 컴포넌트
  ~~~html
  <div ng-app="myApp" ng-controller="personCtrl">
  <p>The name is {{ lastName | uppercase }}</p>
  </div>
  ~~~
  - date / lowercase / orderBy 














