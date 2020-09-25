# Laptop-banner

This little project was designed as a handling practices of NODE.JS starting from reading the content of the JSon file and then parse it into a JavaScript object. Node.JS comes with the powerful module system and most of the functionality that we have in Node is always in one of the Node packages. In this particular project I decided to use the following three core Node modules below:

1. const fs = require('fs'); - "File System" module;
2. const http = require('http'); - "HTTP" module was used to create a WEB server;
3. const url = require('url'); - "URL" module was used for implementing the ROUTING.

! I found a good idea to give to variables the same names as the package names.

***

In the "FS" module, I used the "Synchronous call" and in order to display the content of the file as a string, I used the (UTF-8) code.

const json = fs.readFileSync(${__dirname}/data/data.json, 'utf-8');

***

Creating the server, I passed a CallBack function that works each time when someone accesses the WEB server, therefore I have added the "request" and the "response" objects.

const server = http.createServer((req, res) => {...}
\\ please see the full code in my repository.

***

In order to respond a different ways to different URLs, I have also added the third module called "ROUTING" into this project

const pathName = url.parse(req.url, true).pathname;
\\ please see the full code in my repository.

***

These are all the key points I have just briefly described about this project however for more details you are always welcome to visit my repository.
