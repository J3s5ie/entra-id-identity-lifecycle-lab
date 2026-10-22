# Lab 2: Mover — Employee Role Change

## Objective

Practice updating an employee's identity attributes and security group membership to reflect a change in job role or department using Microsoft Entra ID.

## Scenario

An employee transitions from IT Support to Human Resources. Their identity details and group membership must be updated to reflect the new responsibilities.

## Environment

- **Platform:** Microsoft Entra ID
- **Lab type:** Identity and Access Management (IAM)
- **Test user:** Jordan Lee
- **Previous group:** `NS-IT-Support`
- **New group:** `NS-HR`

## Tasks Completed

### 1. Created the New Department Group

Created the `NS-HR` security group with Assigned membership and a description identifying it as part of the Northstar Services IAM training lab.

### 2. Added the User to the New Group

Added Jordan Lee to `NS-HR` and verified that the user appeared in the group's Members list.

### 3. Updated User Attributes

Updated Jordan Lee's user properties in Microsoft Entra ID:

- **Department:** Human Resources
- **Job title:** HR Specialist

Verified that both changes were saved successfully.

### 4. Removed the Previous Group Membership

Removed Jordan Lee from `NS-IT-Support` after verifying the new group membership.

### 5. Verified the Final State

- **New group membership:** Jordan Lee is a member of `NS-HR`.
- **Old group membership:** Jordan Lee is no longer a member of `NS-IT-Support`.
- **Department:** Human Resources.
- **Job title:** HR Specialist.
- **Lab status:** Completed.

## IAM Concepts Demonstrated

- Identity lifecycle management
- Mover workflow
- User attribute administration
- Security group management
- Role-based access assignment fundamentals
- Access review and verification
- Least privilege principles
- IAM change documentation

## Security Considerations

The lab uses a fictional test identity. In a production environment, role changes should follow approved access-change procedures, including appropriate authorization and validation of application permissions. Group membership changes alone do not prove that every connected application's access has been updated.

## Evidence

Recommended screenshots to add after removing sensitive information:

1. Jordan Lee's updated department and job title.
2. Jordan Lee listed in `NS-HR`.
3. Jordan Lee absent from `NS-IT-Support`.

## Outcome

Successfully completed a simulated Mover workflow by updating identity attributes, assigning new group membership, removing the previous group membership, and verifying the final state.

## Next Lab

Lab 3 — Leaver: Practice disabling a test account and verifying the relevant offboarding steps.
