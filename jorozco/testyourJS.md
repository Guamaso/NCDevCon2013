#Test yo JS.

by: Ryan Anklam, BitterSweetRyan

###Decisions

Decide on BDD or TDD. Are you going to test ASYNC? HTML?

BDD: Jasmine

TDD: QUnit

Both: Mocha, THe intern, BusterJS

###Testing

* Create tests w/in source directories
* Create the test runner (Example shown)

In Mocha, the `spec` director is most important?

TDD is easier with QUnit. Simpler to write. (Example shown)

Write JS using the "object literal pattern"

Be careful...

* writing code within closures of a callback, private function, etc.
* with functions that "do too much"
* with anonymous functions, call function instead.

Don't forget about DRY?

Use "set up" and "clean up" functions (provided by testing framework)

Book: Writing testable JS by Rebecca Murphy (?)

###Spies

Sinon and Jasmine have/do spies

If using a spy on jQuery, use `jQuery.jQuery.fn`

Sinon has special methods for testing AJAX: `Fakeserver` and `fakexmlhttpserver`

Former returns fake json, latter captures request.

###Testing Async code

In Jasmine, do a `runs` method then `wait` then `runs` again.  Wait is a preset timer that allows the async code to complete.

Mocha is about the same, but simpler.

Qunit can do it too with Sinon. Use setTimeout for the `wait`.

###Automation

Use Grunt.

If you're going to minify, which you should, test before and after.

Testem - tests in command line, tests all browsers. Very cool.
