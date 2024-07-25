# **OSSVerse**

## 1. Business Context 

OSSVerse is an open source Marketplace. It is conceptualized as an eco system project comprising of multiple platforms. It is an adaptation of ONDC and Beckn protocol for open source software service delivery . OSSVerse leverages BeSecure(BeS) for delivering open source software security assurance services . OSSVerse aims to establish an open network of OASPs for businesses that will offer trustworthy and reliable open source software assurance services. 

## 1.2 Business Architecture 

1.2.1 **Marketplace Services** 

1.2.1.1 Onboarding services :
   
   ### **Account Creation:**
   
   **OASP**
   
   Creating an OSSVerse Account & OASP profile for OASP 
   The Account creation service will register OASP with OSSVerse Registry and have APIs to update the OASP profile. An OASP profile will have informed related to payments and BAP Seller App end points (e.g instance of BAP compatible adaptation of a BeSLab )
   
   **Business**
   
   Creating an OSSVerse Account for a Business 
 
 1.2.1.2 Search: 
    **Business**
    a) A Business who is a consumer of Open source
    Searching for OASP , open source component and open source support services like 
    1. Open source assessment & Attestation services (Subscription based)
    2. Open source remediation Services (On Demand)
    3. Open source feature enhancement Services (On Demand)

    b) A Business who is a Producer or Distributor of Open source
    Searching for an OASP for an identified open source component for certification (On Demand)

**OASP Services**

1. **Assessment/Assurance Service**:
   1. X checklist for OSS with pointer to Standard check list e.g of checklist

      1. OSS Pol, Mol or TDol are
         1. SAST checks
         2. DAST checks
         3. Compliance checks
         4. Industry specific checks
         5. Other checks..
      2. OSAR Generation and Proof of Attestation as evidence to be shared

2. **Validation & Verification Service**: (validated & verify if attestation has been done in line with the acceptable OSSVerse OASP Assessment Standard)

      1. Check BeS Environments (Exists/Linting)
      2. Check Playbooks w.rt each Check part of Assessment claimed.
      3. OSAR(Open source assessment/attestation Report) updated with Proof of Verfication & Validation as evidence to be shared (This could be inline with an accept standard like Attestation standard like CycloneDX Attestation standard)

3. **Remediation Service**:
4. **Pentesting Service**:
5. **Feature Addition**:
6. **TAVOSS Version & Certification Service**: (Certification with or without/Distribution?/hosting?)
  
**Business Support Services**

# Technical Architecture

# Communication between BeSlab & OSSVerse

# OSSVerse as A BAP/BG/Open Network Registry

![Component Diagram](/docs/images/component-diagram.png)

# OASP as BPP 

  Extending BeSLab as a BPP

# BeS : Establish provenance & presentation of Proofs
  
# BeS : OSAR 






