#H1 How browsers work
**********
Alt-H5 What is a browser? 
it is a software application for retrieving, presenting, and traversing information resources on the *World Wide Web*. 
 An information resource is identified by a Uniform Resource Identifier (URI/URL) and may be a web page, image, video or other piece of content.
 The browser main functionality is to present the web resource you choose, by requesting it from the server and displaying it on the browser window. The resource format is usually HTML but also PDF, image and more. The location of the resource is specified by the user using a URI (Uniform resource Identifier)
 The way the browser interprets and displays HTML files is specified in the HTML and CSS specifications. These specifications are maintained by the **World Wide Web Consortium** organization, which is the standards organization for the web.
A browser has a user interface that most commonly includes an address bar, back/forward button, and reload button, sometimes refered to this as the “chrome”  of a browser (little “c”, not Chrome by Google). When you navigate to a URL in the address bar you are making a “request” for the content at that URL.
That URL you typed into the address bar maps to an IP address. This is called a DNS lookup. DNS stands for __Domain Name System__ and it maps numeric computer addresses to human readable names. All computers have an IP address. Once the browser has the IP address it sends an HTTP request to the web server at that address. HTTP stands for “Hypertext Transfer Protocol” and is used to facilitate requests from your client (the browser) and responses from the server. As this HTML response is being sent to your browser, the browser’s rendering engine is displaying the requested content on your screen. To accomplish this the rendering engine “parses” the HTML and creates a DOM tree.
__What is DOM?__ It is the output tree - the parse tree is a tree of DOM element and attribute nodes. DOM is short for Document Object Model. It is the object presentation of the HTML document and the interface of HTML elements to the outside world like JavaScript. The root of the tree is the "Document" object.
 

**********
REFERENCES
http://skillcrush.com/2013/02/24/how-browsers-work/
http://ptgmedia.pearsoncmg.com/images/9780789736260/samplechapter/0789736268_Sample_Chapter_18.pdf