# Identity and Access Management (IAM) Lifecycle Lab – Microsoft Entra ID

## Overview
This project demonstrates enterprise Identity and Access Management (IAM) practices using Microsoft Entra ID (Azure AD). The lab focuses on identity lifecycle management, group-based access control, and auditability.

## Technologies Used
- Microsoft Entra ID (Azure Active Directory)
- Microsoft Entra ID P1
- Enterprise Applications
- Security Groups
- Audit Logs

## Project Objectives
- Implement least-privilege access using security groups
- Enforce group-based application access
- Demonstrate Joiner, Mover, and Leaver lifecycle scenarios
- Capture audit logs for governance and compliance

## Architecture
- Users are assigned to department-based security groups
- Enterprise application access is restricted to assigned groups
- No direct user-to-application assignments are used

## Lifecycle Scenarios

### Joiner
- New user (HR-NewHire) created
- User added to HR security group
- Application access granted automatically

### Mover
- User moved from HR group to Finance group
- Application access automatically revoked

### Leaver
- User account disabled
- Sign-in blocked at the identity level
- Access fully removed

## Security Controls
- Assignment required enabled on enterprise application
- Group-based authorization model
- Role-based access control (RBAC)
- Full audit logging for identity changes

## Audit & Governance
- All identity changes are recorded in Microsoft Entra audit logs
- Logs capture actor, target, action, and timestamp

## Key Takeaways
- Group-based access reduces risk and simplifies identity lifecycle management
- Blocking sign-in immediately mitigates insider risk
- Audit logs provide compliance and traceability
