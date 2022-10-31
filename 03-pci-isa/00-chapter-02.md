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

