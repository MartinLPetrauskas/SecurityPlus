## Application Attacks

### Application Hardening
* Use proper authentication
* Encrypt sensitive data
* Validate user input
* Avoid and remediate known exploits
* Promptly applying security patches

### Application Configuration
* Type/Scope of encryption
* Users with access to the application
* Access granted to authorized users
* Security of the underlying infrastructure

### SQL Injection Attacks
* Common SQL injection: OR 1=1
* Validate all user input

### Cross-Site Scripting (XSS) Attacks
* XSS Attacks occur when an attacker embeds malicious scripts in a third-part website that are later run by innocent visitors on that site
* XSS Attackers embed scripts on sites without permission
* Can be prevented with input validation with any user input, especaially the <script> tag

### Cross-Site Request Forgery (CSRF) Attacks
* Goes by CSRF or XSRF, or "sea surf"
* CSRF attacks leverage the fact that users are often logged into multiple sites at the same time and use one site to trick the browser into sending malicious requests to another site without the user's knowledge
* Use CSRF tokens to prevent this
* Prevent the use of HTTP Get requests
* Log users out after a certain period of time

### Clickjacking Attack
* Attacker hides elements of a webpages behind other elements so that a user cannot see what he or she is actually clicking
* Cursorjacking: specialized form of clickjacking that tricks the user about the cursors location on the screen

### Directory Traversal Attacks
* When an attacker uses directory navigation references to search for unsecured files on a server

### Cookies
* Privacy risks include cookies being used across different websites, tracking user activity, de-anonymization

### Malicious Add-Ons
* Might not know who wrote the browser add-on
* Excessive permissions
* May have a trojan horse

### Code-Execution Attacks
* Occurs when an attacker exploits a vulnerability in a system that allows the attacker to run commands in the system
* Arbitrary code execution: when the attackers runs commands of their choice