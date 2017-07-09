---
layout: post

#event information
title:  "$npm install gitlist"
cover: "img/gl-1212-1.png"
date:   2016-05-07

#event organiser details
organiser: "Lucas Gatsas"


---
<h2 class="section-heading"> Create npm packages</h2>


We have created a package for our OS @npmjs.com
Getting Started with Gitlist OS <a href="https://www.npmjs.com/package/gitlist/tutorial"> $npm install gitlist </a>


download the package via npm 

<code> $ npm install gitlist </code> 




<h2> To Create a Package </h2>


Go to your Folder which the App is Created:

Open it with the Terminal <code> ls </code>
your App. Create your package.json file. 

<code> $npm run build </code>

Going back to your Folder <code>cd</code>

<code>$ vi package.json</code>

Include your Node Tree like Name of the package, the Version etc. 

<pre>
{
  "name": "gitlist",
  "version": "1.0.7",
  "description": "Gitlist OS",
  "keywords": [],
  "dependencies": {
    "bcrypt": "~0.8.0",
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

after you want to publish your package: 
going back to your Terminal


prompt the Terminal 

<code> $ npm adduser</code>

<pre>
Password: 
Email: (this IS public) npm.demo.user@gmail.com

....
</pre>

wait a Moment 

prompt after this Commandline 


<code> npm config ls </code>
do you will see your informationa which one do you have submited to your <code>$ npm adduser </code>

going to the Webiste of Npmjs.com like :

<a href="https://www.npmjs.com/~spaceg"> https://www.npmjs.com/~spaceg </a>

Right now, your are fix to publishing your package!
with the Commandline 

<code> $ npm publish</code>

do you will see the Version Number of the App which do you have included to the package.json file !

<pre>
cyberspace$ npm publish
+ gitlist@1.0.6
</pre>

Now, do you can chec your npm package to see if it published and to see its possible to download...


press to see your package & to download. 
<code>$ npm install yourpackage name </code>
mine also:
<code> $npm install gitlist </code>


you can test it with the commandline to see the Message  from the Console like : <code>node test.js</code>  

i have created a<code> index.js</code> file in the root of the Folder of the App.

and put in this export Message :

<pre>
exports.printMsg = function() {

	console.log("Thanks using npm install gitlist");
}
</pre>


dyou can see the Version patch with the Commandline 

<code> $ npm version patch </code>
it give the Output of the Version Informations. 


Thats it! Have fun with the Modern npm packages !





See the Current Install Video:

<iframe width="100%" height="425" src="https://www.youtube.com/embed/mOZGPi0grTw" frameborder="0" allowfullscreen></iframe>

Current Work Flow  : gitlist V.1.0.2 - Testing App - Notify me of follow-up comments & posts by email.

<iframe width="100%" height="425"  src="https://www.youtube.com/embed/ibCQfTGpriw" frameborder="0" allowfullscreen></iframe>


<a href="http://www.github.com/spaceG/gitlist.io">Gitlist OS Source </a>

<code> $ git clone https://github.com/SpaceG/gitlist.io.git </code>

<code> $ sudo sails lift </code>

<code> $ npm install </code> 

<code> $ npm install sails-mongo --save  </code> 



first remove the <code> node_module </code>  folder, then install npm packages <code> $npm install</code>  then after, <code> $ sudo sails lift </code> , do you will see, it give a error back, becuase do you haven't install MongoDB packages.. install Mongo DB : via commandline in the same dictory which you launch the full app : run <code> npm install sails-mongo --save  </code> then it will intsall all MongoDB Packages : then run again <code> $ sudo sails lift </code>  .


Clone The Master Branch to your Desktop: <a href="https://github.com/SpaceG/gitlist.io/"> Clone Gitlist Master  </a>

Read the Full Documentation here on my Github : <a href="https://github.com/SpaceG/gitlist.io/blob/master/README.md"> Gitlist Documentation </a>

If you find a Bug or Update the Source give a Note about a Issue :
 <a href="https://github.com/SpaceG/gitlist.io/issues
"> Gitlist OpenSource Issues </a> 


Big dedicated to my Friends Stellardrone: 

<iframe width="100%" height="425" src="https://www.youtube.com/embed/YPRTIonMVQY" frameborder="0" allowfullscreen></iframe>


