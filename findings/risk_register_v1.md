# AegisGovern_v1 Risk Register

## Finding 001

Asset:
AegisGovern-VM

Threat:
Brute Force SSH Attempts

Likelihood:
Medium

Impact:
High

Risk Score:
6/10

Mitigation:
Restrict SSH source IPs
Enable MFA where possible
Monitor authentication logs

---

## Finding 002

Asset:
AegisGovern-NSG

Threat:
Misconfigured Inbound Rules

Likelihood:
Medium

Impact:
High

Risk Score:
7/10

Mitigation:
Periodic NSG reviews
Least privilege access

---

## Finding 003

Asset:
AegisGovern-VNet

Threat:
Network Reconnaissance

Likelihood:
Medium

Impact:
Medium

Risk Score:
5/10

Mitigation:
Network monitoring
Traffic analysis
Segmentation controls


## Finding 004

Title:
Storage Account Accessible from Public Networks

Asset:
aegisgovstorage001

Severity:
Medium

Risk Description:
The Azure Storage Account currently permits public network access from all networks.

Potential Impact:
Unauthorized external access attempts may target storage resources if additional controls are misconfigured.

Evidence:
Storage Account Overview
Public network access = Enabled
Scope = All Networks

Recommendation:
Restrict access using selected networks, private endpoints, or approved IP ranges where business requirements permit.

Status:
Open

## Finding 005

Title:
Privileged Owner Role Assigned at Subscription Scope

Asset:
Azure Subscription

Severity:
Low

Risk Description:
Owner privileges grant full administrative access to all resources within the subscription.

Potential Impact:
Compromise of the owner account could result in complete control over cloud resources.

Evidence:
Access Control (IAM)
Role = Owner
Scope = Subscription (Inherited)

Recommendation:
Apply least privilege principles.
Use separate administrative and operational accounts in production environments.

Status:
Accepted Risk (Lab Environment)

## Finding 006

Title:
Secrets Stored Outside Secure Vault

Asset:
AegisGovern-VM

Severity:
Medium

Risk Description:
Sensitive credentials may be stored within configuration files, scripts, or local storage instead of Azure Key Vault.

Potential Impact:
Credential exposure may allow unauthorized access to cloud resources.

MITRE ATT&CK:
T1552 - Unsecured Credentials

Recommendation:
Store secrets within Azure Key Vault and implement access controls.

Status:
Mitigated

---

## Finding 007

Title:
Key Vault Public Network Access Enabled

Asset:
aegisgov-kv001

Severity:
Medium

Risk Description:
Azure Key Vault accepts connections from public networks.

Potential Impact:
Expanded attack surface and increased exposure to unauthorized access attempts.

MITRE ATT&CK:
T1190 - Exploit Public Facing Application

Recommendation:
Restrict network access using private endpoints or approved IP ranges.

Status:
Open

---

## Finding 008

Title:
Missing Least Privilege RBAC Controls

Asset:
Azure Subscription

Severity:
Medium

Risk Description:
Permissions exceed operational requirements and increase the risk of unauthorized actions.

Potential Impact:
Compromise of privileged accounts could result in full control over cloud resources.

MITRE ATT&CK:
T1078 - Valid Accounts

Recommendation:
Implement Role Based Access Control and Least Privilege principles.

Status:
Open

## Finding 009

Title:
Insufficient Key Vault RBAC Permissions

Asset:
aegisgov-kv001

Severity:
Low

Risk Description:
Initial RBAC configuration prevented authorized administrators from managing secrets.

Potential Impact:
Operational delays and inability to manage credentials.

Evidence:
Secret creation initially failed.
RBAC permissions assigned.
Secret creation succeeded.

Recommendation:
Review RBAC assignments during deployment.

Status:
Resolved
