# api-node

Hello Everyone,

In this project we will learn how to create a simple API RESTFFul Node + Express + MongoDb!
Let's go!

First you need downloading this project and then install all dependencies for starting

# Dependencies

body-parser
express
mongoose
request

# How to install

git clone https://github.com/nathsilv/api-node.git
npm install

Now you have this project on your PC and all dependencies are installed.
Let's understand  each file!

# FILE: package.json

In this file we have our signature and dependencies that project will need!
Once that you have all dependencies in this file you just need to execute: 'npm install' to install them.
This way is practice for exporting your project and you don't have a hard word for installing each dependency manually.

# FILE: server.js

Here we have our server that we will up!
This file has all routes and verbs that API will use.

API ROUTES AND VERBS

POST   - router.route('/series')           => To add a serie
GET    - router.route('/series')           => to get all series
GET    - router.route('/series/:serie_id') => To get a specific serie
PUT    - router.route('/series/:serie_id') => To update a specific serie
DELETE - router.route('/series/:serie_id') => To delete a specific serie

# FILE: serie.js

Now we define how will be our schema on BD and exports this model to be used in POST, GET, PUT or DELETE.

# After you know all this, how do you up the server?

node server.js

A messange should be displayed: 'Starting API on port 5000'

# Ready! Our API has been started!

You can use Postman for testing if API is working
With postman open, choose a any verb, for exemple: 'GET' and put a url: 'http://localhost:5000/api/series/'
It should to return all series on BD if it exists.

PS: on server.js you need a uri for connecting on bd

mongoose.connect('mongodb://root:12345678@jello.modulusmongo.net:27017/Hira2hyp');

You can access this link: https://xervo.io/, create account and create a database, then get uri and put in this line

mongoose.connect('your_uri');


Do not get stuck in this simple project, always seek more knowledge

"There are no strings on me" - Ultron - The Avengers
