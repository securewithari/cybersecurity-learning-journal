# 📊 Risk Register — SmallBiz Tech

**Organization:** SmallBiz Tech (Fictional)
**Assessment Date:** May 2026
**Assessor:** Arielle Zayas
**Framework:** NIST CSF / CIA Triad

---

## 🧮 Risk Scoring Method

Each risk is scored using this formula:

> **Risk Score = Likelihood × Impact**

| Score | Likelihood | Impact |
|---|---|---|
| 1 | Rare | Minimal |
| 2 | Unlikely | Minor |
| 3 | Possible | Moderate |
| 4 | Likely | Major |
| 5 | Almost Certain | Severe |

**Risk Level:**
| Score Range | Risk Level |
|---|---|
| 1–4 | 🟢 Low |
| 5–9 | 🟡 Medium |
| 10–14 | 🟠 High |
| 15–25 | 🔴 Critical |

---

## 📋 Risk Register

### Risk 1 — Weak Employee Passwords
| Field | Detail |
|---|---|
| **Asset** | User accounts / systems |
| **Threat** | Unauthorized access via credential attack |
| **Vulnerability** | No password policy enforced |
| **Likelihood** | 4 — Likely |
| **Impact** | 4 — Major |
| **Risk Score** | 🔴 16 — Critical |
| **NIST CSF Function** | Protect |
| **Recommended Control** | Enforce strong password policy + MFA on all accounts |
| **Control Type** | Preventive |
| **Treatment** | Mitigate |

---

### Risk 2 — No Data Backups
| Field | Detail |
|---|---|
| **Asset** | Customer data, financial records |
| **Threat** | Ransomware attack or accidental deletion |
| **Vulnerability** | No backup strategy in place |
| **Likelihood** | 3 — Possible |
| **Impact** | 5 — Severe |
| **Risk Score** | 🔴 15 — Critical |
| **NIST CSF Function** | Recover |
| **Recommended Control** | Implement automated daily backups to S3 with versioning |
| **Control Type** | Corrective |
| **Treatment** | Mitigate |

---

### Risk 3 — Unpatched Software
| Field | Detail |
|---|---|
| **Asset** | Employee laptops, servers |
| **Threat** | Exploitation of known vulnerabilities |
| **Vulnerability** | No patch management process |
| **Likelihood** | 4 — Likely |
| **Impact** | 3 — Moderate |
| **Risk Score** | 🟠 12 — High |
| **NIST CSF Function** | Protect |
| **Recommended Control** | Establish monthly patch management schedule |
| **Control Type** | Preventive |
| **Treatment** | Mitigate |

---

### Risk 4 — No Incident Response Plan
| Field | Detail |
|---|---|
| **Asset** | Entire organization |
| **Threat** | Security breach with no coordinated response |
| **Vulnerability** | No documented IR procedures |
| **Likelihood** | 3 — Possible |
| **Impact** | 4 — Major |
| **Risk Score** | 🟠 12 — High |
| **NIST CSF Function** | Respond |
| **Recommended Control** | Develop and test a basic Incident Response Plan |
| **Control Type** | Corrective |
| **Treatment** | Mitigate |

---

### Risk 5 — Overprivileged User Accounts
| Field | Detail |
|---|---|
| **Asset** | AWS environment, internal systems |
| **Threat** | Insider threat or compromised admin account |
| **Vulnerability** | Users have more access than their role requires |
| **Likelihood** | 3 — Possible |
| **Impact** | 4 — Major |
| **Risk Score** | 🟠 12 — High |
| **NIST CSF Function** | Protect |
| **Recommended Control** | Implement least privilege — review and restrict all user permissions |
| **Control Type** | Preventive |
| **Treatment** | Mitigate |

---

### Risk 6 — No Security Awareness Training
| Field | Detail |
|---|---|
| **Asset** | Employees, company data |
| **Threat** | Phishing attacks, social engineering |
| **Vulnerability** | Employees untrained on security threats |
| **Likelihood** | 4 — Likely |
| **Impact** | 3 — Moderate |
| **Risk Score** | 🟠 12 — High |
| **NIST CSF Function** | Protect |
| **Recommended Control** | Implement quarterly security awareness training |
| **Control Type** | Preventive |
| **Treatment** | Mitigate |

---

## 📈 Risk Summary

| Risk | Score | Level |
|---|---|---|
| Weak Passwords | 16 | 🔴 Critical |
| No Data Backups | 15 | 🔴 Critical |
| Unpatched Software | 12 | 🟠 High |
| No IR Plan | 12 | 🟠 High |
| Overprivileged Accounts | 12 | 🟠 High |
| No Security Training | 12 | 🟠 High |

**Total Risks Identified:** 6
**Critical:** 2 | **High:** 4 | **Medium:** 0 | **Low:** 0

---

## ✅ Recommended Priority Order

1. Enforce MFA and strong passwords immediately
2. Set up automated backups to AWS S3
3. Begin monthly patch management
4. Restrict user permissions to least privilege
5. Develop a basic Incident Response Plan
6. Schedule security awareness training

---
*Risk assessment completed as part of cybersecurity portfolio work.*
*Organization and scenarios are fictional and for educational purposes.*
