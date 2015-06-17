---
layout:     post
title:      "OpenSSL - Os X - Linux on nginx Server Linux"
subtitle:   "Run it over https"
date:       2015-05-18 14:00:44
author:     "Lucas Gatsas"
header-img: "img/tumblr_static_2014-07-30_09.18.41_1.jpg"
---
<h2 class="section-heading">How To Create a SSL Certificate on nginx for Ubuntu 12.04</h2>
<h2 class="section-heading">Install Transport Layer Security - Secure Sockets Layer (SSL)</h2>

<strong> Set Up </strong> 


<code> $ sudo apt-get install nginx </code>


<strong> Step One—Create a Directory for the Certificate </strong> 


<code>sudo mkdir /etc/nginx/ssl</code>


We will perform the next few steps within the directory:


<code>  cd /etc/nginx/ssl </code> 


<strong>Step Two—Create the Server Key and Certificate Signing Request</strong> 


<code> sudo openssl genrsa -des3 -out server.key 2048 </code>


Follow up by creating a certificate signing request:


<code>sudo openssl req -new -key server.key -out server.csr</code>





You are about to be asked to enter information that will be incorporated
into your certificate request.
What you are about to enter is what is called a Distinguished Name or a DN.
There are quite a few fields but you can leave some blank
For some fields there will be a default value,
If you enter '.', the field will be left blank.-----
Country Name (2 letter code) [AU]:CH
State or Province Name (full name) [Some-State]:St. Gallen
Locality Name (eg, city) []:Saint City
Organization Name (eg, company) [Internet Widgits Pty Ltd]:lucasgatsas.ch 
Organizational Unit Name (eg, section) []:Dept of Engineering - IT NERDS
Common Name (e.g. server FQDN or YOUR name) []:lucasgatsas@gmail.com                  
Email Address []:lucasgatsas@example.com






<strong> Step Three—Remove the Passphrase </strong> 


<code> sudo cp server.key server.key.org </code> 
<code> sudo openssl rsa -in server.key.org 
	-out server.key </code> 


<strong> Step Four— Sign your SSL Certificate </strong> 


<code>  sudo openssl x509 -req -days 365 -in server.csr 
	-signkey server.key -out server.crt </code>




<strong> Step Five—Set Up the Certificate </strong> 


<code>sudo cp /etc/nginx/sites-available/default
 /etc/nginx/sites-available/example</code>


Then go ahead and open up that new file:




<code> sudo nano /etc/nginx/
	sites-available/example </code>



Scroll down to the bottom of the file and find the section that begins with this:


	# HTTPS server

	server {
	        listen 443;
	        server_name example.com;

	        root /usr/share/nginx/www;
	        index index.html index.htm;

	        ssl on;
	        ssl_certificate /etc/nginx/ssl/server.crt;
	        ssl_certificate_key /etc/nginx/ssl/server.key; 
	}





	# Make site accessible from http://localhost/
	# server_name localhost;


<strong> Step Six—Activate the Virtual Host </strong> 


The last step is to activate the host by creating a symbolic link between the sites-available directory and the sites-enabled directory.


<code>  sudo ln -s /etc/nginx/sites-available/example 
	/etc/nginx/sites-enabled/example </code>


Then restart nginx:


<code>  sudo service nginx restart </code>


Visit https://youraddress



Cheers! 



Link: <a href="https://github.com/openssl/openssl">OpenSSL</a> Link: <a href="http://www.openssl.org/source/">OpenSSL Website</a>


<br>
<blockquote>
“Wir leben alle unter dem gleichen Himmel, aber wir haben nicht alle den gleichen Horizont.” 
</blockquote>

