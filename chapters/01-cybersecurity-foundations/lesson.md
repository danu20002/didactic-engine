# Chapter 01 — What Is Cybersecurity?

## Learning goals

After this chapter, you should be able to:

- Explain cybersecurity in simple words
- Distinguish an asset, threat, vulnerability, exploit, control and risk
- Explain confidentiality, integrity and availability
- Recognize common cybersecurity roles
- Apply the concepts to one of your own applications

## 1. Simple meaning

Cybersecurity is the practice of protecting computers, applications, networks and data from unauthorized access, damage, disruption or misuse.

Security is not only about stopping hackers. It also protects systems from mistakes, weak configurations, failed hardware and dishonest insiders.

## 2. The six foundation words

### Asset

Something valuable that should be protected.

Examples:

- Customer data
- A PostgreSQL database
- Source code
- An SAP destination
- A cloud server
- A person's account

### Threat

Something that could cause harm.

Examples:

- An attacker
- Malware
- A dishonest employee
- Fire or power failure
- A developer's mistake

### Vulnerability

A weakness that could be used or triggered.

Examples:

- A weak password
- Missing authorization checks
- Old software
- A public database port
- An API key committed to GitHub

### Exploit

A method that takes advantage of a vulnerability.

A vulnerability is the weakness. An exploit is the technique used against that weakness.

### Security control

A safeguard that reduces risk.

Examples:

- Multi-factor authentication
- Input validation
- Backups
- Firewall rules
- Code review
- Monitoring alerts

Controls can be:

- **Preventive:** Try to stop an incident
- **Detective:** Discover an incident
- **Corrective:** Help recover from an incident

### Risk

The possibility that a threat will use a vulnerability and cause harm.

A useful beginner model is:

**Risk ≈ likelihood × impact**

This is a thinking tool, not an exact universal formula.

## 3. CIA triad

### Confidentiality

Only authorized people and systems can access information.

Example: only payroll employees may view salary information.

### Integrity

Information remains correct and is changed only in authorized ways.

Example: an attacker must not change an invoice amount.

### Availability

Systems and information are accessible when authorized users need them.

Example: an order API should remain usable during business hours.

Good security balances all three.

## 4. Example: Spring Boot application

Imagine a Spring Boot API connected to PostgreSQL.

| Concept | Example |
|---|---|
| Asset | Customer records |
| Threat | Internet attacker |
| Vulnerability | API endpoint has no authorization check |
| Exploit | Attacker changes the URL to access another customer's record |
| Impact | Privacy breach and loss of trust |
| Control | Enforce ownership and role checks on every request |

This is an example of broken access control.

## 5. Authentication versus authorization

- **Authentication:** Proves who you are.
- **Authorization:** Decides what you are allowed to do.

Logging in does not mean a user may access everything.

## 6. Common cybersecurity roles

- **Security analyst:** Monitors and investigates suspicious activity.
- **Application security engineer:** Helps developers build secure software.
- **Cloud security engineer:** Protects cloud identities, networks and workloads.
- **Penetration tester:** Performs authorized testing to find weaknesses.
- **Incident responder:** Contains and investigates security incidents.
- **Security architect:** Designs security across systems and organizations.
- **GRC specialist:** Works with governance, risk and compliance.

Your Java, Spring Boot, SAP BTP and cloud background can later support application security, cloud security and DevSecOps.

## 7. Common beginner mistakes

- Thinking cybersecurity means only hacking
- Installing many tools before learning fundamentals
- Testing public targets without permission
- Memorizing commands without understanding network and application behavior
- Treating authentication as complete authorization
- Hiding mistakes instead of documenting and fixing them

## 8. English vocabulary

| Word | Simple meaning | Example sentence |
|---|---|---|
| Protect | Keep safe | We protect customer data. |
| Prevent | Stop before it happens | MFA can prevent some account attacks. |
| Detect | Discover | Monitoring helps detect unusual activity. |
| Vulnerable | Open to harm because of a weakness | The old server is vulnerable. |
| Breach | An incident where protected data or systems are accessed improperly | The company investigated the data breach. |
| Mitigate | Reduce the likelihood or impact | Rate limiting can mitigate abuse. |
| Authorized | Officially permitted | Only authorized users may view the report. |

## 9. Grammar practice

Use this structure:

**A threat can exploit a vulnerability and harm an asset. A security control reduces the risk.**

Example:

> An attacker can exploit missing authorization and read customer records. An ownership check reduces the risk.

## 10. Summary

Cybersecurity protects valuable assets. Threats may use vulnerabilities to create harmful outcomes. Security controls reduce risk and support confidentiality, integrity and availability. Ethical cybersecurity work always requires authorization.
