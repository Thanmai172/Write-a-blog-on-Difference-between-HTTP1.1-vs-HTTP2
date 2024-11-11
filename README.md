Write a blog on Difference between HTTP1.1 vs 
HTTP2 


The Hypertext Transfer Protocol (HTTP) is the backbone of the web, 
facilitating the communication between web browsers and servers. 
1. Multiplexing vs. Pipelining 
• HTTP/1.1: Utilizes pipelining, where multiple requests can be 
sent out before receiving responses. However, responses are 
returned in the same order as the requests, leading to head-of
line blocking. 
• HTTP/2: Introduces multiplexing, allowing multiple requests 
and responses to be sent concurrently over a single connection 
without head-of-line blocking, significantly improving 
efficiency. 
2. Header Compression 
• HTTP/1.1: Headers are sent as plain text, leading to significant 
overhead, especially with repetitive headers. 
• HTTP/2: Uses HPACK compression to reduce the size of 
headers, which decreases latency and improves load times. 
3. Binary Protocol vs. Text Protocol 
• HTTP/1.1: Operates as a text-based protocol, making it easier 
for developers to debug but slower to parse. 
• HTTP/2: Is a binary protocol, which is more efficient to parse 
and less prone to errors, leading to faster processing and 
transmission. 
4. Server Push 
• HTTP/1.1: Does not support server push, meaning the server 
can only respond to client requests. 
• HTTP/2: Introduces server push, allowing servers to send 
resources to the client proactively, even before they are 
requested, reducing the time needed to load web pages. 
5. Connection Management 
• HTTP/1.1: Often requires multiple TCP connections to load a 
single web page, leading to increased overhead and slower 
performance. 
• HTTP/2: Uses a single, long-lived connection to serve multiple 
requests, reducing the overhead associated with establishing 
multiple TCP connections. 
6. Prioritization 
• HTTP/1.1: Lacks built-in prioritization for requests, making it 
difficult to optimize the loading of resources. 
• HTTP/2: Allows clients to prioritize requests, ensuring that 
critical resources are loaded first, which improves the user 
experience. 
7. Security 
• HTTP/1.1: Can be used with or without TLS (HTTPS), 
although many sites have adopted HTTPS for security. 
• HTTP/2: Requires HTTPS in most implementations, ensuring 
that all communications are encrypted, which enhances security 
across the board. 
8. Latency and Performance 
• HTTP/1.1: Suffers from higher latency due to the limitations of 
pipelining and lack of multiplexing. 
• HTTP/2: Significantly reduces latency with multiplexing, 
header compression, and other optimizations, leading to faster 
web page load times. 
9. Adoption and Compatibility 
• HTTP/1.1: Is universally supported by all web browsers and 
servers, making it a widely adopted standard. 
• HTTP/2: Is supported by most modern browsers and servers but 
falls back to HTTP/1.1 if not supported, ensuring compatibility. 
10. Resource Usage 
• HTTP/1.1: Uses more resources due to multiple connections 
and larger headers, which can strain both the client and the 
server. 
• HTTP/2: Is more resource-efficient, thanks to its optimized 
connection management and header compression, leading to 
better overall performance. 
Read about IP address, port, HTTP methods, 
MAC address. 
IP Address: An IP address is like your home address on the 
internet. It tells other computers where to send information when 
you're browsing the web or using an app. Every device connected 
to the internet has its own IP address. 
Port: Think of a port as a specific door or entryway on your 
computer for different types of online activities. For example, 
when you visit a website, your computer uses a specific port to 
communicate with the web server. Different activities use different 
ports. 
HTTP Methods: HTTP methods are actions that your web 
browser can perform when talking to a website. For example, when 
you visit a page, your browser uses a "GET" method to request that 
page. If you're submitting a form, it might use a "POST" method to 
send the information to the server. 
MAC Address: A MAC address is like a serial number for your 
device's network card (the part that connects to the internet). It's 
unique to each device and is used to identify your device on a local 
network, like your home Wi-Fi. 
Difference Between IP and MAC Address: The IP address helps 
devices find each other on the internet, like a global map, while the 
MAC address identifies devices on a local network, like naming 
each device in your house. 
Understanding Objects and Their Internal 
Representation in JavaScript 
1. What is an Object in JavaScript? 
• An object in JavaScript is a collection of key-value pairs. These 
keys (also called properties) can be strings or symbols, and the 
values can be anything: numbers, strings, functions, or even 
other objects. 
2. Internal Representation: Property Descriptors 
• Under the hood, JavaScript objects are built using property 
descriptors. Each property in an object has a descriptor that 
defines characteristics like whether the property is writable (can 
be changed), enumerable (shows up in loops), or configurable 
(can be deleted or modified). 
3. Prototype Chain 
Every JavaScript object has a hidden link to another object called 
its prototype. This link forms what’s known as the prototype chain. 
4.Objects as Hash Maps 
• Internally, JavaScript objects are often implemented as hash 
maps. This means that each key (property name) is hashed, and 
this hash is used to quickly find the corresponding value.  
5. Garbage Collection and Memory Management 
• JavaScript manages memory automatically through a process 
called garbage collection. When an object is no longer needed 
(i.e., there are no references to it), the memory it occupies is 
freed up.