---
layout:     post
title:      "Add X-UA Compatibility Mode"
subtitle:   "Cross Browser Check IE Microsoft"
date:       2015-04-04 14:00:44
author:     "Lucas Gatsas"
header-img: "img/Quadrat-Kubus.png"
---


<h2 class="section-heading"><strong> Front-End Development</strong> </h2>
<h2 class="section-heading">Add X-UA Compatibility Mode</h2>


<strong>META tags for Document Compatibility</strong>

For individual websites a corresponding meta element can be recorded in the head section of the page. Note: this element must be in the header above all other elements. The only exception is the title element and other meta-elements

      

<code> < meta http-equiv="X-UA-Compatible" content="IE=8" /> </code>

The Internet Explorer 8 accepts the special value for the http-equiv attribute: X-UA-Compatible (uppercase and lowercase does not matter).
The content attribute can be one or more of the following values:


<table class="table">
        <thead>
          <tr>
            <th>Value</th>
            <th id="fadeout-1">Mean</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td> <code> IE=5 </code></td>
            <td id="fadeout-1">The code of the page as indicated by the quirks mode in Internet Explorer 7 </td>
          </tr>
          <tr>
            <td><code>IE=7</code></td>
            <td id="fadeout-1">The code of the page as indicated by the standards mode in Internet Explorer 7, excluding the / a DOCTYPE statement</td>
          </tr>
          <tr>
            <td><code>IE=EmulateIE7</code></td>
            <td id="fadeout-1">The code of the page is displayed as Internet Explorer 7, but considering the / a DOCTYPE statement (standards compliant mode as indicated by IE7 and quirks-mode, as the IE 5)</td>
          </tr>
               <tr>
            <td><code>IE=EmulateIE8</code></td>
            <td id="fadeout-1">The website contains a standards-compliant DOCTYPE statement, it is in the "IE8" mode, on the other hand, in quirks mode (IE5 mode) shown</td>
          </tr>
                        <tr>
            <td><code>IE=8</code></td>
            <td id="fadeout-1">The IE8- or IE8 standards mode. Note: This is the default setting for Internet Explorer 8!</td>
          </tr>
                       <tr>
            <td><code>IE=edge</code></td>
            <td id="fadeout-1">With this mode, the Internet Explorer (8) is instructed to use the maximum available mode. This mode is only recommended for testing.</td>
          </tr>
        </tbody>
      </table>


<br>

<strong>The following diagram shows how Internet Explorer determines the appropriate document mode based on the meta element or HTTP header.</strong>
 

<a href="{{ site.baseurl }}/img/IC777593.jpg">
    <img src="{{ site.baseurl }}/img/IC777593.jpg" alt="Lucas Gatsas"  style="width:100%">
</a>


<table class="table">
        <thead>
          <tr>
            <th>Value</th>
            <th id="fadeout-1">Mean</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td> <code> X-UA-Compatible value </code></td>
            <td id="fadeout-1">Document modes </td>
          </tr>
          <tr>
            <td><code>IE=5</code></td>
            <td id="fadeout-1">Quirks mode</td>
          </tr>
          <tr>
            <td><code>IE=7</code></td>
            <td id="fadeout-1">IE7 mode</td>
          </tr>
               <tr>
            <td><code>IE=8</code></td>
            <td id="fadeout-1">IE8 mode</td>
          </tr>
                        <tr>
            <td><code>IE=9</code></td>
            <td id="fadeout-1">IE9 mode</td>
          </tr>
                       <tr>
            <td><code>IE=10</code></td>
            <td id="fadeout-1">IE10 mode</td>
          </tr>
                                <tr>
            <td><code>IE=11</code></td>
            <td id="fadeout-1">IE11 mode</td>
          </tr>
                                 <tr>
            <td><code>IE=edge</code></td>
            <td id="fadeout-1">The highest supported document mode of the browser</td>
          </tr>
                                     <tr>
            <td><code>IE=EmulateIE7</code></td>
            <td id="fadeout-1">IE7 mode (if a valid <!DOCTYPE> declaration is present)
Quirks mode (otherwise)</td>
          </tr>
                                      <tr>
            <td><code>IE=EmulateIE8</code></td>
            <td id="fadeout-1">IE8 mode (if a valid <!DOCTYPE> declaration is present)
Quirks mode (otherwise)</td>
          </tr>
                                    <tr>
            <td><code>IE=EmulateIE9</code></td>
            <td id="fadeout-1">IE9 mode (if a valid <!DOCTYPE> declaration is present)
Quirks mode (otherwise)</td>
          </tr>
                                     <tr>
            <td><code>IE=EmulateIE10</code></td>
            <td id="fadeout-1">IE10 mode (if a valid <!DOCTYPE> declaration is present)
Quirks mode (otherwise)</td>
          </tr>
                                      <tr>
            <td><code>IE=EmulateIE11</code></td>
            <td id="fadeout-1">IE11 mode (if a valid <!DOCTYPE> declaration is present)
Quirks mode (otherwise)</td>
          </tr>
        </tbody>
      </table>


<strong> Programmatic Configuration </strong>


Of course, it may also be necessary for programmers and application / server operators to specify these settings for their site / application.

Here, too, there are two options (in order of priority):


<strong> “Per Page” </strong>


The "Per Page" setting has the highest priority. The meta tag entry must come first within the header tags.

The following options are available:

(1). <code> < meta http-equiv="X-UA-Compatible" content="IE=5"/> </code> 

This is the only way to IE8 all pages in sog "Quirks Mode" to be represented. The information about the <meta ...> tag has the highest priority. Even if a !DOCTYPE is specified, it is ignored.

(2). <code> < meta http-equiv="X-UA-Compatible" content="IE=EmulateIE7"/>  </code>

If a valid DOCTYPE exists. the page is in "IE7 standards mode" shown.

(3). <code> < meta http-equiv="X-UA-Compatible" content="IE=7"/> </code>

The page is always displayed in "IE7 Standards mode", even if no "DOCTYPE" is present

(4). <code> < meta http-equiv="X-UA-Compatible" content="IE=EmulateIE8"/> </code>

If a valid DOCTYPE exists. the page is in "IE8 standards mode" shown.

(5). <code> < meta http-equiv="X-UA-Compatible" content="IE=8"/> </code>

The page is always displayed in "IE8 Standards mode", even if no "DOCTYPE" is present

(6). <code> < meta http-equiv="X-UA-Compatible" content="IE=EmulateIE9"/>  </code>

If a valid DOCTYPE exists. the page is in "IE9 standards mode" shown.

(7). <code> < meta http-equiv="X-UA-Compatible" content="IE=9"/>  </code>

The page is always displayed in "IE9 Standards mode", even if no "DOCTYPE" is present

(8). <code> < meta http-equiv="X-UA-Compatible" content="IE=EmulateIE10"/>  </code>

If a valid DOCTYPE exists. the page is in "IE10 standards mode" shown.

(9). <code> < meta http-equiv="X-UA-Compatible" content="IE=10"/> </code>

 The page is always displayed in "IE10 Standards mode", even if no "DOCTYPE" is present

(10). <code> < meta http-equiv="X-UA-Compatible" content="IE=EmulateIE11"/> </code>

If a valid DOCTYPE exists. the page is in "IE11 standards mode" shown.

(11). <code> < meta http-equiv="X-UA-Compatible" content="IE=11"/> </code>

 The page is always displayed in "IE11 Standards mode", even if no "DOCTYPE" is present

(12). <code> < meta http-equiv="X-UA-Compatible" content="IE=edge"/> </code>

With this setting, the latest version of the rendering engine is used. It is irrelevant whether a "DOCTYPE" was specified or not. The operation can be compared to "IE = 7" and "IE = 8". 



<strong> “Per Site”  </strong> 


The "Per Site" setting has higher priority than a "DOCTYPE" indication.
However, subject to the "Per Page" setting.


In principle, the Web server must also send a header "X-UA-Compatible".
The value corresponds to the data as in "Per Page", also “5”

”EmulateIE7”,”7”,

”EmulateIE8”,”8”, 

“EmulateIE9”, “9” , 

“EmulateIE10”, “10” , 

“EmulateIE11", “11” 

and “edge”. 


If using IIS using web.config <a href="https://msdn.microsoft.com/en-us/library/cc817572.aspx">http://msdn.microsoft.com/ </a>

When using an Apache: <a href="https://msdn.microsoft.com/en-us/library/cc817573.aspx">https://msdn.microsoft.com/</a>

VGL: <a href="http://msdn.microsoft.com/library/cc817574.aspx">http://msdn.microsoft.com/</a> 


<strong>HTTP-Header</strong>

With the help of an HTTP header you can specify the document compatibility mode for Internet Explorer 8 for the entire site.
For the Apache Web server, the custom header should look like this:

<code>X-UA-Compatible: IE=EmulateIE7 </code>

This header 8 would cause Internet Explorer to the website to make the way the Internet Explorer 7 it would be.
For Apache 2.2, you can also use the headers_module. This one should make sure that the headers_module is loaded:

<code>LoadModule headers_module modules/mod_headers.so</code>

Then you can see the line:

<code>Header set X-UA-Compatible "IE=EmulateIE7"</code>

paste the <code>httpd.conf </code> file behind the LoadModule lines. This directive can be also in the various configuration sections

<code> (< Location>, < Directory>,< Files> und < VirtualHost>) </code>


Insert the server in order to more precisely control which pages should be displayed in the mode.

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



<blockquote>
  "For every Developer is the Internet Explorer from Microsoft the badest Explorer of all the Time.! - Word -"
</blockquote>