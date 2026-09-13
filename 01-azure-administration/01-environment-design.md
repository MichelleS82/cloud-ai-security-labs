# 01 - Environment Design

## Project

Contoso Legal Azure Environment

## Scenario

Contoso Legal is a fictional 100-user legal organisation requiring a secure and manageable Azure environment.

The environment is designed as a miniature production-style environment for demonstrating Azure administration, identity, networking, security, monitoring and automation skills.

## Design Objectives

- Establish a structured Azure resource hierarchy
- Apply Azure RBAC using least-privilege principles
- Separate administrative responsibilities using security groups
- Apply consistent resource tagging
- Establish cost controls and budget monitoring
- Design a secure network architecture
- Build an environment suitable for future Microsoft 365, AVD and AI workloads

## Azure Region

Primary region:

- UK South

## Resource Group

| Resource Group | Region | Purpose |
|---|---|---|
| rg-contoso-prod | UK South | Primary Contoso Legal production lab resources |

## Resource Tags

| Tag | Value |
|---|---|
| Environment | Production |
| Company | ContosoLegal |
| Owner | IT |
| Project | CloudLab |

## Identity Model

The lab uses Microsoft Entra ID identities and security groups to demonstrate role-based access control.

Initial security groups:

- GRP-Contoso-IT-Admins
- GRP-Contoso-Finance
- GRP-Contoso-Legal

## Security Principles

The environment follows:

- Least privilege
- Role-based access control
- Separation of duties
- No unnecessary public exposure
- Controlled administrative access
- Cost monitoring
- Consistent resource naming and tagging

## Future Architecture

The environment will be expanded to demonstrate:

- Azure networking
- Compute
- Storage
- Monitoring
- Backup
- Azure Virtual Desktop
- Microsoft Intune
- Microsoft Entra security
- PowerShell automation
- AI-assisted IT operations

## Status

Day 1 - Environment foundation completed.
