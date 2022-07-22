# OSI - Open Systems Interconnection Model

Not perfectly but need to understand OSI model effectively as a engineer and need to know where our application lives out of all these 7 layers of OSI Model.

Why OSI model ?

- because without a standard protocols and rules for communication then it will be difficult for the application to understand underlaying network protocol.
- Without a standard model, upgrading network equipments will be difficult.
- innovations can be done at each layer without distrubing the rest of the layers.


> **I think it is because of standardizing of networks based on a OSI model or simplfied TCP/IP model we don't have differnt applications for differnt networks such as LTE,
WIFI, Fiber e.t.c**

Protocol suffication ??

7 Layers

-------------

**Layer 7 - Application - HTTP/FTP/gRpc**

As a backend engineer we don't don't interact with layer 7 also because most of the protocols such as gRPC and rest sits on top of HTTP. Engineers use client library.

--------

**Layer 6 -  Presentation - Serilazation/Encoding**

If we send a JSON object(JS) or dictionary(Python) it needs to converted to string this is serialization, this is what happens at presentation layer.

-----------

**Layer 5 - Session - Connection Establishment, TLS **

This is where TLS happens, connection establisnments, This is where you store state in client and server.

---------------

As we know HTTP is stateless protocol so it will not have a session layer and TCP is a stateful layer this will have a session layer. At this layer session management 
happens.

**Layer 4 - Tranport Layer - TCP(Segments)/UDP(Datagram)**

Visibility of Ports

- new protocol in this layer QUIC 
- HTTP 1,  HTTP 2, are built on top of TCP
- HTTP 3 is built on top of QUIC
- QUIC is built on top of UDP

----------------

**Layer 3 - Network Layer**

Packets
Routing, IP address

--------------

**Layer 2 - Data Link Layer**

Frames
Deals with MAC addess and know about protocol we use such as Ethernet, WIFI e.t.c

--------------

**Layer 1 - Physical Layer**

It is a bare metal. Deals with how a frame taken from above data link layer is transported using medium such as Radio waves (WIFI), Ethernet(Electricity),
FIber(Light)


--------------




























































why we only send data as stream of bytes over network ?
why do we need to serialize objects while sendind a request from a applciation ?
why can't we send objects over the network ?

https://coderanch.com/t/515943/java/Object-serialized-sending-network

https://snyk.io/blog/serialization-and-deserialization-in-java/

https://en.wikipedia.org/wiki/Bitstream#:~:text=A%20bytestream%20is%20a%20sequence,translation%20between%20bytestreams%20and%20bitstreams.

https://www.alpharithms.com/byte-stream-411116/

https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/serialization/

https://en.wikipedia.org/wiki/Serialization
