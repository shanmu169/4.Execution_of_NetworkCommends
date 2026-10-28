# 4.Execution_of_NetworkCommands
## AIM :Use of Network commands in Real Time environment
## Software : Command Prompt And Network Protocol Analyzer
## Procedure: To do this EXPERIMENT- follows these steps:
<BR>
In this EXPERIMENT- students have to understand basic networking commands e.g cpdump, netstat, ifconfig, nslookup ,traceroute and also Capture ping and traceroute PDUs using a network protocol analyzer 
<BR>
All commands related to Network configuration which includes how to switch to privilege mode
<BR>
and normal mode and how to configure router interface and how to save this configuration to
<BR>
flash memory or permanent memory.
<BR>
This commands includes
<BR>
• Configuring the Router commands
<BR>
• General Commands to configure network
<BR>
• Privileged Mode commands of a router 
<BR>
• Router Processes & Statistics
<BR>
• IP Commands
<BR>
• Other IP Commands e.g. show ip route etc.
<BR>

## Output
```
Microsoft Windows [Version 10.0.26200.9711]
(c) Microsoft Corporation. All rights reserved.
ipconfig:
C:\Users\acer>ipconfig

Windows IP Configuration


Ethernet adapter Ethernet:

   Media State . . . . . . . . . . . : Media disconnected
   Connection-specific DNS Suffix  . :

Ethernet adapter Ethernet 2:

   Connection-specific DNS Suffix  . :
   Link-local IPv6 Address . . . . . : fe80::d07d:aed9:2e79:8b65%7
   IPv4 Address. . . . . . . . . . . : 192.168.56.1
   Subnet Mask . . . . . . . . . . . : 255.255.255.0
   Default Gateway . . . . . . . . . :

Wireless LAN adapter Local Area Connection* 1:

   Media State . . . . . . . . . . . : Media disconnected
   Connection-specific DNS Suffix  . :

Wireless LAN adapter Local Area Connection* 2:

   Media State . . . . . . . . . . . : Media disconnected
   Connection-specific DNS Suffix  . :

Wireless LAN adapter Wi-Fi:

   Connection-specific DNS Suffix  . :
   IPv6 Address. . . . . . . . . . . : 2405:201:e00a:6143:d3bf:ffad:21eb:2831
   Temporary IPv6 Address. . . . . . : 2405:201:e00a:6143:45cc:c696:e5f9:a8ca
   Link-local IPv6 Address . . . . . : fe80::f555:b7fb:2ebf:eb7e%3
   IPv4 Address. . . . . . . . . . . : 192.168.29.171
   Subnet Mask . . . . . . . . . . . : 255.255.255.0
   Default Gateway . . . . . . . . . : fe80::5a95:d8ff:fe22:11c3%3
                                       192.168.29.1
2. ping:
C:\Users\acer>ping google.com

Pinging google.com [2404:6800:4007:82e::200e] with 32 bytes of data:
Reply from 2404:6800:4007:82e::200e: time=9ms
Reply from 2404:6800:4007:82e::200e: time=21ms
Reply from 2404:6800:4007:82e::200e: time=15ms
Reply from 2404:6800:4007:82e::200e: time=14ms

Ping statistics for 2404:6800:4007:82e::200e:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 9ms, Maximum = 21ms, Average = 14ms
3. tracert:
C:\Users\acer>tracert google.com

Tracing route to google.com [2404:6800:4007:82e::200e]
over a maximum of 30 hops:

  1     4 ms     1 ms     1 ms  2405:201:e00a:6143:5a95:d8ff:fe22:11c3
  2     *        *        *     Request timed out.
  3    10 ms     *        *     2405:203:400:100:172:31:0:209
  4     *        *        *     Request timed out.
  5    10 ms     4 ms     4 ms  2405:200:80c:3168:61::6
  6     *        *        *     Request timed out.
  7    11 ms     6 ms     6 ms  2405:200:801:900::1292
  8     *        *        *     Request timed out.
  9    13 ms     8 ms     8 ms  2001:4860:1:1::170
 10    13 ms     7 ms     7 ms  2001:4860:1:1::170
 11     8 ms     6 ms     6 ms  pnmaaa-bd-in-x0e.1e100.net [2404:6800:4007:82e::200e]

Trace complete.
4. nslookup
C:\Users\acer>  nslookup wikipedia.org
Server:  reliance.reliance
Address:  2405:201:e00a:6143::c0a8:1d01

Non-authoritative answer:
Name:    wikipedia.org
Addresses:  2001:df2:e500:ed1a::1
          103.102.166.224

5. netstat:
C:\Users\acer>netstat -ano

Active Connections

  Proto  Local Address          Foreign Address        State           PID
  TCP    0.0.0.0:80             0.0.0.0:0              LISTENING       4
  TCP    0.0.0.0:135            0.0.0.0:0              LISTENING       2000
  TCP    0.0.0.0:445            0.0.0.0:0              LISTENING       4
  TCP    0.0.0.0:1309           0.0.0.0:0              LISTENING       4932
  TCP    0.0.0.0:5040           0.0.0.0:0              LISTENING       8548
  TCP    0.0.0.0:49664          0.0.0.0:0              LISTENING       1696
  TCP    0.0.0.0:49665          0.0.0.0:0              LISTENING       1536
  TCP    0.0.0.0:49666          0.0.0.0:0              LISTENING       2428
  TCP    0.0.0.0:49667          0.0.0.0:0              LISTENING       3400
  TCP    0.0.0.0:49668          0.0.0.0:0              LISTENING       4280
  TCP    0.0.0.0:49673          0.0.0.0:0              LISTENING       1640
  TCP    0.0.0.0:58995          0.0.0.0:0              LISTENING       4660
  TCP    127.0.0.1:4343         0.0.0.0:0              LISTENING       4520
  TCP    127.0.0.1:4449         0.0.0.0:0              LISTENING       4588
  TCP    127.0.0.1:5141         0.0.0.0:0              LISTENING       4572
  TCP    127.0.0.1:5141         127.0.0.1:63772        ESTABLISHED     4572
  TCP    127.0.0.1:9993         0.0.0.0:0              LISTENING       5800
  TCP    127.0.0.1:15152        0.0.0.0:0              LISTENING       6976
  TCP    127.0.0.1:19443        0.0.0.0:0              LISTENING       4528
  TCP    127.0.0.1:46753        0.0.0.0:0              LISTENING       11068
  TCP    127.0.0.1:46760        0.0.0.0:0              LISTENING       11068
  TCP    127.0.0.1:46934        0.0.0.0:0              LISTENING       9052
  TCP    127.0.0.1:46935        0.0.0.0:0              LISTENING       9052
  TCP    127.0.0.1:46935        127.0.0.1:63827        ESTABLISHED     9052
  TCP    127.0.0.1:46936        0.0.0.0:0              LISTENING       11860
  TCP    127.0.0.1:46936        127.0.0.1:49683        ESTABLISHED     11860
  TCP    127.0.0.1:46937        0.0.0.0:0              LISTENING       11860
  TCP    127.0.0.1:46937        127.0.0.1:49684        ESTABLISHED     11860
  TCP    127.0.0.1:49669        127.0.0.1:49670        ESTABLISHED     4604
  TCP    127.0.0.1:49670        127.0.0.1:49669        ESTABLISHED     4604
  TCP    127.0.0.1:49675        127.0.0.1:49676        ESTABLISHED     11860
  TCP    127.0.0.1:49676        127.0.0.1:49675        ESTABLISHED     11860
  TCP    127.0.0.1:49677        127.0.0.1:49678        ESTABLISHED     11860
  TCP    127.0.0.1:49678        127.0.0.1:49677        ESTABLISHED     11860
  TCP    127.0.0.1:49679        127.0.0.1:49680        ESTABLISHED     11788
  TCP    127.0.0.1:49680        127.0.0.1:49679        ESTABLISHED     11788
  TCP    127.0.0.1:49681        127.0.0.1:49682        ESTABLISHED     11788
  TCP    127.0.0.1:49682        127.0.0.1:49681        ESTABLISHED     11788
  TCP    127.0.0.1:49683        127.0.0.1:46936        ESTABLISHED     11788
  TCP    127.0.0.1:49684        127.0.0.1:46937        ESTABLISHED     11788
  TCP    127.0.0.1:49685        127.0.0.1:49686        ESTABLISHED     11068
  TCP    127.0.0.1:49686        127.0.0.1:49685        ESTABLISHED     11068
  TCP    127.0.0.1:51779        0.0.0.0:0              LISTENING       4604
  TCP    127.0.0.1:51780        0.0.0.0:0              LISTENING       4604
  TCP    127.0.0.1:51781        0.0.0.0:0              LISTENING       4604
  TCP    127.0.0.1:51782        0.0.0.0:0              LISTENING       4604
  TCP    127.0.0.1:58995        127.0.0.1:63769        ESTABLISHED     4660
  TCP    127.0.0.1:58995        127.0.0.1:63784        ESTABLISHED     4660
  TCP    127.0.0.1:58995        127.0.0.1:63800        ESTABLISHED     4660
  TCP    127.0.0.1:63769        127.0.0.1:58995        ESTABLISHED     14824
  TCP    127.0.0.1:63772        127.0.0.1:5141         ESTABLISHED     14464
  TCP    127.0.0.1:63784        127.0.0.1:58995        ESTABLISHED     5800
  TCP    127.0.0.1:63800        127.0.0.1:58995        ESTABLISHED     5036
  TCP    127.0.0.1:63821        127.0.0.1:63822        ESTABLISHED     9052
  TCP    127.0.0.1:63822        127.0.0.1:63821        ESTABLISHED     9052
  TCP    127.0.0.1:63823        127.0.0.1:63824        ESTABLISHED     9052
  TCP    127.0.0.1:63824        127.0.0.1:63823        ESTABLISHED     9052
  TCP    127.0.0.1:63825        127.0.0.1:63826        ESTABLISHED     17400
  TCP    127.0.0.1:63826        127.0.0.1:63825        ESTABLISHED     17400
  TCP    127.0.0.1:63827        127.0.0.1:46935        ESTABLISHED     17400
  TCP    192.168.29.171:139     0.0.0.0:0              LISTENING       4
  TCP    192.168.29.171:52905   172.188.155.25:443     ESTABLISHED     1720
  TCP    192.168.29.171:53526   192.168.29.14:8009     ESTABLISHED     15080
  TCP    192.168.29.171:54779   23.9.30.24:443         ESTABLISHED     6244
  TCP    192.168.29.171:57791   31.7.60.154:85         ESTABLISHED     14688
  TCP    192.168.29.171:60884   172.188.155.25:443     ESTABLISHED     17304
  TCP    192.168.29.171:62302   13.69.239.69:443       TIME_WAIT       0
  TCP    192.168.56.1:139       0.0.0.0:0              LISTENING       4
  TCP    [::]:80                [::]:0                 LISTENING       4
  TCP    [::]:135               [::]:0                 LISTENING       2000
  TCP    [::]:445               [::]:0                 LISTENING       4
  TCP    [::]:49664             [::]:0                 LISTENING       1696
  TCP    [::]:49665             [::]:0                 LISTENING       1536
  TCP    [::]:49666             [::]:0                 LISTENING       2428
  TCP    [::]:49667             [::]:0                 LISTENING       3400
  TCP    [::]:49668             [::]:0                 LISTENING       4280
  TCP    [::]:49673             [::]:0                 LISTENING       1640
  TCP    [::]:58995             [::]:0                 LISTENING       4660
  TCP    [::1]:15161            [::]:0                 LISTENING       5800
  TCP    [::1]:15161            [::1]:63787            ESTABLISHED     5800
  TCP    [::1]:15161            [::1]:63788            ESTABLISHED     5800
  TCP    [::1]:15161            [::1]:63796            TIME_WAIT       0
  TCP    [::1]:42050            [::]:0                 LISTENING       15864
  TCP    [::1]:63787            [::1]:15161            ESTABLISHED     5800
  TCP    [::1]:63788            [::1]:15161            ESTABLISHED     16428
  TCP    [2405:201:e00a:6143:45cc:c696:e5f9:a8ca]:49408  [2603:1040:a06:6::1]:443  ESTABLISHED     5396
  TCP    [2405:201:e00a:6143:45cc:c696:e5f9:a8ca]:49409  [2603:1040:a06:6::1]:443  ESTABLISHED     5396
  TCP    [2405:201:e00a:6143:45cc:c696:e5f9:a8ca]:52976  [2603:1040:a06:6::1]:443  ESTABLISHED     18392
  TCP    [2405:201:e00a:6143:45cc:c696:e5f9:a8ca]:54778  [2001:4860:4844:400::]:443  ESTABLISHED     15080
  TCP    [2405:201:e00a:6143:45cc:c696:e5f9:a8ca]:55198  [2603:1063:2001:190c::365:ff1]:443  ESTABLISHED     9212
  TCP    [2405:201:e00a:6143:45cc:c696:e5f9:a8ca]:55199  [2603:1063:2001:190c::365:ff1]:443  ESTABLISHED     9212
  TCP    [2405:201:e00a:6143:45cc:c696:e5f9:a8ca]:55200  [2603:1063:2001:1946::365:ff1]:443  ESTABLISHED     9212
  TCP    [2405:201:e00a:6143:45cc:c696:e5f9:a8ca]:58448  [2404:6800:4013:813::bc]:5228  ESTABLISHED     15080
  TCP    [2405:201:e00a:6143:45cc:c696:e5f9:a8ca]:63361  [2404:6800:4013:807::5e]:443  ESTABLISHED     15080
  UDP    0.0.0.0:5050           *:*                                    8548
  UDP    0.0.0.0:5353           *:*                                    14840
  UDP    0.0.0.0:5353           *:*                                    2420
  UDP    0.0.0.0:5353           *:*                                    14840
  UDP    0.0.0.0:5353           *:*                                    14840
  UDP    0.0.0.0:5353           *:*                                    14840
  UDP    0.0.0.0:5355           *:*                                    2420
  UDP    0.0.0.0:49383          *:*                                    5036
  UDP    127.0.0.1:1900         *:*                                    14344
  UDP    127.0.0.1:49382        *:*                                    5036
  UDP    127.0.0.1:59952        127.0.0.1:59952                        4892
  UDP    127.0.0.1:60975        *:*                                    14344
  UDP    192.168.29.171:137     *:*                                    4
  UDP    192.168.29.171:138     *:*                                    4
  UDP    192.168.29.171:1900    *:*                                    14344
  UDP    192.168.29.171:60974   *:*                                    14344
  UDP    192.168.56.1:137       *:*                                    4
  UDP    192.168.56.1:138       *:*                                    4
  UDP    192.168.56.1:1900      *:*                                    14344
  UDP    192.168.56.1:60973     *:*                                    14344
  UDP    [::]:5353              *:*                                    14840
  UDP    [::]:5353              *:*                                    2420
  UDP    [::]:5353              *:*                                    14840
  UDP    [::]:5355              *:*                                    2420
  UDP    [::1]:1900             *:*                                    14344
  UDP    [::1]:60972            *:*                                    14344
  UDP    [fe80::d07d:aed9:2e79:8b65%7]:1900  *:*                                    14344
  UDP    [fe80::d07d:aed9:2e79:8b65%7]:60970  *:*                                    14344
  UDP    [fe80::f555:b7fb:2ebf:eb7e%3]:1900  *:*                                    14344
  UDP    [fe80::f555:b7fb:2ebf:eb7e%3]:60971  *:*                                    14344
6. arp:
C:\Users\acer>arp -a

Interface: 192.168.29.171 --- 0x3
  Internet Address      Physical Address      Type
  192.168.29.1          58-95-d8-22-11-c3     dynamic
  192.168.29.14         38-06-e6-8d-21-02     dynamic
  192.168.29.255        ff-ff-ff-ff-ff-ff     static
  224.0.0.22            01-00-5e-00-00-16     static
  224.0.0.251           01-00-5e-00-00-fb     static
  224.0.0.252           01-00-5e-00-00-fc     static
  239.255.255.250       01-00-5e-7f-ff-fa     static
  255.255.255.255       ff-ff-ff-ff-ff-ff     static

Interface: 192.168.56.1 --- 0x7
  Internet Address      Physical Address      Type
  192.168.56.255        ff-ff-ff-ff-ff-ff     static
  224.0.0.22            01-00-5e-00-00-16     static
  224.0.0.251           01-00-5e-00-00-fb     static
  224.0.0.252           01-00-5e-00-00-fc     static
  239.255.255.250       01-00-5e-7f-ff-fa     static
7. route:
C:\Users\acer>route print
===========================================================================
Interface List
 18...74 d4 dd d0 c8 b9 ......Realtek PCIe GbE Family Controller
  7...0a 00 27 00 00 07 ......VirtualBox Host-Only Ethernet Adapter
 17...fc 6d 77 8c a8 ee ......Microsoft Wi-Fi Direct Virtual Adapter
 12...fe 6d 77 8c a8 ed ......Microsoft Wi-Fi Direct Virtual Adapter #2
  3...fc 6d 77 8c a8 ed ......Intel(R) Wi-Fi 6E AX211 160MHz
  1...........................Software Loopback Interface 1
===========================================================================

IPv4 Route Table
===========================================================================
Active Routes:
Network Destination        Netmask          Gateway       Interface  Metric
          0.0.0.0          0.0.0.0     192.168.29.1   192.168.29.171     40
        127.0.0.0        255.0.0.0         On-link         127.0.0.1    331
        127.0.0.1  255.255.255.255         On-link         127.0.0.1    331
  127.255.255.255  255.255.255.255         On-link         127.0.0.1    331
     192.168.29.0    255.255.255.0         On-link    192.168.29.171    296
   192.168.29.171  255.255.255.255         On-link    192.168.29.171    296
   192.168.29.255  255.255.255.255         On-link    192.168.29.171    296
     192.168.56.0    255.255.255.0         On-link      192.168.56.1    281
     192.168.56.1  255.255.255.255         On-link      192.168.56.1    281
   192.168.56.255  255.255.255.255         On-link      192.168.56.1    281
        224.0.0.0        240.0.0.0         On-link         127.0.0.1    331
        224.0.0.0        240.0.0.0         On-link      192.168.56.1    281
        224.0.0.0        240.0.0.0         On-link    192.168.29.171    296
  255.255.255.255  255.255.255.255         On-link         127.0.0.1    331
  255.255.255.255  255.255.255.255         On-link      192.168.56.1    281
  255.255.255.255  255.255.255.255         On-link    192.168.29.171    296
===========================================================================
Persistent Routes:
  None

IPv6 Route Table
===========================================================================
Active Routes:
 If Metric Network Destination      Gateway
  3     56 ::/0                     fe80::5a95:d8ff:fe22:11c3
  1    331 ::1/128                  On-link
  3     56 2405:201:e00a:6143::/64  On-link
  3    296 2405:201:e00a:6143:45cc:c696:e5f9:a8ca/128
                                    On-link
  3    296 2405:201:e00a:6143:d3bf:ffad:21eb:2831/128
                                    On-link
  7    281 fe80::/64                On-link
  3    296 fe80::/64                On-link
  7    281 fe80::d07d:aed9:2e79:8b65/128
                                    On-link
  3    296 fe80::f555:b7fb:2ebf:eb7e/128
                                    On-link
  1    331 ff00::/8                 On-link
  7    281 ff00::/8                 On-link
  3    296 ff00::/8                 On-link
===========================================================================
Persistent Routes:
  None
8. hostname:
C:\Users\acer>hostname
shanmuu
9. getmac:
C:\Users\acer>getmac

Physical Address    Transport Name
=================== ==========================================================
FC-6D-77-8C-A8-ED   \Device\Tcpip_{05DFA269-CEFB-4295-ADCE-7123750CCF35}
74-D4-DD-D0-C8-B9   Media disconnected
0A-00-27-00-00-07   \Device\Tcpip_{262029EF-76E6-49A7-B8E5-370ABE242E8D}
C:\Users\acer>netsh interface show interface

Admin State    State          Type             Interface Name
-------------------------------------------------------------------------
Enabled        Disconnected   Dedicated        Ethernet
Enabled        Connected      Dedicated        Ethernet 2
Enabled        Connected    
```
## Result
Thus Execution of Network commands Performed 
