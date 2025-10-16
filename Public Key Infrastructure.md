### **Public Key Infrastructure (PKI)**
A framework used to manage **digital certificates** and **public key encryption**.

---

### **Active Directory Certificate Services (ADCS)**
Microsoft’s implementation of a **PKI system**.

---

### **Certificate Authority (CA)**
A **trusted organization** that validates identities and issues **digital certificates**.

- **Trusted Root CA:**  
  The CA’s **public key** is pre-installed in web browsers and operating systems, making it automatically trusted.

---

### **Certificate Template**
A **set of configurations and policies** that define how and when a **CA** can issue a certificate.

---

### **Certificate Signing Request (CSR)**
- A file sent to a **Certificate Authority** to request a signed certificate.  
The **Private Key is never included** in the CSR.

---

### **Key Pair Generation (Applicant’s Role)**

- **Private Key (Applicant):**  
  Must remain secret; used for **digitally signing** data and **decrypting** information.

- **Public Key:**  
  Shared openly; used by others to **encrypt data** and **verify digital signatures**.

---

### **Process of Trust (HTTPS Communication)**

1. The **server** sends its **signed certificate** to the **client**.  
2. The **client’s browser** finds the CA’s **public key** in its list of **Trusted Root CAs**.  
3. The **browser** uses the CA’s public key to **verify the digital signature** on the certificate.  
4. Once verified, the browser **trusts the server’s public key** and establishes a **secure (HTTPS) connection**.
