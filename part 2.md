##NYCDA Backend Exam - Part 2

##Given that we have a "customer" resource/model in our web server,

##1 - How would you design the routes of your server based on REST convention? List them with VERB and /route

CREATE

app.post // post user data to db

app.post('/new', (req, res) => {
  customer.create(request.body).then(() => {
    response.redirect('/home');
  });
});

READ

app.get // register as a user page

app.get('/home', (req, res) => {
    res.render(index.pug);
});

UPDATE

app.put // edit user data

app.put('/:id', (req, res) => {
  customer.update(req.params, {
    where: {
      id: req.params.id
    }
  }).then(() => {
    res.redirect('/customer/' + request.params.id);
  });
});

DESTROY

app.delete // delete user from db

app.delete('/:id', (req, res) => {
  customer.destroy({
    where: {
      id: req.params.id
    }
  }).then(() => {
    res.redirect('/board');
  });
});




##2 - Which pages would require templates, and how would you name them? List them with /route and template-name.extension

new.pug or new.hbs         //creates new user page
edit.pug or edit.hbs      //edits user data page
index.pug or index.hbs   //list users - incl delete and edit buttons

##3 - What is a database constraint? Name the 3 types of database constraints you have learned.

Null constraint - the input cannot be null (empty)
Unique constraint - the input must not be the same in another row of the table
Foreign key constraint - the input must reference a column in another table

##4 - What is a foreign key? Given that you have a Factory that has many cars and car that belongs to a factory, What would be your foreign key column?

The cars model would contain a foreign key constraint that references the factory where it is made.

##5 - List all the model lifecycle hooks you have learned from sequelize and explain them briefly if necessary.

beforeUpdate - code that runs before an update, e.g. always set a value on a model before saving it

beforeCreate - code that runs before an update

hasMany - add this hook to a model if there is a another model which takes a foreign key constraint from the current model.

belongsTo - add this hook to a model to reference a foreign key constraint from another model.

beforeDestroy - for example, delete data from other models that have foriegn keys referencing model data to be deleted.
      onDelete: 'cascade'

##6 - What is the difference between database-level validations and application-level validations?

Application-level validations are things like 'is this an an email address?'

Application-level validations compare user input to the constraints such as weather a password is long enough or that an email input is a valid email (contains '@')


##7 - Why do we use bcrypt. Write down 3 reasons why we use it if you can.

To save passwords in a db in an encrypted way, so that backend devs cannot have access to user passwords.

Hackers are slowed down when they try different password options.

It's widely used and thus widely supported.

##8 - What is a flash message?

An error or info message that appears without requesting a new page.

##9 - What is the difference between minifying and obfuscating JavaScript?

Minifying deletes white space, so JS appears in one line, not indented.

Obfuscating changes variable names to 1 character, in order to save memory.

##10 - What are the 3 reasons that makes Gulp a good choice as an asset build library?

Has the most features of all build-tools

Flexible

Can batch build-tool tasks together to save time.
