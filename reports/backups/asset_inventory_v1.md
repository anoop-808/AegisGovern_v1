# AegisGovern_v1 Asset Inventory

## Environment Summary

Project Name: AegisGovern_v1

Purpose:
Cloud Security Risk Assessment and Governance Simulation

---

## Asset 1

Resource Name: AegisGovern-RG

Type:
Azure Resource Group

Purpose:
Logical container for cloud resources

Business Criticality:
Medium

Security Notes:
Compromise could affect all contained assets

---

## Asset 2

Resource Name: AegisGovern-VNet

Type:
Azure Virtual Network

Purpose:
Provides network isolation

Business Criticality:
High

Security Notes:
Improper segmentation may expose resources

---

## Asset 3

Resource Name: default

Type:
Azure Subnet

Purpose:
Network segment for workloads

Business Criticality:
High

Security Notes:
Should be monitored for unauthorized traffic

---

## Asset 4

Resource Name: AegisGovern-NSG

Type:
Network Security Group

Purpose:
Traffic filtering and access control

Business Criticality:
High

Security Notes:
Misconfigured rules may expose services

---

## Asset 5

Resource Name: AegisGovern-VM

Type:
Ubuntu Virtual Machine

Purpose:
Cloud workload for assessment activities

Business Criticality:
Critical

Security Notes:
Primary attack surface in environment

---

## Asset 6

Resource Name: aegisgovstorage001

Type:
Azure Storage Account

Purpose:
Cloud storage for governance assessment artifacts

Business Criticality:
High

Security Notes:
Public network access currently enabled
