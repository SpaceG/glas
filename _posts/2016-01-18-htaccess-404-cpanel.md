---
layout: post

#event information
title:  "htaccess 404 cPanel Server"
cover: "img/stork_v3.jpg"
date:   2015-06-01
start_time: "10:00"
end_time: "17:00"

#event organiser details
organiser: "Lucas Gatsas"


---
<h2 class="section-heading">Modify .htaccess</h2>
<h2 class="section-heading">"Separat Things on cPanel"</h2>

To Run a .htaccess File on your cPanel Server. <code> ErrorDocument 404 /404.html</code> Create One, Save it as <code>.htaccess</code> and create a <code>404.html</code> or <code>505.html</code>. <strong>Notice:</strong> Do you don't will see this File on your Machine or Computer. Becuase it's a invisible and hidden File.


<a href="http://space.lucasgatsas.ch/64376473647637467364634376437647364736473647356736537657365763576375673657365763756376">space.lucasgatsas.ch</a>

<br><br>

<strong>Redirect from HTTP to HTTPS</strong>


<pre>

for any domain .htaccess takes effect on:

         RewriteEngine On
         RewriteCond %{HTTPS} off 
         RewriteRule (.*) https://%{HTTP_HOST}%{REQUEST_URI} 


</pre>

<strong>for a certain domain, example.com:</strong>

<pre>

         RewriteCond %{SERVER_PORT} 80      
         RewriteCond %{HTTP_HOST} ^example\.com$ [OR] 
         RewriteCond %{HTTP_HOST} ^www\.example\.com$ 
         RewriteRule ^(.*)$ https://www.example.com/$1 [R,L] 

<pre>


<strong>Redirect from non-WWW to WWW</strong>


<strong>for any domain .htaccess takes effect on:</strong>

<pre>
         RewriteEngine On 
         RewriteCond %{HTTP_HOST} !^www\. 
         RewriteRule ^(.*)$ http://www.%{HTTP_HOST}/$1 [R=301,L] 
</pre>

<strong>for a certain domain, example.com:</strong>

<pre>
         RewriteEngine On     
         RewriteCond %{HTTP_HOST} ^example\.com$ [NC] 
         RewriteRule ^(.*)$ http://www.example.com/$1 [R=301,L] 

</pre>

<strong>Redirect from WWW to non-WWW</strong>

<strong>for any domain .htaccess takes effect on:</strong>

<pre>
         RewriteEngine On
         RewriteCond %{HTTP_HOST} ^www\.(.*)$ [NC] 
         RewriteRule ^(.*)$ http://%1/$1 [R=301,L]
</pre>

<strong>for a certain domain, example.com:</strong>

<pre>
         RewriteEngine On 
         RewriteCond %{HTTP_HOST} ^www\.example\.com [NC] 
         RewriteRule (.*) http://example.com/$1 [R=301,L]
</pre>

<strong>Changes the directory root for the main domain to public_html/subfolder</strong>

<pre>
         RewriteEngine on 
         RewriteCond %{HTTP_HOST} ^(www.)?example.com$ 
         RewriteCond %{REQUEST_URI} !^/subfolder/ 
         RewriteCond %{REQUEST_FILENAME} !-f 
         RewriteCond %{REQUEST_FILENAME} !-d 
         RewriteRule ^(.*)$ /subfolder/$1 
         RewriteCond %{HTTP_HOST} ^(www.)?example.com$ 
         RewriteRule ^(/)?$ subfolder/index.php [L] 
</pre>

<br>



