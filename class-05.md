## Read: 05 - Heroku Deployment:

## what is Heroku: 
**Heroku** is a cloud service provider and software development platform which facilitates fast and effective building, deploying and scaling of web applications. It has 140 inbuilt add-ons, ranging from alerts, analytic tools security services which are used for purpose like monitoring, caching and mailing or networking add-ons.

The tool can provide you with built-in instant run-time application services. Moreover, you don't need to think about infrastructure because it managed automatically by the software itself. Heroku is owned by Salesforce.

### How can I do this with Heroku?
using **Node.js** for our project. **Node.js**: is an open source, cross-platform runtime environment, which allows us to build server-side and networking applications. It's written in **JavaScript** and can be run within the 
**Node.js** runtime on any platform. 
 folwing the steps:
 1.  create a JavaScript file. :

 ``
 var http = require("http");
http.createServer(function(request, response) {
  response.writeHead(200, {"Content-Type": "text/plain"});
  response.write("It's alive!");
  response.end();
}).listen(3000);
``
 2. Run at your terminal: ```node server.js```
 3. Then check it in your browser. 

 >>Node allows you to use the so-called event loop, which works faster because of non-blocking behavior. 
 >>

 ### How to Make it worldwide:
useing **Heroku** cloud application platform for this. by running a spesfic commands in the terminal after doing the server itself using **Node**.

