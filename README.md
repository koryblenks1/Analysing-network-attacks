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


## Conclusion
<strong>Here are some questions I considered when determining what type of attack occurred:</strong>

<strong>1. What do I currently understand about network attacks?</strong>

Network attacks are malicious activities that disrupt networks, steal information, or gain unauthorized access to systems.

<strong>2. Which type of attack would likely result in the symptoms described in the scenario?</strong> 

A TCP SYN flood attack, a type of Denial-of-Service (DoS) attack.

<strong>3. Why is the website taking a long time to load and reporting a connection timeout error?</strong>

The server is overwhelmed by excessive TCP SYN requests, exhausting its resources and preventing legitimate users from connecting.


<strong>When writing the report, discuss the network devices and activities that are involved in the interruption. Include the following information in your explanation:</strong>

1. Describe the attack. What are the main symptoms or characteristics of this specific type of attack? 

2. Explain how it affected the organization’s network. How does this specific network attack affect the website and how it functions?

3. Describe the potential consequences of this attack and how it negatively affects the organization. 

4. Suggest potential ways to secure the network so this attack can be prevented in the future.


