# Lab 3: Leaver Workflow — Microsoft Entra ID

## Overview

**Project:** Entra ID Identity Lifecycle Lab  
**Scenario:** Employee offboarding  
**Platform:** Microsoft Entra ID  
**Test user:** Jordan Lee (fictional lab account)  
**Status:** Completed

## Objective

Simulate an employee leaving an organization by disabling the user's account, removing group membership, and verifying that the user no longer has access through the lab's assigned security group.

## Environment

- Microsoft Entra ID
- Fictional test user: Jordan Lee
- Security group: `NS-HR`
- Lab organization: Northstar Services (fictional)

## Steps Performed

1. Located the Jordan Lee test account in Microsoft Entra ID.
2. Disabled the account.
3. Verified that **Account enabled** was set to **No**.
4. Reviewed the user's group memberships.
5. Removed Jordan Lee from the `NS-HR` security group.
6. Verified that the account remained disabled and no lab group memberships remained.

## Verification Results

| Check | Expected result | Result |
|---|---|---|
| Account status | Disabled | Verified |
| `NS-HR` membership | Removed | Verified |
| Remaining lab group memberships | None | Verified |

## Security Relevance

The leaver process helps reduce the risk of former employees retaining access to organizational resources. Disabling an account and removing group memberships are important identity lifecycle controls.

In a production environment, offboarding may also require revoking active sessions, reviewing application-specific assignments, recovering company devices, and confirming that other access paths have been removed. Those additional actions were outside the scope of this lab.

## Skills Practiced

- Microsoft Entra ID user administration
- Account disablement
- Security group membership management
- Identity lifecycle management (Joiner, Mover, Leaver)
- Access removal and verification
- Technical documentation

## Outcome

Successfully completed the Leaver workflow for the fictional Jordan Lee account. Verified that the account remained disabled and that no lab group memberships remained.

**Note:** This was a training exercise using a fictional account, not a production offboarding event.
