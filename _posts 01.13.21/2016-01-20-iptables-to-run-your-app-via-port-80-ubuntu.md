---
layout: post

#event information
title:  "ipTabels Port 80 Ubuntu"
cover: "img/the-matrix-red-pill-blue-pill-1.jpg"
date:   2015-01-18
start_time: "10:00"
end_time: "17:00"

#event organiser details
organiser: "Lucas Gatsas"


---
<h2 class="section-heading">ipTables</h2>

<h2 class="section-heading">Run Your Web App via port 80 on Ubuntu Linux Machine - Sails.js</h2>

{% highlight ruby %}


--iptables -A INPUT -i eth0 -p tcp --dport 80 -j ACCEPT
--iptables -A INPUT -i eth0 -p tcp --dport 8080 -j ACCEPT
--iptables -A PREROUTING -t nat -i eth0 -p tcp --dport 80 -j REDIRECT --to-port 8080

{% endhighlight %}


<!--

<a href="{{ site.baseurl }}/img/p-4.png">
    <img src="{{ site.baseurl }}/img/p-4.png" alt="Lucas Gatsas lucas gatsas" title="lucas gatsas Lucas Gatsas"  style="width:100%">
</a>


--> 




Link: <a href="https://github.com/balderdashy/sails/issues/1361" target="_blank"> Github Issues 1361</a> 
Link: <a href="https://github.com/balderdashy/sails/issues/3292" target="_blank"> Github Issues 3292</a> 



<blockquote>
"Port Running on Linux Ubuntu Servers"
</blockquote>


