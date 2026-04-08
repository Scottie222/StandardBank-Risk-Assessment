# Standard Bank SA — ISO 27001 Risk Assessment Dashboard

> Interactive single-file web dashboard based on the real **Experian SA data breach (August 2020)** — one of the largest data breaches in South African history, exposing ~24 million individuals and 793,749 businesses.

---

## Live dashboard

Open `index.html` in any browser — **no install, no server, no Python required.**

---

## What's included

| Feature | Detail |
|---|---|
| Risk register | 20 risks across 14 information assets |
| ISO standard | ISO/IEC 27001:2022 Clause 6.1.2 |
| Filters | By rating, department, asset, or free-text search |
| CSV export | One-click download of the full risk register |
| Heat map | 5×5 likelihood × impact matrix with all 20 risks plotted |
| Charts | Inherent vs residual, department breakdown, top 10, clause coverage |
| POPIA scoring | Sections 19, 20, 21, 22 and 55 assessed with findings |

---

## Risk summary

| Rating | Inherent | Residual |
|---|---|---|
| Critical | 4 | 1 |
| High | 7 | 5 |
| Medium | 9 | 14 |
| Low | 0 | 0 |

---

## How to run locally

```powershell
git clone https://github.com/Scottie222/StandardBank-Risk-Assessment.git
cd StandardBank-Risk-Assessment
```

Then double-click `index.html` — opens in your default browser instantly.

---

## How to deploy (GitHub Pages)

1. Push to GitHub (see setup steps below)
2. Go to `Settings → Pages`
3. Source: **Deploy from branch → main → / (root)**
4. Your live URL: `https://scottie222.github.io/StandardBank-Risk-Assessment/`

---

## The real incident

On **19 August 2020**, SABRIC announced that Experian South Africa suffered a data breach caused entirely by **social engineering** — a fraudster posing as a legitimate company director submitted a fraudulent data inquiry and was handed records for ~24 million South Africans on 24 and 27 May 2020. Standard Bank confirmed its credit customers were among those affected.

### Breach timeline

| Date | Event |
|---|---|
| 24 & 27 May 2020 | Fraudster obtains data from Experian |
| 22 July 2020 | Experian discovers the fraud |
| 19 August 2020 | SABRIC public announcement; Standard Bank confirms impact |
| 1 September 2020 | Breach data found on WeSendIt (public file sharing) |
| September 2021 | Suspect arrested by Hawks in Gauteng |
| October 2021 | Data re-emerges on Telegram |

---

## Regulatory context

| Regulation | Relevance |
|---|---|
| POPIA Act 4 of 2013 | Sections 19, 20, 21, 22, 55 — safeguards, operator duties, breach notification |
| National Credit Act | Legal basis for credit data disclosure to bureaus |
| Cybercrimes Act 19 of 2020 | Criminal prosecution of the fraudster |
| SARB Prudential Authority | Notified by Experian as part of regulatory response |

---

## References

1. Standard Bank statement — https://www.standardbank.co.za/southafrica/news-and-media/newsroom/external-credit-bureau-data-breach
2. Experian SA FAQ — https://www.experian.co.za/fraudulent-data-incident/faqs
3. POPIA Act 4 of 2013 — https://www.justice.gov.za/inforeg/docs/InfoRegSA-POPIA-act4of2013.pdf
4. ISO/IEC 27001:2022 — https://www.iso.org/standard/82875.html
5. Information Regulator SA — https://inforegulator.org.za

---

## Related projects

- [GRC Controls Lab](https://github.com/Scottie222/GRC-Controls-Lab)
- [POPIA-GDPR Compliance Tracker](https://github.com/Scottie222/POPIA-GDPR-Compliance-Tracker)
- [TechCorp Resilience Assessment](https://github.com/Scottie222/TechCorp-Resilience-Assessment)
- [Cyber-Resilience-SS-Consulting](https://github.com/Scottie222/Cyber-Resilience-SS-Consulting)