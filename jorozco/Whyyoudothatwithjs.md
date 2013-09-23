#Why are you doing that with JS?

by Adrian Pomilio

Book: Functional JS (O'Reilly)

* Scripts move to bottom of page.
* Move assets to a CDN.
* Even better, use a script loader. Loads dynamically, doesn't lock up threads.
	* Lazyload simple, small. 1k minified (compressed?)
* Use Namespacing! Namespace helps organization and prevents others from overwriting your stuffs.
* Learn and use patterns!  Makes code more reusable, cleaner, etc.
* Use Prototype - helps with performance and memory when using many objects.
* The `new` keyword always instantiates an object, but be careful, it doesn't always do it the way you think it will. Write object so it is automatically instantiated properly.
* Use `while` for object literals (arrays) not `for in`. 
* Even better, do a `for` loop backwards using `--`!
* Duff's Device!!!! As Marty McFly said, "That's heavy."
* Might make more sense to create your own "vanilla JS" library of DOM manipulators, events, script loading, etc.  No need to download a full framework for these tasks.
* JD Doc for JS documentation from comments (Run via Grunt?)
* Use HTML templating! Handlebars, mustache, etc.
* Check out Todomvc.com for comparisons on JS MVC frameworks.