<div align="center">

# 🔐 IAM500 — Identity and Access Management

**Hands-on Microsoft Entra ID and Azure identity security labs**

![Microsoft Entra ID](https://img.shields.io/badge/Microsoft_Entra_ID-0078D4?logo=microsoft&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0089D6?logo=microsoftazure&logoColor=white)
![MFA](https://img.shields.io/badge/MFA-Conditional_Access-2ea44f)
![OAuth](https://img.shields.io/badge/OAuth_2.0-OIDC-orange)

</div>

---

## 📌 Overview

Coursework from **IAM500 (Fall 2026, Seneca Polytechnic)**. These labs cover the full identity lifecycle in a Microsoft cloud tenant: provisioning users and groups, federating external identities, enforcing MFA, controlling access with RBAC, protecting secrets, and governing applications. Each week has a report with an objective, step-by-step screenshots and key takeaways.

## 🔬 Labs

| Week | Topic | Highlights | Report |
|---|---|---|---|
| 1 | **Users, roles and groups** | Least-privilege role delegation, bulk CSV provisioning, licensing, custom domain, dynamic groups | [Open](week01/README.md) |
| 2 | **External identities and MFA** | Google federated as an external IdP (B2B guests); Conditional Access policy enforcing MFA | [Open](week02/README.md) |
| 3 | **Azure RBAC and account protection** | Entra ID sign-in to an Azure VM, role assignment lifecycle, Smart Lockout tuning | [Open](week03/README.md) |
| 4 | **Secrets and threat protection** | Managed identity with Key Vault, Defender for Cloud Apps (app risk, unsanctioning Dropbox), Identity Protection policies and alerts | [Open](week04/README.md) |
| 5 | **Application identity** | App registration, redirect URIs, exposed API scopes, enterprise app assignment, admin consent | [Open](week05/README.md) |

## 🧩 Concepts demonstrated

| Area | Concepts |
|---|---|
| **Authentication** | MFA, Conditional Access, federation with external IdPs, Smart Lockout |
| **Authorization** | Entra ID roles, Azure RBAC, least privilege, role lifecycle (assign and remove) |
| **Governance** | Group-based access, dynamic membership rules, licensing |
| **Workload identity** | Managed identities, Azure Key Vault, app registrations, OAuth 2.0 scopes, admin consent |
| **Threat protection** | Identity Protection risk policies, Defender for Cloud Apps (CASB) |

---

<sub>Author: <b>Rabbi Muhammad Aman</b> · Academic coursework done in a temporary lab tenant. Screenshots show configuration only; no secret values appear.</sub>
