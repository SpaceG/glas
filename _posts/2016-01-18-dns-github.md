---
layout: post

#event information
title:  "DNS - Set UP"
cover: "img/8557ecd4_vlcsnap-2010-10-07-21h28m24s95.png"
date:   2014-10-13

#event organiser details
organiser: "Lucas Gatsas"


---
<h2 class="section-heading">Setting up a custom domain with GitHub Pages</h2>
<h2 class="section-heading">DNS for GitHub Pages</h2>





Get Ready with Sub-domain and Apex Domain @  Github. I will get a new Blog Name in the next Days or Weeks. However, i think i will do that right now, when i have more Time to do it. I have always a very nice New name in Mind. I Think it will be .io Domian Name. Maybe i will use a custome Blog Name (Apex-Domian) or a (Sub-Domian). We will see it. - 

<h2 class="section-heading">Sub Domains</h2>
A subdomain is configured with a CNAME record through your DNS provider (There where your  domain is Registered). 
We strongly recommend that you use a custom subdomain for these reasons:


It gives your GitHub Pages site the benefit of our Content Delivery Network.[Content Delivery Network. -Wikipedia](http://en.wikipedia.org/wiki/Content_delivery_network)
It will not be affected by changes in the underlying IP addresses of GitHub's servers.
Pages will load significantly faster because [Denial-of-service Attack](http://en.wikipedia.org/wiki/Denial-of-service_attack) protection can be implemented more efficiently.


<h2 class="section-heading">Apex Domains</h2>
An apex domain is usually configured with an <code>A</code>, <code>ALIAS</code>, or <code>ANAME</code> record through your DNS provider and is often assigned to one or more IP addresses.



I will set up my  Apex Domain @ Github, because i do host my Stuff and Website on Github. - There also some Points to set up one to your  Repositories. So far i have create a [User, Organization, and Project Pages](https://help.github.com/articles/user-organization-and-project-pages/). Which one can do everybody, if you have a Github account. You need also One to get Set Up your [Github Pages](https://pages.github.com/) .


So now we use a Apex Domain Name (www.yourdomain.com) or a Sub-Domian Name (www.hello.yourdomain.com). So we have get some Functions of the Cname.  [About custom domains for GitHub Pages sites](https://help.github.com/articles/about-custom-domains-for-github-pages-sites/)



If you're using a [Custom Domain](https://help.github.com/articles/about-custom-domains-for-github-pages-sites/) to redirect your GitHub Pages site, you must create and commit a CNAME file to your GitHub Pages repository that contains the custom domain.
[Adding a CNAME file to your Repository](https://help.github.com/articles/adding-a-cname-file-to-your-repository/)



ps: I give everysite a SSL Certificate to be mostly Safe - Both types of Pages are served over HTTP, not HTTPS. You shouldn't use them for sensitive transactions, like sending passwords or credit card numbers. - 






<h2 class="section-heading">Submit a CNAME file to your GitHub Repo</h2>
<h2 class="section-heading">Set Up the DNS </h2>


Add New file save ass CNAME 

<code>yourdomain.com</code>


Login in your NameCheap Account got to  All Host Records. Then set up the DNS  
and configuring (IP/ Adress/URL to <code> 192.30.252.153 </code> and the Record Type to <code>A</code> and TTL 1800)


set the Subdomain @  IP Adress/URL to <code> username.github.io  </code> and the Record Type to <code> CNAME (Alias) </code>



in the Sub-Domian Settings add an @ in the first - field. and add the IP Adress with the end <code>.154 </code>  

<code> 192.30.252.154 </code> and type Record Type A (Adress) and TTL 1800

<a href="#">
    <img src="{{ site.baseurl }}/img/lucasgatsas.ch-1.png" style="width:100%" alt="Lucas Gatsas">
</a>


Save a ll your Settings ! 

<!--
<a href="#">
    <img src="{{ site.baseurl }}/img/googleanalstic.png" alt="Post Sample Image" style="width:100%">
</a>
-->

<!--
<strong> Waterfall View</strong>

DNS Lookup,
Initial Connection,
SSL Negotiation,
Time to First Byte,
Content Download,
 3xx response,
 4xx+ response,
Start Render,
msFirstPaint,
DOM Content Loaded,
On Load,
Document Complete,


<a href="#">
    <img src="{{ site.baseurl }}/img/waterfall-view-001.png" style="width:100%" alt="Lucas Gatsas">
</a>



<strong> Connection View</strong>


DNS Lookup,
Initial Connection,
SSL Negotiation,
Start Render,
DOM Content Loaded,
On Load,
Document Complete,


<a href="#">
    <img src="{{ site.baseurl }}/img/connenction-view.png" style="width:100%" alt="Lucas Gatsas">
</a>





<a href="#">
    <img src="{{ site.baseurl }}/img/content.png" style="width:100%" alt="Lucas Gatsas">
</a>


-->

Do you can see the Web Page Test <a href="https://www.webpagetest.org/result/150430_1T_ER/">here</a> 



Update to the <a href="https://www.cloudflare.com">CloudFlare. </a> 


First Sigin in your CLoudFlare Setting up the <code>CNAME</code> and <code> A </code> Record. 


<a href="#">
    <img src="{{ site.baseurl }}/img/dns-cloudflare-2.png
" style="width:100%" alt="Lucas Gatsas">
</a>



Add the Nameserver to your Domainpoint! 


<a href="#">
    <img src="{{ site.baseurl }}/img/namecheap-servers-to-cloudflare.png" style="width:100%" alt="Lucas Gatsas">
</a>



Set Up your <code> https:// </code>


<a href="#">
    <img src="{{ site.baseurl }}/img/offline_over_https Kopie.png" style="width:100%" alt="Lucas Gatsas">
</a>


Set your ssl to Flexible inside your Interface @ Cloudflare. Wait for a Moment. 
If you Stuck, contact they. Awesome Supporters Outhere! 

<a href="#">
    <img src="{{ site.baseurl }}/img/ssl-cloudflare.png" style="width:100%" alt="Lucas Gatsas">
</a>




Open your Terminal : See your Changes : 


Dig your domian : <code> $ dig yourdomian.com </code> 

and <code> curl -I yourdomian.com </code> 


After 24 Hours i checked out my Nameservers! Awesome to see the Changes! 




<a href="#">
    <img src="{{ site.baseurl }}/img/dig-lucas-gatsas.png" style="width:100%" alt="Lucas Gatsas">
</a>



Status: 
<a href="#">
    <img src="{{ site.baseurl }}/img/ssl-cludflare-best.png" style="width:100%" alt="Lucas Gatsas">
</a>


To automatically forward HTTP requests to <code>HTTPS </code>, you can create a Page Rule by:

Open the Page Rules interface.
Entering <code> http://*lucasgatsas.ch/* </code> as the URL pattern.

Choose <code> "Always use https."</code>

Click <code> "Add rule." </code>

<a href="#">
    <img src="{{ site.baseurl }}/img/page-rules-01.png" style="width:100%" alt="Lucas Gatsas">
</a>


<!--

<a href="#">
    <img src="{{ site.baseurl }}/img/ssl-cludflare.png" style="width:100%" alt="Lucas Gatsas">
</a>

-->

Link: 
<a href="https://namecheap.com/">namecheap.com</a> 
Link: 
<a href="https://cloudflare.com">cloudflare.com</a> 
Link: 
<a href="https://github.com">github.com</a> 



<blockquote>
This is a SwissWatch! :)

	

</blockquote>