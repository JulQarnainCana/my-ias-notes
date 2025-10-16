#### [!ATTACK] OS Command Injection
 **Definition:** A severe **command injection attack** where an adversary aims to **execute arbitrary commands on the host operating system** through a vulnerable application.

---

 #### **Impact:**
 * A successful attack grants the attacker **full control of the victim's machine**.
 * If the vulnerable application runs with **elevated privileges** (e.g., as root or administrator), the attacker's injected commands inherit these high-level permissions, leading to significantly increased potential damage and a wider attack surface. * This risk extends to applications like **web applications** where the attacker has no direct OS access.
 ---

#### **Prevention & Core Issue:**
 * The root cause is incorporating **external, untrusted user input** directly into the command string that's executed by the system shell.
* **Command Separators** are the key exploit vector. Characters such as:
     ```bash
    &  &&  |  ||  ;  ( )  <  >  `  $
    ```
   When these characters are not properly **escaped, sanitized, or filtered**, the shell interprets them as new command delimiters, allowing the attacker to inject and execute additional, malicious commands.