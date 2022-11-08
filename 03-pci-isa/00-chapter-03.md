# PCI ISA 3.2.1

- Certification Website
- <https://home.pearsonvue.com/pci>

- Training Website:
- <https://programs.pcissc.org/user/scorm_training/SCORM_Training_Sessions.aspx>

---
Chapter 3 | Module 3

---

Compliance Programs and PCI Program Roles

- Payment Brand Compliance Programs
- SAQ Overview
- PA-DSS Overview
- Qualified Integrator/Reseller (QIR)
- P2PE Overview
- PCI Roles and Responsibilities

---

- Payment Brand Compliance Programs
 -- The Founding Payment Brands

- American Express
  - Data Security Operating Policy (DSOP)
- Discover
  - Discover Information Security Security Compliance (DISC)
- JCB International
  - Data Security Program
- MasterCard
  - Site Data Protection (SDP)
- Visa Inc
  - Cardholder Information Securiy Program (CISP)
- Visa Europe
  - Account Information Security (AIS) Program

Payment Brands Compliance Programs include

1. Tracking and enforcement
2. Penalties, fees, compliance deadlines
3. Validation process and who needs to validate
4. Approval and posting of compliant entities
5. Definition of merchant and service provider levels

[Payment Brand Websites](https://pcissc.secure.force.com/faq/articles/Frequently_Asked_Question/How-do-I-contact-the-payment-card-brands?q=contact+brand&l=en_US&fs=Search&)

PCI DSS Validation Levels
Merchant Levels

- Defined by the payment brands based on transaction volume.
- Transaction volume determined by the acquirer

Service Provider Levels

- Defined by the payment brands according to transaction volume and/or type of service provider
- Determined by the payment brands or acquirer, or sometimes the service provider

Compliance Validation Requirements vary by the payment brand.

#### Merchant Levels

---

PCI DSS Validation Requirements Overview

### Merchants

|   | Level 1 | Level 2 | Levels 3 & 4 | 
| ----------- | ----------- | ----------- | ----------- |
| Type of Assessment: | Onsite Assessment | Self Assessment | Determined by Payment Brand or Acquirer |
| Reporting Requirements | ROC & ASV Scan Report | SAQ & ASV Scan Report | Determined by Payment Brand or Acquirer |

### Service Providers

|   | Level 1 | Level 2 | Levels 3 (American Express) | 
| ----------- | ----------- | ----------- | ----------- |
| Type of Assessment: | Onsite Assessment | Self Assessment | Self Assessment | 
| Reporting Requirements | ROC & ASV Scan Report | SAQ & ASV Scan Report | Determined by Payment Brand or Acquirer |

### Merchant Levels

| Payment Brand | Level 1 | Level 2 | Level 3 | Level 4 | 
|----------- | -----------| -----------| -----------| -----------|
|American Express |2.5M+ |50K - 2.5M|<50K |N/A  |
|Discover |6M+ |1M - 6M|20K+ 1M (Card Not Present)|N/A|
|JCB International |1M+ |< 1M |N/A |N/A|
|MasterCard |6M+ |1M+  - 6M |20K - <1M| N/A|
|Visa Inc.|6M+ |1M+ - <6M |20K+ <1M (e-Commerce)|20K< - <1M |
|Visa Europe |6M+ |1M+ - <6M |20K+ <1M (e-Commerce)|20K< - <1M |

### Merchant Validation Requirements

| Level | American Express | Discover | JCB International | MasterCard | Visa |
|----------- | -----------| -----------| -----------| -----------| -----------|
|1|Annual - Onsite - QSA - Quarterly Scan ASV |Annual - Onsite - QSA - Quarterly Scan ASV |Annual - Onsite - QSA - Quarterly Scan ASV |Annual - Onsite - QSA - Quarterly Scan ASV |Annual - Onsite - QSA - Quarterly Scan ASV - AOC|
|2|Annual SAQ - Quarterly ASV|Annual SAQ - Quarterly ASV|Annual SAQ - Quarterly ASV|Annual SAQ - Quarterly ASV|Annual SAQ - Quarterly ASV - AOC|
|3|Annual SAQ - Quarterly ASV|Annual SAQ - Quarterly ASV|N/A|Annual SAQ - Quarterly ASV|Annual SAQ - Quarterly ASV - AOC|
|4|N/A|Annual SAQ - Quarterly ASV|N/A|Annual SAQ - Quarterly ASV|Annual SAQ - Quarterly ASV - Visa Europe AOC|


### Self-Assessment Questionnaire (SAQ)

- SAQ is a validation tool to assist merchants and service providers in self-avluating their compliance with the PCI DSS.
- Multiple versions of the PCI DSS SAQ to meet various scenarios.
- PCI DSS SAQ is a validation tool for merchants and service providers not required to submit an onsite data security assessment Report on Compliance.

- SAQ-A
    - Card Not Present Transactions (eCom or Mail Order / Telephone Order)