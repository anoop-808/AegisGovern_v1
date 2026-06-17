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

# AegisGovern_v1 Risk Register

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
