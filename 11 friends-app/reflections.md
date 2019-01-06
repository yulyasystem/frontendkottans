## Friends App

Even week ago I did not realize that I can do my own app in one day, month ago that I  just can  write something. Thanks to Kottans and reviews, I used obtained knowledge in this app.

My first experience of using API was interesting, It is easier and more convinient to use api than write data by your own.  

### Async JS
*The Call Stack* tracks functions that are currently active and are being processed. *The Event Queue* keeps track of tasks that are waiting to be on the cal stack. *Event loop* : when stack is empty it takes first task and moves to call stack an execute. 

Web APIs add tasks to the  event queue. For example, they are DOM Event Handlers, Network Requests. They are used in my Friends App. 

Asynchronous programming in JS is achieved by using Web APIs that processes code on seperate threads O_O. They send their results as tasks on event queue. Tasks are defined by callback funcs passed into APIs. Ooo, so haaard... 

Async code will only run when the call stack is empty.
