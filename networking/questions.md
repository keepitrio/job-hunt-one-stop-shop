**Describe how a browser gets content to display.** 

When a URL is entered into the browser, the browser checks if this HTTP request object exists in the cache. If not cached, the browser asks the OS to make a DNS lookup, which upon success, replies with the IP address to the browser. Then, the browser opens a TCP connection to the server, and through this, sends an HTTP request. The browser then checks the status code — 200 indicates success. If the response is cacheable, it’s stored in the cache to prevent any future unnecessary DNS lookups. The browser then decodes the response, and determines how to parse it.

To display the contents, the browser processes the HTTP response and the document type to construct a DOM tree of nodes corresponding to HTML elements and a CSSOM tree of nodes corresponding to CSS selectors. These trees combine into the render tree, which matches each HTML element with the specific style from the CSSOM tree. The browser then runs layout on the render tree to paint these nodes of pixels onto their designated positions within the viewport. Any dynamic changes (e.g. scrolling around a page, jQuery, etc.) are repainted for the affected nodes. 
 
**What are HTTP headers, and why are they used?** 

HTTP headers are additional key-value pairs of information sent directly after the request or response line, that do not belong in the body. They’re commonly used to specify the content types to accept or be accepted, authentication, caching, cookies, CORS, and more. If "Fastly-debug: true" is added to an HTTP Request, more information otherwise unseen can be seen regarding the cache servers hit, TTL information, and more.

**How would you test if an HTTP request is working as expected?**

I’d immediately check the status code of a request. 5xx status code indicate a failure by the server. 4xx codes indicate an error within the request itself (e.g. bad syntax, authorization necessary). 3xx codes indicate a redirect to a new URI or that a request should got o a different address. 2xx codes indicate success. 

In the command line, I would use `curl -svo /dev/null link.us’, which will show the details of the request and response. I can verify the status code by looking at the line:
`HTTP/1.1 ???’

**Difference between UDP and TCP?**

**Difference between CNAME and A record?**

**Port numbers for HTTP and HTTPs**

**What's FTP?**



