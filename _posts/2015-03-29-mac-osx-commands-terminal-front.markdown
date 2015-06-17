---
layout:     post
title:      "Mac Os X - CommandLines"
subtitle:   "Terminal CommandLines Mac Os X System Control"
date:       2015-03-29 14:00:44
author:     "Lucas Gatsas"
header-img: "img/yR1gv2aRQDHN36RE.jpeg"
---

<h2 class="section-heading"><strong> Mac Os X - CommandLines</strong> </h2>

<table class="table">
        <thead>
          <tr>
            <th>Kommando#</th>
            <th id="fadeout-1">Aktion</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td><code>$ chflags nohidden ~/Library</code></td>
            <td id="fadeout-1">Library-Ordner unter Mac OS Lion anzeigen</td>
          </tr>
          <tr>
            <td><code>$ ping 127.0.0.1</code></td>
            <td id="fadeout-1">pingt ein Netzwerkgerät
um unter Mac OS Ping zu stoppen CTRL+C drücken</td>
          </tr>
          <tr>
            <td><code>$ top</code></td>
            <td id="fadeout-1">Zeigt eine Liste von laufenden Prozessen an, ähnlich der Aktivitätsanzeige.</td>
          </tr>
          <tr>
            <td><code>$ defaults write com.apple.
            	Finder AppleShowAllFiles

            	 TRUE; 
            	 killAll Finder</code></td>
            <td id="fadeout-1">Zeigt versteckte Dateien im Finder an.</td>
          </tr>
          <tr>
            <td><code>$ defaults write com.apple.
            	Finder AppleShowAllFiles 

            	TRUE; 
            	killAll Finder</code></td>
<td id="fadeout-1">Zeigt <strong>versteckte Dateien</strong> im <a href="https://spaceg.github.io/" title="Mac Explorer - Finder">Finder</a> an. <span title="eingeführt in OS X Lion" class="label label-info">Mavericks</span></td>          </tr>
    	<tr>
            <td><code>$ defaults write  com.apple.
            	ScreenCapture type JPG; 
            	killAll SystemUIServer</code> </td>
            <td id="fadeout-1">Stellt das Format für Screenshots auf JPG, weitere mögliche Formate sind: PNG, PDF, TIFF, JPEG, BMP, GIF, PSD.</td>
          </tr>
           <td><code>$ defaults write 
           	com.apple.Screencapture location 
           	/Users/benutzername; 
           	killAll SystemUIServer</code>
           </td>
            <td id="fadeout-1">Ändert den Speicherordner für Screenshots auf Euren Benutzerordner.</td>
          </tr>
           <tr>
            <td><code>$ dscacheutil -flushcache</code></td>
            <td id="fadeout-1">Startet Quick Look neu & läd ggf. neue Plugins.</td>
          </tr>
               <tr>
            <td><code>$ ipconfig getifaddr en0</code></td>
            <td id="fadeout-1">Get Your Network IP Address</td>
          </tr>
           <tr>
            <td><code>$ curl ipecho.net/plain;
             echo</code></td>
            <td id="fadeout-1">Get Your External IP Address</td>
          </tr>
          <tr>
            <td><code>$ ping -c 10 www.example-
            	site.com</code></td>
            <td id="fadeout-1">Test Network Connectivity</td>
          </tr>
           <tr>
            <td><code>$ system_profiler</code></td>
            <td id="fadeout-1">A Closer Look at System Information</td>
          </tr>
            <tr>
            <td><code>$ pwd</code></td>
            <td id="fadeout-1">The current directory</td>
          </tr>
              <tr>
            <td><code>$  ps -ax</code></td>
            <td id="fadeout-1">Job control While Activity Monitor is useful, it's not quite as useful as working with the shell.
To get a list of every running process on your computer, type this:</td>
          </tr>
              <tr>
            <td><code>$  hostname</code></td>
            <td id="fadeout-1">To get your current location, use the "hostname" command.</td>
          </tr>
        </tbody>
      </table>
      
<blockquote>
	"Learn & Understand how Machine Works!"
</blockquote>