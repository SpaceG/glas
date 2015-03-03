---
layout:     post
title:      "Bootstrap Currently v3.3.1 - Front-End Framework"
subtitle:   "Bootstrap makes front-end web development faster and easier."
date:       2015-01-10 13:00:40
author:     "Lucas Gatsas"
header-img: "img/lucas-gatsas-05.jpg"
---
<h2 class="section-heading">Bootstrap is the most popular HTML, CSS, and JS framework for developing responsive, mobile first projects on the web.</h2>


<p>Bootstrap makes front-end web development faster and easier. It's made for folks of all skill levels, devices of all shapes, and projects of all sizes. </p>

What is Bootstrap? Bootsrap is a Fast Farmaework for Front-End Developers. To build fast, sleek, clean Front-End Design. Watch the Opensource base [Bootstrap Currently v3.3.1](http://getbootstrap.com/getting-started/) for Sass or dist files check out here [Sass Bootstrap Currently v3.3.1](http://github.com/twbs/bootstrap-sass/archive/v3.3.1.tar.gz/) . For Introduction and how to work with Bootstrap. See the Docs. [Docs Bootstrap v3.3.1](http://getbootstrap.com/getting-started/#whats-included) . Get Started with Bootstarp. See the Basic Set Up [Template Bootstrap v3.3.1](http://getbootstrap.com/getting-started/#template). Compiling CSS and JavaScript with 
[Grunt](http://gruntjs.com/Grunt/) 
let's see the Available Grunt commands for Bootstrap. [Commands on Bootsrap](http://getbootstrap.com/getting-started/#grunt).

Then, from the command line:
Install <code>grunt-cli</code> globally with <code>npm install -g grunt-cli.</code>
Navigate to the root <code> /bootstrap/ </code> directory, then run <code> npm install </code>. npm will look at the <code> package.json </code> file and automatically install the necessary local dependencies listed there.   



Download
[Bootstrap Currently v3.3.1](http://getbootstrap.com/)


<!--
<a href="#">
    <img src="{{ site.baseurl }}/img/bootstrap-wordpress-themes.jpg" alt="Post Sample Image" style="width:100%">
</a>

-->

<!--
<a href="#">
    <img src="{{ site.baseurl }}/img/gitlist.io.png" alt="Post Sample Image">
</a> -->

<h2 class="section-heading">Javascript Library</h2>

<p>
Varying modal content based on trigger button
Have a bunch of buttons that all trigger the same modal, just with slightly different contents? Use event.relatedTarget and HTML data-* attributes (possibly via jQuery) to vary the contents of the modal depending on which button was clicked. See the Modal Events docs for details on relatedTarget, </p>

<div style="overflow:auto; height=200; width=100%;">
<pre style="color:black;background:white;"><pre>$('#exampleModal').on('show.bs.modal', function (event) {
  var button = $(event.relatedTarget) // Button that triggered the modal
  var recipient = button.data('whatever') // Extract info from data-* attributes
  // If necessary, you could initiate an AJAX request here (and then do the updating in a callback).
  // Update the modal's content. We'll use jQuery here, but you could use a data binding library or other methods instead.
  var modal = $(this)
  modal.find('.modal-title').text('New message to ' + recipient)
  modal.find('.modal-body input').val(recipient)
})
</pre></pre></div>



<blockquote>Your work is going to fill a large part of your life, and the only way to be truly satisfied is to do what you believe is great work. And the only way to do great work is to love what you do. If you haven't found it yet, keep looking. Don't settle. As with all matters of the heart, you'll know when you find it.

- Steve Jobs

</blockquote>


<!-- 
<a href="#">
    <img src="{{ site.baseurl }}/img/jekyllthemewhite.png" alt="Post Sample Image">
</a> 



 -->



