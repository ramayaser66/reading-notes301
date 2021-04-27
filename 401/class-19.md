
# WebSocket

![](https://miro.medium.com/max/1022/1*YBhmJDuON35aF6lBlILTjA.png)


WebSocket is a computer communications protocol, providing full-duplex communication channels over a single TCP connection. The WebSocket protocol was standardized by the IETF as RFC 6455 in 2011, and the WebSocket API in Web IDL is being standardized by the W3C. WebSocket is distinct from HTTP.

It is a thin, lightweight layer above TCP, its suitable for using “subprotocols” to embed messages.

 we use STOMP which is a subprotocol operating on top of the lower-level WebSocket, with messaging with Spring to create an interactive web application. 

  ## Note that: 
 In the traditional request-response model used in HTTP, the client requests resources, and the server provides responses.

HTTP and WebSocket both are communication protocols used in client-server communication.

 ![](https://media.geeksforgeeks.org/wp-content/uploads/20191203183648/WebSocket-Connection.png)

WebSocket is bidirectional, a full-duplex protocol that is used in the same scenario of client-server communication, unlike HTTP it starts from ws:// or wss://. It is a stateful protocol, which means the connection between client and server will keep alive until it is terminated by either party (client or server). after closing the connection by either of the client and server, the connection is terminated from both the end.


  ![](https://media.geeksforgeeks.org/wp-content/uploads/20191203183429/HTTP-Connection.png)


When can a web socket be used:

- Real-time web application
- Gaming application 
- Chat application 



## When not to use WebSocket:
 WebSocket can be used if we want any real-time updated or continuous streams of data which is being transmitted over the network. If we want to fetch old data, or want to get the data only once to process it with an application we should go with HTTP protocol, old data which is not required very frequently or fetched only once can be query by the simple HTTP request, so in this scenario better not use WebSocket.

