---
layout:     post
title:      "Installing nginx on OS X Yosemite"
subtitle:   "Use nginx for Bigger Websites and Start Ups."
date:       2015-04-12 14:00:44
author:     "Lucas Gatsas"
header-img: "img/tumblr_n5e4viuHai1r4v7ypo1_1280-1.jpg"
---

<h2 class="section-heading"><strong>Installing nginx on OS X Yosemite</strong> </h2>
<h2 class="section-heading">Localhost - Server </h2>






<strong> Install Brew</strong> : First you have also Install [brew.sh](http://git-scm.com/)  on your Machine! Go Install Brew and all Packages:

<code>ruby -e"$(curl -fsSL https://raw.githubusercontent.com/
Homebrew/install/master/install)"</code> 

More About: [ruby.org](https://www.ruby-lang.org/de/documentation/installation/#building-from-source) 


<a href="{{ site.baseurl }}/img/5-things-you-didnt-know-nginx-could-do-velocity-3-638.jpg">
    <img src="{{ site.baseurl }}/img/5-things-you-didnt-know-nginx-could-do-velocity-3-638.jpg" alt="Lucas Gatsas"  style="width:100%">
</a>


After Install Brew: Follow these Steps : 

<h2 class="section-heading">Installing nginx on OS X
</h2>


To install nginx, simply open up the Terminal and enter the following command.

<code> brew install nginx</code>

That’s it! Assuming that no errors occurred, then nginx is ready to start. But let’s first change the default port.

<a href="{{ site.baseurl }}/img/install-nginx.png">
    <img src="{{ site.baseurl }}/img/install-nginx.png" alt="Lucas Gatsas"  style="width:100%">
</a>



Bingo! :) Here we GO Run Nginx : 



<a href="{{ site.baseurl }}/img/nginx-install-4-700.png">
    <img src="{{ site.baseurl }}/img/nginx-install-4-700.png" alt="Lucas Gatsas"  style="width:100%">
</a>




<strong>Notice: if you get an error : </strong>

<div style="overflow:auto; height=200; width=100%;">
<pre style="color:black;background:white;"><pre>

Space-Odysseys-Mac-Pro:~ cyberspace$ brew install nginx
/usr/local/bin/brew: /usr/local/Library/brew.rb: /System/Library/Frameworks/Ruby.framework/Versions/1.8/usr/bin/ruby: bad interpreter: No such file or directory
/usr/local/bin/brew: line 21: /usr/local/Library/brew.rb: Undefined error: 0 

</pre></pre></div>


<a href="{{ site.baseurl }}/img/done-ruby-.png">
    <img src="{{ site.baseurl }}/img/done-ruby-.png" alt="Lucas Gatsas"  style="width:100%">
</a>

<blockquote> :) >> Warning: fast-forwarding your working tree from </blockquote>


Try this out: very simple: 

Open Terminal and Type : 

<code> cd /usr/local/Library </code>

<code>git pull origin master  </code>

Or if you go with sudo, then type :

<code> sudo git pull origin master </code> 






In case you have changes in the directory (/usr/local/Library), the git pull will throw an error. In that case, you'll have to fetch the master branch and set it forcibly as master:



<code> git fetch --all </code> 

<code> git reset --hard origin/master </code> 



  This will upgrade your homebrew and you can use brew again.


<a href="{{ site.baseurl }}/img/ruby-done-1.png">
    <img src="{{ site.baseurl }}/img/ruby-done-1.png" alt="Lucas Gatsas"  style="width:100%">
</a>


If you installed Homebrew as a non-root user, you'll need to cd to <code> /Users/yourusername/homebrew/Library</code> instead of <code>/usr/local/Library.</code>



<h2 class="section-heading"><strong>Changing nginx’ Default Port to 80</strong> </h2>
<h2 class="section-heading">8080 - default port</h2>


By default, nginx listens to <code> port 8080 </code>, but let us change that to the default HTTP port, which is 80. To do that, we need to make a simple change to the configuration file <code>  /usr/local/etc/nginx/nginx.conf. </code> You can do this with any text editor such as <code>vi</code> or <code>nano</code>


<code>sudo vi /usr/local/etc/nginx/nginx.conf</code>


Scroll a bit down and you should see the following.


<div style="overflow:auto; height=200; width=100%;">
<pre style="color:black;background:white;"><pre>

server {
        listen       8080;
        server_name  localhost;

        #charset koi8-r;

        #access_log  logs/host.access.log  main;

        location / {
            root   html;
            index  index.html index.htm;
        }
        
        ...       
}

</pre></pre></div>

What you want to do is to simple change the number 8080 to 80 next to the listen keyword.



<h2 class="section-heading">Testing</h2>


To start up nginx, simply enter the following command in the Terminal.


<code>sudo nginx</code>

nginx should now start up, and you can test that everything works by navigating to <code>http://localhost</code> in your browser.





If you have problems starting up nginx, a common problem is that the port that nginx is configured to listen to is already in use. If you changed the port to <code>80</code>, then this could be an Apache web server or Skype, for instance.

Should you need to stop nginx, then you can do so with the below command.

<code>sudo nginx -s stop</code>

As you have seen, nginx is very simple to install and set up on OS X Yosemite!



<blockquote>
“Best startups generally come from somebody needing to scratch an itch.” -Michael Arrington, TechCrunch 
</blockquote>

