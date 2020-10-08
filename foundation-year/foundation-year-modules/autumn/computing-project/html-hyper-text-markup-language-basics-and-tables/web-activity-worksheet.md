# Web Activity Worksheet

### Worksheet can be found [here](https://github.com/AdnanTech/UniversityOfSussex/blob/master/ComputingProject/WebActivityWorksheet.pdf)

### W3C

World Wide Web Consortium \(W3C\) is an organization created by Tim Bernes Lee , they overlook the rules of web, such as protocols, guidelines

### Have you created a website?

1. Yes, I have created my own Django \(python\) framework to make a blog that I use offline as a local server, planned to move it to a NGINX server but a bit overloaded with time currently, and it doesnt have all the features I wanted to implement
2. I also work currently as a back-end developer with the ASP.NET \(C\#\) core framework for [FinancialJuice](https://www.financialjuice.com/home), currently working on an new NLP machine learning feature
3. In the past I've worked at [Tradeviews](https://tradeviews.net/) where we had a PHP backend, with no framework
4. I have roughly dabbled in flask \(python\) for some \(unfinished\) side projects
5. Looking to redesign my blog in PHP and js, without any frameworks, to get a stronger grasp on the programming languages

### FTP

File transfer protocols are the standard network protocol used for the transfer of files between a client  \(personal machine\) and server on a computer network. Basically, they connect your web pages, in the form of files to the server where the website is being hosted.

1. At Tradeviews I used FileZilla to connect to the server
2. At FinancialJuice I use Microsoft azure web services
3. For personal projects, SiteGround have an FTP backend, or you can integrate FileZilla
4. For static pages, Github have [Github pages ](https://pages.github.com/)that I use for free hosting for static websites

### ISP

An Internet service provider \(ISP\) is an organisation that provides services for accessing, the internet. Examples are Virgin Media, BT, Sky Broadband for the UK, AT&T and comcast for the US

### URL

Uniform Resource Locators \(URLs\) are used by web browsers. The browser looks up the IP address for the domain name \(URL\) via their DNS. The browser sends a HTTP request to the server. The server sends back a HTTP response.

### IP

The Internet Protocol \(IP\) is the principal communications protocol in the Internet protocol suite for relaying datagrams \(A datagram is a basic transfer unit associated with a packet-switched network\). across network boundaries. Its routing function enables internetworking, and essentially establishes the Internet.

* **IPv4** 
  * Denary notation
  * 32-bit number 
  * 2^32
  * 8.8.8.8 \(Google's IPv4 address\)
* **IPv6** 
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

### What happens when you enter a URL?

In simple terms, the web address entered points to a IP address for the domain name via DNS. The browser sends a **Hyper text transfer protocol** HTTP request to the server. The server sends back a HTTP response of the webpage

### DNS

A Domain Name Server connects the following together:

* Domain name \(URL address\)
* Domain Structure \(server\)
* Domain Registars \(companies that ensure URLs are unqiue and keep a log of who they belong to, if someone purchases a domain through the company\)

### HTML Semantics analysis

[Web page](http://ww12.somesite.com/) that has the following elements

* h1 tag for header
* title for somesite.com
* javascript function to show policy on click as a pdf, function called showPolicy\(\);
* a tag \(link\) that runs the function above when clicked on click
* empty classes and id's to wrap the document, no css applied
* adblock key? defines specific marketing ads? -&gt; have adblock

### Testing HTML5 [browsers](https://html5test.com/)

firefox developer edition has a score of 466/555, chrome has score of 476/555, still close, likely chrome is has a wider array of html5 functionality and optimization due to more developer budget

### HTML History

HTML history can be found [here](https://www.w3schools.in/html-tutorial/history/), major events:

* _HTML 1.0_ was released in _1993_
* _HTML 2.0_, published in _1995_; which contains all the features of HTML 1.0 along with that few additional features
* _HTML 3.0_, where _Dave Raggett_ who introduced a fresh paper or draft on HTML. It included improved new features of HTML, giving more powerful characteristics for webmasters in designing web pages. But these powerful features of new HTML slowed down the browser in applying further improvements.
* _HTML 4.01_ which is widely used and was a successful version of HTML before _HTML 5.0_, which is currently released and used worldwide. 
* _HTML 5_ can be said for as an extended version of HTML 4.01 which was published in the year _2012_.

### Wayback Machine

\*\*\*\*[**GatesNotes** ](https://www.gatesnotes.com/)\*\*\*\*

* [May 2014](https://web.archive.org/web/20140502185738/http://www.gatesnotes.com/) - Original design concept blog layout
* [June 2014](https://web.archive.org/web/20140622204426/https://www.gatesnotes.com/) - New design concept, 4 by 4 table of blog entry thumbnails, fixed width for content, large banner, likely designed for lower resolution monitors \(not 1920x1080\)
* [August 2016 ](https://web.archive.org/web/20160802152437/https://www.gatesnotes.com/)- Minor to no change
* [September 2018](https://web.archive.org/web/20180929104554/https://www.gatesnotes.com/) - New banner clickable banner thats an a tag
* [October 2020](https://www.gatesnotes.com/) - Clean blog layout, dynamic, a tag underline on hover feature

### HTML Error Fixing

Lots of errors, tags arent closed properly, random spaces, no indentation makes it harder to read, semantics are the wrong way around. Here is a clean, working version:

{% code title="index.html" %}
```php
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>FYiCS</title>
</head>

<body>
    <h1>Welcome to Foundation Year in Computing Sciences</h1>
    <p>HTML basics and <center>beyond session</center></p>
</body>

</html>
```
{% endcode %}

### Static Page requests

A **static web page** is a web page that is delivered to the user's web browser exactly as stored, using a web server interacting with one or more files \(HTML, CSS, JS\) for one web page

Advantages of a static website:

* Provide improved security over dynamic websites \(dynamic websites are at risk to web shell attacks if a vulnerability is present\)
* Improved performance for end users compared to dynamic websites
* Fewer or no dependencies on systems such as databases or other application servers
* Cost savings from utilizing cloud storage, as opposed to a hosted environment

Disadvantages of a static website:

* Dynamic functionality must be performed on the client side

### Dynamic Page requests

Dynamic web pages are produced by dynamic web apps, in which HTML pages interact with the web server, application server, database server, which recreates a web page from data to the user.

A **server-side dynamic web page** is a web page whose construction is controlled by an **application server** processing server-side scripts. In server-side scripting, parameters determine how the assembly of every new web page proceeds, including the setting up of more client-side processing.

A **client-side dynamic web page** processes the web page using HTML scripting running in the **browser software** as it loads. JavaScript and other scripting languages determine the way the HTML in the received page is parsed into the Document Object Model \(DOM\), that represents the loaded web page. The same client-side techniques can then dynamically update or change the DOM in the same way. Even though a web page can be dynamic on the client-side, it can still be hosted on a static hosting service such as GitHub Pages or Amazon S3 as long as there isn't any server-side code included.

Advantages:

* You can have a template of the website that can be used across every webpage on the website
* You can create a back-end to update the website without adding any new code functionality to the website

Disadvantages:

* Dynamic hosting of web applications can be expensive

### _**My**_ Three key elements for success for web dev

1. Start small and constantly improve, have a growth mindeset, you can build twitter overnight by following tutorials, but true web developers know their tools and how they work
2. No project is too big, if you arent struggling, you are not improving, this refers to the Goldilocks rule
3. Stick to one framework at a time, until you fully understand the framework, dont context switch all the time

### Resources

A good resource for web dev, for me has always been Mozilla's \(creator of firefox\) [docs](https://developer.mozilla.org/en-US/)

### SEO

Search Engine Optimization is _the process of improving the quality and quantity of website traffic to a website or a web page from search engines_. It is also what has caused so much bloat on the internet and the decline of good content, due to marketing from SEO spam unfortunately

### Scripting Languages

A Scripting language is a programming language for a special run-time environment that automates the execution of tasks; the tasks could alternatively be executed one-by-one by a human operator. An example is JavaScript, where functions can be run on a website, once clicked, if working as intended and implemented in the web pages' files, they are interpreted, not compiled.

### UDP vs TCP

UDP has no handshaking \(confirming correct packet transfer\) dialogues, and thus exposes the user's program to any unreliability of the underlying network; there is no guarantee of delivery, ordering, or duplicate protection, therefore less reliable than TCP

