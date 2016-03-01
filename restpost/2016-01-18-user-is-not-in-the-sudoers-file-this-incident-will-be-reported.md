---
layout: post

#event information
title:  "sudoers file  Add Premission to any User"
cover: "img/der-wanderer-ueber-dem-nebelmeer-_357909-45.jpg"
date:   2013-06-11
start_time: "10:00"
end_time: "17:00"

#event organiser details
organiser: "Lucas Gatsas"


---
<h2 class="section-heading"><strong>Sudoers</strong> </h2>

<h2 class="section-heading">Add a User to Sudoers in Mac OS X</h2>

(1.) Launch Terminal : type : 

<code>sudo visudo</code>




(2.) Change your User Privilege specification

<code># User privilege specification </code>

<code>root  ALL=(ALL) ALL</code>

<code>%admin    ALL=(ALL) ALL</code>



(3.) Add Below the User Privilege specification 

<code>
youradminusername ALL=(ALL) ALL
</code>

 See The Blue Marked Window in the Terminal : 

<a href="#">
    <img src="{{ site.baseurl }}/img/sudoerspic.png" style="width:100%" alt="Lucas Gatsas">
</a>


(4.)  Now press “ESC” (escape) key to stop editing the file

(5.) Enter the : key (colon) and then type <code>“wq”</code> followed by the Return key to save changes and <code> exit vi</code>




Go to the Finder:  Do you can find the file in the phat <code>etc/sudoers</code>

(1.) Open it with right Mouse Click and << Open with other >> 

(2.) the Finder Menu will Open 

(3.) Open with enable  << All Applications >> with your Text Editor

(4.) After changes Save the File. Enter ! :)


<blockquote>
    "Open Terminal and do crazy Things! :) "
</blockquote>