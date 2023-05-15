Importance of website Navigation  
Website navigation is way by which one can easily increase audience or number of visitors on website. If website navigation is not good and effective, there is not point of having a creative website because users won’t be able to navigate easily around it to find information they want. So, it’s very important to keep to simple, effective to increase user experience and keep clients and visitors happy. Below are given some reasons that will tell you why website navigation is important. Let’s have a look.  

Increase duration of visit: Website navigation helps people to find information they want to see very easily and effectively. Good website navigation provides clear and simple navigation bars and links that encourages visitors or peoples to explore more and more. This in turn increase duration of their visit on website because navigation is very easy to use and understand and nowadays everyone wants it easy to get things.
Increased chance of sales: Website navigation generally helps in showing visitors what website is actually about without any wastage of time. This in turn increase time spent by visitors on website and visitors stays on website for longer time.  Visitors then go through website and purchase product effortlessly and easily. This will automatically increase purchase of products and sale.
Improved user experience: Navigation is very important for website because without navigation, websites won’t look good, and appear unorganized. Nowadays, no one to waste their time on determining how website works. Everyone wants to easily find what they want. Good navigation generally helps visitors to find information they want to search and increase speed of visitors search. Clear and simple navigation is simply to understand that in turn increase user experience.
Good Design: Good navigation make website look more attractive, effective and good. Navigation has a greater impact on how website is viewed by users or visitors and how longer they will stay on website. Design of website navigation have a greater impact on success of website. It almost affects traffic, SEO ranking, user experience, conversions, sales, etc. So, good navigation is very useful to boost website design and brand of company or business. Good navigation keeps visitors happy and satisfied.

![Image]{/q1_1.png}

![Image]{/q1_2.png}

ADD NAV BY ANGULAR
CODE:
<pre>
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <title>Website Navigation Example</title>
  <script src="https://unpkg.com/angular/angular.js"></script>
  <script src="https://unpkg.com/@angular/router/angular1/angular_1_router.js"></script>
</head>

<body ng-app="myApp">

  <nav>
    <a ng-href="#/">Home</a>
    <a ng-href="#/about">About</a>
    <a ng-href="#/products">Products</a>
    <a ng-href="#/contact">Contact</a>
  </nav>

  <div ng-view></div>

  <script>
    var app = angular.module('myApp', ['ngComponentRouter']);

    app.value('$routerRootComponent', 'myApp');

    app.component('home', {
      template: 'Home Component'
    });

    app.component('about', {
      template: 'About Component'
    });

    app.component('products', {
      template: 'Products Component'
    });

    app.component('contact', {
      template: 'Contact Component'
    });

    app.controller('MyController', ['$router', function($router) {
      $router.config([
        { path: '/', component: 'home' },
        { path: '/about', component: 'about' },
        { path: '/products', component: 'products' },
        { path: '/contact', component: 'contact' },
        { path: '/**', redirectTo: '/' }
      ]);
    }]);
  </script>

</body>

</html>

</pre>


  
