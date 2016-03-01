---
layout: post

#event information
title:  "NMAP MAC OSX"
cover: "img/hiking-2.jpg"
date:   2016-01-13
start_time: "10:00"
end_time: "17:00"

#event organiser details
organiser: "Lucas Gatsas"


---

<h2 class="section-heading">Nmap for Mac Os X - Linux</h2>
<h2 class="section-heading">Nmap Security Scanner for Linux-MAC-UNIX </h2>



<strong> Was ist Nmap ? </strong> 


       Nmap ("Network Mapper") ist ein Open-Source-Werkzeug fA1/4r die
       Netzwerkanalyse und SicherheitsA1/4berprA1/4fung. Es wurde entworfen, um
       groAe Netzwerke schnell zu scannen, auch wenn es bei einzelnen Hosts auch
       gut funktioniert. Nmap benutzt rohe IP-Pakete auf neuartige Weise, um
       festzustellen, welche Hosts im Netzwerk verfA1/4gbar sind, welche Dienste
       (Anwendungsname und -version) diese Hosts bieten, welche Betriebssysteme
       (und Versionen davon) darauf laufen, welche Art von
       Paketfiltern/-Firewalls benutzt werden sowie Dutzende anderer
       Eigenschaften. Auch wenn Nmap A1/4blicherweise fA1/4r
       SicherheitsA1/4berprA1/4fungen verwendet wird, wird es von vielen Systemen
       und Netzwerkadministratoren fA1/4r Routineaufgaben benutzt, z.B.
       Netzwerkinventarisierung, Verwaltung von AblaufplAxnen fA1/4r
       Dienstaktualisierungen und die Aberwachung von Betriebszeiten von Hosts
       oder Diensten.



<strong> Install and Set Up </strong> 



Download it here <a href="https://nmap.org/download.html#macosx">nmap-6.47.dmg</a> or Run it with Terminal: First installl <a href="http://www.bzip.org/">bzip.org</a>! Promt
in your Temrinal follow the Commanlines: 

To install using <a href="https://www.macports.org/">MacPorts</a>, run <code> sudo port install nmap </code>. Nmap will be installed as <code> /opt/local/bin/nmap </code>. To uninstall, run sudo port uninstall nmap.

<strong> Example Ports Show Up after entire NetWork Scanning! </strong>

<div style="overflow:auto; height=200; width=100%;">
<pre style="color:black;background:white;"><pre>

PORT STATE SERVICE

22/tcp open ssh

80/tcp open http

445/tcp open microsoft-ds

548/tcp open afp

6817/tcp open unknown

</pre></pre></div> 

<code> nmap hostname </code> 



1.What computers did you find running on the local network?

2.What IP addresses did you find running on the local network?

3.What is the operating system of your target machine?

4.Find out what ports are open on the machine that you just scanned?

5.Find out if the system is infected with malware or virus.

6.Search for unauthorized servers or network service on your network.

7.Find and remove computers which don't meet the organization's minimum level of security.


<strong> Scan & List a Range of Local Network IP’s </strong> 

You will find some Information about other Machines on your Localhost Network. Your Lan has an IP range of example  <code> 192.169.0.1</code> to <code> 192.169.0.25 </code> change numbers as appropritae: 


<code>nmap -sP 192.168.0.1-25</code>


If you don’t know the range, you can also use wildcards:



<code>nmap 192.168.0.*</code>


<strong>Scan & Detect Operating System</strong>


<code>
nmap -O 192.168.0.1-5</code>



<code>
nmap --osscan-guess 192.168.0.2 </code>


Exmaple Diagram: 



                              +---------+
        +---------+           | Network |         +--------+
        | server1 |-----------+ swtich  +---------|server2 |
        +---------+           | (sw0)   |         +--------+
                              +----+----+
                                   |
                                   |
                         +---------+----------+
                         | wks01 Linux/OSX    |
                         +--------------------+



<blockquote id="strict-alert-red">
Port scanning may be illegal in some jurisdictions and Countrys. So be Aware! Scan Only <strong>your Network </strong> and <strong> Computers, Websites </strong> etc.  as follows:
</blockquote>


At last i have to lol. because i found this crazy thing here : 
<a href="http://nmap.org/movies/#elysium">Nmap in Movies!</a> 

Link: 
<a href="http://nmap.org/download.html#macosx">nmap.org</a> 







<blockquote>
This is a SwissWatch! :)
</blockquote>
