# Standard Bank SA — ISO 27001 Risk Assessment Dashboard

**Bakithi Scott Ngcampalala** — Cybersecurity & GRC Professional  
[github.com/Scottie222](https://github.com/Scottie222) · [LinkedIn](https://www.linkedin.com/in/bakithi-scott-ngcampalala-0051a4105)

**Live dashboard:** [scottie222.github.io/StandardBank-Risk-Assessment](https://scottie222.github.io/StandardBank-Risk-Assessment/)

---

## What this project is

This is a fully interactive, browser-based ISO 27001:2022 risk assessment dashboard built around the **real Experian South Africa data breach of August 2020** — one of the largest data breaches in South African history, affecting approximately 24 million individuals and 793,749 business entities.

The project is part of an 11-project GRC portfolio grounded in real South African breach incidents. It was rebuilt from a Python CLI tool into a production-quality single-file web dashboard with live filtering, visual charts, a 5×5 risk heat map, and POPIA compliance scoring — all running in the browser with no install required.

The assessment is conducted from Standard Bank's perspective, examining the systemic third-party control failures, vendor oversight gaps, and authentication weaknesses that the breach exposed.

---

## The real incident

On **19 August 2020**, SABRIC (South African Banking Risk Information Centre) publicly announced that Experian South Africa had suffered a major data breach. The breach was not caused by a technical hack — it was pure **social engineering**. A fraudster posing as a director of a legitimate company submitted a fraudulent data inquiry to Experian and was handed records for approximately 24 million South Africans on 24 and 27 May 2020.

Experian only discovered the fraud on **22 July 2020** — nearly two months after the data was handed over. Standard Bank officially confirmed that its credit customers were among those impacted, as the National Credit Act legally requires banks to disclose customer data to registered credit bureaus including Experian.

### Data exposed

| Field | Exposed |
|---|---|
| Full name | Yes |
| SA ID number | Yes |
| Phone number | Yes |
| Email address | Yes |
| Physical address | Yes |
| Employer, job title, start date | Yes |
| Banking credentials or financial data | No |

### Breach timeline

| Date | Event |
|---|---|
| 24 & 27 May 2020 | Fraudster obtains data from Experian via fraudulent inquiry |
| 22 July 2020 | Experian discovers the fraud — 8 weeks after the fact |
| 19 August 2020 | SABRIC public announcement; Standard Bank confirms impact |
| 1 September 2020 | Breach data found on WeSendIt public file sharing site |
| September 2021 | Suspect arrested by the Hawks in Gauteng |
| October 2021 | Breach data re-emerges on Telegram |

---

## What the dashboard includes

| Feature | Detail |
|---|---|
| Risk register | 20 risks across 14 information assets, ISO 27001:2022 Clause 6.1.2 aligned |
| Filters | Filter by risk rating, department, asset, or free-text search |
| CSV export | One-click download of the full risk register |
| Heat map | 5×5 likelihood × impact matrix with all 20 risks plotted by ID |
| Charts | Inherent vs residual by rating, risks by department, top 10 risks, ISO clause coverage |
| POPIA compliance | Sections 19, 20, 21, 22 and 55 scored with detailed findings per control |

### Risk summary

| Rating | Inherent | Residual |
|---|---|---|
| Critical | 5 | 1 |
| High | 11 | 5 |
| Medium | 4 | 14 |
| Low | 0 | 0 |

---

## ISO 27001:2022 Clause 6.1.2 alignment

| Clause | Requirement | How it is implemented |
|---|---|---|
| 6.1.2(a) | Establish risk criteria | 5×5 likelihood × impact scale with defined thresholds |
| 6.1.2(b) | Identify information security risks | 20 risks across 14 assets |
| 6.1.2(c) | Analyse risk levels | Inherent score calculated from likelihood × impact |
| 6.1.2(d) | Evaluate risks against criteria | Residual risk scored after controls applied |
| 6.1.2(e) | Prioritise risks for treatment | Named owners, treatment controls, due dates |

---

## POPIA regulatory context

The Experian breach directly implicates five sections of the Protection of Personal Information Act 4 of 2013:

| Section | Relevance to this breach |
|---|---|
| Section 19 — Security safeguards | Standard Bank and Experian were required to implement appropriate technical and organisational measures to prevent unlawful access |
| Section 20 — Processing by operators | Experian as an operator was required to process data only with Standard Bank's authorisation and under binding conditions |
| Section 21 — Operator accountability | Standard Bank's Information Officer was responsible for ensuring Experian complied with POPIA obligations |
| Section 22 — Breach notification | Standard Bank was required to notify the Information Regulator and affected data subjects as soon as reasonably possible |
| Section 55 — Information officer duties | The Information Officer is responsible for ensuring POPIA compliance across the organisation and its operators |

---

## How to view the live dashboard

Open this link in any browser — no login, no install, no setup required:

```
https://scottie222.github.io/StandardBank-Risk-Assessment/
```

---

## How to run it locally

Clone the repo and open the file — no Python, no server, no dependencies:

```bash
git clone https://github.com/Scottie222/StandardBank-Risk-Assessment.git
cd StandardBank-Risk-Assessment
```

Then double-click `index.html` to open it in your browser. If you are using VS Code, right-click `index.html` in the Explorer panel and select **Open with Live Server**.

---

## Project structure

```
StandardBank-Risk-Assessment/
├── index.html        # Complete dashboard — all HTML, CSS and JS in one file
├── README.md         # This file
├── .gitignore        # Excludes outputs folder and system files
└── outputs/          # Local exports (gitignored)
```

---

## References

1. Standard Bank official statement — https://www.standardbank.co.za/southafrica/news-and-media/newsroom/external-credit-bureau-data-breach
2. Experian SA breach FAQ — https://www.experian.co.za/fraudulent-data-incident/faqs
3. POPIA Act 4 of 2013 — https://www.justice.gov.za/inforeg/docs/InfoRegSA-POPIA-act4of2013.pdf
4. Information Regulator South Africa — https://inforegulator.org.za
5. ISO/IEC 27001:2022 — https://www.iso.org/standard/82875.html
6. National Credit Act 34 of 2005 — https://www.gov.za/documents/national-credit-act
7. Cybercrimes Act 19 of 2020 — https://www.gov.za/documents/cybercrimes-act

---

## Related GRC portfolio projects

All projects are grounded in real South African breach incidents and available at [github.com/Scottie222](https://github.com/Scottie222):

| Project | Domain | Real incident |
|---|---|---|
| [CloudSec-Assessment-SA](https://github.com/Scottie222/CloudSec-Assessment-SA) | Cloud security | Dis-Chem 2022, Experian 2020 |
| [RetailCo-Security-Awareness](https://github.com/Scottie222/RetailCo-Security-Awareness) | Security awareness | R200M SA phishing losses 2023 |
| [VendorRisk-SA](https://github.com/Scottie222/VendorRisk-SA) | Third-party risk | Experian, Dis-Chem, MTN, TransUnion |
| [LifeHealthcare-BCP](https://github.com/Scottie222/LifeHealthcare-BCP) | BCP/DR | Life Healthcare ransomware 2020 |
| [MTN-ISMS-Audit](https://github.com/Scottie222/MTN-ISMS-Audit) | Internal audit | MTN SA breach April 2025 |
| [OpenVantage-ISMS](https://github.com/Scottie222/OpenVantage-ISMS) | ISMS Suite | Live certification project |
| [POPIA-GDPR-Compliance-Tracker](https://github.com/Scottie222/POPIA-GDPR-Compliance-Tracker) | Data privacy | WhatsApp 2024 enforcement |
| [GRC-Controls-Lab](https://github.com/Scottie222/GRC-Controls-Lab) | Controls lab | Capital One 2019 |
| [TechCorp-Resilience-Assessment](https://github.com/Scottie222/TechCorp-Resilience-Assessment) | Cyber resilience | FinTech post-breach |
| [Cyber-Resilience-SS-Consulting](https://github.com/Scottie222/Cyber-Resilience-SS-Consulting) | Insider threat | SS-Consulting |