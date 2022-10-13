API - Application Programming Interface

- Application - Software that does a task. - Ebay/google search/skype ....
- Programming - Programming that does a task in the Application. - Zomato uses a program for placing a order.
- Interface - is a place to tell the program to run.

- An API exists where you can tell (I) a computer program(P) to run in an application (A).
- An API means telling a program to run a task in a piece of software or application.


What makes API's great ?
1. Just use the program don't write it.
2. Platfrom Independent.

Cycle of API Request(Transaction):
1. A request is made for something to be done.
2. A program id run to complete that request.
3. The program sends back a response.

Example google search : 

www.google.com/search?q=code

location where program exists : google.com

program/Folder : Search

search term : code => We can add this using a parameter here it is a query after `?`.

response: a web page with results.

params are separated by `&`.

Api's calling API's.


----------------------------------------------------------------------

WEB SERVICE :

Web => Internet => connected systems.

Service => API

Web Service => API that uses internet.

`All web services are API but not all APIs are web services because not all APIs use internet.`

Web Service Components:
- XML/JSON to format data over the internet.
- REST, SOAP, OR XML/RPC to transfer the data. => **Protocol** 

-------------------------------------------------------

HTTP

When we are sending a request over the internet to a computer we use something called HTTP/ Hyper Text Transfer Protocol.
and also the response is sent using HTTP.

HyperText - Contains links to another text/document. => https://www.google.com

Request components - 

1. Start Line => **mandatory** => Tells the program what to do.
2. Headers => Additional Inforamtion
3. Blank LIne
4. Body => Actual Information.

Response also uses the same as above 


|   HTTP      |    REQUEST     |      RESPONSE   |
| ----------- | -------------- | --------------- |

**Request:**

- Startline - version of HTTP, method type - POST/GET/PUT/DELETE, parameters (/search?q=code) - also know as Request line.
- Headers - HOST(www.google.com), Token for authorization
- API Program folder - Yes example: /search
- Parameters - Yes example: ?q=code
- status code - No

- Blankline -
- Body - sending information in post
- StartLine Format - Method(Space)API Program Folder LOcation+Parameters(space)HTTP Version
- Example: GET/search?q=code HTTP/1.1

**Response:**

- Startline - Status code, version of HTTP -  also know as response line or staus line
- Headers - Cookies, file size, type(HTML)
- API Program folder - No
- Parameters - No
- status code - Yes example:200
- Startline Format - HTTP version + Status Code
- Example - HTTP/1.1 200 OK


- Blankline - 
- Body - HTML document


**Idempotance** - Can do as many times as you want and result stays the same => In other words safe to repeat the request.

GET, PUT, DELETE - Yes
POST - No


**Headers** :

https://developer.mozilla.org/en-US/docs/Glossary/HTTP_header#:~:text=An%20HTTP%20header%20is%20a,format%20of%20the%20returned%20body.

**BlankLine** - Tells where hearders finish and body begins

**Body**  - Contains content.

It can be a image, video, HTML web page, Text data - data you would like to send to am API

Content-Type - header specifies type of content that is being sent or received in the body - Type/Subtype

----------------------------------

**Stateless** 

State => Current Situation (in context)

State (HTTP) => Web request and response 

less =>Without

HTTP Stateless => Request Unknow

HTTP is stateless buy default 

HTTP methods are in RESRT and SOAP

example of stateful protocol => FTP (File Transfer Protocol )

Best example can be a old landline where you don't know who is calling until you pick the call.

So, server does not know what is happening between HTTP calls then how to server know who you are ? => by cookies
HTTP Header : SET-Cookie => this request response from application sends back to browser this makes browser to set a cookie and sends a response.


-----------------------------

**HTTP Security**
- Cookies are not executable.
- Cookies don't store passwords (e.g: can use tokens)
- Applications store data with session id
- MFA
- Biometrics
- Antivirus Software


---------------------------------
**Application Infrastructure:** 

- Application - Amazon, Flipkart e.t.c 
- Client (Requester) -Browser/Programs
- Initial Receiver - Load Balancer/Server
- Server - Application Server
- Client-server communication - Cables or satellite
- Memory - Database

This infrastructure can be compared to telephones infrastructure in 1980's

`Stateless Infrastructure benefits: `
- Scalability
- Resilience
- Less Memory Needed

--------------------------------------------











