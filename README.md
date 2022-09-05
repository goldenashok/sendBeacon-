# sendBeacon-
The SendBeacon method, we can asynchronously send small amount of data over an HTTP requst to the sever
The browser does not wait for the response for the request sent through sendBeacon. The sendBeacon will send an HTTP POST request.
We are sending data to the server on **unload** or **beforeunload** event. once the event is fired, listern the data, collect the data and send data to the server. this will make delay the page unloading.

To Overcome the above problem we can use the **sendBeacon**
1. it send data asynchronously
2. it doesn't block the unloading of the current page
3. it doesn't wait for the response
4. The requests will be initiated before a page unloads, even when the browser is closed

>Syntax
```
navigator.sendBeacon(url, data)
```
