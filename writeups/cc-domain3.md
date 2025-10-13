# CC Domain 3 — Access Control Concepts

## Core concepts
- **I-A-A-A**: Identification → Authentication → Authorization → Accounting (audit)
- **Principles**: least privilege, need-to-know, separation of duties, privilege review
- **Account lifecycle**: provisioning → change (role moves) → periodic review → de-provisioning
- **Auth factors**: 
  - *Something you know* (password, PIN) 
  - *Something you have* (OTP token, smart card) 
  - *Something you are* (biometrics)
  - *Somewhere you are / something you do* (location, behavior) — context
- **MFA**: combine factors from different categories (stronger than passwords alone)
- **Credential hygiene**: complexity, length, rotation policy, lockout, timeout

## Authorization models
- **DAC** (Discretionary): owner decides permissions (ACLs)
- **MAC** (Mandatory): labels/classifications; policy enforced centrally
- **RBAC** (Role-based): rights via job roles
- **ABAC** (Attribute-based): rules using user/resource/environment attributes
- **RuBAC** (Rule-based): allow/deny by explicit rules (e.g., time, network)

## Access enablement
- **SSO**: one set of credentials for multiple systems
- **Federation**: trust across orgs/domains (e.g., SAML/OIDC)
- **Provisioning controls**: joiner-mover-leaver, approvals, recertifications

## Why this matters
Good access control shrinks blast radius, prevents privilege creep, and leaves auditable trails so you can prove *who did what, when*.

![CC Domain 3 Certificate](./images/cc-domain3-cert.png)
