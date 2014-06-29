# notes when playing around with wireless networking

## turn on monitor mode for wireless
$ sudo iw phy phy0 interface add moni0 type monitor

## reminder for monitoring with scapy
$ sudo scapy
>>> pkts = sniff(iface="moni0", count=3, prn=lambda x: x.summary())
