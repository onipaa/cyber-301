## Flashcards for Quiz 4-1

---

### **Question 1:**
**Which boot security mode sends information on the boot process to a remote server?**

**Correct Answer:**  
**Measured Boot**

**Explanation:**  
- **Measured Boot** provides a report of the boot process to a remote server, helping to ensure that a secure boot occurred. It measures the integrity of the boot process by recording each step.
- **Trusted Boot** verifies that Windows components have been started correctly.
- **Secure Boot** ensures that only trusted software is loaded during startup.
- **UEFI Native Mode** is the environment in which these security features can operate.

---

### **Question 2:**
**An IOC occurs when what metric exceeds its normal bounds?**

**Correct Answer:**  
**KRI (Key Risk Indicator)**

**Explanation:**  
- **Key Risk Indicators (KRI)** are thresholds used to measure the level of risk. If a KRI exceeds its set limits, it can indicate a security threat, commonly referred to as an **IOC (Indicator of Compromise)**.
- **IRR (Internal Rate of Return)**, **LRG (Large Resource Groups)**, and **EXR (Execution Rate)** are not related to security metrics.

---

### **Question 3:**
**Which of these is a list of preapproved applications?**

**Correct Answer:**  
**Whitelist**

**Explanation:**  
- **Whitelist** refers to a list of trusted, preapproved applications or users that are allowed to operate in a system.
- **Blacklist** includes blocked or unapproved applications.
- **Greenlist** and **Redlist** are not common terms used in this context.

---

### **Question 4:**
**Which of the following is not an improvement of UEFI over BIOS?**

**Correct Answer:**  
**Support of USB 3.0**

**Explanation:**  
- **UEFI** has several advantages over **BIOS**, including networking functionality, stronger boot security, and the ability to access larger hard drives.
- **Support of USB 3.0** is not an inherent improvement brought by UEFI, as this functionality is supported independently of UEFI.

---

### **Question 5:**
**Which of the following tries to detect and stop an attack?**

**Correct Answer:**  
**HIPS (Host-based Intrusion Prevention System)**

**Explanation:**  
- **HIPS** is designed to detect and prevent attacks by monitoring system behavior.
- **HIDS (Host-based Intrusion Detection System)** detects attacks but does not prevent them.
- **SOMA** and **RDE** are not relevant to attack prevention.

---

### **Question 6:**
**While going through the network log, Sarah, a network security administrator, noticed substantial outbound network traffic. Which activity did Sarah perform?**

**Correct Answer:**  
**IOC (Indicator of Compromise)**

**Explanation:**  
- **IOC** is used to identify malicious activity, such as abnormal outbound traffic, which might indicate a security breach or data exfiltration.
- **HTTP** and **Telnet** are network protocols, while **STIX** is a framework for sharing threat intelligence, not a type of log activity.

---

### **Question 7:**
**A machine where the operating system runs an application on top of an operating system is called _______.**

**Correct Answer:**  
**A virtual machine**

**Explanation:**  
- **Virtual machines** (VMs) allow multiple operating systems to run on a host system by using virtualization technology. This environment is useful for running applications in isolated environments.
- **Sandbox** is similar but generally used for security testing.
- **Quarantine** is used for isolating infected files or programs.

---

### **Question 8:**
**What additional measure should be enacted to increase the security on a computer network after secure boot, protective measures from attacks like antimalware, and intrusion detection systems are implemented in all the computers on the network?**

**Correct Answer:**  
**Implement hardening at endpoints with patch management and operating system safeguards**

**Explanation:**  
- **Endpoint hardening** involves implementing stronger security configurations, such as patch management, to prevent vulnerabilities. This measure strengthens existing security mechanisms.
- Disabling OS patch updates would reduce security, and disabling Wi-Fi connections is not always practical.
- Antimalware would already be in place as part of the base protection.

---

### **Question 9:**
**A learning management system application has been written in Python. While running the application code, the specific program or application that converts the program into machine language is called what?**

**Correct Answer:**  
**Compiler**

**Explanation:**  
- **Compilers** convert high-level code, such as Python, into machine language (binary code) so that the system can execute the program.
- **Application software** refers to software designed for end users, and **antimalware** is for protecting systems from malware.
- **Operating systems** manage hardware and software resources but do not perform the conversion of code into machine language.

---

### **Question 10:**
**Your manager has requested you to consider SecDevOps. Which of the following is a significant and key feature of using SecDevOps that can be considered for selecting this project's development model?**

**Correct Answer:**  
**Automation**

**Explanation:**  
- **Automation** is one of the key features of **SecDevOps**, integrating security into the development lifecycle and allowing for continuous testing and deployment.
- **Reuse of code** and **rigid process** do not capture the collaborative, iterative nature of SecDevOps.
- **Quarantine** refers to isolating threats, not relevant to SecDevOps.

---

### **Question 11:**
**You are looking to find new information on vulnerabilities like the attack that occurred. Which of the following actions would help achieve this objective?**

**Correct Answer:**  
**Checking the dark web**

**Explanation:**  
- The **dark web** can be a source of information about new vulnerabilities, exploits, and attack techniques not found on the surface web.
- **Surface web** and **green web** are not as likely to provide access to emerging threats.
- **TCP/IP protocol** does not provide access to vulnerability information.

---

### **Question 12:**
**Which of the following can be used to mitigate a limitation of public sharing centers in OSINT?**

**Correct Answer:**  
**AIS (Automated Indicator Sharing)**

**Explanation:**  
- **AIS** is a method used to automatically share threat indicators across organizations and agencies to improve Open Source Intelligence (OSINT).
- **HTTPS** is for secure communication, while **KRI** and **TTP** refer to risk indicators and attack patterns.

---

### **Question 13:**
**Ronald has been approached to develop a critical application for a finance company. The company requests that the project be completed in a few months, with a minimum version provided first. Which development process would be ideal?**

**Correct Answer:**  
**Ronald can employ an agile development model to meet the requirements with penetration testing done on the modules.**

**Explanation:**  
- **Agile development** focuses on iterative development, allowing a minimum viable product to be delivered quickly with additional functionalities added later.
- **Waterfall** is more rigid and would not be suitable for fast iteration.
- **SecDevOps** could be an option, but it focuses more on integrating security within DevOps.

---

### **Question 14:**
**Which of the following can denote the upper and lower bounds of network activity?**

**Correct Answer:**  
**KRI (Key Risk Indicator)**

**Explanation:**  
- **Key Risk Indicators (KRI)** measure thresholds of activity and can help indicate abnormal or malicious behavior.
- **OSI model** is a framework for network communication, not used for monitoring activity.
- **TTP** refers to **Tactics, Techniques, and Procedures** of attackers.
- **Threat maps** display known threat activity but do not define bounds.

---

### **Question 15:**
**What is the secure coding technique that organizes data within the database for minimum redundancy?**

**Correct Answer:**  
**Normalization**

**Explanation:**  
- **Normalization** is the process of structuring a database to reduce redundancy and improve data integrity.
- **Dead code** refers to parts of the code that are never executed.
- **Stored procedures** are precompiled SQL queries, and **code signing** refers to digitally signing code to verify its integrity.

---

Checking the **dark web** for new vulnerabilities is a task that should be approached with caution. Accessing the dark web for legitimate security research can yield valuable information, but it is important to follow **strict legal guidelines** and **best practices** to avoid legal, ethical, or security risks.

Here’s a **step-by-step guide** on how a security professional might safely and responsibly check the dark web for potential "new" vulnerabilities:

---

### **Step 1: Understand the Legal Implications**
Before accessing the dark web, it’s crucial to ensure that:
- **You have explicit permission** from your organization to access the dark web for research purposes.
- **Local laws** permit this type of research. Accessing certain content or participating in activities on the dark web might be illegal in your region.
- **Document your process** to prove you are conducting research ethically and lawfully.

---

### **Step 2: Install the TOR Browser**
To access the dark web safely, you will need the **TOR (The Onion Router) browser**. This browser allows you to navigate websites on the **.onion** domain, which are part of the dark web.
1. Go to the official **TOR Project website**: [https://www.torproject.org](https://www.torproject.org)
2. Download and install the **TOR browser**.
3. Launch the TOR browser. It will automatically connect to the TOR network, anonymizing your connection.

---

### **Step 3: Use a VPN for Extra Security**
While TOR helps anonymize your traffic, using a **Virtual Private Network (VPN)** adds an extra layer of security by masking your IP address:
1. Choose a **reputable VPN service** that does not log user activity.
2. Connect to a VPN **before** launching the TOR browser. This will ensure your IP is protected if TOR fails for any reason.

---

### **Step 4: Use Search Engines for the Dark Web**
There are search engines specifically designed for navigating dark web content. Popular dark web search engines include:
- **Ahmia** ([https://ahmia.fi](https://ahmia.fi)): A search engine for the TOR network.
- **DuckDuckGo** ([https://3g2upl4pq6kufc4m.onion](https://3g2upl4pq6kufc4m.onion)): A privacy-focused search engine available on TOR.

You can search for specific vulnerabilities, forums, or marketplaces where exploits and vulnerabilities are discussed. Use relevant search terms like:
- "Zero-day exploits"
- "New vulnerabilities"
- "Exploit databases"
- "Hacker forums"

---

### **Step 5: Explore Dark Web Forums and Marketplaces**
Security researchers often focus on dark web **forums** and **marketplaces** where threat actors discuss vulnerabilities and sell exploits:
1. Use the search engines mentioned above to find reputable **cybersecurity forums** on the dark web.
2. Look for forums where **security professionals** or **malware developers** discuss the latest vulnerabilities. These forums often require registration, so proceed with caution.
3. **Marketplaces** might offer exploit kits or sell zero-day vulnerabilities, but **do not purchase illegal content**. Instead, monitor discussions around new techniques and exploits.

---

### **Step 6: Look for Known Vulnerability and Exploit Databases**
There are known dark web websites where threat actors post information about new vulnerabilities. Look for:
- **Exploit databases** (both legitimate and underground).
- **Data dump sites** where attackers might leak stolen data or vulnerabilities.

Examples of relevant dark web sites (if available) will be listed on dark web search engines or forums.

---

### **Step 7: Analyze and Document Findings**
- Document everything you find during your research. Keep a detailed log of:
  - What forums or marketplaces you accessed.
  - Any relevant vulnerabilities or exploits discussed.
  - Any potential malware samples or indicators of compromise (IOCs) that could help in threat detection.

---

### **Step 8: Ensure Safety with Virtual Machines and Isolation**
It is important to isolate your research environment:
- Use a **virtual machine (VM)** or a **sandbox** environment to access the dark web. This will protect your main system from potential malware or attacks.
- Make sure to **snapshot** your virtual machine before conducting research so that you can revert it to a clean state afterward.

---

### **Step 9: Report Findings Through the Right Channels**
Once you have gathered relevant information:
1. **Report your findings** to your security team or management, especially if you identify a new vulnerability that could impact your organization.
2. If the vulnerability affects a third party, consider **responsible disclosure** by notifying the affected party or vendor.

---

### **Step 10: Stay Vigilant and Avoid Suspicious Links**
Dark web forums and sites can be filled with malicious links, so be cautious:
- **Avoid downloading files** unless you're in a secure, isolated environment.
- **Don’t click on suspicious links**. Always verify the authenticity of any site or file before interacting with it.

---

### **Bonus Tip: Automate Dark Web Monitoring (If Possible)**
If your organization allows, you can use specialized tools that monitor the dark web for discussions about your company’s software, infrastructure, or potential vulnerabilities:
- **Dark web threat intelligence services** (e.g., Recorded Future, DarkOwl) can monitor dark web activity for you and provide alerts.

---

### **Summary**
While searching the dark web can be a useful tool for security research, it must be done responsibly and carefully. Ensure you have:
- The right tools (TOR, VPN).
- A secure environment (VM, sandbox).
- Legal and organizational permission.
And always follow ethical guidelines when gathering information from these environments.
