#H1 How browsers work
*****************




###What is a browser? 

....it is a software application for retrieving, presenting, and traversing information resources on the *World Wide Web*. 
 An information resource is identified by a Uniform Resource Identifier (URI/URL) and may be a web page, image, video or other piece of content.

 The browser main functionality is to present the web resource you choose, by requesting it from the server and displaying it on the browser window. The resource format is usually HTML but also PDF, image and more. The location of the resource is specified by the user using a URI (Uniform resource Identifier) 

 A Web browser knows how to go to a Web server on the Internet and request a page, so that the browser can pull the page through the network and into your machine. A Web browser knows how to interpret the set of HTML tags within the page in order to display the page on your screen as the page's creator intended it to be viewed.


**Web server** - A Web server is a piece of computer software that can respond to a browser's request for a page, and deliver the page to the Web browser through the Internet. You can think of a Web server as an apartment complex, with each apartment housing someone's Web page. In order to store your page in the complex, you need to pay rent on the space. Pages that live in this complex can be displayed to and viewed by anyone all over the world. Your landlord is called your host, and your rent is usually called your hosting charge. Every day, there are millions of Web servers delivering pages to the browsers of tens of millions of people through the network we call the Internet. 
 The way the browser interprets and displays HTML files is specified in the HTML and CSS specifications. These specifications are maintained by the **World Wide Web Consortium** organization, which is the standards organization for the web.
A browser has a user interface that most commonly includes an address bar, back/forward button, and reload button, sometimes refered to this as the “chrome”  of a browser (little “c”, not Chrome by Google). When you navigate to a URL in the address bar you are making a “request” for the content at that URL.
That URL you typed into the address bar maps to an IP address. This is called a DNS lookup. DNS stands for __Domain Name System__ and it maps numeric computer addresses to human readable names. All computers have an IP address. For example, one IP address for Google is 74.125.134.102. You can enter 74.125.134.102 in the address bar and it will show the contents at www.google.com. Once the browser has the IP address it sends an HTTP request to the web server at that address. HTTP stands for “Hypertext Transfer Protocol” and is used to facilitate requests from your client (the browser) and responses from the server. As this HTML response is being sent to your browser, the browser’s rendering engine is displaying the requested content on your screen. To accomplish this the rendering engine “parses” the HTML and creates a DOM tree.
__What is DOM?__ It is the output tree - the parse tree is a tree of DOM element and attribute nodes. DOM is short for Document Object Model. It is the object presentation of the HTML document and the interface of HTML elements to the outside world like JavaScript. The root of the tree is the "Document" object.
The browser then parses style data (CSS or inline styles) and together with the HTML it constructs a render tree. The render tree displays rectangles (that represent divs, paragraphs, headlines, etc.) with a few visual attributes such as color and size dimensions. These rectangles are displayed in order on the page. Next, the browser lays out the contents in the position they will appear in the browser. The last step is “painting” where the elements are drawn on the screen. As the browser is rendering the HTML it will find tags that require files from other URLs. The browser will send a request to the web server to get each of these files.
 ~~Firefox uses the Gecko rendering engine, a Mozilla product. Both Safari and Chrome (and now Opera on mobile?) use Webkit as a rendering engine, which is an open source project. IE uses the Trident rendering engine.~~


**********
REFERENCES
http://skillcrush.com/2013/02/24/how-browsers-work/
http://ptgmedia.pearsoncmg.com/images/9780789736260/samplechapter/0789736268_Sample_Chapter_18.pdf
http://computer.howstuffworks.com/web-page1.htm
