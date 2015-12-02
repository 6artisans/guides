# Rails

In the project within the app directory there are builders, delegates, facades, presenters, and processes.

All of the classes in those directories are just POROs.

Adding and extending features has been pretty simple. The small classes and abstractions make everything easy to understand. Making changes and additions is fairly painless.

Sandi Metz' Rules For Developers:

- Classes can be no longer than one hundred lines of code.
- Methods can be no longer than five lines of code.
- Pass no more than four parameters into a method. Hash options are parameters.
- Controllers can instantiate only one object. Therefore, views can only know about one instance variable and views should only send messages to that object (@object.collaborator.value is not allowed).

Use Facade Pattern to abstract models from views.

Sources:
  Rails Code review - https://github.com/thoughtbot/guides/tree/master/protocol/rails#code-review

  project structure, testing, discipline - https://robots.thoughtbot.com/a-client-project-two-years-later

  https://robots.thoughtbot.com/sandi-metz-rules-for-developers

## Testing

### TDD

- Unit tests: [Test Driven Development for RailsGirls](http://guides.railsgirls.com/test-driven-development/)
- Controller tests: [BDD on Rails with MiniTest](https://semaphoreci.com/blog/2014/10/27/bdd-on-rails-with-minitest-part-1-up-and-running.html)

There are both TestCase and MiniTest classes in Rails. TestCase is older and backwards compatible to Rails 2 and it is based on assertions:

```
assert_equal(function(x), "expected result")
```

while MiniTest is based on expectations:

```
function(x).must_equal("expected result")
```

### Other sources

- How to set up Rails to work with MiniTest - generators and a basic syntax guide: [Getting Started with MiniTest](http://6ftdan.com/allyourdev/2015/04/04/getting-started-with-minitest/)
- A complete, detailed book: [The MiniTest Cookbook](http://chriskottom.com/minitestcookbook/)
