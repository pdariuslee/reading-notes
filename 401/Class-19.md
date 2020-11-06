# Readings: Message Queues
<!-- ### Author -->

## [socket.io](https://socket.io/get-started/chat/)

What Socket.IO is

Socket.IO is a library that enables real-time, bidirectional and event-based communication between the browser and the server. It consists of:

- a Node.js server: Source | API

- a Javascript client library for the browser (which can be also run from Node.js): Source | API


How does that work?

The client will try to establish a WebSocket connection if possible, and will fall back on HTTP long polling if not.

WebSocket is a communication protocol which provides a full-duplex and low-latency channel between the server and the browser. More information can be found here.

So, in the best-case scenario, provided that:

the browser supports WebSocket (97% of all browsers in 2020)
there is no element (proxy, firewall, …) preventing WebSocket connections between the client and the server
you can consider the Socket.IO client as a “slight” wrapper around the WebSocket API. Instead of writing:


What Socket.IO is not

Socket.IO is NOT a WebSocket implementation. Although Socket.IO indeed uses WebSocket as a transport when possible, it adds additional metadata to each packet. That is why a WebSocket client will not be able to successfully connect to a Socket.IO server, and a Socket.IO client will not be able to connect to a plain WebSocket server either.


Features

Its main features are:

Reliability
Connections are established even in the presence of:

proxies and load balancers.
personal firewall and antivirus software.
For this purpose, it relies on Engine.IO, which first establishes a long-polling connection, then tries to upgrade to better transports that are “tested” on the side, like WebSocket. Please see the Goals section for more information.

Auto-reconnection support

Unless instructed otherwise a disconnected client will try to reconnect forever, until the server is available again. Please see the available reconnection options here.

Disconnection detection

A heartbeat mechanism is implemented at the Engine.IO level, allowing both the server and the client to know when the other one is not responding anymore.

That functionality is achieved with timers set on both the server and the client, with timeout values (the pingInterval and pingTimeout parameters) shared during the connection handshake. Those timers require any subsequent client calls to be directed to the same server, hence the sticky-session requirement when using multiples nodes.

Binary support

Any serializable data structures can be emitted, including:

- ArrayBuffer and Blob in the browser

- ArrayBuffer and Buffer in Node.js

Multiplexing support

In order to create separation of concerns within your application (for example per module, or based on permissions), Socket.IO allows you to create several Namespaces, which will act as separate communication channels but will share the same underlying connection.

---

[Back to Home](https://pdariuslee.github.io/reading-notes/)