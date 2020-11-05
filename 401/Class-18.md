# Readings: Socket.io
<!-- ### Author -->

## [WebSocket](https://en.wikipedia.org/wiki/WebSocket)

WebSocket is a computer communications protocol, providing full-duplex communication channels over a single TCP connection. The WebSocket protocol was standardized by the IETF as RFC 6455 in 2011, and the WebSocket API in Web IDL is being standardized by the W3C.

WebSocket is distinct from HTTP. Both protocols are located at layer 7 in the OSI model and depend on TCP at layer 4. Although they are different, RFC 6455 states that WebSocket "is designed to work over HTTP ports 443 and 80 as well as to support HTTP proxies and intermediaries," thus making it compatible with the HTTP protocol. To achieve compatibility, the WebSocket handshake uses the HTTP Upgrade header[1] to change from the HTTP protocol to the WebSocket protocol.

The WebSocket protocol enables interaction between a web browser (or other client application) and a web server with lower overhead than half-duplex alternatives such as HTTP polling, facilitating real-time data transfer from and to the server. This is made possible by providing a standardized way for the server to send content to the client without being first requested by the client, and allowing messages to be passed back and forth while keeping the connection open. In this way, a two-way ongoing conversation can take place between the client and the server. The communications are usually done over TCP port number 443 (or 80 in the case of unsecured connections), which is of benefit for those environments which block non-web Internet connections using a firewall. Similar two-way browser-server communications have been achieved in non-standardized ways using stopgap technologies such as Comet.

Most browsers support the protocol, including Google Chrome, Microsoft Edge, Internet Explorer, Firefox, Safari and Opera.


---


[Difference Between WebSocket and Socket.io](https://www.educba.com/websocket-vs-socket-io/)

WebSocket is the communication Protocol which provides bidirectional communication between the Client and the Server over a TCP connection, WebSocket remains open all the time so they allow the real-time data transfer. When clients trigger the request to the Server it does not close the connection on receiving the response, it rather persists and waits for Client or server to terminate the request.

Socket.IO is a library which enables real-time and full duplex communication between the Client and the Web servers. It uses the WebSocket protocol to provide the interface. Generally, it is divided into two parts, both WebSocket vs Socket.io are event-driven libraries

Client Side: it is the library that runs inside the browser
Server Side: It is the library for Node.js


WebSocket

Below are the features:

Key features of WebSocket 

WebSocket helps in real-time communication between the Client and the web server.

This protocol helps in transforming to cross-platform in a real time world between the server and the client.

This also enables the business around the world for real-time web application to enhance and to increase the feasibility.
The major advantage it stands over an HTTP connection that it provides full duplex communication.

Why do we need WebSocket?

It provides the full duplex communication which helps in persisting the connection established between the Client and the Web Server.

It also lives up to the standards and provides the accuracy and efficiency stream events to and from with negligible latency.
WebSocket removes the overhead and reduce complexity.
It makes real-time communication effortless and efficient.


Socket.IO

Below are the features

Key features of Socket.IO

It helps in broadcasting to multiple sockets at a time and handles the connection transparently.

It works on all platform, server or device ensuring the equality, reliability, and speed.

It automatically upgrades the requirement to WebSocket if needed.
It is a custom real-time transport protocol implementation on top of other protocols.

It requires both libraries to be used Client side as well as a server-side library.

IO works on work-based events. there are some reserved events which can be accessed using the Socket on server side like Connect, message, Disconnect, Ping and Reconnect.
There are some Client based reserved events like Connect, connect- error, connect-timeout and Reconnect etc.

Why do we need Socket.IO:

I handle all the degradation of your technical alternatives to get full duplex communication in real time.
It also handles the various support level and the inconsistencies from the browser.

It also gives the additional feature room support for basic publish infrastructure and thinks like automatic reconnect.
Currently, AFAIK is the most used one and easier to help with vanilla web sockets.

---

[Back to Home](https://pdariuslee.github.io/reading-notes/)