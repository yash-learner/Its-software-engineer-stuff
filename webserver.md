# What is a Web Server ? 

A web server is a software that servers web content using HTTP protocol. 
The web content can be static or dynamic.
It is used to host web pages, build APIs.


Working :

The web client such as your laptop with a web browser and IP address will make a HTTP request to the webserver with url 
running on port 80 for HTTP requests and 443 for HTTPS then the web server will process the request(it can query databse, or return a web page, or a status code)
return corresonding response such as HTML page with headers and status code.

HTTP protocol is a request response protocol(statelesss) so, before making a HTTP request the TCP protocol will run at transport layer to 
etablish two way communication(Handshake, tls establishment) between server and client.

This TCP request will allocate a bunch of memory on the server this is called TCP socket(This where all the DOS attacks happens) then the HTTP request will be 
executed. For the second request from the same client it will use same memory.


```
If you have  a TCP connection and not using jt then you are wasting server memory.
```

Blocking single threaded vs Multi threading web server => pending
