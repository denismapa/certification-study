# PCI ISA 3.2.1

- Certification Website
- <https://home.pearsonvue.com/pci>

- Training Website:
- <https://programs.pcissc.org/user/scorm_training/SCORM_Training_Sessions.aspx>

---

## PCI Fundamentals

### Chapter II: PCI SSC Overview

#### Module Topics

- PCI SSC & Standards Overview
- Payment Industry Terminology
- Payment Transaction Flow
- Service Provider Relationship

#### Module Objectives

After completing this module, you will be able to:

- Describe the role of the Payment Card Industry Security Standards Council
- Outline the Payment Card Industry Security Standards
- Describe the lifecycle followed for changes to standards
- Define Payment Card Industry terminology
- Define the processes involved in card processing: Authorization, Clearing, and Settlement
- Define service provider relationships

### What is the PCI SSC

- Definition
  - Payment Card Industry Security Standards Council (PCI SSC)
- Independent Industry Standards comprised of Several Payment brands.

  - American Express
  - Discover Financial
  - JCB International
  - MasterCard
  - Visa Inc.

### Resources Provided by the Council (PCI SSC)

#### Standards Overview

- PCI DSS
  - Payment Card Industry Data Security Standard
- PA-DSS
  - Payment Application Data Security Standard
- P2PE
- PTS (POI, HSM and PIN)
  - PCI PTS - POI
    - Payment Card Industy
    - PTS: Pin Transaction Security
    - POI: Point of Interaction
- Card Production and supporting Documents

#### Resources

- Roster of QSAs, PA-QSAs, PCIPs
- ASVs
- Validated Payment Applications
- PTS Devices
- P2P2E Solutions
- PCI Security Standards Council FAQs
- Education & Outreach Programs
- Participating Organization Membership
- Community Meetings (Annual)
- Feedback
- 600 Participating Organizations
  - Merchants
  - Financial Institutions
  - Service Providers
  - Vendors etcs

#### PCI Standards Overview

- PCI DSS
  - Payment Card Industry Data Security Standard
    - Covers Security of the environments that store, process or transmit account data.
- PCI PA-DSS
  - Payment Card Industry Payment Application Data Security Standard
    - Covers secure payment applications to support PCI DSS Compliance
      - Payment Application Receives account data from PIN entry Devices or other devices and begin payment transaction
- PCI P2PE
  - Covers Encryption, Decryption and Encryption Key Management Standards for PPP (Point to Point) Encryption Solutions
- PCI PTS - POI
  - This standard covers the protection of sensitive data at POI (Point of Interaction) devices
- PCI PTS - PIN Security
  - Secure management processing and transmittion of personal identification (PIN) during online and offline payment card transaction processing.
- PCI PTS - HSM
  - Hardware Security Modules
- PCI Card Production
  - Physical And Logical Security Requirements for systems and business processes.

#### PA-DSS

- Applies to Third-party payment applications
  - If application performs authorization and/or settlement (POS, Shopping carts, etc,)

- Ensures a payment application can function in a PCI DSS Compliant manner
- Use of PA-DSS application does not guarantee PCI DSS Compliance

- PA-DSS Applications are in scope for PCI DSS
  - Assessor must validate the payment application is installed:
  - Per Instructions in the PA-DS Implementation Guide provide by payment application vendor.
  - In a PCI DSS Compliance Manner

#### PCI Point-to-Point Encryption

- A PCI P2PE Solution must include all of the following:
  - Secure encryption of payment card data at the point-of-interaction (POI)
  - P2PE-validated Applications at the point-of-interaction
  - Secure management of encryption and decryption devices
  - Management of the decryption environment and all decrypted account data
  - Use of secure encryption methodologies and cryptographic key operations, including key generation, distribution, loading/injection, administration and usage

- Merchants may be able to reduce their PCI DSS Scope when using Council-listed P2PE solutions
  - Merchant has no access to account data within encryption device (POI) or decryption environment (at Solution Provider)
  - Merchant has no involvement in encryption or decryption operations, or cryptographic key management
  - All cryptographic operations managed by third party Solution Provider

#### PCI DSS: Relationship to PA-DSS and P2PE

Applies to all entities involved in payment card processing, and any entity that stores, processes, or transmits account data

- Applies to the following:
  - Merchants
  - Processors
  - Acquirers
  - Issuers
  - Service providers

- Also applies to any entity that performs the following:
  - Stores
  - Processes
  - Transmits

#### PCI PTS (PIN Transaction Security)

If a PTS Device is integrated into a POS or other payment systems implementation. The PTS Standard only applies to the PTS features and PA-DSS Applies to the Payment Application Features

PCI PTS Applies to the following:

- Attended Point-of-Sale Devices: Devices used at Cash Registers

- Encrypting Pin Pads which are used for unattended environments
  - Bank ATM Pin Pads

- Unattended payment terminals for Automated Fuel Dispensers and Kiosks

#### PCI PIN Security Requirements

- These requirements provide for secure PIN:
  - management
  - processing
  - transmission

- Protection of personal identification number (PIN) data during online and offline payment card transaction processing at:
- ATMs
- attended point-of-sale (POS) terminals
- unattended point-of-sale (POS) terminals

- The Requirements also pvoide guidance on key management and key handling associated with the PIN

#### PCI DSS and PCI PTS Standards

##### PCI DSS

- Requires that account data be protected both when stored and when transmitted across open public networks
- Payment Card Industry (PCI) Pin Transaction Security (PTS) Point-of-Interaction (POI) validates how POIs protectPIN and account data and manage cryptographic keys
- PCI PTS POI-approved devices may form part of a PCI DSS compliant environment.

##### PCI PTS - Pin Security Standard and PCI DSS

- PCI DSS Prohibits storage of encrypted PIN Blocks
- No Overlap

##### PCI Card Production and PCI DSS

- No Overlap
- Procedures for assessing card production facilities are defined and managed by the payment brands not by PCI SSC

##### PCI PTS - HSM and PCI DSS

- PCI DSS requires that stored cardholder data be protected and cryptographic keys be managed in a secure manner
- User of a Hardware Security Module is not required by PCI DSS but may help with managing keys used to protect stored CHD (Card holder data)

### Payment Industry Terminology

Payment Network Flow

- Authorization
  - Merchant Requests and Receives Authorization

- Clearing
  - Issuer and Acquirer exchange purchase and reconciliation information

- Settlement
  - Issuer pays Acquirer
  - Merchant receives payment
  - Cardholder gets charged

##### Terminology

- Cardholder
  - Customer purchasing goods either as a "Card Present" or "Card Not Present" transaction
  - Receives the payment card and bills the issuer

- Issuer
  - Bank or other orgs issuing a payment card on behalf of a Payment Brand (MasterCard & Visa)
  - Payment brand issuing a payment card directly (e.g. Amex, Discover, JCB)

- Merchant
  - Organization accepting the payment card for payment during a purchase

- Acquirer
  - Bank or entity the merchant uses to process their payment card transactions
  - Receive authorization requets from merchant and forward to Issuer for approval
  - Provide authorization, clearing and settlement services to merchants

Acquirer's are also called the following:

- Merchant Bank
- ISO (Sometimes)
- Payment Brand
  - Amex (American Express)
  - Discover
  - JCB
  - Never Visa or MasterCard

AMEX / DISCOVER / JCB

- They are Issuers and Acquirers
- Closed Loop

VISA / MASTERCARD

- Open Loop

#### Card Procesing - Authorization

1. Cardholder Presents Card
2. Acquirer asks payment brand to determine issuer
3. Payment Brand Network determines issuer and requests approval
4. Issuer approves purchase
5. Payment Brand network sends approval to acquirer
6. Acquirer sends approval to merchant

#### Card Processing - Clearing

1. Acquirer sends purchase information to the payment brand network
2. Payment brand network sends purchase information to issuer

- Issuer Prepares data for cardholder statement

3. Payment Brand Network provides complete reconciliation to acquirer

#### Card Processing - Settlement

1. Issuer determines acquirer via the payment brand network
2. Issuer sends payment to acquirer
3. Acquirer pays merchant for cardholder's purchase
4. Issuer bills Cardholder

#### Service Providers

- A business that is not a payment brand, directly involved in the processing, storage or transmission of cardholder data on behalf of another entity.
  - Sometimes a service provider is a merchant

- Includes companies that provide services (to merchants, service providers or entities) which control or could impact the security of cardholder data.

###### Working with Service Providers

- Entities often use a third-party service provider to store, process, or transmit cardholder data on their behalf, or to manage components of their CDE.
  - There are two options for third-party service providers to validate compliance
    - 1 - Undergo a PCI DSS assessment on their own and provide evidence to their customers demonstrating their compliance; or
    - 2 - Have their services reviewed during the course of each of their customers??? PCI DSS assessments

- Entities using hosting facility; the hosting facility will need to provide evidence (AOC) that they are PCI Compliant

- Providing access to public connection like an ISP
  - Is not considered in-scope

- 12.9 - Maintain a Template to provide to their Clients.
- Service Providers must agree to maintain all applicable PCI DSS Controls

#### Service Provider Terms

TPP = Third Party Processor
PSP = Payment Service Proviers
DSE = Data Storage Entity
VNP = VisaNet Processor

1. American Express - TPP
2. Discover - TPP & PSP
3. JCB International - TPP
4. MasterCard - TPP & DSE
5. Visa - VNP