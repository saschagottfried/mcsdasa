# Azure Active Directory

Microsoft Azure Active Directory (Azure AD) is a cloud-based identity and access management solution.

Overview

No-Cloud/Hybrid/PaaS/Cloud-onyl products
- On-premises Active Directory (X.500 directories / LDAP / Forests - orange triangle)
- Active Directory on Azure VM (IaaS)
- Azure Active Directory Domain Services (PaaS)
- Azure Active Directory (identity and access management - yellow triangle)

Features
- multi-tenant by design
- support multi-factor auth (MFA)
- protocols: SAML 1.0/2.0, WS-Federation, OpenId Connect, OAuth

Tiers
- Free
- Basic
- Premium

- [comparing GA features] (https://docs.microsoft.com/en-us/azure/active-directory/active-directory-editions#comparing-generally-available-features)


Azure AD B2B 
- collaboration between partners
- fededate once with Azure AD


Azure AD B2C
- simplifies and standardizes consumer identity management by allowing consumers to sign up with social accounts such as Facebook, Google, Amazon or linkedIn



# Administration


Roles
- [administrator roles in Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-assign-admin-roles)

Administrator permissions
- https://docs.microsoft.com/en-us/azure/active-directory/active-directory-assign-admin-roles#administrator-permissions


Application Access Panel
- https://myapps.microsoft.com


# Managing cloud applications
- token (STS)
- claims based

Example app
- Nerddinner.com
- Consent dialog

Token Formate
- JWT


Configure SSO with apps not in Azure AD gallery
- https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-custom-apps


# Application Management in Azure Active Directory

- https://docs.microsoft.com/en-us/azure/active-directory/active-directory-apps-index



# Directory synchronization in hybrid environments

- Hybrid envs support "Same sign on" as apposed to "Single sign on"

Azure Connect primary components
- Synchronization
- AD Federation Service (AD FS)
- Health monitoring



# Directory Federation Services
