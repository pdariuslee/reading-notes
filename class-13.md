# From the `http://diveinto.html5doctor.com/` docs

## Local storage for web applications

- Cookies were invented early in the web’s history, and indeed they can be used for persistent local storage of small amounts of data.

  - Downsides:
  
    - Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over
    
    - Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL)
    
    - Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful


- problem that HTML5 set out to solve: to provide a standardized API, implemented natively and consistently in multiple browsers, without having to rely
on third-party plugins.

- “HTML5 Storage” is a specification named Web Storage, which was at one time part of the HTML5 specification proper, but was split out into its own 
specification for uninteresting political reasons. Certain browser vendors also refer to it as “Local Storage” or “DOM Storage.”

- HTML5 Storage - a way for web pages to store named key/value pairs locally, within the client web browser. Like cookies, this data persists even after you 
navigate away from the web site, close your browser tab, exit your browser, or what have you. Unlike cookies, this data is never transmitted to the remote 
web server (unless you go out of your way to send it manually). Unlike all previous attempts at providing persistent local storage, it is implemented 
natively in web browsers, so it is available even when third-party browser plugins are not.

- HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key 
is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as 
a string. If you are storing and retrieving anything other than strings, you will need to use functions like parseInt() or parseFloat() to coerce your 
retrieved data into the expected JavaScript datatype.
  
  
  



 




 

[Back to Home](https://pdariuslee.github.io/reading-notes/)
