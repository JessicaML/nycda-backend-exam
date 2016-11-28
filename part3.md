
##NYCDA Backend Exam - Part 3

##1 - What is the difference between git pull and git merge?

Git pull
Pull changes in a repo, after someone else has made amendments

Git merge
Merge a branch with master so that changes from one branch are mixed into the master branch

##2 - Why do we use a pull request on github instead of merging our branch directly to master and then pushing it to github?

To review changes first to make sure we want them.

##3 - Why do we use database migrations?

To change the schema, e.g. add or rename a column

##4 - What is the difference between up and down functions of sequelize migration files?

Down functions allow us to roll back and undo changes if needed later on.

##5 - Name 3 reasons why Sass/SCSS is better than CSS?

Quicker to write - uses indentation instead of curly braces

You can use mixins and variables

You can use @imports and @extends

##6 - What is the right way to include bootstrap to your project?

Best way is to host within project directory, not through url.
The put the css link in html head tag

##7 - Why_variables.scss file is important?

Lists all elements in bootstrap (not minified)
##8 - Lets say you want to change the alert component of bootstrap, what are steps/strategy would you use to make that change?

uncomment out any elements in bootstrap you want to change
