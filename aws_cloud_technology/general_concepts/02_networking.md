# Networking - Introduction

**An IP address is a 32-bit number that uniquely identifies a host (computer or other device, such as a printer or router) on a TCP/IP network.**

IP addresses are normally expressed in dotted-decimal format, with four numbers separated by periods, such as *192.168.123.132*.<br />
For example, the dotted-decimal IP address *192.168.123.132* is (in binary notation) the 32 bit number *110000000101000111101110000100*. This number may be hard to make sense of, so divide it into four parts of eight binary digits.

These eight bit sections are known as octets. The example IP address, then, becomes *11000000.10101000.01111011.10000100*. This number only makes a little more sense, so for most uses, convert the binary address into dotted-decimal format *(192.168.123.132)*. The decimal numbers separated by periods are the octets converted from binary to decimal notation.

An IP address has two parts. The first part of an IP address is used as a network address, the last part as a host address. If you take the example 192.168.123.132 and divide it into these two parts we get the following:
 
   *192.168.123. Network .132 Host*
 
-or-
   *192.168.123.0 - network address. 0.0.0.132 - host address*.

The second item, which is required for TCP/IP to work, is the subnet mask. The subnet mask is used by the TCP/IP protocol to determine whether a host is on the local subnet or on a remote network.

In TCP/IP, the parts of the IP address that are used as the network and host addresses are not fixed, so the network and host addresses above cannot be determined unless you have more information. This information is supplied in another 32-bit number called a subnet mask. In this example, the subnet mask is 255.255.255.0. It is not obvious what this number means unless you know that 255 in binary notation equals 11111111; so, the subnet mask is:
 
   *11111111.11111111.11111111.0000000*
 
Lining up the IP address and the subnet mask together, the network and host portions of the address can be separated:
 
   *11000000.10101000.01111011.10000100* -- IP address (*192.168.123.132*)
   *11111111.11111111.11111111.00000000* -- Subnet mask (*255.255.255.0*)
 
The first 24 bits (the number of ones in the subnet mask) are identified as the network address, with the last 8 bits (the number of remaining zeros in the subnet mask) identified as the host address. This gives you the following:
 
   *11000000.10101000.01111011.00000000* -- Network address (*192.168.123.0*)
   *00000000.00000000.00000000.10000100* -- Host address (*000.000.000.132*)
 
So now you know, for this example using a 255.255.255.0 subnet mask, that the network ID is 192.168.123.0, and the host address is 0.0.0.132. When a packet arrives on the 192.168.123.0 subnet (from the local subnet or a remote network), and it has a destination address of 192.168.123.132, your computer will receive it from the network and process it.

Almost all decimal subnet masks convert to binary numbers that are all ones on the left and all zeros on the right. Some other common subnet masks are:
 
   Decimal                 Binary
   *255.255.255.192*         *1111111.11111111.1111111.11000000*
   *255.255.255.224*         *1111111.11111111.1111111.11100000*


 A subnet mask is used to divide an IP address into two parts. One part identifies the host (computer), the other part identifies the network to which it belongs. To better understand how IP addresses and subnet masks work, look at an IP (Internet Protocol) address and see how it is organized.

#### Below is a table providing typical subnets for IPv4.

**Prefix size**| **Network mask**|**Usable hosts per subnet**
------------|-------------|--------------------
/1          |128.0.0.0    |2,147,483,646
/2          |192.0.0.0    |1,073,741,822
/3          |224.0.0.0    |536,870,910
/4          |240.0.0.0    |268,435,454
/5          |248.0.0.0    |134,217,726
/6          |252.0.0.0    |67,108,862
/7          |254.0.0.0    |33,554,430
|         |**Class A**     |
/8  |255.0.0.0   |16,777,214
/9  |255.128.0.0  |8,388,606
/10  |255.192.0.0  |4,194,302
/11  |255.224.0.0  |2,097,150
/12  |255.240.0.0  |1,048,574
/13  |255.248.0.0  |524,286
/14  |255.252.0.0  |262,142
/15  |255.254.0.0  |131,070
|     | **Class B** |
/16  |255.255.0.0  |65,534
/17  |255.255.128.0  |32,766
/18  |255.255.192.0  |16,382
/19  |255.255.224.0  |8,190
/20  |255.255.240.0  |4,094
/21  |255.255.248.0  |2,046
/22  |255.255.252.0  |1,022
/23  |255.255.254.0  |510
|	|**Class C**|
/24  |255.255.255.0  |254
/25  |255.255.255.128  |126
/26  |255.255.255.192  |62
/27  |255.255.255.224  |30
/28  |255.255.255.240  |14
/29  |255.255.255.248  |6
/30  |255.255.255.252  |2
/31  |255.255.255.254  |0
/32  |255.255.255.255  |0
