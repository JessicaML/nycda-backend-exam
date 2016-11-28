## NYCDA Backend Exam
=====================
Explain the questions well!!

### 1- Why do we should include script tags at the very end of an html file, before closing </body>?

We want the page to load all the content before JS event handler load to the page, so that all content is loaded before interaction takes place, and the JS functions as it is designed to. This also means the static content (html and css) will load faster and give the user a better experience.

### 2 - What is a middleware?

It is a package which acts as glue between the express server and your app interface. It provided functions that are not available on the operating system, such as parsing data from a form or allowing a user to delete content.

### 3 - Why do we use express.static() middleware?

In order to use css and js files in a public directory within an express app.

### 4 - What is favicon.ico ?

Small icon at the left of the URL or on the tab, usually the company logo of the website.

### 5 - Why do we use a bodyParser middleware ?

In order to read form data that is posted from the client.

### 6 - What is the difference in terms of parsing data received from a web form with POST or an AJAX POST request?

AJAX is used for updating a webpage as soon as data comes in, without refreshing the page or going to a different web page. For example, when you post a comment on Facebook, this uses an AJAX POST request. When you send in a contact form, this uses a POST request.

### 7 - Why do we use methodOverride middleware ?

In order to delete content.

### 8 - What are the differences between sessions and cookies ?

Sessions is stored on the server side, cookies on the client side.

### 9 - Why do we use a session middleware ?

In order to use sessions, to store passwords securely (with encryption).

### 10 - Why do we use a build process ?

To help us outline each step of the lifecycle of the model, to decide what to do before and after each step, create, update, delete.
