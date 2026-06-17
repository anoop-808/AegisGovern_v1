# AegisGovern_v1 Cloud Security Risk Assessment Report

## Executive Summary

AegisGovern_v1 is a cloud governance and security assessment project developed within Microsoft Azure using an Azure for Students subscription.

The objective of the project was to simulate the activities performed by cloud security analysts during security reviews, governance assessments, risk identification, and control validation exercises.

The assessment covered virtual infrastructure, networking, identity and access management, cloud storage, and secrets management.

---

## Environment Overview

Resources Assessed:

* AegisGovern-RG
* AegisGovern-VNet
* Default Subnet
* AegisGovern-NSG
* AegisGovern-VM
* aegisgovstorage001
* aegisgov-kv001

Region:

* Central India

---

## Security Controls Implemented

| Control                           | Status      |
| --------------------------------- | ----------- |
| SSH Key Authentication            | Implemented |
| Network Security Group Filtering  | Implemented |
| Virtual Network Segmentation      | Implemented |
| Storage Encryption                | Implemented |
| Azure Key Vault Secret Management | Implemented |
| RBAC Governance                   | Implemented |

---

## Findings Summary

| Finding                               | Severity | Status        |
| ------------------------------------- | -------- | ------------- |
| Brute Force SSH Attempts              | Medium   | Open          |
| Misconfigured Inbound Rules           | Medium   | Open          |
| Network Reconnaissance                | Medium   | Open          |
| Public Storage Access                 | Medium   | Open          |
| Owner Role at Subscription Scope      | Low      | Accepted Risk |
| Secrets Stored Outside Secure Vault   | Medium   | Mitigated     |
| Key Vault Public Access Enabled       | Medium   | Open          |
| Missing Least Privilege RBAC Controls | Medium   | Open          |
| Key Vault RBAC Misconfiguration       | Low      | Resolved      |

---

## Compliance Assessment

Frameworks Reviewed:

* NIST Cybersecurity Framework
* CIS Controls

Overall Compliance Status:

Partially Implemented

Key Strengths:

* Asset inventory maintained
* Risk assessment completed
* Access control review performed
* Secure secret storage implemented

Improvement Areas:

* Network access restrictions
* RBAC hardening
* Recovery planning
* Private endpoint implementation

---

## Conclusion

The AegisGovern_v1 project successfully demonstrates cloud governance, risk assessment, access control validation, and security control implementation within Microsoft Azure.

The project provides practical experience aligned with cloud security analyst and governance-focused cybersecurity roles and serves as a foundational component of the THRAGG cybersecurity portfolio.
