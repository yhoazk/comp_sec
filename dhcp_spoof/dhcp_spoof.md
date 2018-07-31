# DHCP Spoofing

An address `169.254.0.0/16` is allocated for communication between hosts on a
single link. Hosts obtain these addresses by autoconfiguration, shuch as when
a DHCP server cannot be found. The device assings itself a APIPA address so it
can communicate on the network. A windows based computer that is configured to
use DHCP can automatically assign itself an IP address if a DHCP server is not
available. For example, this could occur on a network w/o DHCP server.

APIPA address start at `169.254.0.1` up to `169.254.255.254`

APIPA: Automatic Private IP Address.
