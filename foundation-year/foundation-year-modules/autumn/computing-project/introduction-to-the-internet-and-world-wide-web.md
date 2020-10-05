# The Internet and World Wide Web

### The Internet

Pre Reading

*  The **Internet** is the global system of interconnected computer networks that uses the Internet protocol suite \(TCP/IP\) to communicate between networks and devices. Essentially, a _network of_ private, public, academic, business, and government _networks_ to a global \(WAN\) or local \(LAN\) scale.
* The **infastructure** of the internet consits of different **data networks,** like layers, the most exposed data networks we know today are the WAN, and the LAN :
  * [Nanoscale](https://en.wikipedia.org/wiki/Nanonetwork): A nanonetwork or nanoscale network is a set of interconnected nanomachines \(devices a few hundred nanometers or a few micrometers at most in size\), which are able to perform only very simple tasks such as computing, data storing, sensing and actuation
  * [Near-field \(NFC\)](https://en.wikipedia.org/wiki/Near-field_communication)
  * [Body \(BAN\)](https://en.wikipedia.org/wiki/Body_area_network)
  * [Personal \(PAN\)](https://en.wikipedia.org/wiki/Personal_area_network):  A personal area network \(PAN\) is a computer network for interconnecting electronic devices centered on an individual person's workspace. PAN provides data transmission among devices such as computers, smartphones, tablets and personal digital assistant
    * Wireless Personal Access Network \(WPAN\): a PAN carried over a low-powered, short-distance wireless network technology such as IrDA, Wireless USB, Bluetooth or ZigBee. The reach of a WPAN varies from a few centimeters to a few meters.
  * [Near-me \(NAN\)](https://en.wikipedia.org/wiki/Near-me_area_network)
  * [Local \(LAN\)](https://en.wikipedia.org/wiki/Local_area_network):  **Local Area Network \(LAN\)** is a computer network that interconnects computers within a limited area such as a house, school, laboratory, university campus or office building
    * [Home \(HAN\)](https://en.wikipedia.org/wiki/Home_network):  **home area network** \(**HAN**\) is a type of computer network that facilitates communication among devices within the close vicinity of a home. Devices capable of participating in this network, for example, smart devices such as network printers and handheld mobile computers, often gain enhanced new capabilities through their ability to interact
    * [Storage \(SAN\)](https://en.wikipedia.org/wiki/Storage_area_network): **storage area network** \(**SAN**\) is a [computer network](https://en.wikipedia.org/wiki/Computer_network) which provides access to consolidated, [block-level data storage](https://en.wikipedia.org/wiki/Block_device). SANs are primarily used to access storage devices, such as [disk arrays](https://en.wikipedia.org/wiki/Disk_array) and [tape libraries](https://en.wikipedia.org/wiki/Tape_library) from [servers](https://en.wikipedia.org/wiki/Server_%28computing%29) so that the devices appear to the [operating system](https://en.wikipedia.org/wiki/Operating_system) as [direct-attached storage](https://en.wikipedia.org/wiki/Direct-attached_storage). A SAN typically is a dedicated network of storage devices not accessible through the [local area network](https://en.wikipedia.org/wiki/Local_area_network) \(LAN\).
    * [Wireless \(WLAN\)](https://en.wikipedia.org/wiki/Wireless_LAN):  **Wireless Local Area Network \(WLAN\)** is a wireless computer network that links two or more devices using wireless communication to form a LAN within a limited area such as a home, school, computer laboratory, campus, or office building. This gives users the ability to move around within the area and remain connected to the network. Through a gateway, a WLAN can provide a connection to the wider Internet
  * [Campus \(CAN\)](https://en.wikipedia.org/wiki/Campus_network):  Corporate area network or CAN is a computer network made up of an interconnection of LANs within a limited geographical area
  * [Backbone](https://en.wikipedia.org/wiki/Backbone_network): A backbone or core network is a part of a network which interconnects pieces of various networks, providing a path for the exchange of information between different LANs or subnetworks
  * [Metropolitan \(MAN\)](https://en.wikipedia.org/wiki/Metropolitan_area_network)
    * [Municipal wireless \(MWN\)](https://en.wikipedia.org/wiki/Municipal_wireless_network)
  * [Wide \(WAN\)](https://en.wikipedia.org/wiki/Wide-area_network):  Wide Area Network \(WAN\) is a telecommunications network that extends over a large geographic area for the primary purpose of computer networking.
  * [Cloud \(IAN\)](https://en.wikipedia.org/wiki/Internet_area_network)

{% hint style="info" %}
_Nobody owns the internet, it is an entity_
{% endhint %}

* The largest users of the internet, in order:
  * Asia
  * North America
  * Europe
  * Africa
  * Oceania
* In the UK, as of February 2020, 96% of households have internet access

### World Wide Web

Who invented the World Wide Web \(WWW\)? 

* English scientist **Tim Berners-Lee** invented the World Wide Web in 1989. 
* He wrote the first web browser in 1990 while employed at CERN near Geneva, Switzerland.
* The browser was released outside CERN to other research institutions starting in January 1991
* Then to the general public in August 1991

#### Transmission Control Protocol \(TCP\)

* The **Transmission Control Protocol** \(**TCP**\) is one of the main protocols of the Internet protocol suite. It originated in the initial network implementation in which it complemented the Internet Protocol \(IP\). Therefore, the entire suite is commonly referred to as TCP/IP. TCP provides reliable, ordered, and error-checked delivery of a stream of octets \(bytes\) between applications running on hosts communicating via an IP network. Major internet applications such as the World Wide Web, email, remote administration, and file transfer rely on TCP, which is part of the Transport Layer of the TCP/IP suite. SSL/TLS often runs on top of TCP.
  * TCP is connection-oriented, and a connection between client and server is established before data can be sent. The server must be listening \(passive open\) for connection requests from clients before a connection is established. Three-way handshake \(active open\), retransmission, and error-detection adds to reliability but lengthens latency. Applications that do not require reliable data stream service may use the User Datagram Protocol \(UDP\), which provides a connectionless datagram service that prioritizes time over reliability. TCP employs network congestion avoidance. However, there are vulnerabilities to TCP including denial of service, connection hijacking, TCP veto, and reset attack. For network security, monitoring, and debugging, TCP traffic can be intercepted and logged with a packet sniffer.
  * Though TCP is a complex protocol, its basic operation has not changed significantly since its first specification. TCP is still dominantly used for the web, i.e. for the HTTP protocol, and later HTTP/2, while not used by latest standard HTTP/3.
* Verifies the correct delivery of data from its source to destination It can also: 
  * Detect errors 
  * Detect duplicate messages and discard them
  * Detect lost data
  * Request retransmission of data until it is correct and complete
  * Use flow control to slow down the data transfer if the receiver cannot keep up

#### IPv4 vs IPv6

The Internet Protocol \(IP\) is the principal communications protocol in the Internet protocol suite for relaying datagrams across network boundaries. Its routing function enables internetworking, and essentially establishes the Internet.

IP has the task of delivering packets from the source host to the destination host solely based on the IP addresses in the packet headers. For this purpose, IP defines packet structures that encapsulate the data to be delivered. It also defines addressing methods that are used to label the datagram with source and destination information.

* IPv4 
  * Denary notation
  * 32-bit number 
  * 2^32
  * 8.8.8.8 \(Google's IPv4 address\)
* IPv6 
  * Hexadecimal notation
  * 128-bit number
  * 2^128
  * 2001:4860:4860::8888 \(Google's IPv6 address\)

As we can see, IPv6 has more addresses avaliable, due to the higher nymber of bits

DNS \(Domain Name Server\)

#### Architecture and Components

* hardware
* Software
* Networking
* Protocols

#### Static vs Dynamic Page requests

### Sources

* [https://en.wikipedia.org/wiki/Computer\_network](https://en.wikipedia.org/wiki/Computer_network)

