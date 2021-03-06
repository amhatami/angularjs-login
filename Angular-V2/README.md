# Angular 2
AngularJS was designed by Google to address challenges programmers face building complex, single-page applications. This JavaScript framework takes care of the back end so you can take care of the client side. Angular 2 Essential Training introduces you to the essentials of this "superheroic" framework, including powerful features such as rich templates, change detection, user interactions, two-way data binding, comprehensive routing, and dependency injection.

## TYPESCRIPT
A quick look at Angular basics.

Angular applications are made up of components. A component is the combination of an HTML template and a component class that controls a portion of the screen. Here is an example of a component that displays a simple string:

**src/app/app.component.ts**
```TYPESCRIPT
import { Component } from '@angular/core';

@Component({
  selector: 'my-app',
  template: `<h1>Hello {{name}}</h1>`
})
export class AppComponent { name = 'Angular'; }
```
Every component begins with an @Component decorator function that takes a metadata object. The metadata object describes how the HTML template and component class work together.

The selector property tells Angular to display the component inside a custom <my-app> tag in the index.html.

**index.html (inside <body>)**
```html
<my-app>Loading AppComponent content here ...</my-app>
````
The template property defines a message inside an ```<h1>``` header. The message starts with "Hello" and ends with `{{name}}`, which is an Angular interpolation binding expression. At runtime, Angular replaces `{{name}}` with the value of the component's `name` property. Interpolation binding is one of many Angular features you'll discover in this documentation.

In the example, change the component class's `name` property from `'Angular'` to `'World'` and see what happens.

## A WORD ABOUT TYPESCRIPT
This example is written in TypeScript, a superset of JavaScript. Angular uses TypeScript because its types make it easy to support developer productivity with tooling. You can also write Angular code in JavaScript; this guide explains how.

Also Topics include:
*What is Angular?
*Setting up an Angular template
*Creating a component
*Binding events and properties
*Getting data to components
*Using directives and pipes
*Creating Angular forms
*Validating form data
*Understanding dependency injection
*Providing services
*Making HTTP calls
*Routing
