## Offline Web Applications

Offline first means getting as many things on the screen as possible using caches. The rule that I have learnt from this lesson is to make people haaappy :satisfied:

Service workers througth the js file control web-page, modyfying requests and caching resources. It run on seperate thread than js file so it is designed to be fully async. Service worker is registered by `ServiceWorkerContainer.register()`, if succesfull service worker will be downloaded to page. It has such lifecycle:
* Download
* Install
* Activate

Instalaltion is triggered when page is found to be new. 

After view the course many things are unclear. I have only caught info about caching. I think I will explore Service Workers more.
![image of udacity ](https://github.com/yulyasystem/kottans-frontend/blob/master/%20offline-web-apps/owa.png)


