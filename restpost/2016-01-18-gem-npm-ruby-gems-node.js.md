---
layout: post

#event information
title:  "Gem Npm Packages"
cover: "img/1.jpg"
date:   2015-10-18
start_time: "10:00"
end_time: "17:00"

#event organiser details
organiser: "Lucas Gatsas"


---
<h2 class="section-heading"> RubyGems</h2>
<h2 class="section-heading">Make your Own Gem</h2>

<strong> What is Gem? </strong> 
RubyGems is the official packaging system for <a href="https://www.ruby-lang.org/de/">ruby-lang.org</a>  programming language. It provides a packet format, a tool for managing packages, a repository for their distribution. 

Since Ruby 1.9 RubyGems is part of the standard library of Ruby. If you want to use a RubyGem in a Ruby program, you must first load the required library:

<strong> Use </strong>

  RubyGems be accessed via the command line acc.



<stromg> Example :</strong> 

<div style="overflow:auto; height=200; width=100%;">
<pre style="color:black;background:white;"><pre>

require 'json'        # aktuelle Version
gem 'rake', '= 10.1.0' # mit Versionsangabe


</pre></pre></div> 

<strong>Gem Installation : Rake  </strong>

Download and install rake with the following.
<code> gem install rake </code> 



<strong> Example : </strong> 

First, you must write a “Rakefile” file which contains the build rules. Here's a simple example:

<div style="overflow:auto; height=200; width=100%;">
<pre style="color:black;background:white;"><pre>

task default: %w[test]

task :test do
  ruby "test/unittest.rb"
end

</pre></pre></div> 

This Rakefile has two tasks:

A task named “test”, which – upon invocation – will run a unit test file in Ruby.

A task named “default”. This task does nothing by itself, but it has exactly one dependency, namely the “test” task. Invoking the “default” task will cause Rake to invoke the “test” task as well.

Running the “rake” command without any options will cause it to run the “default” task in the Rakefile:

<div style="overflow:auto; height=200; width=100%;">
<pre style="color:black;background:white;"><pre>

% ls
Rakefile     test/
% rake
(in /home/some_user/Projects/rake)
ruby test/unittest.rb
....unit test output here...

</pre></pre></div> 


Type “rake –help” for all available options.
<br><br>

Link: <a href="https://rubygems.org/">rubygems.org</a>  Link:  <a href="https://www.ruby-lang.org/de/"> ruby-lang.org</a>

<blockquote>
“Grind and Polish your Gems!” 
</blockquote>

