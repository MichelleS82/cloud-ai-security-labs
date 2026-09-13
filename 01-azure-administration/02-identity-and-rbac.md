# 02 - Identity and RBAC

## Objective

Implement a structured identity and access model for the Contoso Legal Azure environment using Microsoft Entra ID and Azure role-based access control (RBAC).

The design follows the principle of least privilege and separates administrative access from standard business-user access.

## Microsoft Entra Users

The initial lab contains four fictional users:

| User | Role | Purpose |
|---|---|---|
| Michelle Admin | IT Administrator | Azure administration |
| Sarah Finance | Finance User | Finance workload testing |
| James Legal | Legal User | Legal workload testing |
| Alex IT | IT User | IT workload testing |

## Security Groups

| Group | Purpose |
|---|---|
| GRP-Contoso-IT-Admins | Azure administration |
| GRP-Contoso-Finance | Finance users |
| GRP-Contoso-Legal | Legal users |

## Group Membership

### GRP-Contoso-IT-Admins

- Michelle Admin
- Jane IT

### GRP-Contoso-Finance

- Betty Finance

### GRP-Contoso-Legal

- Tom Legal

## Azure RBAC

The IT administrator security group is assigned:

**Role:** Contributor

**Scope:** `rg-contoso-prod`

This provides the group with the ability to manage resources within the Contoso Legal resource group without granting unnecessary permissions across the entire Azure subscription.

## Privileged Access Considerations

The lab initially contained a root-scope User Access Administrator assignment associated with the administrative account.

This was identified during an IAM review and is being removed because root-scope elevated access is unnecessary for normal operation of the lab.

The intended resource-group-level Contributor assignment for the IT administrator group is retained.

## Access Control Design

The intended access hierarchy is:

Entra ID Users
↓
Security Groups
↓
Azure RBAC
↓
Resource Group
↓
Azure Resources

This approach reduces the need to assign Azure roles directly to individual users.

## Least Privilege

The design intentionally avoids granting Contributor or Owner permissions to standard business users.

Administrative permissions are assigned through the IT security group and scoped to the Contoso Legal resource group.

## Evidence

- Entra ID user list
- Security group membership
- Resource group IAM role assignments
- RBAC scope
- Removal of unnecessary root-level elevated access

## Status

Day 1 - Identity and RBAC configuration completed.
