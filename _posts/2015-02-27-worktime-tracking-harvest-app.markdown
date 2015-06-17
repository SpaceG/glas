---
layout:     post
title:      "Worktime Tracking App from Havest App"
subtitle:   "Track your Worktime"
date:       2015-02-27 14:00:44
author:     "Lucas Gatsas"
header-img: "img/game_of_thrones_daenerys_targaryen-1548001.jpg"
---
<h2 class="section-heading">Tracking your Worktime </h2>

I have discovered a good App to track the Work Time. Go See [harvestapp.com](https://harvestapp.com/). So far I have used a small Script. I need a clean Time Counter and Harvest App is perfect for. Now i decide to sign up to [spaceggithubio.harvestapp.com](https://spaceggithubio.harvestapp.com/account/login?return_to=%2Ftime).

<!--
<div class="row">
        <div class="col-md-4"></div>
        <div class="col-md-4"><img class="img-circle img-responsive img-center" src="{{ site.baseurl }}/img/9k=.jpg" alt="">  <h3>Helen V. Holmes
                    <small>Designer and Front-End Web Developer @Capital One - U.S.A</small>
                </h3></div>
        <div class="col-md-4"></div>
      </div>
-->


- Links 
[spaceggithubio.harvestapp.com](https://spaceggithubio.harvestapp.com/account/login?return_to=%2Ftime) 

- Links 
[harvestapp.com](https://harvestapp.com/) 


<h2 class="section-heading">Tracking </h2>

<a href="#">
    <img src="{{ site.baseurl }}/img/wf1.png" alt="Post Sample Image" style="width:100%">
</a>


<a href="#">
    <img src="{{ site.baseurl }}/img/week1.png" alt="Post Sample Image" style="width:100%">
</a>


<a href="#">
    <img src="{{ site.baseurl }}/img/week3.png" alt="Post Sample Image" style="width:100%">
</a>


<a href="#">
    <img src="{{ site.baseurl }}/img/week2.png" alt="Post Sample Image" style="width:100%">
</a>



I got this Script to Count Lines of Code of our Start Up. We write alot of Code and Lines.
[Count Lines of Code in Mac OS X](http://www.experimentgarden.com/2010/06/count-lines-of-code-in-mac-os-x.html) 


<code> find . -type f -name '*.php' -exec awk 'END {print NR}' '{}' + 2>/dev/null | awk '{ total+=$1 }END{print total}' </code>




<br>

I have found another Terminal Command [CLOC](http://cloc.sourceforge.net/) Count Lines of Code! You can download it directly @ Sourceforge 
[sourceforge.net](http://sourceforge.net/projects/cloc/files/) 


It’s easy to install on OS X:


<code>$ brew install cloc </code>

And on Debian-based Linuxes:

<code>$ aptitude install cloc </code>


To use it, simply cd into the root directory and run:

<code>$ cloc .</code>


The default output will show you a breakdown by language. Here’s an example of what it’ll look like:
<a href="#">
    <img src="{{ site.baseurl }}/img/cloc-redacted.png" alt="Lucas Gatsas lucas gatsas" title="lucas gatsas Lucas Gatsas" style="width:100%">
</a>

You can, of course, customize the poop out of it as well.

<code>cloc --help</code> to nerd out.

<br>




Quick and easy way to show the current Git branch on your command prompt


If you work with lots of branches in Git it is nice to be able to see at a glance which branch you are on instead of typing git branch each time. Here are 4 quick lines you can add to your bash prompt that will show the current branch. You will need to edit your user bash config which can be in different locations depending on your operating system.

OS X: <code> ~/.profile </code>

Linux General:  <code> ~/.bash_profile </code>

~ represents the path to your user home directory. For my  <code>user, spaceodyssey, </code> on OS X the path is <code> /Users/home/spaceodyssey. </code>


Add in the file the following lines:
<code>
parse_git_branch() {
       git branch 2> /dev/null | sed -e '/^[^*]/d' -e 's/* \(.*\)/ (\1)/'
}
export PS1="\u@\h \W\[\033[31m\]\$(parse_git_branch)\[\033[00m\] $ "
 
</code>


Restart your terminal and change directories to your repository and you should now see the branch in parenthesis at the end of your prompt.

<br>

And Today i hit the 1000 K of contribrutions on Github! [github.com/spaceg](https://github.com/spaceg) 




<br><br>

<h2 class="section-heading"><strong>Work Streak</strong></h2>

<h2 class="section-heading">21 Club Mate's</h2>

<h2 class="section-heading">247 Coffees</h2>

<h2 class="section-heading">363 Hours</h2>

<h2 class="section-heading">7479 Lines of Code</h2>

<br><br>

<blockquote>
“Make every detail perfect and limit the number of details to perfect.” -Jack Dorsey, Twitter co-founder
</blockquote>