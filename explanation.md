# How Browsers work


## Content of study
1. Available-Browsers 
     * 1.0. List of browsers
     * 1.1. Statistic on browsers
2. Browser-Structure
3. Main components of browsers
4. Main functionality
5. Rendering Engine and flow
6. Webkit v/s Gecko 
7. Resources

  1.0. [dzone.com](https://dzone.com/articles/how-browsers-work-behind)
  
  2.1. [Skillcrush.com](http://skillcrush.com/2013/02/24/how-browsers-work/)
  

# 1. Available-Browsers. 
1.0. List of browsers
There are five major browsers used on **desktop** today: 

1. Chrome
2. Internet Explorer
3. Firefox
4. Safari and 
5. Opera. 

On **mobile**, the main browsers are :

* Android Browser
* iPhone
* Opera Mini and Opera Mobile
* UC Browser
* the Nokia S40/S60 browsers and 
* Chrome

>  NB: All are based on WebKit **except** for the Opera browsers

I will give examples from the open source browsers Firefox and Chrome, and Safari (which is partly open source). 
### According to StatCounter statistics (as of June 2013)
>Chrome, Firefox and Safari make up around 71% of global desktop browser usage. 
>On mobile, Android Browser, iPhone and Chrome constitute around 54% of usage. 



## 3. Main components of a browser:

    
* **The user interface**

  This includes the address bar, back/forward button, bookmarking menu etc. Every part of the browser display except the main window where you see the requested page.

* **The browser engine**

  It marshalls the actions between the UI and the rendering engine.
    
* **The rendering engine**

  Responsible for displaying the requested content. For example if the requested content is HTML, it is responsible for parsing the HTML and CSS and displaying the parsed content on the screen.
    
* **Networking**

  Used for network calls, like HTTP requests. It has platform independent interface and underneath implementations for each platform.
    
* **UI backend**

  Used for drawing basic widgets like combo boxes and windows. It exposes a generic interface that is not platform specific.
  Underneath it uses the operating system user interface methods.

* **JavaScript interpreter**

  Used to parse and execute the JavaScript code.
    
* **Data storage**

  This is a persistence layer. The browser needs to save all sorts of data on the hard disk, for examples, cookies. The new HTML specification (HTML5) defines 'web database' which is a complete (although light) database in the browser.
  
  
  ## 4. Main functionality of browsers

The main function of a browser is to present the web resource you choose, by requesting it from the server and displaying it in the browser window. The resource is usually an HTML document, but may also be a PDF, image, or some other type of content. The location of the resource is specified by the user using a URI (Uniform Resource Identifier).

The way the browser interprets and displays HTML files is specified in the HTML and CSS specifications. These specifications are maintained by the W3C (World Wide Web Consortium) organization, which is the standards organization for the web. For years browsers conformed to only a part of the specifications and developed their own extensions. That caused serious compatibility issues for web authors. Today most of the browsers more or less conform to the specifications.

Browser user interfaces have a lot in common with each other. Among the common user interface elements are:


* Address bar for inserting a URI
* Back and forward buttons
* Bookmarking options
* Refresh and stop buttons for refreshing or stopping the loading of current documents
* Home button that takes you to your home page

Strangely enough, the browser's user interface is not specified in any formal specification, it just comes from good practices shaped over years of experience and by browsers imitating each other. The HTML5 specification doesn't define UI elements a browser must have, but lists some common elements. Among those are the address bar, status bar and tool bar. There are, of course, features unique to a specific browser like Firefox's downloads manager. 