# Analysing-network-attacks
Analysis of a TCP SYN flood attack on a web server, covering attack identification, service disruption, impact on users, and mitigation strategies using firewall rules and network security controls.
## Scenario
You work as a security analyst for a travel agency that advertises sales and promotions on the company’s website. The employees of the company regularly access the company’s sales webpage to search for vacation packages their customers might like. 

One afternoon, you receive an automated alert from your monitoring system indicating a problem with the web server. You attempt to visit the company’s website, but you receive a connection timeout error message in your browser.

You use a packet sniffer to capture data packets in transit to and from the web server. You notice a large number of TCP SYN requests coming from an unfamiliar IP address. The web server appears to be overwhelmed by the volume of incoming traffic and is losing its ability to respond to the abnormally large number of SYN requests. You suspect the server is under attack by a malicious actor. 

You take the server offline temporarily so that the machine can recover and return to a normal operating status. You also configure the company’s firewall to block the IP address that was sending the abnormal number of SYN requests. You know that your IP blocking solution won’t last long, as an attacker can spoof other IP addresses to get around this block. You need to alert your manager about this problem quickly and discuss the next steps to stop this attacker and prevent this problem from happening again. You will need to be prepared to tell your boss about the type of attack you discovered and how it was affecting the web server and employees.

## Screenshot Images of Wireshark TCP/HTTP log
<a href="https://myimgs.org/"><img src="https://myimgs.org/storage/images/70698/Screenshot2026-10-29173535.png" alt="myimgs.org image hosting" /><p><strong>Wireshark TCP/HTTP log 1</strong></p></a>

<a href="https://myimgs.org/"><img src="https://myimgs.org/storage/images/70689/Screenshot2026-10-29173515.png" alt="Upload gif - myimgs.org" /><p><strong>Wireshark TCP/HTTP log 2</strong></p></a>

<a href="https://myimgs.org/"><img src="https://myimgs.org/storage/images/70701/Screenshot2026-10-29173611.png" alt="Image host - myimgs.org" /><p><strong>Wireshark TCP/HTTP log 3</strong></p></a>

<a href="https://myimgs.org/"><img src="https://myimgs.org/storage/images/70707/Screenshot2026-10-29173635.png" alt="image.png" /><p><strong>Wireshark TCP/HTTP log 4</strong></p></a>

<a href="https://myimgs.org/"><img src="https://myimgs.org/storage/images/70713/Screenshot2026-10-29173651.png" alt="image" /><p><strong>Wireshark TCP/HTTP log 5</strong></p></a>

<a href="https://myimgs.org/"><img src="https://myimgs.org/storage/images/70718/Screenshot2026-10-29173707.png" alt="Post image - myimgs.org" /><p><strong>Wireshark TCP/HTTP log 6</strong></p></a>

<a href="https://myimgs.org/"><img src="https://myimgs.org/storage/images/70722/Screenshot2026-10-29173802.png" alt="https://myimgs.org" /><p><strong>Wireshark TCP/HTTP log 7</strong></p></a>

## Short Analysis of the network attacks
<a href="https://myimgs.org/"><img src="https://myimgs.org/storage/images/70745/Screenshot2026-10-29184111.png" alt="postimage - myimgs.org" /></a>
