
# Lab 4: MFA and Authentication Security — Microsoft Entra ID

## Overview

**Project:** Entra ID Identity Lifecycle and Authentication Security Lab  
**Scenario:** Read-only review of authentication methods and MFA-related access policies  
**Platform:** Microsoft Entra ID  
**Status:** Read-only inspection completed

## Objective

Inspect Microsoft Entra authentication methods and Conditional Access policies to understand how multifactor authentication (MFA) is managed, without changing tenant settings.

## 1. Authentication Methods Inspection

**Page inspected:** Microsoft Entra ID → Authentication methods → Policies

Findings:
- Microsoft Authenticator was visible.
- Enable status: On.
- Target: All users.
- Authentication mode: Unknown.

## 2. Security Defaults Inspection

**Page inspected:** Microsoft Entra ID → Properties → Security defaults

Finding:
- Security defaults: Unavailable or no permission.
- No settings were changed.

## 3. Conditional Access Inspection

**Page inspected:** Microsoft Entra ID → Conditional Access → Policies

Findings:
- More than one policy was listed.
- MFA was mentioned in at least one policy.
- Policy state observed: Enabled.
- Individual policy assignments, exclusions, conditions, and grant controls were not yet verified.

## 4. License and Permissions

- Tenant license: Unable to identify.
- Microsoft 365 admin center: Not checked.
- Authentication methods page: View access available.
- Conditional Access Policies page: View access available.

## 5. Security Analysis

This lab demonstrated how to inspect authentication method policies and MFA-related Conditional Access settings.

An enabled authentication method does not automatically mean MFA is enforced for every user. An enabled Conditional Access policy mentioning MFA also does not establish universal enforcement without reviewing its assignments, conditions, exclusions, and grant controls.

## 6. Safety and Scope

- Read-only inspection only.
- No tenant settings were changed.
- No authentication methods were enabled or disabled.
- No Conditional Access policies were created or modified.
- No production or personal account security settings were changed.
- MFA enforcement was not independently tested.

## 7. Skills Practiced

- Microsoft Entra ID administration navigation
- Authentication methods policy inspection
- Microsoft Authenticator policy review
- Conditional Access policy inspection
- Multifactor authentication concepts
- Access control analysis
- Security documentation and evidence-based reporting

## Conclusion

Completed a read-only review of Microsoft Entra authentication methods and MFA-related Conditional Access policies. Identified Microsoft Authenticator as enabled for all users in the inspected policy and observed multiple Conditional Access policies, including an enabled policy mentioning MFA.

The tenant license and full MFA enforcement requirements remain unverified.
