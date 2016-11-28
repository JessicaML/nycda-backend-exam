
##NYCDA Backend Exam - Part 3

##1 - What is the difference between git pull and git merge?

Git pull
Runs a git fetch and then a git merge . If you want to bring your local repository up to speed with a remote repository that is what you would run.

Git merge
Merge a branch with master so that changes from one branch are mixed into the master branch, it closes use of the other branch.

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

Best way is to put all css into one application.css, with the css link in html head tag

##7 - Why_variables.scss file is important?

All bootstrap styling values are defined in the_variables.scss. By changes those values we can theme/adjust bootstrap to our needs.

##8 - Lets say you want to change the alert component of bootstrap, what are steps/strategy would you use to make that change?

1) Try to see if you can override the bootstrap_variables.scss file, by changing the variables_alerts.scss uses.

2) If that isnt satisfactory then create your own_alerts.scss file under your custom /bootstrap folder and write the styling scoped to the .alert {}

if your styling is unrelated to the bootstrap alert component you should create your own component file and include it in your build process, application.css
