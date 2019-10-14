
# Chapter 4

## Review questions

### SECTIONS 4.1–4.2

#### R1. Let’s review some of the terminology used in this textbook. Recall that the name of a transport-layer packet is segment and that the name of a link-layer packet is frame. What is the name of a network-layer packet? Recall that both routers and link-layer switches are called packet switches. What is the fundamental difference between a router and link-layer switch? Recall that we use the term routers for both datagram networks and VC networks.

#### R2. What are the two most important network-layer functions in a datagram network? What are the three most important network-layer functions in a virtualcircuit network?

#### R3. What is the difference between routing and forwarding?

#### R4. Do the routers in both datagram networks and virtual-circuit networks use forwarding tables? If so, describe the forwarding tables for both classes of networks.

#### R5. Describe some hypothetical services that the network layer can provide to a single packet. Do the same for a flow of packets. Are any of your hypothetical services provided by the Internet’s network layer? Are any provided by ATM’s CBR service model? Are any provided by ATM’s ABR service model?

#### R6. List some applications that would benefit from ATM’s CBR service model.

### SECTION 4.3
#### R7. Discuss why each input port in a high-speed router stores a shadow copy of the forwarding table.

#### R8. Three types of switching fabrics are discussed in Section 4.3. List and briefly describe each type. Which, if any, can send multiple packets across the fabric in parallel?

#### R9. Describe how packet loss can occur at input ports. Describe how packet loss at input ports can be eliminated (without using infinite buffers).

#### R10. Describe how packet loss can occur at output ports. Can this loss be prevented by increasing the switch fabric speed?

#### R11. What is HOL blocking? Does it occur in input ports or output ports?

### SECTION 4.4
#### R12. Do routers have IP addresses? If so, how many?
#### R13. What is the 32-bit binary equivalent of the IP address 223.1.3.27?
#### R14. Visit a host that uses DHCP to obtain its IP address, network mask, default router, and IP address of its local DNS server. List these values.

#### R15. Suppose there are three routers between a source host and a destination host. Ignoring fragmentation, an IP datagram sent from the source host to the destination host will travel over how many interfaces? How many forwarding tables will be indexed to move the datagram from the source to the destination?

#### R16. Suppose an application generates chunks of 40 bytes of data every 20 msec, and each chunk gets encapsulated in a TCP segment and then an IP datagram. What percentage of each datagram will be overhead, and what percentage will be application data?

#### R17. Suppose Host A sends Host B a TCP segment encapsulated in an IP datagram. When Host B receives the datagram, how does the network layer in Host B know it should pass the segment (that is, the payload of the datagram) to TCP rather than to UDP or to something else?

#### R18. Suppose you purchase a wireless router and connect it to your cable modem. Also suppose that your ISP dynamically assigns your connected device (that is, your wireless router) one IP address. Also suppose that you have five PCs at home that use 802.11 to wirelessly connect to your wireless router. How are IP addresses assigned to the five PCs? Does the wireless router use NAT? Why or why not?

#### R19. Compare and contrast the IPv4 and the IPv6 header fields. Do they have any fields in common?

#### R20. It has been said that when IPv6 tunnels through IPv4 routers, IPv6 treats the IPv4 tunnels as link-layer protocols. Do you agree with this statement? Why or why not?

### SECTION 4.5
#### R21. Compare and contrast link-state and distance-vector routing algorithms.

#### R22. Discuss how a hierarchical organization of the Internet has made it possible to scale to millions of users.

#### R23. Is it necessary that every autonomous system use the same intra-AS routing algorithm? Why or why not?

### SECTION 4.6

#### R24. Consider Figure 4.37. Starting with the original table in _D_, suppose that _D_ receives from _A_ the following advertisement: 

| Destination Subnet | Next Router | Number of Hops to Destinantion |
|        :---:       |    :---:    |              :---:             |
|          z         |      C      |                4               |
|          w         |      -      |                1               |
|          x         |      -      |                1               |
|        ....        |     ....    |              ....              |
> Figure 4.37 pg 386 6th edition

Will the table in _D_ change? If so how?

#### R25. Compare and contrast the advertisements used by RIP and OSPF.

#### R26. Fill in the blank: RIP advertisements typically announce the number of hops to various destinations. BGP updates, on the other hand, announce the __________ to the various destinations.

####  R27. Why are different inter-AS and intra-AS protocols used in the Internet?

#### R28. Why are policy considerations as important for intra-AS protocols, such as
OSPF and RIP, as they are for an inter-AS routing protocol like BGP?

#### R29. Define and contrast the following terms: subnet, prefix, and BGP route.

#### R30. How does BGP use the NEXT-HOP attribute? How does it use the AS-PATH attribute?

#### R31. Describe how a network administrator of an upper-tier ISP can implement policy when configuring BGP.

### SECTION 4.7

#### R32. What is an important difference between implementing the broadcast abstraction via multiple unicasts, and a single network- (router-) supported broadcast?

#### R33. For each of the three general approaches we studied for broadcast communication (uncontrolled flooding, controlled flooding, and spanning-tree broadcast), are the following statements true or false? You may assume that no packets are lost due to buffer overflow and all packets are delivered on a link in the order in which they were sent.

##### a. A node may receive multiple copies of the same packet.

##### b. A node may forward multiple copies of a packet over the same outgoing link.

#### R34. When a host joins a multicast group, must it change its IP address to that of the multicast group it is joining?

#### R35. What are the roles played by the IGMP protocol and a wide-area multicast routing protocol?

#### R36. What is the difference between a group-shared tree and a source-based tree in the context of multicast routing?
