# Table of Contents
X. -[Threat Modeling](threat-modeling)
    -[Infosec Scene](#infosec-scene)
      -a. [Security Hygiene](#security-hygiene)
      -b. [Make-Belief Boogie-Man](#make-belief-boogie-man)
---

## Threat Modeling

### What is Threat Modeling?
Threat modeling is identifying and communicating information about the threats that may impact a system or network. Then defining countermeasures to prevent or mitigate the effects of threats to the system. 

The following question framework can help to organize threat modeling:

- **What are we working on?**  
  We should assess where data flows in a system, identify the boundaries that it crosses, and the technology used.
- **What can go wrong?**  
  Question every possibility of exploiting the hand-offs.
- **What are we going to do about it?**  
  Design defenses against each exploit.
- **Did we do a good job?**  
  We should reflect back on the process, review it, and remind that the work is never really done. We can always make an improvement.

The earlier we identify the threats, the more efficiently we can find solutions to thwart the attack vectors.

### HOW CAN WE DO THE THREAT MODEL PROCESS?
- **Scope your work**  
  We can always draw diagrams, data flow diagrams to identify entry points to see where an attacker could interact with the application. By identifying trust levels is a good way of ensuring the access rights that the application will grant to external entities. 
  
- **Determine threats**  
  The “STRIDE” methodology is frequently used in threat modeling. The goal is to categorize and identify potential threat targets from the attacker’s perspective. This includes a full breakdown of processes, data stores, data flows, and trust boundaries. 

- **Determine countermeasures and mitigation**  
  These countermeasures can be identified using threat countermeasure mapping lists. There are many approaches that exist, and an organization should choose which one will work for them. To choose a convenient approach, it is suitable to consider the likelihood of attack, damage from the attack, complexity, or cost of fix factors. Further, the risk mitigation strategy should evaluate how these threats will impact the business. Then the following options need to be addressed regarding the risk:

  - **Accept**: Decide that the business impact is acceptable, and document who has chosen to accept the risk.
  - **Eliminate**: Remove components that make the vulnerability possible.
  - **Mitigate**: Add checks or controls that reduce the risk impact or the chances of its occurrence.
  - **Transfer**: Transfer risk to an insurer or customer.

- **Assess your work**  
  Finally, we should determine whether we’ve done the work. Are there records showing a diagram, a threat list, and a control list? 

### Threat Modeling Tools:
A simple use of a whiteboard is enough to brainstorm ideas and methods to record threats and mitigations. But the following tools are used in the CMS modeling team to communicate within the team and record ideas and information: 
- Mural (for drawing DFD diagrams)
- CMS Confluence (for recording threats)
- Zoom (for team collaboration)
- YouTube (for additional training)
- OWASP Threat Dragon
- Microsoft Threat Modeling Tool
- IriusRisk
- ThreatModeler
- Devici

### Benefits of Threat Modeling:
- Detecting problems early in the software development life cycle (SDLC)
- Identifying system security requirements 
- Creating a structured plan to address both system requirements and deficiencies
- Evaluating attacks on CMS systems teams might not have considered, even security issues unique to your system
- Staying one step ahead of attackers
- Getting inside the minds of threat agents and their motivations, skills, and capabilities 
- Serving as a resource for CMS Penetration Testing and Contingency Planning activities

### References
- CMS Threat Modeling Handbook : CMS Threat Modeling Handbook | CMS Information Security & Privacy Group
- Threat Model and Security Considerations: RFC 6819 - OAuth 2.0 Threat Model and Security Considerations (ietf.org)
- Braiterman et al 2020: Threat modeling manifesto
- Shostack 2022: Welcome to the World's Shortest Threat Modeling Course (12 parts, about 15 min total, audio is enough for all except video 7 "Data flow diagrams")
- OWASP CheatSheets Series Team 2021: Threat Modeling Cheat Sheet

---

## Infosec Scene

### EP 23: VLADIMIR LEVIN

This episode is about in the early 1990s digital banking emerged with traditional bank robberies began with internet networks like SprintNet (formally known as Telenet).  This is a publicly available network using the X.25 protocol. (X.25 is an ITU-T standard protocol suite for packet-switched data communication in wide area networks (WAN), allows multiple logical channels to use the same physical line. It is used for networks for ATMs and credit card verification.)
The hacker magazine Phrack published a list of Citibank's network nodes in 1993, providing a gateway for two Russian hackers to infiltrate Citibank's systems. Phrack is the longest-running online magazine for hacking. Citibank's SprintNet nodes, including access details. They introduced new methods of online bank robbery. 
Russian hackers accidentally found an open system due to a user not logged out properly. The hacker got access to the username and password. Once the hacker knew one password, they hacked all 363 Citibank passwords and gained access to Citibank devices.
They got access to bank accounts, owner details, account numbers, money transaction details, and where the money went. How to connect usernames and passwords and how to join accounts. 
Citibank IT staff noticed this and triggered an alarm. Then they identified the unauthorized money transactions, monitored the system, and froze the account. After several attempts, the FBI was able to catch the person who went to withdraw money from the bank. They arrested the main hacker involved, seized the computers that were used to do this, and arrested four members of this gang.
This story highlights the importance of robust cybersecurity measures and vigilance in the digital banking era to stay safe from such threats.  

This episode emphasizes the safety of the digital banking world. By following the below tips, we can significantly reduce the risk of falling victim to digital banking fraud: 
- Use Strong, Unique Passwords
- Enable Two-Factor Authentication (2FA)
- Monitor Your Accounts Regularly
- Be Cautious with Public Wi-Fi
- Keep Software Updated
- Beware of Phishing Attempts
- Log Out After Use
- Secure Your Devices
- Educate Yourself

---

### Security Hygiene

#### a) Security Hygiene for Every Company
- Limit access to sensitive data based according to job roles and implement the principle of access control. 
- The company should conduct regular security audits and vulnerability assessments to identify and address security gaps. 
- Encrypt data in companies to prevent information leaks and mitigate the cost of its impact. 
- Patch management: Applying updates to software, drivers, and firmware to protect against vulnerabilities.
- Introduce an incident response plan. To regularly update incidents to quickly address security concerns.
- Regular employee training.
- Use Multi-Factor Authentication (MFA).
- Implement physical security measures like key cards and biometric access for critical areas.
- Regularly Review and Update Security Policies.

#### b) Security Hygiene for Dear Joe
- Joe should always use strong, unique passwords and avoid reusing the same password across different accounts.
- He should enable Two-Factor Authentication (2FA) to add an extra layer of security; this can be any form of verification. 
- Regular software updates can keep Joe’s computer operating system, applications, and secure the software. 
- Joe should always be suspicious when clicking links or downloading attachments from unknown sources. Always verify the sender's identity before sharing personal information. 
- Joe should have regular backups on external hardware or cloud services. 
- Using antivirus and anti-malware software is important to detect and remove threats. 
- Joe should not use public Wi-Fi connections for sensitive transactions and should secure his own Wi-Fi networks using a strong password. 
- It is safe to always practice avoiding untrusted websites and downloading software from unknown sources. Joe should check the web address before doing any of this. 
- Joe should remember to log out of accounts, especially on shared and public computers. 
- It’s better to stay informed about security threats and educate yourself. 

---

### c) Make-Belief Boogie-Man

#### Company: Aurora
#### Business: An online Jewelry Store Specializing in Semi-Precious Stone Jewelry
#### Planning to Extend a Physical Store: Currently in Online Trading. This company secures online payment processing for the E-commerce platform. 

**(1) What are we working on?**
- **Our Assets**
  - **Crown Jewels**: 
    - Personal / Financial data - Customer details, Payment card details, Purchase history, Personal identification information, Personal preferences.
    - Payment Gateway system – System that processes transactions between customer and Aurora (e.g., PayPal).
    - Reputation – The company’s brand and reputation. 
    - Internal networks – Employee workstations, internal databases, email servers, file servers. 
    - Employee credentials - Access to company systems.

- **Draw a diagram of the company systems.**

- **Customer is the king.**  
  Customer should trust that their transaction is secured. And if they have any issues, it can be solved quickly. Also, the payment gateway should be 100% trustworthy. And there should be a cash return policy if the customer is not satisfied with the product and service. 

**(2) What can go wrong?**

- **Threat Models: STRIDE Analysis**
  - **S**POOFING: Attackers spoof customer credentials to make unauthorized transactions. 
  - **T**AMPERING: Alter transaction data between customer and business.
  - **R**EPUTATION: Leakage of customer financial data.
  - **I**NFORMATION DISCLOSURE: Leakage of customer financial data.
  - **D**ENIAL OF SERVICE: An attacker can overwhelm the payment gateway, also attacks to disrupt the online website.
  - **E**LEVATION OF PRIVILEGE: Attacker gains administrative access to the payment gateways.

- **Prioritized Risks**
  - **High Expected Value Risks**:
    - Leakage of customer financial data could result in penalties and loss of business.
    - Gaining administrative control could allow an attacker to manipulate transactions and steal funds.
    - Phishing attacks to trick users into revealing their login credentials. 
    - Reputation damage and legal issues related to sustainability claims or product quality.

- **Targeted Threat Actors**
  - **Hackers**: Motivated by financial gain.
  - **Competitors**: Attempt to sabotage Aurora company operations.

- **Business Continuity Considerations**
  - **Trust Preservation**: Customer trust is crucial. Even a minor breach could cause significant reputation damage where customers will doubt the service and security.
  - **Competitive Losses**: Losing out to competitors and negative word of mouth can lead to business loss.
  - **Post-Breach Communication**: After a breach, it is important to communicate improvements and implementations of security measures.

**(3) What are we going to do about it?**

- **Transparency and Communication**: As a company, it is important to be transparent enough with all parties involved and be the first source to break the news.
- **Comprehensive Attack Surface Analysis**: Scanning the entire network for vulnerabilities, including third-party or adjacent networks.
- **Vulnerability Identification**: Identify exploitable vulnerabilities and misconfigurations. Check potential entry points, including attack vectors that can bypass antivirus, firewall, or other security defenses.
- **Layered Security Controls**: Strengthen layers of defense, such as network security, endpoint security, and access controls.
- **Employee Training**: Increase security awareness among employees, enabling them to make informed decisions in protecting sensitive information.
- **Regular Testing**: Conduct application testing, penetration testing, vulnerability assessments, and social engineering scenarios from an attacker’s perspective to identify and patch vulnerabilities before they result in a data breach.
- **Strong Authentication Measures**: Use multifactor authentication and strong passwords to strengthen the protection of personal data and personally identifiable information (PII) to prevent identity theft.

**(4) Did we do a good enough job?**
- **Regular Security Audits**: Third-party audits and assessments.
- **Continuous Threat Modeling**: Regular threat models to account for changes in the threat landscape and company infrastructure. 
- **Ongoing Employee Training**: Educate employees about company cyber policies. 
- **Post-Breach Analysis**: After any security breach, perform an analysis and understanding of what went wrong and how to improve. 

### References
- [Guide to Business Continuity Planning](https://silentbreach.com/BlogArticles/guide-to-business-continuity-planning/)
- [Data Breach Prevention: 5 Ways Attack Surface Management Helps Mitigate the Risks of Costly Data Breaches](https://www.ibm.com/blog/5-ways-attack-surface-management-helps-mitigate-risks-data-breaches/)
- [Analyzing Company Reputation After a Data Breach](https://www.varonis.com/blog/company-reputation-after-a-data-breach)
