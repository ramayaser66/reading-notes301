

# High level HTTP


![](https://res.cloudinary.com/practicaldev/image/fetch/s--nEVwEz5T--/c_imagga_scale,f_auto,fl_progressive,h_420,q_auto,w_1000/https://dev-to-uploads.s3.amazonaws.com/i/7i2siqphm44ihjh4gfme.png)


> HTTP request:

## 1. Local processing  
requests can be made by:
 - browser
 - cURL
 - API client 

 if the requests is made by the browser, 

 the browser will take the 
 -  `"scheme"/protocol`, host 
 - optional port number 
 - resource path 
 - query strings 

 then the browser
 - resolves an IP address
 - the browser look through its  cache for recently requested URLs
 - the operating system’s cache of recent queries
 -  router’s cache
 - DNS cache

 ## 2. Resolve an IP
  resolving an IP from a "DNS server"
   it is a process that include a lot of steps, if the fist request fails to return an IP address a failover will happen.

 ## 3. Establish a TCP Connection

 TCP: a transport layer protocol like UDP
  the client must open a TCP connection in order to send the request once the client has the IP address. 

 ## 4. Send an HTTP Request
 once the client has a TCP connection and an IP address the request can be sent.
  
  NOTE: a request is made up of a "request line", request header, and a body.

 ## 5. Tearing Down and Cleaning Up
 Once the response is delivered, a FIN packet is sent by the client at the TCP level. 
 the server will respond with ACK and then sends a FIN of its own and many steps follows. 



 # HttpUrlConnection

![](https://cdn.journaldev.com/wp-content/uploads/2015/03/java-HttpURLConnection.png)

___________________________________________
 allows us to create an HTTP requests without using any additional libraries. 

 the disadvantaged of using it is:

 - the code can be more cumbersome than other HTTP libraries
 - the lake of of many advanced functionalities

  ## to create a request 

  - create an HttpUrlConnection instance with the openConnection() method of the URL class, this method creates a connection but doesn't establish it. 

  HttpUrlConnection class can create all types of requests 
   you need to set the requestMethod attribute to one of the values AkA one of the request types. 

  - you can add parameters to a request
  - Add headers to a request 
  - set the connect and read timeouts
  - handel cookies 
  - handel redirects 

 - Read the response
  which can be done by  parsing the InputStream of the HttpUrlConnection instance.

  - Read the response on Failed Requests
  - Build the Full Response















