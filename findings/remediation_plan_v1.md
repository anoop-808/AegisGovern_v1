# AegisGovern_v1 Remediation Plan

| Finding ID | Finding                               | Recommended Remediation                                                             |
| ---------- | ------------------------------------- | ----------------------------------------------------------------------------------- |
| AEGIS-001  | Brute Force SSH Attempts              | Restrict SSH access to approved IP ranges and implement MFA where supported.        |
| AEGIS-002  | Misconfigured Inbound Rules           | Review NSG rules quarterly and apply least privilege principles.                    |
| AEGIS-003  | Network Reconnaissance                | Enable NSG Flow Logs and monitor network activity for abnormal scanning behavior.   |
| AEGIS-004  | Public Storage Access                 | Restrict Storage Account access using selected networks or Private Endpoints.       |
| AEGIS-005  | Excessive Owner Privileges            | Separate administrative and operational accounts and reduce privileged assignments. |
| AEGIS-006  | Secrets Stored Outside Secure Vault   | Store credentials and secrets exclusively within Azure Key Vault.                   |
| AEGIS-007  | Key Vault Public Access Enabled       | Restrict Key Vault access using Private Endpoints or approved IP ranges.            |
| AEGIS-008  | Missing Least Privilege RBAC Controls | Review role assignments and remove unnecessary permissions.                         |
| AEGIS-009  | Key Vault RBAC Misconfiguration       | Validate RBAC permissions during deployment and change management activities.       |

---

## Analyst Recommendation

The highest-priority remediation activities are reducing public network exposure, implementing least-privilege access controls, and enforcing secure secrets management practices.

These actions provide the greatest reduction in overall cloud security risk and improve alignment with NIST CSF and CIS Controls.
