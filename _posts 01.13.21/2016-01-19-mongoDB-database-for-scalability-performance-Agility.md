---
layout: post

#event information
title:  "Mongo DB"
cover: "img/lg.jpg"
date:   2015-07-07
start_time: "10:00"
end_time: "17:00"

#event organiser details
organiser: "Lucas Gatsas"


---
<h2 class="section-heading">Mongo DB</h2>
<h2 class="section-heading">"Agility, Scalability, Performance Database"</h2>


<strong>
PLATFORM SUPPORT
Starting in version 3.0, MongoDB only supports OS X versions 10.7 (Lion) on Intel x86-64 and later.<strong>


<strong>Install MongoDB</strong>

You can install MongoDB with <strong>Homebrew</strong> or manually. This section describes both.


1.<strong> Update Homebrew’s package database.</strong> 
In a system shell, issue the following command: 

<code>brew update </code>


2.<strong>Install MongoDB.</strong> 
You can install MongoDB via brew with several different options. Use one of the following operations:

<strong>Install the MongoDB Binaries</strong> 
To install the MongoDB binaries, issue the following command in a system shell:

<code>brew install mongodb</code>


<code>brew install mongodb --with-openssl</code> 



<strong> Build MongoDB from Source with TLS/SSL Support<strong> 
To build MongoDB from the source files and include TLS/SSL support, issue the following from a system shell:




<strong> Install the Latest Development Release of MongoDB</strong> 
To install the latest development release for use in testing and development, issue the following command in a system shell:



<code> brew install mongodb --devel</code> 


<strong> Install MongoDB Manually </strong> 
Only install MongoDB using this procedure if you cannot use homebrew.






  
1.<strong> Download the binary files for the desired release of MongoDB.</strong> 
Download the binaries from <code> https://www.mongodb.org/
downloads. </code> 

For example, to download the latest release through the shell, issue the following:



<strong> curl -O https://fastdl.mongodb.org/
  osx/mongodb-osx-x86_64-3.0.4.tgz</strong> 


2.<strong>Extract the files from the downloaded archive.</strong> 
For example, from a system shell, you can extract through the tar command:

<code>tar -zxvf mongodb-osx-x86_64-3.0.4.tgz</code>


3.<strong>Copy the extracted archive to the target directory.</strong>
Copy the extracted folder to the location from which MongoDB will run.

<code>mkdir -p mongodb</code>
<code>cp -R -n mongodb-osx-x86_
  64-3.0.4/ mongodb</code>



  
4.<strong>Ensure the location of the binaries is in the PATH variable.</strong>
The MongoDB binaries are in the bin/ directory of the archive. To ensure that the binaries are in your PATH, you can modify your PATH.

For example, you can add the following line to your shell’s rc file <code>(e.g. ~/.bashrc):</code> 

export PATH=<mongodb-install-directory> <code>/bin:$PATH</code>
Replace <mongodb-install-directory> with the path to the extracted MongoDB archive.





Link: <a href="https://www.mongodb.org">Mongo DB</a>



<blockquote>
“Built by developers like you at MongoDB. <strong>Highly Scalable</strong>
Scale up or scale out horizontally, from a single server to thousands of nodes. Deploy in the cloud and across multiple data centers.

 <strong>Flexible Data Model </strong>
MongoDB’s document data model makes it easy for you to store data of any structure and dynamically modify the schema.


 <strong>Fastest-Growing Community </strong>
Join the world’s fastest-growing database community. MongoDB stands behind its software to ensure your success, providing software and services to make life easier.” 
</blockquote>

