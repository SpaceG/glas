---
layout: post

#event information
title:  "Create Commandline Node.js"
cover: "img/blur-background-1680x1050-spectrum-electromagnetic-4k-901-1.jpg"
date:   2016-05-11

#event organiser details
organiser: "Lucas Gatsas"


---
<h2 class="section-heading"> Create Commandline in node.js for your Sails.js</h2>


First: Make sure your App is running on Localhost <code>port:80</code>


Seconds: Clone Tilda : <a href="https://www.npmjs.com/package/tilda">Tilda</a>


Thrid: Create a<code>cli.js</code> file and inpust the following Code below

<div style="overflow:auto; height=200; width=100%;">
<pre style="color:black;background:white;"><pre>

// Make sure that no matter where we call the command from,
// we lift the app that lives in the same directory as this script
process.chdir(__dirname);
// Get an instance of Sails
var sails = require('sails');
// Lift the Sails app in the current working directory
       console.log("Start The GITLIST App");
        console.log("To see your app. visit:");
        console.log(clc.xterm(39).bgBlack.underline('http://127..0.0.1'));
        console.log("To Clone the Repository and Open Source:");
        console.log(clc.xterm(39).bgBlack.underline('see: http://www.github.com/spaceg/github.io'));
        console.log("Bash The Universe by Hello World");
        console.log("©.2016 by Gitlist OS");

        console.log("press c to stop the app");


sails.lift({log:{noShip: true}});

/*  sails.lift(rc('sails'));*/

</pre></pre></div>





Here is a Robost Code for the Commandline and lift your with your own commandline: 
here are the links:


package.json: <a href="https://github.com/SpaceG/gitlist.io/blob/master/package.json">package.json</a>

cli.js : <a href="https://github.com/SpaceG/gitlist.io/blob/master/cli.js">cli.js</a>

app.js : <a href="https://github.com/SpaceG/gitlist.io/blob/master/app.js">app.js</a>

.gitgnore <a href="https://github.com/SpaceG/gitlist.io/blob/master/.gitignore">.gitignore</a>

.local.js <a href="https://github.com/SpaceG/gitlist.io/blob/master/config/local.js">.local.js</a>




create a <code> .gitgnore </code> file for your Branch. Set it to the Root of your Directory. 
but the Following code Below in that file. Save it. 
<pre>
*.swp
*.swo
*~
*.log
node_modules




config/local.js
</pre>



After Include in your <code>package.json</code> the following code from the Tilda for the <code>bin</code>




<pre>
 "bin": {
    "gitlist": "./cli.js"
  },
</pre>


The full package.json file: 

<pre>

{
  "name": "gitlist",
  "version": "1.0.5",
  "description": "Gitlist OS",
  "keywords": [],
  "bin": {
    "gitlist": "./cli.js"
  },
  "dependencies": {
    "bcrypt": "~0.8.0",
    "commander": "^2.9.0",
    "ejs": "~0.8.4",
    "grunt": "0.4.2",
    "grunt-contrib-clean": "~0.5.0",
    "grunt-contrib-coffee": "~0.10.1",
    "grunt-contrib-concat": "~0.3.0",
    "grunt-contrib-copy": "~0.5.0",
    "grunt-contrib-cssmin": "~0.9.0",
    "grunt-contrib-jst": "~0.6.0",
    "grunt-contrib-less": "0.11.1",
    "grunt-contrib-uglify": "~0.4.0",
    "grunt-contrib-watch": "~0.5.3",
    "grunt-sails-linker": "~0.9.5",
    "grunt-sync": "~0.0.4",
    "include-all": "~0.1.3",
    "nodemailer": "~1.4.0",
    "passport": "~0.2.1",
    "passport-github": "^0.1.5",
    "passport-local": "~1.0.0",
    "passport-twitter": "~1.0.2",
    "password-generator": "^0.2.3",
    "progress": "^1.1.8",
    "rc": "~0.5.0",
    "sails": "~0.11.0-rc10",
    "sails-disk": "~0.10.0",
    "sails-hook-autoreload": "^0.11.4",
    "sails-mongo": "^0.12.0",
    "shortid": "~2.1.3",
    "tilda": "^4.2.1"
  },
  "scripts": {
    "start": "node app.js",
    "debug": "node debug app.js"
  },
  "main": "app.js",
  "repository": {
    "type": "git",
    "url": "git://github.com/SpaceG/gitlist.io.git"
  },
  "author": "lucasgatsas",
  "license": "BSD-2-Clause",
  "bugs": {
    "url": "https://github.com/SpaceG/gitlist.io/issues"
  },
  "homepage": "https://github.com/SpaceG/gitlist.io#readme"
}


</pre>


<div style="overflow:auto; height=200; width=100%;">
<pre style="color:black;background:white;"><pre>

#!/usr/bin/env node
// Make sure that no matter where we call the command from,
// we lift the app that lives in the same directory as this script
process.chdir(__dirname);

        console.log("HELLOOOOOOOOO");
        console.log("©.2016 by Gitlist OS");

        console.log("press c to stop the app");

// Get an instance of Sails
var sails = require('sails');
// Lift the Sails app in the current working directory
sails.lift({log:{noShip: true}});

</pre></pre></div>








Thats it. 




See the Issue Detail here on Github <a href="https://github.com/SpaceG/gitlist.io/blob/master/package.json"> package.json</a> 



package.json: <a href="https://github.com/SpaceG/gitlist.io/blob/master/package.json">package.json</a>

cli.js : <a href="https://github.com/SpaceG/gitlist.io/blob/master/cli.js">cli.js</a>

app.js : <a href="https://github.com/SpaceG/gitlist.io/blob/master/app.js">app.js</a>

.gitgnore <a href="https://github.com/SpaceG/gitlist.io/blob/master/.gitignore">.gitignore</a>

.local.js <a href="https://github.com/SpaceG/gitlist.io/blob/master/config/local.js">.local.js</a>


Tools:

Seconds: Clone Tilda : <a href="https://www.npmjs.com/package/tilda">Tilda</a>




