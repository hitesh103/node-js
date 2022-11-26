## How web works ??
- Computers connected to the internet are called clients and servers. A simplified diagram of how they interact might look like this:
![client-server-Model](https://github.com/darshan-trivedi-10/Image/blob/main/node-img/simple-client-server.png)
- Clients are the typical web user's internet-connected devices and web-accessing software usually a web browser like Firefox or Chrome.
- Servers are computers that store webpages, sites, or apps. When a client device wants to access a webpage, a copy of the webpage is downloaded from the server onto the client machine to be displayed in the user's web browser.
- In addition to the client and the server, we also need to say hello to:
  - Your internet connection: Allows you to send and receive data on the web.
  - TCP/IP: Transmission Control Protocol and Internet Protocol are communication protocols that define how data should travel across the internet.
  - DNS: Domain Name System is like an address book for websites. When you type a web address in your browser, the browser looks at the DNS to find the website's IP address before it can retrieve the website. This is like looking up the address of the server so you can access it.
  - HTTP: Hypertext Transfer Protocol is an application protocol that defines a language for clients and servers to speak to each other. 

## What happens when you write www.example.com ? 
1. The browser goes to the DNS server, and finds the real address of the server that the website lives on.
2. The browser sends an HTTP request message to the server, asking it to send a copy of the website to the client. This message, and all other data sent between the client and the server, is sent across your internet connection using TCP/IP and other Protocol depends on usecases.
3. If the server approves the client's request, the server sends the client a "200 OK" message, which means "Of course you can look at that website! Here it is", and then starts sending the website's files to the browser as a series of small chunks called data packets.
4. The browser assembles the small chunks into a complete web page and displays it to you.

## Computer Network
It is a group of interconnected computer systems.

## Internet
It is network of computer networks.

## Client Server Architecture
- client-server architecture, architecture of a computer network in which many clients (remote processors) request and receive service from a centralized server (host computer).


## ALSO Read About This :- 
- TCP, OSI, UDP Model, Monolithic vs Microservices, APIS.

## Some Useful Resources
* [How Netflix Works With ISPs Around the Globe to Deliver a Great Viewing Experience](https://about.netflix.com/en/news/how-netflix-works-with-isps-around-the-globe-to-deliver-a-great-viewing-experience)
* [Amazon study: Every 100ms in Added Page Load Time Cost 1% in Revenue](https://www.contentkingapp.com/academy/page-speed-resources/faq/amazon-page-speed-study/)
* [History of the Internet](https://en.wikipedia.org/wiki/History_of_the_Internet)
* [Computer Networks Book](https://csc-knu.github.io/sys-prog/books/Andrew%20S.%20Tanenbaum%20-%20Computer%20Networks.pdf)
