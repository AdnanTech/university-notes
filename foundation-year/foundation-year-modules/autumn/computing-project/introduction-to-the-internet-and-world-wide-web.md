# The Internet and World Wide Web

### The Internet

*  The **Internet** is the global system of interconnected computer networks that uses the Internet protocol suite \(TCP/IP\) to communicate between networks and devices. Essentially, a _network of_ private, public, academic, business, and government _networks_ to a global \(WAN\) or local \(LAN\) scale.
* The **infrastructure** of the internet consits of different **data networks,** like layers, the most exposed data networks we know today are the WAN, and the LAN :
  * [Nanoscale](https://en.wikipedia.org/wiki/Nanonetwork): A nanonetwork or nanoscale network is a set of interconnected nanomachines \(devices a few hundred nanometers or a few micrometers at most in size\), which are able to perform only very simple tasks such as computing, data storing, sensing and actuation
  * [Near-field \(NFC\)](https://en.wikipedia.org/wiki/Near-field_communication)
  * [Body \(BAN\)](https://en.wikipedia.org/wiki/Body_area_network)
  * [Personal \(PAN\)](https://en.wikipedia.org/wiki/Personal_area_network):  A personal area network \(PAN\) is a computer network for interconnecting electronic devices centered on an individual person's workspace. PAN provides data transmission among devices such as computers, smartphones, tablets and personal digital assistant
    * Wireless Personal Access Network \(WPAN\): a PAN carried over a low-powered, short-distance wireless network technology such as IrDA, Wireless USB, Bluetooth or ZigBee. The reach of a WPAN varies from a few centimeters to a few meters.
  * [Near-me \(NAN\)](https://en.wikipedia.org/wiki/Near-me_area_network)
  * [Local \(LAN\)](https://en.wikipedia.org/wiki/Local_area_network):  **Local Area Network \(LAN\)** is a computer network that interconnects computers within a limited area such as a house, school, laboratory, university campus or office building
    * [Home \(HAN\)](https://en.wikipedia.org/wiki/Home_network):  **home area network** \(**HAN**\) is a type of computer network that facilitates communication among devices within the close vicinity of a home. Devices capable of participating in this network, for example, smart devices such as network printers and handheld mobile computers, often gain enhanced new capabilities through their ability to interact
    * [Storage \(SAN\)](https://en.wikipedia.org/wiki/Storage_area_network): **storage area network** \(**SAN**\) is a computer network which provides access to consolidated, block-level data storage. SANs are primarily used to access storage devices, such as disk arrays and tape libraries from servers so that the devices appear to the operating system as direct-attached storage. A SAN typically is a dedicated network of storage devices not accessible through the local area network \(LAN\).
    * [Wireless \(WLAN\)](https://en.wikipedia.org/wiki/Wireless_LAN):  **Wireless Local Area Network \(WLAN\)** is a wireless computer network that links two or more devices using wireless communication to form a LAN within a limited area such as a home, school, computer laboratory, campus, or office building. This gives users the ability to move around within the area and remain connected to the network. Through a gateway, a WLAN can provide a connection to the wider Internet
  * [Campus \(CAN\)](https://en.wikipedia.org/wiki/Campus_network):  Corporate area network or CAN is a computer network made up of an interconnection of LANs within a limited geographical area
  * [Backbone](https://en.wikipedia.org/wiki/Backbone_network): A backbone or core network is a part of a network which interconnects pieces of various networks, providing a path for the exchange of information between different LANs or subnetworks
  * [Metropolitan \(MAN\)](https://en.wikipedia.org/wiki/Metropolitan_area_network)
    * [Municipal wireless \(MWN\)](https://en.wikipedia.org/wiki/Municipal_wireless_network)
  * [Wide \(WAN\)](https://en.wikipedia.org/wiki/Wide-area_network):  Wide Area Network \(WAN\) is a telecommunications network that extends over a large geographic area for the primary purpose of computer networking.
  * [Cloud \(IAN\)](https://en.wikipedia.org/wiki/Internet_area_network)

{% hint style="info" %}
_Nobody owns the internet, it is an entity as such_
{% endhint %}

* The largest users of the internet, in order:
  * Asia
  * North America
  * Europe
  * Africa
  * Oceania
* In the UK, as of February 2020, 96% of households have internet access

### World Wide Web

The **World Wide Web** is an information system where documents and other web resources are identified by Uniform Resource Locators \(URLs\), which may be interlinked by hypertext, and are accessible over the Internet

Who invented the World Wide Web \(WWW\)? 

* English scientist **Tim Berners-Lee** invented the World Wide Web in 1989. 
* He wrote the first web browser \(called WorldWideWeb\) in 1990 while employed at CERN near Geneva, Switzerland.
* The browser was released outside CERN to other research institutions starting in January 1991
* Then to the general public in August 1991

#### Transmission Control Protocol \(TCP\)

* The **Transmission Control Protocol** \(**TCP**\) is one of the main protocols of the Internet protocol suite. It originated in the initial network implementation in which it complemented the Internet Protocol \(IP\). Therefore, the entire suite is commonly referred to as TCP/IP. TCP provides reliable, ordered, and error-checked delivery of a stream of octets \(bytes\) between applications running on hosts communicating via an IP network. Major internet applications such as the World Wide Web, email, remote administration, and file transfer rely on TCP, which is part of the Transport Layer of the TCP/IP suite. SSL/TLS often runs on top of TCP.
  * TCP is connection-oriented, and a connection between client and server is established before data can be sent. The server must be listening \(passive open\) for connection requests from clients before a connection is established. Three-way handshake \(active open\), re transmission, and error-detection adds to reliability but lengthens latency. Applications that do not require reliable data stream service may use the User Datagram Protocol \(UDP\), which provides a connectionless datagram service that prioritizes time over reliability. TCP employs network congestion avoidance. However, there are vulnerabilities to TCP including denial of service, connection hijacking, TCP veto, and reset attack. For network security, monitoring, and debugging, TCP traffic can be intercepted and logged with a packet sniffer.
  * Though TCP is a complex protocol, its basic operation has not changed significantly since its first specification. TCP is still dominantly used for the web, i.e. for the HTTP protocol, and later HTTP/2, while not used by latest standard HTTP/3.
* TCP verifies the correct delivery of **data from** its **source** to **destination,** It can also: 

  * Detect errors 
  * Detect duplicate messages and discard them
  * Detect lost data
  * Request retransmission of data until it is correct and complete
  * Use flow control to slow down the data transfer if the receiver cannot keep up

#### User Datagram Protocol \(UDP\)

UDP uses a simple connectionless communication model with a minimum of protocol mechanisms. UDP provides checksums for data integrity, and port numbers for addressing different functions at the source and destination of the datagram \(A **datagram** is a basic transfer unit associated with a packet-switched network\). It has no handshaking dialogues, and thus exposes the user's program to any unreliability of the underlying network; there is no guarantee of delivery, ordering, or duplicate protection.

#### Internet Protocol \(IPv4 and IPv6\)

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
    * Benefits of IPv6
      * Has more addresses available, due to the higher number of bits, thus more devices can be registered
      * No more NAT \(Network Address Translation\)
      * Auto-configuration
      * No more private address collisions
      * Better multicast routing
      * Simpler header format
      * Simplified, more efficient routing
      * True quality of service \(QoS\), also called "flow labeling"
      * Built-in authentication and privacy support
      * Flexible options and extensions
      * Easier administration \(no more DHCP\)

#### DNS \(Domain Name System\)

**Domain Name System** \(**DNS**\) is a hierarchical and decentralized **naming system** for computers, services, or other resources connected to the Internet or a private network.

* The **DNS server** connects these computers together, like a phone book
* Domain name
* Domain Structure
* Domain Registars

#### Architecture and Components

* Hardware
* Software
* Networking
* Protocols
* * Web Hosting
* Internet Service Provider
* Domain name, structure and registers
* Web Servers

#### Static Page requests

A **static web page** is a web page that is delivered to the user's web browser exactly as stored, using a web server interacting with one or more files \(HTML, CSS, JS\) for one web page

Advantages of a static website

* Provide improved security over dynamic websites \(dynamic websites are at risk to web shell attacks if a vulnerability is present\)
* Improved performance for end users compared to dynamic websites
* Fewer or no dependencies on systems such as databases or other application servers
* Cost savings from utilizing cloud storage, as opposed to a hosted environment

Disadvantages of a static website

* Dynamic functionality must be performed on the client side

#### Dynamic Page requests

Dynamic web pages are produced by dynamic web apps, in which HTML pages interact with the web server, application server, database server, which recreates a web page from data to the user.

A **server-side dynamic web page** is a web page whose construction is controlled by an **application server** processing server-side scripts. In server-side scripting, parameters determine how the assembly of every new web page proceeds, including the setting up of more client-side processing.

A **client-side dynamic web page** processes the web page using HTML scripting running in the **browser software** as it loads. JavaScript and other scripting languages determine the way the HTML in the received page is parsed into the Document Object Model \(DOM\), that represents the loaded web page. The same client-side techniques can then dynamically update or change the DOM in the same way. Even though a web page can be dynamic on the client-side, it can still be hosted on a static hosting service such as GitHub Pages or Amazon S3 as long as there isn't any server-side code included.

**Advantages**

* You can have a template of the website that can be used across every webpage on the website
* You can create a back-end to update the website without adding any new code functionality to the website

**Disadvantages**

* Dynamic hosting of web applications can be expensive

Question for next session: describe and identify one exampe where hexadecimal numbers used in websites

* colour palette, using cascading style sheets, you can change the colour of a HTML attributes \(id, class or tag\) by linking the attribute to the CSS code \(.body { background-color: \#ff0000 } \)

### Sources

* [https://en.wikipedia.org/wiki/Computer\_network](https://en.wikipedia.org/wiki/Computer_network)

