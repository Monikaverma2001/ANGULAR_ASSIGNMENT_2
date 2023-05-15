QUESTION : Binding HTML content is an essential task in Angular development. 
ANSWER :
Introduction : Data binding allows Internet users to manipulate web page elements with the help of a web browser. 
It includes dynamic HTML and does not require complex programming. Data binding is used in web applications that contain interactive components such as forms, calculators, tutorials, and games. 
The incremental display of a webpage makes data binding convenient when pages contain an extensive amount of data. 
Angular uses the concept of two-way binding. Any UI element-related change is reflected in the corresponding and specific model state.
Conversely, any model state changes reflect in the UI state.
This ensures that the framework is able to connect the DOM to the Model data with the help of the controller.



    
    (b) Discuss the different types of data binding available in Angular and explain  any one.
    
    What is Data Binding?
Data binding is a process that allows developers to create a connection between two parts of an application. It helps to keep data synchronized and up-to-date so that changes made in one part of the application are reflected in the other part.

Types of Data Binding
In Angular, there are four types of data binding: one-way, two-way, event, and template binding. Let's take a look at each one.

One-Way Data Binding
One-way data binding is the most basic type of data binding. It allows you to bind a variable in one part of the application to another variable in another part of the application. This type of binding is used when you want to ensure that changes made in one part of the application won’t affect the other part.

Two-Way Data Binding
Two-way data binding is a more advanced type of data binding. It allows developers to bind a variable in one part of an application to a variable in another part of the application and vice versa. This type of binding is used when you want to ensure that changes made in one part of the application will be reflected in the other part automatically.

For example, let's say you have a text box that displays a user's name. You can use two-way data binding to bind the value of the text box to a user object in another part of your application. That way, when the user changes their name in the text box, the same change will be made to the user object automatically.

Event Data Binding
Event data binding is used to bind events such as clicks and mouseovers to functions or variables. This type of binding is useful when you want to trigger an action when an event occurs.

For example, let's say you want to display a message when the user clicks on a button. You can use event data binding to bind the click event of the button to a function that displays the message.

Template Data Binding
Template data binding is used to bind template variables or expressions to functions or variables. This type of binding is useful when you want to display dynamic information in your templates.

For example, let's say you have a list of users that you want to display on your website. You can use template data binding to bind each user object in your list to a template variable that displays their information dynamically on your website.


example of template data binding:


example :  <script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.6.9/angular.min.js"></script>
<script>
var app = angular.module("myApp", ['ngSanitize']);
app.controller("myCtrl", function($scope) {
    $scope.myText = "<div>Welcome <%= m.name %></div>";
});
</script>

<script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.6.9/angular-sanitize.js"></script>
<div ng-app="myApp" ng-controller="myCtrl">

        <h1 ng-bind-html="myText"></h1>
    
    </div><hr><hr>
    
    
    //adready implement in my project
