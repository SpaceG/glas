---
layout:     post
title:      "An Introduction To Object Oriented CSS (OOCSS)"
subtitle:   "OOCss - Object Orient"
date:       2015-01-13 14:00:44
author:     "Lucas Gatsas"
header-img: "img/lucas-gatsas-10.png"
---
<h2 class="section-heading">Introduction to OOCSS</h2>



Go See: 
[OOCss on GitHub](https://github.com/stubbornella/oocss/wiki/)

Go See: 
[OOCss Docs](http://oocss.org/grids_docs.html)


Go See: 
[SEXIST BY DESIGN?](http://www.stubbornella.org/content/2014/05/09/sexist-by-design/)

<!--

<a href="#">
    <img src="{{ site.baseurl }}/img/static.squarespace.jpg" alt="Post Sample Image">
</a>
-->


<!--
<a href="#">
    <img src="{{ site.baseurl }}/img/gitlist.io.png" alt="Post Sample Image">
</a> -->

<h2 class="section-heading">OOCSS </h2>


<p>Have you ever heard the phrase “Content is King”? Being a Web developer, and therefore having a job that’s often linked to content creation, it’s likely you have. It’s a fairly overused but true statement about what draws visitors to a site.</p>


The Other Question is how do you can Go 
[speed is king](http://www.stevesouders.com/blog/)
 up your site during less code in your app. Best Practices for Speeding Up Your Web Site by Yahoo : 
[speed up](https://developer.yahoo.com/performance/rules.html)




Go See: 
[speed is king](http://www.stevesouders.com/blog/2009/10/06/business-impact-of-high-performance/)

<h2 class="section-heading">The Media Object</h2>

One of the pioneers of the OOCSS movement is[Nicole Sullivan](http://www.stubbornella.org/content/2014/05/09/sexist-by-design/). She’s created a reusable module called the [media object](https://github.com/stubbornella/oocss/wiki/Content)  which, as she explains, can [save hundreds of lines of code.](http://www.stubbornella.org/content/2010/06/25/the-media-object-saves-hundreds-of-lines-of-code/) 

<h2 class="section-heading">Example of a OOcss </h2>


<div style="overflow:auto; height=200; width=100%;">
<pre style="color:#000000;background:#ffffff;"><pre>.header-inside {
	width: <span style="color:#9D9D9D; ">980</span>px;
	height: <span style="color:#9D9D9D; ">260</span>px;
	padding: <span style="color:#9D9D9D; ">20</span>px;
	margin: <span style="color:#9D9D9D; ">0</span> auto;
	position: relative;
	overflow: hidden;
}
</pre></pre></div>



<div style="overflow:auto; height=200; width=100%;">
<pre style="color:#000000;background:#ffffff;"><pre>.globalwidth {
	width: <span style="color:#9D9D9D; ">980</span>px;
	margin: <span style="color:#9D9D9D;  ">0</span> auto;
	position: relative;
	padding-left: <span style="color:#9D9D9D;  ">20</span>px;
	padding-right: <span style="color:#9D9D9D;  ">20</span>px;
	overflow: hidden;
}

.header-inside {
	padding-top: <span style="color:#9D9D9D;  ">20</span>px;
	padding-bottom: <span style="color:#9D9D9D;  ">20</span>px;
	height: <span style="color:#9D9D9D;  ">260</span>px;
}
</pre></pre></div>



<div style="overflow:auto; height=200; width=100%;">
<pre style="color:#000000;background:#ffffff;"><pre><span style="color:#BABABA; ">&lt;</span><span style="color:#BABABA; ">header</span><span style="color:#BABABA; ">&gt;</span>
	<span style="color:#BABABA; ">&lt;</span><span style="color:#BABABA; font-weight:bold; ">div</span><span style="color:#BABABA; "> </span><span style="color:#BABABA; ">class</span><span style="color:#BABABA; ">=</span><span style="color:#BABABA; ">"header-inside globalwidth"</span><span style="color:#BABABA; ">&gt;</span>
	<span style="color:#BABABA; ">&lt;/</span><span style="color:#BABABA; font-weight:bold; ">div</span><span style="color:#BABABA; ">&gt;</span>
<span style="color:#BABABA; ">&lt;/</span><span style="color:#BABABA; ">header</span><span style="color:#BABABA; ">&gt;</span>

<span style="color:#BABABA; ">&lt;</span><span style="color:#BABABA; font-weight:bold; ">div</span><span style="color:#BABABA; "> </span><span style="color:#BABABA; ">class</span><span style="color:#BABABA; ">=</span><span style="color:#BABABA; ">"main globalwidth"</span><span style="color:#BABABA; ">&gt;</span>
<span style="color:#BABABA; ">&lt;/</span><span style="color:#BABABA; font-weight:bold; ">div</span><span style="color:#BABABA; ">&gt;</span>

<span style="color:#BABABA; ">&lt;</span><span style="color:#BABABA; ">footer</span><span style="color:#BABABA; ">&gt;</span>
	<span style="color:#BABABA; ">&lt;</span><span style="color:#BABABA; font-weight:bold; ">div</span><span style="color:#BABABA; "> </span><span style="color:#BABABA; ">class</span><span style="color:#BABABA; ">=</span><span style="color:#BABABA; ">"footer-inside globalwidth"</span><span style="color:#BABABA; ">&gt;</span>
	<span style="color:#BABABA; ">&lt;/</span><span style="color:#BABABA; font-weight:bold; ">div</span><span style="color:#BABABA; ">&gt;</span>
<span style="color:#BABABA; ">&lt;/</span><span style="color:#BABABA; ">footer</span><span style="color:#BABABA; ">&gt;</span>
</pre></pre></div>




<blockquote> "Find a Job you Love and you'll never work a day in your life". - 

</blockquote>



<a href="#">
    <img src="{{ site.baseurl }}/img/the-cascade-grids-headings-and-selectors-from-an-oocss-perspective-ajax-experience-2009-1-728.jpg" alt="Post Sample Image" style="width:100%">
</a> 







