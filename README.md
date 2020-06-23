This is a basic app we're working on to learn about Angular.

# Good Tutorials and resources:
Main Angular documentation and tutorial from Google: https://angular.io/guide/setup-local

Practical tutorial: https://developer.okta.com/blog/2019/01/30/first-angular-pwa

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).

# Commands to create

make sure you have node installed 

% npm install -g @angular/cli@8.3.12

% ng new Angular-Starter
	//--routing? yes
	//--scss

cd Angular-Starter

# Run the App

% ng serve --aot //bundles code with webpack using live reload (can leave out the aot if this creates errors)

//go to localhost:4200 to view the app 

# Clean out app.component.html

This is the spot that serves up the view.

It comes with a lot of boilerplate. To clean it up, you can delete everything in that file, EXCEPT <router-outlet></router-outlet> 

Leave the router outlet in. That's where your code is sent to the view.

# Create components

% ng generate component amazing-first-component

//if that causes error, can run instead: % ng g c amazing-first-component --module app

Creating a component will add a folder with an HTML file (the view), a TS file (the logic), a SCSS file (styling), and spec.ts file (for tests)

It also adds this componnt to app.module.ts

You'll want to create a route for it in app-routing.module.ts

[Note: the app.module and app-routing.module stuff will be different if you are doing lazy-loading, which is a good practice.]

# Discussed June 19, 2020
-why Angular 
-AngularJS v Angular
-what a framework does
-basic structure of Angular
-setting up an Angular app
-inserting typescript variables
-changing typescript variables (with "this")

# Discussed June 23, 2020
-environmental variables
-don't include api keys on the front end (house them on the backend)
-ngIf
-ngFor
-inserting one component into another
-introduction to components talking to each other through a service
-introduction to https and fetch requests

# Next
-I will code up an example of communication through a service
-I will code up an example of routing

# Further Concepts to explore (tbd)
-calling an api (http and fetch)
-ngClass
-design/styling with Angular Material
-forms


