### **HTTP Request Methods**

- **GET:** Retrieves data from a server without modifying it.  
- **POST:** Sends data to the server to create or update a resource.  
- **PUT:** Updates or replaces an existing resource on the server.  
- **HEAD:** Retrieves headers from a resource without the actual content.  
- **OPTIONS:** Displays supported HTTP methods and communication options for a target resource.

---

### **Common Ports Targeted During a Hack**

- **443 (HTTPS):** Secure web traffic; often targeted for encrypted attacks or data interception.  
- **3389 (RDP - Remote Desktop Protocol):** Used for remote access; a frequent target for brute-force attacks.  
- **5650:** Sometimes exploited by attackers for unauthorized connections or backdoor access.

---

### **OWASP (Open Web Application Security Project)**

- A **nonprofit organization** dedicated to improving software security.  
OWASP provides **guidelines, tools, and documentation** that help developers identify and mitigate vulnerabilities in **web applications**.

---

### **XSS (Cross-Site Scripting) Payload Examples**

Used by attackers to inject malicious scripts into web pages viewed by other users.

```html
<script>alert(window.origin)</script>
<script>alert(document.cookie)</script>
<img src="" onerror=alert(document.cookie)>
