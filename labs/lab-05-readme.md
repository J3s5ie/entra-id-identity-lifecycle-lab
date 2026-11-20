# IAM Lab 5: Access Governance & Security Audit

## Project Overview
This lab demonstrates Identity and Access Management (IAM) access governance using Microsoft Entra ID.

The objective was to perform a read-only audit of security groups, user accounts, application access, group ownership, and directory role assignments in a simulated organization called Northstar Services.

## Environment
- Platform: Microsoft Entra ID
- Organization: Northstar Services (simulated)
- Test User: Jordan Lee
- Security Groups: NS-IT-Support and NS-HR
- Audit Type: Read-only access governance review

## 1. User Account Review

Test account: Jordan Lee

Audit findings:
- Account status: Disabled
- Assigned applications: None
- Directory roles: None
- Group ownership: Not an owner

## 2. Group Membership Review

Two security groups were inspected.

**NS-IT-Support**
- Membership type: Assigned
- Members: Empty
- Description: IT Support employees — Northstar Services IAM training lab

**NS-HR**
- Membership type: Assigned
- Membership: Previously verified during the Mover lab
- Description: HR employees — Northstar Services IAM training lab

## 3. Group Ownership Audit

Ownership was inspected for both security groups.

Results:
- NS-IT-Support: No owners listed
- NS-HR: No owners listed

Security observation:

Neither group displayed an assigned owner. Establishing group ownership would improve administrative accountability and access governance.

## 4. Enterprise Application Access Review

Application assignments were inspected.

Results:
- NS-IT-Support: No applications assigned
- NS-HR: No applications assigned
- Jordan Lee: No applications assigned

Security observation:

No enterprise application assignments were visible during the inspection.

## 5. Directory Role Assignment Audit

Assigned directory roles were inspected for both groups.

Results:
- NS-IT-Support: No roles assigned
- NS-HR: No roles assigned
- Jordan Lee: No roles assigned

Security observation:

No group-based directory role assignments were visible during the inspection.

## 6. Membership Configuration Review

Both groups were verified to use Assigned membership.

Results:
- NS-IT-Support: Assigned
- NS-HR: Assigned

This means group membership is managed manually rather than through dynamic membership rules.

## 7. Security Findings and Recommendations

Findings:
1. Both groups have department-specific descriptions.
2. Both groups use manually managed membership.
3. Neither group has a listed owner.
4. Neither group has assigned enterprise applications.
5. Neither group has assigned directory roles.
6. Jordan Lee's test account remains disabled.

Recommendations:
- Establish appropriate group owners.
- Review group membership regularly.
- Apply least privilege when assigning application access.
- Review privileged directory role assignments.
- Maintain documentation of access changes.
- Follow Joiner, Mover, and Leaver procedures when managing employee access.

## 8. Skills Demonstrated

- Microsoft Entra ID administration
- Identity lifecycle management
- Access governance
- Security group auditing
- Group ownership inspection
- Enterprise application access review
- Directory role auditing
- Least privilege principles
- Security documentation

## 9. Lab Conclusion

Successfully completed a read-only access governance audit using Microsoft Entra ID.

The exercise demonstrated how IAM professionals inspect user accounts, security groups, group ownership, application assignments, and directory role assignments to identify potential access governance improvements.

All findings were documented without changing production or personal account security settings.

**Lab Status:** Completed  
**Environment:** Northstar Services IAM Training Lab  
**Technology:** Microsoft Entra ID
