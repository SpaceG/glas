---
layout:     post
title:      "Ready For MacPorts"
subtitle:   "MacPorts to Run some Applications on your Machine"
date:       2015-03-23 14:00:44
author:     "Lucas Gatsas"
header-img: "img/lucas-gatsas-doberman-white.png"
---
<h2 class="section-heading"><strong>MacPorts</strong> </h2>

<h2 class="section-heading">2.2.1. OS X Package Install</h2>




The OS X package installer automatically installs MacPorts, [sets the shell environment](https://guide.macports.org/chunked/installing.shell.html), and runs a
[selfupdate](https://guide.macports.org/chunked/using.html#using.port.selfupdate)  operation to update the ports tree and MacPorts base with the latest release.



(1.) Download the latest <strong>MacPorts-2.3.1-....pkg</strong> installer from the <strong> [MacPorts download directory](https://distfiles.macports.org/MacPorts/) </strong> . Here are direct links for the latest versions of OS X:


OS X 10.9 Mavericks:
[MacPorts-2.3.1-10.9-Mavericks.pkg](https://distfiles.macports.org/MacPorts/MacPorts-2.3.1-10.9-Mavericks.pkg)


OS X 10.8 Mountain Lion:
[MacPorts-2.3.1-10.8-MountainLion.pkg](https://distfiles.macports.org/MacPorts/MacPorts-2.3.1-10.8-MountainLion.pkg)


OS X 10.7 Lion:
[MacPorts-2.3.1-10.7-Lion.pkg](https://distfiles.macports.org/MacPorts/MacPorts-2.3.1-10.7-Lion.pkg)


(2.) Double-click the downloaded package installer to perform the default “easy” install.

(3.) After this step you are done already, MacPorts is now installed and your shell environment was set up automatically by the installer. To confirm the installation is working as expected, now try using the port command in a new terminal window.


<code>$ port version</code>

<strong>Version: 2.3.1</strong>

In case of problems such as “command not found”, make sure that you opened a new terminal window or consult Section 2.5, [ “MacPorts and the Shell”](https://guide.macports.org/chunked/installing.shell.html) . Otherwise, please skip the remainder of this chapter and continue with [Chapter 3, Using MacPorts](https://guide.macports.org/chunked/using.html) in this guide.




<h2 class="section-heading"><strong>2.2.2. Source Install</strong> </h2>


<h2 class="section-heading">Install Macports via Terminal</h2>

If you installed MacPorts using the package installer, skip this section. To install MacPorts from the source code, follow the steps below.


(1.) Download and extract the [MacPorts 2.3.1 tarball](https://distfiles.macports.org/MacPorts/MacPorts-2.3.1.tar.bz2). Either do so using your browser and the Finder, or use the given commands in a terminal window.


<code>$ curl -O https://distfiles.macports.org/
	MacPorts/MacPorts-2.3.1.tar.bz2</code> 

<code>$ tar xf MacPorts-2.3.1.tar.bz2</code> 



(2.) Afterwards, perform the commands shown in the terminal window. If you wish to use a path other than <code>/opt/local</code>, follow the instructions for installing multiple copies of MacPorts instead.



<code>$ cd MacPorts-2.3.1/</code> 

<code>$ ./configure</code> 

<code>$ make</code> 

<code>$ sudo make install</code> 


<strong>[GO SEE MacPorts-2.3.3 INSTALL VIDEO](https://plus.google.com/u/0/101826267816845608605/posts/Lit9AU1msaY)</strong> 



<iframe width="100%" height="515" src="https://www.youtube.com/embed/RBriCmHGrXk?autoplay=1&loop=1" frameborder="0" allowfullscreen></iframe>


(3.) Please continue with  [Section 2.5, “MacPorts and the Shell”](https://guide.macports.org/chunked/installing.macports.html#installing.macports.source.multiple)  to set up your shell environment.




install macports 




<code>port version</code> 

<code>port list</code>  

<code>port search git</code>  

<code>port info git-core</code> 

<code>port installed</code> 

<code>sudo install git-core</code>  

<code>git —version</code> 

<code>port installed</code> 

<code>port outdated</code> 

<code>sudo port upgrade</code> 

<code>sudo port upgrade git-core</code> 

<code>sudo port upgrade outdated</code> 

<code>sudo port selfupdate</code> 

<code>sudo port uninstall git-core</code> 

<code>sudo port install git-core</code> 









[MacPorts Website](https://www.macports.org/install.php)



<blockquote>
	"Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency."
</blockquote>