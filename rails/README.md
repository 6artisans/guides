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
