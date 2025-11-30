# MFA Inventory Report – EVM Rail
**Author:** Pasquale Fabio Cioffo  
**Role:** Inventory Owner – MFA Security  
**Date:** _To be completed_

---

## 1. Overview
This report provides an assessment of the current Multi-Factor Authentication (MFA) adoption across Microsoft 365 accounts used by EVM Rail personnel.  
The goal is to identify exposure to identity-based attacks and establish the minimum security posture for user authentication.

---

## 2. Scope
- **Platform:** Microsoft 365 / Entra ID  
- **Services:** Outlook, Teams, OneDrive  
- **Total users analyzed:** 11  
- **Devices:** Mobile and desktop (corporate + personal)

---

## 3. User Categories & Risk Level
| Category        | Risk Level | Notes |
|-----------------|------------|------------------------------------------------|
| Operational     | Medium     | Frequent access via personal smartphones       |
| Administrative  | High       | Access to internal documents and sensitive data |
| Managerial      | Very High  | Primary targets for phishing & BEC attacks      |

---

## 4. MFA Status Summary
| Total Users | MFA Enabled | MFA Disabled |
|------------:|------------:|--------------:|
| 11          | **1**       | **10**        |

**Authentication method (enabled user):** Microsoft Authenticator App.

---

## 5. Technical Observations
- **90.9%** of accounts currently operate **without MFA**, significantly increasing exposure.
- Frequent mobile access increases risk of:
  - session hijacking  
  - MFA fatigue / push bombing  
  - token theft  
  - phishing OTP bypass  
- Absence of MFA on administrative and managerial accounts increases likelihood of:
  - Business Email Compromise (BEC)  
  - unauthorized access to internal documents  
  - impersonation of leadership  
  - mailbox takeover and lateral movement  

---

## 6. Minimum Operational Plan
This plan minimizes impact on internal organization and relies on remote IT where needed:

| Action                               | Estimated Time | Responsible        |
|--------------------------------------|----------------|--------------------|
| Identify accounts without MFA        | 1 day          | Internal           |
| Schedule MFA activation windows      | 30–60 min/group| Remote IT          |
| User onboarding + MFA configuration  | 15–20 min/user | Internal + Remote IT |

**Expected Impact:**  
Risk reduction **> 99%**, according to Microsoft Security baselines.

---

## 7. Notes
This is an **inventory report**, not an enforcement document.  
Its purpose is to support internal planning, IT coordination, and alignment with modern identity security best practices.

---

## 8. Signature
**Pasquale Fabio Cioffo**  
_Inventory Owner – MFA Security_
