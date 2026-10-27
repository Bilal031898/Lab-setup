# Cybersecurity Virtual Lab Setup

**Zyroo Internship Program — Task 01**
**Author:** Muhammad Bilal

## Objective
Build a safe cybersecurity practice lab using Kali Linux, Docker, and OWASP Juice Shop.

## Tools Used
- Kali Linux
- Docker
- OWASP Juice Shop

## Lab Setup
OWASP Juice Shop runs as a Docker container on Kali Linux. A custom Docker bridge network named `zyroo-lab` was created for the lab.

## Connectivity Verification
The application was checked with:

```bash
curl -I http://127.0.0.1:3000
```

An `HTTP/1.1 200 OK` response confirmed that Juice Shop is reachable from the Kali Linux host.

## Network Safety
The application port is bound to `127.0.0.1:3000`, so the published port is only reachable from the local host. The Docker bridge network is not configured as internal-only.

## Evidence
The `screenshots` folder contains images showing:
- OWASP Juice Shop in the browser
- Docker network configuration
- Kali Linux network configuration
- Successful connectivity test
- Additional lab evidence

## Conclusion
The OWASP Juice Shop environment was deployed with Docker and local HTTP connectivity was verified successfully.

> This lab is intended for authorized cybersecurity learning and testing only.
