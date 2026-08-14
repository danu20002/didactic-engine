# Safe Lab Setup

Do not install every tool immediately. Each chapter will tell you exactly what is required.

## Stage 1 — Chapters 1 to 5

Required:

- Your normal computer
- A modern browser
- Terminal or PowerShell
- Git
- Java 21 for later secure-coding exercises
- A text editor such as VS Code

## Stage 2 — Linux and networking

Add:

- VirtualBox or another local hypervisor
- One Ubuntu LTS virtual machine
- NAT networking by default
- Snapshots before risky changes

## Stage 3 — Web security

Add only inside an isolated lab:

- Docker
- OWASP Juice Shop or another intentionally vulnerable target
- OWASP ZAP Community Edition

## Stage 4 — Defensive and professional work

Add:

- Log-analysis exercises
- Dependency and secret scanning in GitHub Actions
- Container scanning
- A small Spring Boot and PostgreSQL capstone

## Lab safety

- Never bridge a vulnerable VM directly to an untrusted network.
- Do not store real company data in lab machines.
- Use unique test passwords.
- Keep the host operating system and hypervisor updated.
- Stop containers and VMs when they are not required.
- Never commit secrets. Use environment variables and example files.

## Repository rule

Do not commit:

- Passwords, tokens, API keys or private certificates
- Real vulnerability data from employers or customers
- Malware or weaponized payloads
- Large VM images, packet captures containing personal data or build outputs
