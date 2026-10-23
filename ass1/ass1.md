# Assignment 1 – What Happens Between Typing a URL and Seeing the Page?

When I type a URL into the browser and press Enter, several steps happen behind the scenes before the webpage appears on the screen.

### 1. URL Parsing
The browser checks the URL to identify the protocol (HTTP or HTTPS), domain name, and requested path.

### 2. Browser Cache Check
The browser checks its cache to see whether it already has the required resources. If valid resources are available, it may reuse them.

### 3. DNS Lookup
The browser finds the IP address associated with the domain name (e.g., `example.com`) by checking available DNS caches or querying a DNS resolver.

### 4. Establishing a Connection
The browser connects to the server using the appropriate network protocol. With HTTP/1.1 or HTTP/2 over HTTPS, this typically involves a TCP connection followed by a TLS handshake. HTTP/3 uses QUIC, which integrates the transport connection and TLS security differently.

### 5. Sending an HTTP Request
Once the connection is ready, the browser sends an HTTP request, such as:

```http
GET /index.html HTTP/1.1
Host: example.com
```

### 6. Server Processing
The server receives the request, processes it, and sends back an HTTP response containing a status code (such as `200 OK`) and the requested content.

### 7. Receiving HTML and Other Resources
The browser receives the HTML document and starts parsing it. While parsing, it discovers additional resources such as CSS files, JavaScript files, images, and fonts, which may be requested separately.

### 8. Building the DOM and CSSOM
The browser converts the HTML into the **DOM (Document Object Model)** and parses CSS into the **CSSOM (CSS Object Model)**.

### 9. Creating the Render Tree
The browser combines the DOM and CSSOM to create a render tree containing the elements that need to be displayed.

### 10. Layout and Painting
The browser calculates the size and position of elements during layout, then paints text, colors, borders, images, and other visual content.

### 11. JavaScript Execution
The browser executes JavaScript to add interactivity and update the page when necessary. Some scripts can also affect HTML parsing and rendering.

### Conclusion
Typing a URL and pressing Enter triggers a sequence of networking and rendering operations. The browser resolves the domain name, establishes a connection, requests resources, processes HTML, CSS, and JavaScript, and renders the webpage on the screen.

This process allows users to access websites and interact with them smoothly.