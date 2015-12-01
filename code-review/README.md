# Code Review

- Accept that many programming decisions are opinions. Discuss tradeoffs, which you prefer, and reach a resolution quickly.
- Ask questions; don't make demands. ("What do you think about naming this :user_id?")
- Ask for clarification. ("I didn't understand. Can you clarify?")
- Avoid selective ownership of code. ("mine", "not mine", "yours")
- Avoid using terms that could be seen as referring to personal traits. ("dumb", "stupid").
- Don't use hyperbole. ("always", "never", "endlessly", "nothing")
- Don't use sarcasm.
- Explain why the code exists. ("It's like that because of these reasons. Would it be more clear if I rename this class/file/method/variable?")
- Offer alternative implementations, but assume the author already considered them. ("What do you think about using a custom validator here?")
- Review data integrity closely, such as migrations that make irreversible changes to the data, and whether there is a related todo to make a database backup during the staging and production deploys.

- Review whether dependency upgrades include a reason in the commit message, such as a link to the dependency's ChangeLog or NEWS file.
- Review whether new database indexes are necessary if new columns or SQL queries were added.
- Review whether new scheduler (cron) tasks have been added and whether there is a related todo in the project management system to add it during the staging and production deploys.
- Pair programming is not a code review.

Source: https://github.com/thoughtbot/guides/tree/master/code-review
