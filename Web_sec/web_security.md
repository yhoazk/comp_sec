# Web Security: Vulnerabilities and access control

Basics of Web Security:
* HTML, HTML5, HTTP, HTTPS, JS, Apache, PHP
* Session ID, Cookies, DOM Objects
* Same Origin Polic

### Vulnerabilities and Attacks
* Cross-site scripting ([XSS](./WHXSSThreats.pdf))
* [Worm Floods MySpace](https://it.slashdot.org/story/05/10/14/126233/cross-site-scripting-worm-floods-myspace)



### Cross sire request forgery

### SQL Injection Attacks

### ClickJacking Attacks
  * [UI Redressing](./uiRedressing.pdf)
### Web tracking and privacy
  *
### Access Control in the Web
* Vulnerabilities in web applications
* Escudo: A fine grained protection model for web browsers
* Scuta: A server side access control system for web applications
### Running Native code inside browsers
* [Native client](NativeClient.pdf)



### SYN Flood attack

The SYN flood or _half open attack_ is a type of DoS attack which aims to make
a server unavailable to legitimate traffic by consuming all available sever
resources. By repeteadly sending initial connection request `SYN` packets, the
attacker is able to overwhelm all available ports on a server, causing the
target to respond legitimate traffic sluggishly or not at all.

There are 3 variants of this attack:
1. Direct attack:
  - A SYN flood where the IP address is not spoofed
  - The attacker does not mask their IP
2. Spoofed Attack:
  - The IP address on each SYN packet they send is spoofed in order to inhibit
  mitigation efforts and make their identity difficult to discover, while the IP
  is spoofed the packets can be traced back to the source.
3. Distributed attack:
  - If an attack is created using a botnet the likehood of tracing the attack back
  to its source is low. For an added level of obfuscation an attacker may have
  each distributed device also spoof the IP address from which sends pkgs.

#### Mitigation of SYN flood

* Increase backlog queue
* Recycling the oldest half-open TCP connection
- SYN Cookies

### ICMP Echo attack

Also called ping flood, is a denial-of-service attack in which the attacker
attempts to overwhelm the target with ICMP echo-request pkgs.

The network diagnostic tools traceroute and ping both operate using ICMP. Commonly
ICMP echo-request and echo-reply messages are used to ping a network device for
the purpose of diagnostic the connectivity of the device and the connection.

Every ICMP request requires some server resources to process and to respond.
This request also requires bandwidth on both the incoming and outgoing message.
The ping flood aims to overwhelm the targeted device's ability to respond to
the high number of requests or overloaded network.

#### Mitigation

Disabling a ping flood is most easy accomplished by disabling the ICMP
functionality on the router, computer or other device. This makes the device
unresponsive to ping requests, traceroute requests, and other network activities



### ICMP Redirection attack

### LAND attack

### Smurf attack

### WinNuke attack

### Ping Sweep Attack
