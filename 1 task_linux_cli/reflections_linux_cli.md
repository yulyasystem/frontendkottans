# Command Line Basics
I finished the course on CLI. It was interactive, also I made pro projects and quizes. Projects was sometimes repeatable, but now I strongly remember commands :smiley: 

One thing that suprise me was nano editor just in terminal. And I tried to use it in my local and it is working. What the magic!

![Image of Completed cource](https://github.com/yulyasystem/kottans-frontend/blob/master/1%20task_linux_cli/cli-completed.png)

![Image of Completed cource pro version](https://github.com/yulyasystem/kottans-frontend/blob/master/1%20task_linux_cli/cli-completed-adittional.png)

`pwd` print working directory

`ls` list files in working dirs

`cd ..` move up one dir

`mkdir` make directory

`touch` new file in working directory


# HTTP Basics
### Key points:
* http follows client/server or request/repsonse model (web-browsers are clients- HTTP and servers are like applications)
* it is stateless protocol: every single transaction you make through http is independent and is not related to any other transactions
* application layer: http uses TCP/IP as transport level, application level is above it, TCP cares about how data is sent, transmitted, and hhtp do not.
* client actions(verbs): whenever the client requests something from the server it specifies as a special action(method), for example, method get want to get page.
* server status codes: it defines response status codes that the server make back to the client, for example, popular 404 not found. Status code helps the client understand the servers response.
##### Classification of status codes:
  * 1xx Information messages

  * 2xx Succesful (202 accepted)

 * 3xx Redirection

 * 4xx Client Error

 * 5xx Server Error

* headers: tiny bits of custom info that you send along with your request and responses, for example, content type like JSON, XML or just text. Headers and included both in request side and response one.
request messages are sent via uniform resource locator.
Communication of client and server: client sends request with url and verb(get,post etc)-> server responses with client code+message body. 

**What was new for me?**
The whole HTTP sphere was new for me. I know a pieces of info about that and I want to know more, because it is still abstract for me.

**What did suprise me?**
I was suprised that I have already faced with server status codes and these codes are just information from server, by means of what client interpret respond of server.

**What will I intend?**
I read only a few info about http but I wanna know how to view http traffic and how that can help me in building applications.

##### HTTPS 
It is secured version of http, where new additional layer was added called SSL or TLS. 
**Steps to establish connections between endpoints :**
 * resolve IP from host via DNS(domain-name-system)

 * establish a connection with server

 * send a request

 * wait for response

 * close connection

**Identification and Authentication**
Identification means verify that someone is valid user
Autentification related to login/password, server denies request and send code unathorized and then web browser diaplays login prompt, info is sent in request header, then server validate info and allow if is valid.


**What was new for me?**
Https was new for me. I found out that this protocol has additional layer and is safåty

**What did suprise me?**
I was suprised that I can set cache headers to optimize pages. And http caching is pretty good thing in general. When we setting headers on everything is loaded from cache. Caching can have a big impact on perforamnce of web pages.

**What will I intend?**
I will intend https protocol building Basic Authentification in app and I will set caching headers on.
