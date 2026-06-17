# AegisGovern_v1 Control Assessment

## Control 001

Asset:
AegisGovern-VM

Control:
SSH Key Authentication

Framework:
CIS Control 5

Status:
Implemented

Notes:
Password-based access disabled in favor of SSH key authentication.

---

## Control 002

Asset:
AegisGovern-NSG

Control:
Network Traffic Filtering

Framework:
CIS Control 4

Status:
Implemented

Notes:
Inbound SSH access controlled through NSG rules.

---

## Control 003

Asset:
AegisGovern-VNet

Control:
Network Segmentation

Framework:
NIST PR.AC

Status:
Implemented

Notes:
Resources isolated within dedicated virtual network.

---

## Control 004

Asset:
aegisgovstorage001

Control:
Storage Encryption

Framework:
CIS Control 3

Status:
Implemented

Notes:
Azure Storage encryption enabled by default.

---

## Control 005

Asset:
aegisgov-kv001

Control:
Secrets Management

Framework:
NIST PR.AC

Status:
Implemented

Notes:
Administrative credentials stored within Azure Key Vault.
