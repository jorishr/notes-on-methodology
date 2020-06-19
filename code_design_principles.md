# S.O.L.I.D. Code Design principles

## 1. Single-responsibility principle
A class or module should have one, and only one, reason to be changed (i.e. rewritten).

As an example, consider a module that compiles and prints a report. Such a module can be changed for two reasons. First, the content of the report could change. Second, the format of the report could change. These two things change for very different causes: one substantive, and one cosmetic. 

The single-responsibility principle says that these two aspects of the problem are really two separate responsibilities, and should therefore be in separate classes or modules.

If there is a change to the report compilation process, there is greater danger that the printing code will break if it is part of the same class.


## 2. Open-closed principle
Classes, modules, functions, etc. should be open for extension, but closed for modification. 

A module will be said to be open if it is still available for extension. For example, it should be possible to add fields to the data structures it contains, or new elements to the set of functions it performs.

A class is closed, since it may be compiled, stored in a library with a well-defined, stable description. But it is also open, since any new class may use it as parent, adding new features. When a descendant class is defined, there is no need to change the original or to disturb its clients (inheritance).

## 3. Liskov substitution principle
In OOP the object generated by a child class should work flawlessly with the functionaliy defined in the parent class.

Example: shape -> square

## 4. Interface-segregation principle
No client should be forced to depend on methods it does not use. Example: a printer with a job class that holds all the functionality for printing, scanning and stapling will be hard to maintain. A solution would be to have an overarching job class with subclasses or interfaces for each specific functionality: print, scan, staple.

## 5. Dependency inversion principle
The dependency inversion principle is a specific form of decoupling software modules. Would you solder a lamp directly to electrical wiring in the wall? No, you use interfaces so that the lamp does not directly depend on the electrical grid. 

High-level modules should not depend on low-level modules. Both should depend on abstractions or interfaces.

Abstractions should not depend upon details. Details should depend upon abstractions.

Consider an Ajax call
```Javascript
$.get("/address/to/data", function (data) {
    $("#thing1").text(data.property1);
    $("#thing2").text(data.property2);
});
```
With dependency inversion it would look like:
```Javascript
getFromServer("/address/to/data", thingView);

function getFromServer(url, view) {
    $.get(url, function (data) {
        view.setValues(data);
    });
}

var thingView = {
    setValues: function (data) {
        $("#thing1").text(data.property1);
        $("#thing2").text(data.property2);
    }
};
```
getFromServer belongs in a low-level module, handling as it does the low-level interaction between the server and the view. 

Similarly, getromServer does not depend on specifics of the DOM elements and their IDs to perform its work; instead, it depends on the abstraction of a view, which for its purposes is any type that has a setValues method.

If one day you would have change the JQUERY view functionality with plain JS you could do so without changing the getFromServer code:
```Javascript
var textViewNoJQuery = {
   setValues: function (data) {
        document.getElementById("text1").value = data.property1;
        document.getElementById("text2").value = data.property2;
   }
};
```