# AWS EC2 Security Hardening Audit

## Project Overview

This project simulates a security audit of AWS EC2 infrastructure for a fictional company, SecureShop Pvt Ltd.

The objective was to identify security misconfigurations, assess associated risks, and implement remediation measures following AWS security best practices.

---

## Findings

### Finding 1: SSH Open to the Internet (HIGH)

**Issue**
- Port 22 (SSH) was exposed to 0.0.0.0/0.

**Risk**
- Unauthorized access attempts.
- Brute-force attacks.

**Remediation**
- Restricted SSH access to authorized IP addresses only.

---

### Finding 2: Insecure Default Security Group (CRITICAL)

**Issue**
- Default security group allowed overly permissive inbound traffic.

**Risk**
- Increased attack surface.
- Potential unauthorized access.

**Remediation**
- Removed unnecessary inbound rules.

---

## Additional Assessment

### IAM Role Review

- Verified EC2 instance IAM configuration.
- Documented absence of IAM role attachment.
- Recommended least-privilege IAM implementation.

---

## Security Best Practices Applied

- Principle of Least Privilege
- Security Group Hardening
- Restricted Administrative Access
- IAM Security Review
- Resource Lifecycle Management

---

## Tools Used

- AWS EC2
- AWS Security Groups
- AWS IAM
- AWS CloudWatch

---

## Outcome

Successfully identified and remediated critical EC2 security misconfigurations and documented security recommendations for future hardening efforts.
