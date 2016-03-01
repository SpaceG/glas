---
layout: post

#event information
title:  "SSH Key on Mac OsX"
cover: "img/Lucas_Gatsas_lucas_gatsas_0268.jpg"
date:   2015-01-29
start_time: "10:00"
end_time: "17:00"

#event organiser details
organiser: "Lucas Gatsas"


---

<h2 class="section-heading"><strong> Secure Shell - SSH - Key on Mac Os X </strong> </h2>
<h2 class="section-heading">The Key Set Up.</h2>




<a href="{{ site.baseurl }}/img/bash-ssh-1.png">
    <img src="{{ site.baseurl }}/img/bash-ssh-1.png" alt="Lucas Gatsas lucas gatsas" title="lucas gatsas Lucas Gatsas"  style="width:100%">
</a>


Enter Commandlines :


<code>ssh-keygen -t rsa</code>

after enter your path again :

<code>/Users/cyberspace/.ssh/id_rsa</code>

Overwrite <code> (y/n)?  </code> press <code>yes</code>


Enter: if you don't want a passphrase

press Enter to get your Key - Gen ! 



<a href="{{ site.baseurl }}/img/bash-ssh-2.png">
    <img src="{{ site.baseurl }}/img/bash-ssh-2.png" alt="Lucas Gatsas lucas gatsas" title="lucas gatsas Lucas Gatsas" style="width:100%">
</a>



Type <code> ssh-add </code> and press Enter!

add <code> ssh-add -l </code> to see your <code> .ssh/id_rsa  </code>



<a href="{{ site.baseurl }}/img/bash-ssh-3.png">
    <img src="{{ site.baseurl }}/img/bash-ssh-3.png" alt="Lucas Gatsas lucas gatsas" title="lucas gatsas Lucas Gatsas"  style="width:100%">
</a>


follow steps : 

<code> ls </code> show list :

enter your rsa id like here <code> cat id_rsa </code> 

This is The Private Key !

-----BEGIN RSA PRIVATE KEY-----






<a href="{{ site.baseurl }}/img/bash-ssh-4.png">
    <img src="{{ site.baseurl }}/img/bash-ssh-4.png" alt="Lucas Gatsas lucas gatsas" title="lucas gatsas Lucas Gatsas"  style="width:100%">
</a>



Now : Check out the Public Key : 

Type following Commandline : <code>cat id_rsa.pub </code>


<a href="{{ site.baseurl }}/img/bash-ssh5.png">
    <img src="{{ site.baseurl }}/img/bash-ssh5.png" alt="Lucas Gatsas lucas gatsas" title="lucas gatsas Lucas Gatsas"  style="width:100%">
</a>


Next Step ! Login In your Root Server!
Update Post soon. ! 




<br>


	


Diagramm of my SSH Sketches! 






<a href="{{ site.baseurl }}/img/lucasgatsas_grafic.png">
    <img src="{{ site.baseurl }}/img/lucasgatsas_grafic.png" alt="Lucas Gatsas"  style="width:100%">
</a>




<a href="{{ site.baseurl }}/img/dia_01_ssh_tube_bylucas-gatsas.png">
    <img src="{{ site.baseurl }}/img/dia_01_ssh_tube_bylucas-gatsas.png" alt="Lucas Gatsas"  style="width:100%">
</a>


Sketches by Lucas Gatsas : Free to Use

<!--
<strong> Diagram of the SSH private-public key pair transactions, as defined within the SSH defined architecture model </strong>

<a href="#">
    <img src="{{ site.baseurl }}/img/SSH_public_private_key.gif" alt="Lucas Gatsas"  style="width:100%">
</a>
-->





<blockquote>
“Best startups generally come from somebody needing to scratch an itch.” -Michael Arrington, TechCrunch 
</blockquote>

