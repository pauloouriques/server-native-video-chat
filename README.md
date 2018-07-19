Native Video Chat Signaling server
==================================

## Installation

Native Video Chat Signaling server requires [Node.js](https://nodejs.org/) v6+ to run.

Install the dependencies and devDependencies and start the server.

```sh
$ cd server-native-video-chat
$ npm install -d
$ node bin/www
```

## Deploy on Heroku

In order to publish our server and get a public HTTPS (riquired by WebRTC)
URL we recommend to use [Heroku](https://heroku.com/):

Install the Heroku CLI
Download and install the [Heroku CLI](https://devcenter.heroku.com/articles/heroku-cli).

If you haven't already, log in to your Heroku account and follow the prompts to create a new SSH public key.

```sh
$ heroku login
```
Clone the repository
Use Git to clone server-native-video-chat's source code to your local machine.


```sh
$ git clone git@github.com:pauloouriques/server-native-video-chat.git
```

Add your heroku app remote to our repository

```sh
$ cd server-native-video-chat
$ heroku git:remote -a your-heroku-app-name
```

#### Deploy your changes
Make some changes to the code you just cloned and deploy them to Heroku using Git.

```sh
$ git add .
$ git commit -am "make it better"
$ git push heroku master
```