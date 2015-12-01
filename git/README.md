# Git

We don't know how to use git properly. I think gitflow is not for us.

I propose few simple, but painful changes

- don't use staging a production branches, I see it as bureaucracy with no real benefit for us
- lets have one master branch, which should contain only tested, reviewed and production ready code
- unfinished changes should be in feature branch
- when feature is ready create PR with following info:
     - are we waiting for some third party change (eg. IPAS update)
     - more to come?
- code review, merge and live happily ever after

More: https://github.com/thoughtbot/guides/tree/master/protocol/git

How to write commit messages:

- Limit the subject line to 50 characters
- Capitalize the subject line
- Do not end the subject line with a period
- Use the imperative mood in the subject line
    - e.g. Odstranit nepouzivane funkce, Aktualizovat dokumentaci
- Use the body to explain what and why vs. how

More: http://chris.beams.io/posts/git-commit/

TODO: rebases...
