# simpleWebCalculator
## description
this project is used to solidify my knowledge on nodeJS, expressJS, npm, nodemon. the project contains two routes:
  - calculates the sum of two numbers given by user on the website
  - calcualte BMI
the server runs on Express framework, and it provides sendFile() method allow me to .html file.

## some of the command used and notes for myself
  1. basic setup
      - `mkdir Calculator`
      - `touch calculator.js`
      - `npm init` : set up a new NPM package
      - `npm install express`: use NPM install **express** module
      - `const express = require("express")`: require express in .js
      - `const app = express()` : set up express
      - Create a root route get method with `app.get()`
      - Send the words **Hello World** from the root route as the response : for testing 
      - Spin up  server on port 3000 with `app.listen()`
      - `nodemon calculator.js` : run sever
   2. responding to Requests with HTML files
      - `touch index.html`
      -  set up html barebone code then add related code for this project
      - `res.sendFile(__dirname + "/index.html")` in **calculator.js** 
   3. processing Post Request with Body parser
      - `npm install body-parser` : allow us to parse the info that's send through POST request, so we can do calculations in this project
      -  require body-parser
      - by using `bodyParser`, we are able to parse the http request that we get.
      - by using `urlencoded({extended: true})`, we can get access to url form data.
