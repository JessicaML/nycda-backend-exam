## NYCDA Backend Exam
=====================
Explain the questions well!!

### 1- Why do we should include script tags at the very end of an html file, before closing </body>?

We want the page to load all the content before JS event handler load to the page, so that all content is loaded before interaction takes place, and the JS functions as it is designed to. This also means the static content will load faster and give the user a better experience.

### 2 - What is a middleware?

Middleware adds features to Express code.


### 3 - Why do we use express.static() middleware?

In order to use css and js files in a public directory within an express app. It wraps the send module in order to support client-side caching.

### 4 - What is favicon.ico ?

Small icon at the left of the URL or on the tab, usually the company logo of the website.

### 5 - Why do we use a bodyParser middleware ?

In order to read form data that is posted from the client.

### 6 - What is the difference in terms of parsing data received from a web form with POST or an AJAX POST request?

AJAX post requests use JQUERY and JSON. 

### 7 - Why do we use methodOverride middleware ?

It provides provides faux HTTP method support, in order to use app.delete or app.put to edit and delete content.


### 8 - What are the differences between sessions and cookies ?

Sessions is stored on the server side, cookies on the client side. Cookies store data as objects, sessions store data as strings. Sessions is a more secure way of saving data. Cookies can be saved for a longer period of time.



### 9 - Why do we use a session middleware ?

In order to use sessions, to store data when a user is logged in. This means that



### 10 - Why do we use a build process ?

Gulp or Grunt is used to keep css and js file sizes as small (e.g. by minifying or uglifying files) as possible to give a good user experience. They are used to compile css and optimize images too.
