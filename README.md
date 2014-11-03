# m2sid-biblio

Welcome on this project page. This project is very simple library web tool management demonstration written with [Sails.js](http://sailsjs.org) and Node.js.
It was written under a school project, means that it cover just mandatory functionaries about library management.. 
There are many exception, logic which are not written. eg: (protect app against hack, some integrity through database management about library, etc).
The front-end use as less dependencies as possible. The logic is handled by Jquery. The dashboard is served by the web server and then interacts with it through REST request.

### The application is basically composed by three parts:
- A front end (The dashboard) written with HTML, CSS, Jquery. The code is as simple and clear as possible.
- The web server which serve the dashboard (Node.js under Sails.js)
- The REST part of the web server. (The front-end interact with the server through REST principle).

### All of this is a good showcase for "how to implement with sails.js":
- authentication.
- REST api.
- DB management (associations, ..).
- Layout and view management.
- Use of promises.
- Using flash messages.
- And other forgotten..

I know this app looks a bit like "unfinished" and a lot of comments are missing to makes things clear, so don't hesitate to open issues or contact me for any questions you have.

## Useful information
- Access account: maxime / password
- DB used is disk (like SQLite)

## Application composition
- **.tmp** Temporary and public folder. Generated by application when lifted. All public files are accessible and served via this folder.
- **api** Core of the application. Controllers, models, policies etc are component of web server applications.
- **api/models** This is the directory that holds your models. In Sails, models are the structures that contain data for your Sails App.
- **api/controllers** This is the directory that holds your controllers. In Sails, controllers are javascript files that contain logic for interacting with models and rendering appropriate views to the client.
- **api/policies** This is the folder you will store your policy files in. A policy file is a .js file that contains what is essentially express middleware for authenticating access to controller actions in your app.
- **api/responses** This folder holds the logic for issuing server responses to your clients.
- **api/services** This folder contains your services. 'Services' are similar to controller actions but are typically used for things that don't necessarily have to happen between the time when the user sends a request and when the server sends back a response.
- **assets** This folder contain all assets for the front side application.
- **config** This folder contain all configuration files necessary for web server application.
- **node_modules** npm downloaded modules.
- **tasks** Used by sails to write task about front side application deploying.
- **view** Contain all view files related to front side application.

## Get started
- Install Node.js
- Run `npm install` inside project root
- Launch web server with `sails lift` (Check autoLogon to true/false on the config/env/development depend of your need)
- Visit [http://localhost:1337](http://localhost:1337)
- Server logs are visible inside running console.

## Troubleshooting
- Be sure that no other app run on same port.
- Be sure that node process has rights to write in .tmp.

## How to make this app better (Not relative to library management)?
- Protect params against hack in a better way.
- Unify errors messages sent by REST api.
- Write tests.
- Make it multi-users
- Use a front-end framework like (Angular, Ember, ...) to make a very clear and powerful one page application.
- And it's impossible to list everything as it has not limit in fact :p.
