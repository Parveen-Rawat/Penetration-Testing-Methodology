## Legal and Ethical Issues


Make sure you are working for a legitimate organization performing assessments only after explicit coordination between the target company and client.

Criminal Organization hire talent to assist with their illegal actions

- Keep a copy of scope of work/contact and formal document listing the scope testing also signed by the client
- Stay within the scope of testing.
- When in Doubt document and overcommunicate
- Analyse and dig deeper and question everything

## The HTB Methodology

### Pre-Engagement

- This is where main commitments, tasks, scope, limitations and related agreements are documented in writing.
- Contractual documents are drawn and essential information is exchanged during this stage

CheckMarks 
- Non-Disclosure Agreement
- Goals
- Scope
- Time Estimation
- Rules of Engagement

The entire pre-engagement process consists of three essential components:
1. Scoping questionnaire
2. Pre-engagement Meeting
3. Kick-Off Meeting

Before this an NDA is signed by both parties

Documents requires before conducting penetration test

1. Non-Disclosure Agreement (NDA)	After Initial Contact
2. Scoping Questionnaire	Before the Pre-Engagement Meeting
3. Scoping Document	During the Pre-Engagement Meeting
4. Penetration Testing Proposal (Contract/Scope of Work (SoW))	During the Pre-engagement Meeting
5. Rules of Engagement (RoE)	Before the Kick-Off Meeting
6. Contractors Agreement (Physical Assessments)	Before the Kick-Off Meeting
7. Reports	During and after the conducted Penetration Test


### Information Gathering 

- Enumerate and Gain as much as information about the target

Ways to obtain information:
1. Open-Source Intelligence
2. Infrastructure Enumeration
3. Service Enumeration
4. Host Enumeration


### Vulnerability Assessment

- Use the information we found to identify potential weaknesses in the system or infrastructure
- Divided in two: One use of vulnerablity scanners in automation fashion to scan and probe for known vulnerablities. Other is use of information we find to identify the potential weakness in system manually

### Exploitation

- Attack performed against a system or application based on potential weakness we found during information gathering phase
- Information Gathering to gather enough information and analyze it via Vulnerablitiy Assessment and prepare potential attacks


### Post-Exploitation

- Bypassing security mechanisms and obtaining highest possible privileges on the compromised system

### Lateral Movement

- Move from one system to another in a coorporate environment done after intial compromised or after gaining the highest possible privileges on the compromised system which might be dual homed

### Proof-Of-Concept (POC)

- PoC are the proof that the vulnerability exist and is exploitable. It is given with detailed steps to reproduce the entire attack chain to proof the vulnerability

### Post-Engagement

- Cleaning up the systems and polishing report

Document should contain the following:
- An attack chain detailing steps taken to achieve compromise
- A strong executive summary for technical and also one for non-tech individuals
- Risk rating, finding impact and remediation recommendation
- Steps to reproduce  


## Precautionary Measure or Engagement Checklist

-   Obtain written consent from the owner or authorized representative of the computer or network being tested
-  the testing within the scope of consent obtained only and respect any limitations specified
-   Take measures to prevent causing damage to the systems or networks being tested
-   Do not access, use or disclosure personal data or any other information obtained during the testing without permissions
-   Do not intercept electronic communications without the consent of one of the parties to the communicaton
-   Do not conduct testing on systems or networks that are covered by the Health Insure Portabilty and Accountability Act (HIPPA) without proper authorization


#### InfoSec Specialization
- Network and infrastructure security
- Application Security
- Security Testing
- Systems auditing
- Business continuity planning
- Digital forencis
- Incident Detection and response

**One way to find the vulnerability is to take a assumed guess that is backed up with experience and after seeing the repeatative misconfigurations. Assume and then proceed likely to find a potential vulnerability**

`


# 1. Service Enumeration & Exploitation

# 2. Web Enumeration & Exploitation

## Passive Enumeration

### Banner Grabbing & Fingerprinting

Retrieving server header information andget good picture of what is hosted on the web server

```bash
curl -IL <Target-Website-URL>
```

**Whatweb** extract the version of webservers, supporting frameworks and applications using the command-line tool `whatweb`

```bash

whatweb --no-errors 10.x.x.0/24
```

### Certificates

- SSL/TLS certs can potentially contains email address and company name.
- *This could potentially be used to conduct a phising attack*

https://cdn.services-k8s.prod.aws.htb.systems/content/modules/77/cert.png


### Robots.txt

- Common for websites and instructs the google bots which resources can and cannot be accessed for indexoing
- Could potentially the wealth of privileged endpoints

```bash
curl -s http://10.x.x.x/robots.txt
```

### Source Code

- Could potentially contain sensitive information --> [CTRL + U]


# 3. Application Enumeration & Exploitation

# 4. Active Directory Enumeration & Exploitation

# 5. Linux Enumeration, Exploitation and Pivoting

# 6. Windows Enumeration, Exploitation and Pivoting


# 7. Documentation & Reporting
