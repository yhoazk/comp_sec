# Digital forensics

## DShell
- stream reassemble
- custom output handlees 
- chained decoders

https://github.com/USArmyResearchLab/Dshell

Prerequisites:
- pygeoip
- pycrypto
- dpkt
- IPy
- pycap
- elasticsearch-py

With python virtual enviromnent, the pkgs installed remain in the environment not in the site-packages main directory.
```
virtual env <dir>
pip install <pkg>
source <dir>/bin/activate
deactivate
```

### DShell commands
- liost availabe decoders
`# decode -l`



- enable decoder
`# decode -d <decoder> <path/to/pcap>`


#### double pulsar vulnerability

## Working with scapy:

Read pcap file:
`pcap = rdcap("<pcap>")

Get conversations in the pcap file
`pcap.conversations()`
This generates a graph woth all the conversations in the pcap file


Get sessions
`pcap.sessions()`

Get a list of packages:
`pcap.display()`

Print signle package hex representation:
`hexdump(pkg)`

Pretty print of a package:
`pkt.show()`

Get properties according to the layer:
`pkt[<layer>].<property>` Where layer can be Ethernet, IP, TCP


### Impacket https://github.com/SecureAuthCorp/impacket

`pip install impacket pcapy`

Impacket provides low-level programatic access to packets and some protocols
- Ethernet
- IP


Windows registry:

- Database to strore windows settings
- key:value pairs
- e.g. Malaware locations
+ Microsoft\windows\currentversion\run
+ WOW6432node\microsoft\windows\currentversion\run
+ microsift\windows NT\currentversion\winlogon\system


#### Access windows registry in python

Allows to read/write and query keys and values
```py
import winreg
```