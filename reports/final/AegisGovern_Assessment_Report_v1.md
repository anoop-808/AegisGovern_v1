# AegisGovern_v1 Cloud Security Risk Assessment Report

## Executive Summary

A cloud governance and security assessment was conducted against the AegisGovern_v1 Microsoft Azure environment to evaluate identity management, network security, storage security, secrets management, and governance controls.

The assessment identified nine security findings across cloud resources, including public network exposure, excessive privilege assignments, secrets management risks, and access control weaknesses. Security controls such as SSH key authentication, Azure Key Vault integration, storage encryption, and Network Security Group filtering were successfully implemented and validated.

Assessment Results:

* Total Findings: 9
* Medium Severity Findings: 7
* Low Severity Findings: 2
* Critical Findings: 0
* High Findings: 0

Overall Risk Rating: Medium

The environment demonstrates a solid baseline cloud security posture and alignment with governance best practices. Additional hardening efforts related to RBAC governance, network access restrictions, and recovery planning are recommended to further reduce organizational risk.

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
