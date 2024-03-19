## Pre-engagement meeting scenario

### 1 - Presentation of Fenrir.pro and its auditor(s)

- Fenrir.pro started as a project of Jeremie Amsellem's auto-entreprise, the website was created in 2018 and it was mainly one consultant + some freelancers or students
- We did Pentest (mainly), Code Audit (sometimes) + Incident Response (more rarely)
- It became a company in May 2023 and we started doing "in-house" training, on ethical hacking at first
- Our main activity sector is the medical and medical/scientific research
  - We collaborate regularly with two very big research and learning campuses in Paris
  - We audited 20+ companies with innovatives projects (software or hardware) related to medical
- Today, fenrir.pro is a company, with one lead auditor/director + some employees

#### Personal Achievements

- Ex Full Stack dev in the medical field (IoT/Android Apps/Back-end) -> ingress of patient data via IoT objects and an Android app to a back-end
- Works with Epitech, Epita, Jedha, ESGi as a freelance cybersecurity teacher in my time out of fenrir.pro
- Trained/trains teams in London, Luxembourg, Bruxelles 
- Created an online training platform accessible as a private training PaaS/SaaS
- Creates content online, classes, videos, featured in articles, has participated in a series "Autopsie d'une cyberattaque" on TV
- Have been C|EH, C|EI, CySA+, PentesT+ at some point

---

### 2 - Presentation of the audited company

- Presentation of the company
- Presentation of the project to be audited
- (Here the auditor can also look online before the meeting for the subdomains + web stack used for the project)

### 3 - Audit planification

- Objectives of the audit

#### IF not flash audit (3,4 days)

- Small threat modeling
  - Who could attack the project (external, malicious client, malicious internal for instance)? What is the most likely to happen?
  - What are the main associated risks (theft of personnal/user data, theft of the company's intellectual property, disruption of the services)? What is the most impactful?
- Audit scenarios
  - Definition of the audit scenarios from the threat modeling

#### ENDIF
- Definition of the type of pentest (blackbox, whitebox, graybox) (potentially depending of the scenarios)
- Definition of the audit duration + timeline (usually from 09:00 to 02:00)
- Testing boundaries (DDoS, Bruteforce)
- Infrastructure cloud provider's CSA (Cloud Service Agreement), ToS (Terms of Sale) and policy for pentest
- Credentials/Info to be given before the audit starts
- Are we testing in production? Validation that all of the systems audited are backed up and can be reset easily
- Language of the report (important!)

> The difference between the flash audit and the full audit is that the flash audit does not contain threat assessment, we directly jump to scenarios and the risk matrix is not included as well. The report will be less detailed, not every thing tested will be included, but more the general methodology and all of the vulnerability found + their details.

### 4 - Audit presentation

#### Methodology

- Pre-audit meeting

- Audit Autorization Document Signature (!)

- Beginning of the audit
  - Reconnaissance
    - Looking at technical and organizational info available online, for instance source code, emails, tools version numbers in job offers, veryfing IPs and domains and subdomains in databases etc...
  - Scan/Enumeration
    - Actually making sure of the open ports on the servers and their version numbers, checking if there are already available vulns or pieces of information
  - Exploitation
    - Exploiting the found vulns, testing logic issues, fuzzing APIs, checking permissions, authentication etc... 
  - Post-Exploitation
    - If possible, planting backdoors using found vulnerabilities (for instance a upload form)
    - Removing tracks after the technical part is done
  - Final reporting
    - Writing/compilation of the final report (usually 1/3 of the audit duration), adding ressources, remediation advice

Here you can show the sample pentest report https://github.com/FenrirSec/Documentation/blob/report2024/rapport.pdf

- Post-audit meeting
  - Debriefing session, exchanges
    
### Pricing

- total price = (TJM * (n - number of technical tests + (n * 1/3)) + 99 euros for the debriefing session)