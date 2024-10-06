# 24 September 2024 Reading
I finished module 2 this morning; however, I know that the quiz is going to ask
questions like I poured over and memorized every sentance. Maybe I should get
used to memorizing everything I read. The only path to that end is to start
doing my BoM memorization like I have wanted to but did not. I need to get my
mind to the point that I really do memorize everything after a 1 time through
the material. I used to be much better, but COVID 3x and Cancer left me scatter
brained. Many times, it feels like my mind is going in several directions at
once.


## Module 2
Page 56 (review and glossary of terms) VIP page. Most of this module was about
"frameworks" and "regulations."

**adversary tactics, techniques, and procedures (TTP)** A database of the behavior of threat actors and how they orchestrate and manage attacks.

**benchmark/secure configuration guides** Guidelines for configuring a device or software usually distributed by hardware manufacturers and software developers.

**Blue Team** A penetration testing team that monitors for Red Team attacks and shores up defenses as necessary.

## Module 3
Questions:

**01. Which of the following attacks targets the external software component that is a repository of both code and data?**

- Book: Page 83, Paragraph 4 (bullet point):
Dynamic-link library (DLL). A dynamic-link library (DLL) is a repository of both code and data that can be used by more than one program at the same time. For example, in the Windows operating systems, the Comdlg32.DLL performs common dialog box related functions. Attackers use a technique called DLL injection for inserting code into a running process through a DLL to cause a program to function in a different way than intended.

**02. Which of the following attacks is based on the principle that when a user is currently authenticated on a website and then loads another webpage, the new page inherits the identity and privileges of the first website?**

Sure! Here are descriptions for each of the other terms provided:

### 1. **SSFR (Server-Side Request Forgery)**
   **Description**: In a Server-Side Request Forgery (SSRF) attack, the attacker tricks a server into making unintended requests on behalf of itself. The attacker sends a request to the server, which then makes another request to an internal service or external URL that the attacker cannot directly access. The goal is often to access sensitive data or internal resources that are otherwise protected.

   **Key characteristic**: The attack leverages a server to send unauthorized requests to internal resources.
---
### 2. **DLLS (Dynamic Link Library Spoofing)**
   **Description**: This is not a standard security acronym, but if you meant **DLL Injection or Spoofing**, this type of attack involves the malicious insertion of a Dynamic Link Library (DLL) into a process. The attacker can inject malicious code via a fake or altered DLL that a legitimate application loads, potentially gaining control over the target application or executing arbitrary code in the context of the application.

   **Key characteristic**: Exploiting DLL loading mechanisms to execute malicious code.
---
### 3. **CSRF (Cross-Site Request Forgery)**
   **Description**: Cross-Site Request Forgery (CSRF) is a type of attack where an attacker tricks an authenticated user into sending requests to a web application in which the user is already authenticated. This can cause the web application to execute unintended actions, such as changing user details or making purchases.

   **Key characteristic**: Exploits the trust that a web application has in the user's browser, using the user’s credentials to perform malicious actions.
---
### 4. **DRCR (Data Relay Cross Repetition)**
   **Description**: DRCR does not correspond to a known or common security attack type. It may be a typo or a rarely used term in cybersecurity contexts. However, if this was meant to represent something specific, further clarification would be needed. 

   **Key characteristic**: Likely not a recognized term in cybersecurity.
---
In summary, CSRF is the attack that relies on a user’s authenticated session being exploited across different websites, while SSRF and DLL injection/spoofing target server-side or application-level vulnerabilities in different ways.


**03. Randall’s roommate is complaining to him about all of the software that came pre-installed on his new computer. He doesn’t want the software because it slows down the computer. What type of software is this?**

Here are descriptions for the terms you requested:

### 1. **PUP (Potentially Unwanted Program)**
   **Description**: A PUP is software that may not be inherently malicious but is often unwanted by the user. These programs can be bundled with legitimate software and get installed unknowingly. PUPs often display ads, alter browser settings, or perform other tasks that users may find intrusive. They typically don’t pose a significant security threat but can be an annoyance, degrade system performance, or even collect user data without consent.

   **Key characteristic**: Software that is installed without the user’s clear intention and can be disruptive or invasive.

---

### 2. **Keylogger**
   **Description**: A keylogger is a type of malware or software that records every keystroke a user makes on their keyboard. This data is then sent to the attacker, who can use it to steal sensitive information such as passwords, credit card numbers, or personal messages. Keyloggers can be hardware devices attached to a keyboard or software-based programs installed on a machine.

   **Key characteristic**: Captures and logs keystrokes to steal sensitive information like passwords and credentials.

---

### 3. **Bot**
   **Description**: In the context of cybersecurity, a **bot** refers to an automated program that performs tasks over the internet, often maliciously when part of a botnet. A botnet is a network of compromised computers that an attacker controls to perform coordinated attacks, such as Distributed Denial of Service (DDoS), spamming, or spreading malware. Bots can operate without the user’s knowledge and are often part of larger attack networks.

   **Key characteristic**: Automates tasks, potentially under malicious control, and can be part of a botnet.

---

### 4. **Spyware**
   **Description**: Spyware is malicious software designed to secretly monitor and collect information from a user's computer without their knowledge. Spyware can track browsing activity, record passwords, capture keystrokes (acting as a keylogger), and even gather personal or financial data. The collected data is typically sent back to the attacker for malicious purposes, such as identity theft or targeted advertising.

   **Key characteristic**: Covertly monitors user activity and collects sensitive information.

---

In summary:
- **PUPs** are annoying or intrusive programs installed without clear user consent.
- **Keyloggers** record and transmit keystrokes for stealing sensitive information.
- **Bots** automate tasks, sometimes maliciously, and can be part of a larger botnet.
- **Spyware** covertly collects data about the user’s activities for malicious purposes.

**04. Which of the following attacks is based on a website accepting user input without sanitizing it?**

Here are the descriptions of the terms you requested:

### 1. **SQLS (SQL Injection)** (I think this is the answer)
   **Description**: SQLS most likely refers to **SQL Injection (SQLi)**, a type of attack where an attacker manipulates a web application's SQL query by injecting malicious SQL code into input fields. The goal is to trick the database into executing unintended queries, which can result in data leaks, unauthorized access, or even total control of the database.

   **Key characteristic**: Exploits vulnerabilities in SQL queries to execute arbitrary code or access sensitive data in a database.

---

### 2. **SSXRS (Server-Side Cross-Site Request Forgery)** 
   **Description**: SSXRS is not a commonly recognized term in cybersecurity. However, it could be a reference to **Server-Side Request Forgery (SSRF)** or a combination of **CSRF** and **XSS** principles. If it refers to SSRF, the attacker exploits a vulnerable server to send unauthorized requests on behalf of that server. There is no well-known attack specifically named SSXRS.

   **Key characteristic**: Likely an error or an uncommon term in cybersecurity, but SSRF refers to manipulating a server to make unintended requests to internal or external resources.

---

### 3. **RSS (Really Simple Syndication)**
   **Description**: RSS is a web feed format that allows users and applications to access updates to websites in a standardized format. It is not inherently related to cybersecurity but is used for distributing content, like blog posts or news articles, from one site to multiple users or platforms.

   **Key characteristic**: A technology used to syndicate web content, not related to security attacks.

---

### 4. **XSS (Cross-Site Scripting)**
   **Description**: Cross-Site Scripting (XSS) is a type of security vulnerability found in web applications. XSS allows attackers to inject malicious scripts into web pages that are viewed by other users. When the users visit the infected page, the malicious scripts are executed in their browsers, potentially allowing the attacker to steal session cookies, capture user inputs, or perform actions on the users' behalf.

   **Key characteristic**: Injects malicious scripts into web pages, executed by users' browsers, leading to potential data theft or session hijacking.

---

### Summary:
- **SQLS** refers to **SQL Injection**, a database attack that manipulates queries.
- **SSXRS** is likely a mistaken term but may hint toward **SSRF** or related vulnerabilities.
- **RSS** is a web feed format used to syndicate content, not a cybersecurity concept.
- **XSS** is **Cross-Site Scripting**, where malicious scripts are injected into websites and executed by users' browsers.

**05. Which of the following is NOT a means by which a bot communicates with a C&C device?**

### Explanation:
While bots can use various creative means to communicate with their Command and Control (C&C) servers, such as:

- **Signing in to a third-party website**: Bots may connect to forums, social media platforms, or legitimate websites where commands are hidden in plain sight.
- **Command sent through Twitter posts**: Bots can be designed to follow specific Twitter accounts and extract commands from posts.
- **Signing in to a website the bot herder operates**: Bots often connect directly to a website controlled by the attacker to receive commands.

Using **email** as a communication method is uncommon and inefficient for botnet C&C communication due to delays and a lack of real-time interaction, making it an impractical choice for controlling bots.

A **Command and Control (C&C or C2) device** refers to the server or infrastructure that attackers use to communicate with and control compromised systems, typically part of a **botnet** or other types of malware operations. The C&C server acts as the central point from which the attacker issues commands to infected devices and receives data, such as stolen credentials or other sensitive information.

### Key Components and Functionality:

1. **Command Distribution**: 
   - The C&C server sends commands to the compromised devices (bots) to perform specific actions like launching Distributed Denial of Service (DDoS) attacks, stealing data, spreading malware, or mining cryptocurrency.
   - These commands can be sent using various methods such as HTTP requests, encrypted communications, or even social media (like Twitter or third-party websites).

2. **Control Infrastructure**:
   - The C&C infrastructure can be centralized (one C&C server controlling all bots) or decentralized (a peer-to-peer network where each bot communicates with others).
   - In a centralized model, if the C&C server is taken down, the entire botnet may be crippled, making it a key target for law enforcement and security researchers.
   - In a decentralized model, bots can continue to function without a single point of failure.

3. **Stealth and Evasion**:
   - C&C servers often use techniques to hide their true location, such as proxy servers, encryption, or the Tor network, to avoid detection by security systems.
   - Attackers may frequently change the C&C server (known as "fast flux" or using a Domain Generation Algorithm, or DGA) to evade takedown efforts by law enforcement or security researchers.

4. **Data Collection**:
   - In addition to issuing commands, the C&C device also collects data from compromised machines. This can include stolen credentials, keystrokes from keyloggers, screenshots, or other sensitive information.
   - The botmaster (person controlling the C&C server) can then use or sell this data.

### Communication Methods:
- **HTTP/HTTPS**: Bots often communicate with C&C servers over standard web protocols to blend in with normal internet traffic.
- **IRC (Internet Relay Chat)**: Historically, botnets often used IRC channels to communicate commands.
- **P2P (Peer-to-Peer)**: Some advanced botnets use decentralized P2P communication, where each bot can act as both a client and server, making the network more resilient.
- **Social Media & Other Websites**: Bots can receive commands through hidden messages in public platforms like Twitter, forums, or even images (using techniques like steganography).

### Example of C&C Attack:
1. **Initial Infection**: The attacker infects a system with malware, which connects back to a C&C server.
2. **Command Execution**: The infected system receives commands from the C&C device, such as sending spam emails or participating in a DDoS attack.
3. **Data Exfiltration**: If the malware is designed for espionage or theft, it will send collected data (such as passwords or personal files) back to the C&C server.

### Summary:
A C&C device is critical for coordinating attacks in malware campaigns, botnets, or other cybercriminal activities. It enables the attacker to control compromised systems remotely, issue commands, collect data, and manage their malicious operations. The C&C infrastructure is often a key target for cybersecurity efforts to disrupt these attacks.

**06. What type of attack occurs when the threat actor snoops and intercepts the digital data transmitted by the computer and resends that data, impersonating the user?**

The correct answer is **Replay**.

### Explanation:
A **Replay attack** occurs when a threat actor intercepts and captures data during transmission (such as login credentials or session tokens) and then later resends that data to impersonate the user. In this type of attack, the attacker does not necessarily need to decrypt the data but instead captures it and "replays" it to trick the system into thinking it is legitimate.

Here are the descriptions of the other choices:

- **Trojan**: A type of malware that disguises itself as legitimate software but performs malicious actions once executed.
- **Buffer overflow**: An attack where a program writes more data to a buffer than it can hold, leading to crashes or execution of malicious code.
- **Device driver manipulation**: Involves modifying or exploiting device drivers (software that controls hardware components) to perform malicious actions, often allowing attackers to gain kernel-level privileges.

Thus, **Replay** is the correct answer for an attack where intercepted data is retransmitted to impersonate the user.

**7. An attacker has changed the value of a variable used when copying files from one cloud server to a local drive. What is the most likely motive behind the attack?**

Here’s a breakdown of each of the scenarios you described, along with explanations:

### 1. **The attacker is using a buffer overflow to initiate an integer overflow attack that can allow access to private data on the local drive.**

   **Description**: In this case, the attacker uses a **buffer overflow** vulnerability to corrupt memory in such a way that it causes an **integer overflow**. Integer overflows occur when arithmetic operations exceed the maximum size that an integer data type can hold, resulting in wrapping or incorrect values. If an attacker exploits this condition, they may manipulate pointers or array indices to access unintended areas of memory, such as private data on the local drive.

   **Key point**: A **buffer overflow** leads to an **integer overflow**, allowing unauthorized access to sensitive data stored on the drive.

---

### 2. **The attacker is using an integer overflow attack that will change the state of the local drive's memory.**

   **Description**: An **integer overflow attack** can result in incorrect calculations or memory access. If the attacker can manipulate the integer values that control memory allocation or pointer arithmetic, they could potentially modify memory on the local drive. This could allow them to change or corrupt critical data structures, leading to various consequences, such as application crashes or privilege escalation.

   **Key point**: The **integer overflow** allows the attacker to manipulate memory allocations or addresses, changing the memory state of the local drive.

---

### 3. **The attacker is using a buffer overflow to initiate an integer overflow attack that will give them access to the machine's OS code.**

   **Description**: In this scenario, the attacker exploits a **buffer overflow** vulnerability to cause an **integer overflow**, which then gives them access to the machine’s **operating system (OS) code**. By manipulating memory addresses or control flow through the integer overflow, the attacker could potentially overwrite critical parts of the OS, allowing them to inject malicious code or access sensitive areas of the system.

   **Key point**: A **buffer overflow** is used to trigger an **integer overflow**, leading to unauthorized access to or manipulation of the machine's OS.

---

### 4. **The attacker is using an integer overflow attack to initiate a buffer overflow that can allow them to take over the machine.**

   **Description**: In this case, the attacker uses an **integer overflow** to initiate a **buffer overflow**. For example, an integer overflow could cause improper memory allocation (allocating too little memory for a buffer), leading to a buffer overflow. Once the buffer overflow is triggered, the attacker could inject malicious code or overwrite return addresses, allowing them to take control of the machine.

   **Key point**: The **integer overflow** causes a **buffer overflow**, which allows the attacker to execute arbitrary code and potentially take over the machine.

---

### Summary of the Attacks:
- **Buffer overflow**: Occurs when more data is written to a buffer than it can hold, leading to memory corruption. It can allow an attacker to inject malicious code or control program execution.
- **Integer overflow**: Happens when an arithmetic operation results in a number larger than the maximum value the data type can hold, causing unintended behavior or memory corruption.

In all cases, these vulnerabilities can lead to serious security risks such as unauthorized access, memory corruption, or complete system takeover, depending on how the attacker manipulates the overflow conditions.

**08. Shanise is an IT security professional for a large private bank. She got an alert that the bank website received a funds transfer request that was correctly credentialed but flagged as being out of the account owner's usual pattern. If the alert is correct, what type of attack has likely occurred?**

Here are the descriptions of each attack type:

### 1. **CSRF Attack (Cross-Site Request Forgery)**
   **Description**: A CSRF attack occurs when a malicious website, email, or script causes a user’s browser to perform an unwanted action on a trusted site where the user is authenticated. The attacker tricks the user into making unintended requests (such as changing account details, making a purchase, or performing admin actions) without their knowledge, using the user’s credentials.
   
   **Key characteristics**:
   - Exploits a user’s authenticated session with a website.
   - The attacker tricks the user into performing actions unknowingly on the trusted site.
   - Mitigated by implementing anti-CSRF tokens, SameSite cookies, or checking the origin of requests.

---

### 2. **SQL Injection**
   **Description**: SQL Injection (SQLi) is a type of attack where an attacker inserts malicious SQL code into an input field or URL parameter that is passed to a web application’s database. If the input isn’t properly sanitized, the malicious SQL code is executed by the database, which can result in unauthorized data access, data modification, or even full control over the database.
   
   **Key characteristics**:
   - Exploits vulnerabilities in SQL queries.
   - Can lead to unauthorized access to sensitive data, database manipulation, or data breaches.
   - Prevented by input validation, parameterized queries, and using ORM (Object Relational Mapping) frameworks.

---

### 3. **Replay Attack**
   **Description**: In a replay attack, an attacker intercepts and captures valid communication between two parties (such as login credentials or session tokens) and retransmits the same data at a later time to impersonate one of the parties. The attacker does not modify the intercepted data but reuses it to trick the system into performing the same action as if it were legitimate.
   
   **Key characteristics**:
   - The attacker reuses intercepted data to impersonate the user.
   - Common in weakly secured systems where tokens or timestamps are not properly used.
   - Mitigated by using nonces (unique, one-time numbers) or timestamp mechanisms to ensure data cannot be reused.

---

### 4. **XSS Attack (Cross-Site Scripting)**
   **Description**: XSS is a vulnerability that allows an attacker to inject malicious scripts into web pages viewed by other users. The injected scripts are executed in the context of the victim’s browser, allowing the attacker to steal session cookies, capture input data, or execute malicious code. There are three main types of XSS: **Stored XSS**, **Reflected XSS**, and **DOM-based XSS**.
   
   **Key characteristics**:
   - Injects malicious scripts into web pages that are executed by the victim’s browser.
   - Can be used to steal session data, hijack accounts, or perform malicious actions.
   - Mitigated by properly sanitizing and validating user input, escaping output, and using Content Security Policy (CSP).

---

### Summary:
- **CSRF**: Exploits user sessions and trust in a website, causing unintended actions.
- **SQL Injection**: Targets databases by injecting malicious SQL code to manipulate or access data.
- **Replay Attack**: Reuses intercepted communication to impersonate a user without modifying the data.
- **XSS**: Injects malicious scripts into web pages, which are then executed by other users’ browsers.

**09.  A few computers at a high-security software firm location have been compromised. The threat actor took user videos, confidential information like bank account IDs and passwords, email IDs and passwords, and computer screenshots. These confidential data have been shared every three hours from the computers to the threat actor. Which of the following is correct, based on the evaluation of the above observation?**

Here is a description of all four options you provided:

### 1. **A PUP pretends to perform natural activities while also performing malicious activities.**
   **Description**: This option describes the behavior of **Trojan horse** malware rather than a PUP. A **Trojan** disguises itself as legitimate software or performs normal-looking functions while secretly executing malicious actions in the background. For example, a Trojan may appear to be a useful application while it steals data, installs other malware, or opens a backdoor for attackers.

   **Key characteristic**: It masquerades as legitimate software but performs hidden, malicious activities.

---

### 2. **A PUP gives access to the computer, program, or a service, circumventing the system's normal security protections.**
   **Description**: This option describes the behavior of **exploits** or **backdoors** rather than a PUP. **Backdoor** software is often malicious, installed to bypass normal authentication processes and security protections to give an attacker remote access to a system. This type of software can be used to control or compromise the target system without the user’s knowledge.

   **Key characteristic**: Provides unauthorized access to a system or network, often bypassing security measures.

---

### 3. **A PUP gives the threat agent remote access to the user's device using specially configured communication protocols.**
   **Description**: This option describes a **Remote Access Trojan (RAT)** or **remote administration tool**, which is malware designed to allow remote control of an infected system. RATs can give attackers full access to the victim's system, allowing them to steal information, modify files, and even use the system for malicious activities like launching further attacks.

   **Key characteristic**: Grants remote access to a device, often controlled by an attacker.

---

### 4. **A PUP interferes and obstructs the user with web browsing and pop-up windows.**
   **Description**: This is the correct description of a **Potentially Unwanted Program (PUP)**. PUPs often bundle with other legitimate software and are not strictly classified as malware. However, they interfere with the user experience by generating ads, redirecting web searches, showing pop-ups, or changing browser settings. PUPs are often installed without the user's full understanding and can be difficult to remove.

   **Key characteristic**: Interrupts normal web browsing with pop-ups, ads, and browser redirection.

---

### Summary:
- **Option 1** describes a **Trojan** that disguises itself as a normal program but secretly performs malicious activities.
- **Option 2** describes a **backdoor** or exploit, giving unauthorized access to systems by bypassing security.
- **Option 3** describes a **Remote Access Trojan (RAT)** that allows remote control of a victim's machine.
- **Option 4** correctly describes a **PUP**, which interferes with user activities through ads, pop-ups, and unwanted changes to browser settings.


**11. Which type of malware can hide its agenda inside other processes, making it undetectable, and what is it usually used for?**

### Explanation:
A **rootkit** is a type of malware that is designed to remain hidden by integrating itself deeply into the operating system (OS), often at the kernel level or in undocumented parts of the OS. This allows it to evade detection by hiding its presence and the presence of other malicious activities. Rootkits can alter system processes, modify files, and make system changes without being detected by antivirus software or system monitoring tools. They are often used to maintain persistent access to a compromised system while concealing the attacker’s activities.

### Key characteristics:
- **Hides its presence** by embedding itself in the lower layers of the OS.
- **Undetectable by standard security software** because it manipulates core system processes.
- **Used for long-term control**, allowing attackers to maintain access to the system undetected.

---

### Descriptions of the other options:
- **RAT (Remote Access Trojan)**: A RAT gives an attacker unauthorized remote access to a user's computer, enabling full control over the system. It’s typically used to steal data or manipulate the system remotely, but it doesn’t have the deep system-hiding characteristics of a rootkit.
  
- **Trojan**: A Trojan disguises itself as legitimate software while secretly performing malicious actions. It doesn’t inherently have the ability to hide its presence inside other processes like a rootkit.
  
- **Backdoor**: A backdoor is software or malware that allows bypassing normal security protections to give an attacker unauthorized access to a system or program. While it provides access, it doesn’t focus on concealing its activity at the same depth as a rootkit.

**11. Which type of malware can hide its agenda inside other processes, making it undetectable, and what is it usually used for?**

### Explanation:
A **rootkit** is a type of malware designed to hide its presence and the presence of other malicious activities by embedding itself deep within the operating system (often at the kernel level). Rootkits can modify system processes and hide files, making them extremely difficult to detect using traditional antivirus or security tools. Rootkits are often used to maintain persistent, undetectable access to a compromised system, allowing attackers to control the system, steal data, or facilitate other attacks without being detected.

### Why the other options are less correct:
- **RAT (Remote Access Trojan)**: While a RAT allows remote control over an infected system, it does not typically hide itself within other processes at the same depth as a rootkit.
  
- **Trojan**: A Trojan disguises itself as legitimate software but doesn't have the deep-level hiding capabilities of a rootkit. It may perform malicious actions, but it usually isn't designed to be as undetectable as a rootkit.
  
- **Backdoor**: A backdoor provides unauthorized access to a system, bypassing normal security protections. While it can be a stealthy entry point, it typically doesn't hide itself in system processes the way a rootkit does.

Thus, **rootkits** are specifically known for their ability to hide within the system, making them nearly invisible to standard detection methods.

**12. Kia recently noticed that when she browses her favorite online shopping site, she is immediately redirected to a competitor's site. What is happening here, and what is the best option for Kia to fix this situation?**

The correct answer is:

**Kia must uninstall the toolbar software and the accompanying components she has recently installed on her browser.**

### Explanation:
The behavior Kia is experiencing — being redirected to a competitor's site — is a common symptom of **adware** or a **potentially unwanted program (PUP)**, often installed alongside toolbar software or browser extensions. These programs modify browser settings, such as search engines or homepage defaults, and cause redirections to sites that generate revenue for the software developers.

### Steps to Fix:
- **Uninstall the unwanted toolbar or browser extension** that was likely installed recently.
- **Clear the browser’s settings** to remove any lingering changes the adware or toolbar might have made (such as homepage and search engine defaults).
- **Run a good anti-malware scan** to ensure no other unwanted software remains on the system.

---

### Why the other options are less appropriate:
- **Kia has accidentally installed a virus**: While possible, the symptoms are more indicative of adware or PUP rather than a virus.
- **Kia has installed spyware**: Spyware collects data without the user's knowledge. While spyware can cause unusual behavior, being redirected to competitor websites is more commonly linked to adware or PUPs.
- **Reinstalling the operating system**: This is an extreme measure and unnecessary for what seems to be a minor issue like a toolbar or PUP causing redirection.

Thus, **uninstalling the toolbar and its components** is the most direct and effective solution.

**13. Juan, a cybersecurity expert, has been hired by an organization whose networks have been compromised by a malware attack. After analyzing the network systems, Juan submits a report to the company mentioning that the devices are infected with malware that uses a split infection technique on files.**

### Explanation:
A **virus** is a type of malware that can use a variety of infection techniques, including **split infection**, to compromise files. A **split infection** involves breaking malicious code into pieces and injecting those pieces into different locations within a file. Some parts of the code may be placed in the beginning, some in the middle, and others at the end of the file, making it more difficult to detect the virus using signature-based detection methods.

### Why the other options are less appropriate:
- **RAT (Remote Access Trojan)**: RATs provide remote access and control over a compromised system but do not typically use a split infection technique to hide in files.
- **Spyware**: Spyware is designed to secretly gather user information without their knowledge, but it doesn’t use split infection techniques to compromise files.
- **Cryptomalware**: Cryptomalware is used to encrypt files and hold them for ransom (ransomware), but it does not split and hide code fragments within infected files.

Thus, Juan is likely reporting a **virus** infection, as this type of malware is known to employ split infection techniques to spread and avoid detection.

**Split infection** is a technique used by certain types of **viruses** or **malware** to make detection and removal more difficult. In a split infection, the malicious code is not placed in one continuous section of a file. Instead, the virus splits its code into several pieces and distributes them throughout different parts of the infected file, sometimes even embedding itself across multiple files or sections.

### How Split Infection Works:
1. **Breaking the Code**: The virus code is divided into several segments.
   
2. **Scattering**: These segments are injected into various parts of a file (or multiple files), such as the beginning, middle, and end, or even across several different files in the system.
   
3. **Reassembly**: When the infected file or program is executed, the virus pieces reassemble themselves in memory to execute the malicious payload.

### Why Split Infection is Used:
- **Evasion of Detection**: Traditional antivirus programs scan files looking for known signatures (patterns of malicious code). By splitting the code into fragments, the virus can avoid matching common signatures, making it harder to detect.
  
- **Obfuscation**: Splitting the infection helps to obfuscate (hide) the presence of the virus, as it doesn’t appear as a complete, recognizable malicious file.
  
- **Resilience**: If some pieces of the virus code are detected and removed, the remaining parts can still function or reassemble themselves, maintaining the infection.

### Example:
Imagine a virus that splits its code into three parts. Part 1 might be placed at the start of an executable file, part 2 might be hidden in the middle of a legitimate program file, and part 3 might be inserted into the end of another file. When any of these files are run, the virus pieces come together and execute their malicious actions.

### Consequences:
- **Difficult to Detect**: This technique makes the malware harder to detect using signature-based scanning tools.
- **Harder to Remove**: Even if one part of the virus is found and removed, the remaining parts might still be able to reassemble and execute, keeping the system infected.

### Summary:
A **split infection** is a sophisticated malware technique where the virus divides its code into fragments and hides them across different parts of a file (or multiple files), evading detection and making removal more challenging.

**14. Which of the following is a subset of artificial intelligence?**

### Explanation:
**Machine learning (ML)** is a subset of **artificial intelligence (AI)**. AI refers to the broad concept of machines or systems simulating human intelligence to perform tasks such as problem-solving, decision-making, or pattern recognition. Machine learning, as a subset, focuses specifically on the ability of machines to learn from data without being explicitly programmed. ML algorithms are trained on data to identify patterns and make predictions or decisions.

### Why the other options are less appropriate:
- **Artificial intelligence algorithm**: This is not a subset of AI but rather a component or method used within AI systems to solve specific problems.
- **Machine intelligence**: This is a broader term that can be synonymous with AI but is not a subset.
- **Data science**: This is a field that focuses on extracting insights from data and overlaps with AI but is not a subset of AI. Data science uses AI and machine learning as tools for analyzing and interpreting data.

Thus, **machine learning** is the correct answer as it directly falls under the umbrella of AI.

**15. Ian, a systems administrator, was checking systems on Monday morning when he noticed several alarms on his screen. He found many of the normal settings in his computer and programs changed, but he was sure no one had physically entered his room since Friday. If Ian did not make these changes, which of the events below is the most likely reason for the anomalies?**

The correct answer is:

**A backdoor was installed previously and utilized over the weekend to access the computer and the programs.**

### Explanation:
A **backdoor** is a type of malware or method that allows unauthorized access to a system, bypassing normal authentication mechanisms. Once installed, attackers can remotely access the system at any time, including during periods when the legitimate user is not present. Since Ian found that settings had been changed without physical access and no one had entered his room, the most likely explanation is that a backdoor was used to access and modify the system over the weekend.

### Why the other options are less likely:
- **Power outage**: While a power outage could reset some system settings, it's unlikely to cause significant changes to settings in both the computer and its programs, and it would not trigger alarms.
- **Penetration test**: If a security administrator ran a penetration test, they should have informed the necessary personnel, and this would not explain the specific changes to the settings and alarms triggered.
- **Firewall scan**: A firewall scan is unlikely to cause system or program settings to change or trigger alarms unless there was some exploit, but the scenario provided does not indicate this.

Thus, the most likely reason for the anomalies is that a **backdoor** was used to access the system remotely and make changes.