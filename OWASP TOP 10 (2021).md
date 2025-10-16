### A01:2021-Broken Access Control

- **Description:** Occurs when an application doesn't properly enforce restrictions on what authenticated users are allowed to do.
    
- **Example (IDOR):** An attacker changes an ID parameter in a URL (e.g., `id=12345` to `id=67890`) to view another user's account without authorization.
    
- **Impact:** Data exposure/theft, unauthorized actions.
    

### A03:2021-Injection

- **Description:** Flaws occur when an application sends **untrusted data to an interpreter** (like a database query or OS command) without proper validation, allowing an attacker to execute unintended commands.
    
- **Impact:** Remote Code Execution (RCE), system backdoors, data corruption.
    

### A04:2021-Insecure Design

- **Description:** Risks related to **design and architectural flaws**, not just flaws in code implementation.
    
- **Example:** A "forgot password" feature that asks for a widely known, static piece of information (e.g., mother's maiden name) instead of a temporary reset token.
    
- **Impact:** Widespread vulnerabilities (as the flaw is architectural), expensive remediation.
    

### A07:2021-Identification and Authentication Failures

- **Description:** Flaws in functions responsible for user identity, authentication, and session management (e.g., weak password handling, poor MFA implementation).
    
- **Example:** Lack of rate limiting on login attempts (Brute-Force Attack).
    
- **Impact:** Account takeover, impersonation.
    

### A09:2021-Security Logging and Monitoring Failures

- **Description:** Flaws where logging, alerting, and real-time active security monitoring are insufficient or ineffective.
    

### A10:2021-Server-Side Request Forgery (SSRF)

- **Description:** A web application is tricked into fetching a remote resource from a user-supplied URL. The request is performed on the attacker's behalf, often targeting **internal resources** not exposed to the public internet.
    
- **Example:** An attacker supplies a URL like `http://localhost/admin` or an AWS metadata service endpoint to read internal data or access restricted services.
    
- **Impact:** Internal service exposure, cloud credential theft.