---
layout:     post
title:      "X-UA Compatible Part II"
subtitle:   "Cross Browser Check IE Microsoft"
date:       2015-04-09 14:00:44
author:     "Lucas Gatsas"
header-img: "img/Quadrat-Kubus.png"
---


<h2 class="section-heading"><strong> Front-End Development for our Start Up.</strong> </h2>
<h2 class="section-heading">X-UA Compatibility Modus - Cross Browser Check IE Microsoft</h2>


<strong>Browser Check!</strong>



<table class="table">
        <thead>
          <tr>
            <th>Value</th>
            <th id="fadeout-1">Mean</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td> <code> IE=11 </code></td>
            <td id="fadeout-1">My Blog use the Current IE=11. for the Compatibility Modus!</td>
          </tr>
        </tbody>
      </table>


<br>

 


<a href="{{ site.baseurl }}/img/cross-browser-test-1.png">
    <img src="{{ site.baseurl }}/img/cross-browser-test-1.png" alt="Lucas Gatsas lucas gatsas" title="lucas gatsas Lucas Gatsas"  style="width:100%">
</a>

<blockquote> This is just an Example from my Blog! Safari, Google Chrome, Firefox, Opera Browser check! </blockquote>



<h2 class="section-heading"><strong> Javascript</strong> </h2>
<h2 class="section-heading"> Internet Explorer 8 - Microsoft</h2>

For Internet Explorer 8 Microsoft has a new proprietary property of the document object, the document mode introduced. This property returns a numeric value that corresponds to the document compatibility mode of the page.


<div style="overflow:auto; height=200; width=100%;">
<pre style="color:black;background:white;"><pre>

var IE = null;

if (window.navigator.appName == "Microsoft Internet Explorer") {
  
  if (document.documentMode) {

    // Internet Explorer 8

    IE = document.documentMode; // documentMode = 8

    } else {


      // Internet Explorer 5-11

        IE = 5; //setzt the Quirks-Modus

          if (document.compatMode) {
  
      if (document.compatMode == "CSS1Compat")


      IE = 11; // IE11 Modus

      }
    }
  }

</pre></pre></div>



<strong>Warning:</strong> The introduced with Internet Explorer 6 CompatMode property has been deprecated in favor document mode. Scripts that are based on CompatMode will continue to work in Internet Explorer 8, but should be switched to the use of document mode to prevent future problems.



<a href="{{ site.baseurl }}/img/microsoft.-ie-1.jpg">
    <img src="{{ site.baseurl }}/img/microsoft.-ie-1.jpg" alt="Lucas Gatsas lucas gatsas" title="lucas gatsas Lucas Gatsas"  style="width:100%">
</a>

<blockquote> After </blockquote>


See the example result here of my Blog, of course we are Testing Now our 
WebApp for the Microsoft IE Compatibility Modus/ IE Explorer.
<a href="https://www.modern.ie/de-de/screenshots#http%3A%2F%2Fspaceg.github.io">https://www.modern.ie/de-de/
  screenshots#http/
  spaceg.github.io</a>


Top Browsers: 


<a href="https://firefox.com/">www.firefox.com</a>

<a href="http://www.opera.com/de">www.opera.com/de/</a>

<a href="https://www.google.de/chrome/browser/desktop/">www.google.de/chrome/</a>

<a href="https://www.apple.com/chde/safari/">www.apple.com/chde/safari/</a>


<blockquote>
  "For every Developer is the Internet Explorer from Microsoft the badest Explorer of all the Time.! - Word -"
</blockquote>

