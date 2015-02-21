
# AngularJS
# Overview

---

# Introductions

---

## Who We Are

* James Churchill - _Developer/App Dev Practice Manager_
* Ken Howard - _Front End Developer_
* Jason Domogalla - _Front End Developer_

---

## Who CSG Pro Is

* Portland based consultancy
* 30 (or so) employees/contractors
* 22 years in business
* Custom Application Development
* Business Intelligence

---

## ng-conf extended Event

### March 5th and 6th  

### Tickets: $20 at [Eventbrite](http://www.eventbrite.com/e/ng-conf-extended-pdx-tickets-15750808091?aff=eac2)

---

# Agenda

---

* (Optional) Brief History of Web Apps
* Our Evolution
* Why AngularJS???
* Example Apps
* "Hello World" Walkthrough
* Q&A
* Resources

---

# Brief History of Web Apps

---

# Collection
# of Pages

### "Thick Server" or "Thin Client"

---

* Full page response with each request
 * Both presentation and data are sent to the client every time
* Data is packaged with each page response
* Routing and view rendering on the server
* Various tricks to maintain state
 * Session cookie
 * Hidden frame

---

# Single Page
# Apps (SPA)

### "Thick Client" or "Thin Server"

---

* Single initial page load
 * All HTML/CSS/JS is loaded on the intial request (typically)
* AJAX is used to load data as needed (driven by user events)
* Routing and view rendering on the client
* State is maintained in the browser (in JS)
* Increased complexity in the client
 * Mitigated by using popular patterns like MVC and DI

---

# SPA Components

---

## SPA Component Categories

* Templating
* Controllers
* Routing
* Local Storage

---

## SPA Component "Lego" Pieces

Combine libraries like "lego" pieces to build applications

* Knockout.js - Templating and Controllers
* Crossroads.js - Routing
* RequireJS - Module Loading

---

# SPA Frameworks

---

## Popular SPA Frameworks

* AngularJS
* Ember.js
* Meteor

---

## SPA Framework Pros

* Provide a single, cohesive solution for building SPAs
 * Fewer choices to make
* Evolving APIs
* Strong communities

---

## SPA Framework Cons

* Steep learning curve
* Frequent API changes
* Sometimes poor documentation
* Monolithic solution
* Lock-in

---

# Our Evolution

---

## Classic ASP

* Page based
* Light abstractions
 * Application, Request, Response, Server, and Session
* VB Script - Interpreted on the server
* Some JS

---

## ASP.NET Web Forms

* Page based
* Attempted to make the "stateless" web stateful
* Heavy abstractions
 * New versions of ASP abstractions
 * Introduction of page and control events
 * Control abstractions

---

## ASP.NET Web Forms

* C# - Compiled and executed on the server
* More JS, AJAX, and the introduction of jQuery
* Difficult to unit test

---

## ASP.NET MVC

* Response to Ruby on Rails
* Route based
* Embraced the web as being "stateless"
* Fewer abstractions
 * Brings the developer closer to HTTP and response/request

---

## ASP.NET MVC

* Introduction of MVC pattern
* C# - Compiled and executed on the server
* Even more JS, AJAX, and jQuery
* Easier to unit test

---

## AngularJS and Web APIs

* Single page applications
* Stateful, richer UI, "desktop" like applications
* Server simplifies to a web API
* More easily allows division of labor between the front and back end

---

## Why AngularJS???

* Very popular
* Strong community
* Future looks promising
* Backed by Google

---

## AngularJS Key Features

* Declarative two-way data binding
* Ability to extend HTML via Directives
* Fully unit testable

---

## Example Apps

* BBSI Policy App (screenshots)
* Simplot Regulated (screenshots)
* APM Galveston (screenshots)
* Time Tracking Apps (live demo)

---

# "Hello World" Walkthrough

---

_Heavily inspired by Dan Wahlin's AngularJS in 20ish Minutes_  
[See https://www.youtube.com/watch?v=tnXO-i7944M](https://www.youtube.com/watch?v=tnXO-i7944M)

---

## Quick and Dirty

* Bootstrapping the app with "ng-app"
* Data Binding with "ng-model"
* Data with "ng-init"
* Repeating data with "ng-repeat"
* Filtering the data with a filter

---

## Improving the design

* Modules
* Controllers with "ng-controller"
* Routing with ngRoute module
* Route configuration
* Views with "ng-view"
* Project structure

---

# Q&A

---

## Resources

* [AngularJS Site](https://angularjs.org/)
* [AngularJS YouTube Page](https://www.youtube.com/user/angularjs)
* [John Papa's AngularJS Style Guide](https://github.com/johnpapa/angularjs-styleguide)
* [Code School AngularJS Free Course](https://www.codeschool.com/paths/javascript#angular-js)
