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

## OASP Services

**1. Assurance & Assessment Service:** Open-source software undergoes rigorous evaluation for security, compliance, and quality, culminating in comprehensive reports and proof of attestation to ensure trustworthiness. 

**1.1 Assurance Levels & Services**

Based on the depth and scope of the assessment required, different assurance levels are offered, each encompassing specific checks and activities:

| Assurance Level | Description                                                             | Key Emphasis/Requirement                                                                                | Example Checks/Activities                                                                        |
|----------------|-------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------|
| 0              | No Assurance                                                         | No formal assessment                                                                                  | - Project information gathering                                                                 |
| 1              | Basic Assurance                                                       | Basic automated security checks, with proof of attestation                                       | - SAST (static code analysis)                                                              |
| 2              | Standard Assurance                                                    | Everything in Basic (including proof of attestation) + Dependency & license compliance checks           | - Dependency vulnerability checks <br> - License compliance audit <br>- SAST                      |
| 3              | Comprehensive Assurance                                               | Everything in Standard (including proof of attestation) + Dynamic and manual security review          | - Dynamic application security testing (if applicable) <br> - Expert code review (optional) <br>- Fuzzing  |
| 4              | Domain-Specific Assurance                                          | Everything in Comprehensive (including proof of attestation) + Industry-specific safety and security checks  | - Adherence to e.g. ISO 26262 and other domain specific standards. <br> - Hardware-in-the-loop (HIL) testing. <br> - Fuzzing and symbolic execution. |

**1.2 Open-Source Software (OSS) Assurance Service Checklist**

This checklist outlines the key steps involved in assessing the security, quality, and compliance of open-source software, especially in the automotive domain.

**1.2.1 Standard Checks**

| Assurance Check Category   | Subcategory (Intent)                     | BeS Env Name                             | Example Playbook Name                                                   | Open-Source Tools                                             |
| -------------------------- | ---------------------------------------- | -------------------------------------------- | ------------------------------------------------------------ | --------------------------------------------------------- |
| SAST (Static Analysis)    | Security Vulnerability Scan              | `besman-code_analysis-env.sh`                  | `besman-sast-sonarqube-playbook.sh`, `besman-sast-codeql-playbook.sh` | SonarQube (Community Edition), PVS-Studio, CodeQL, Semgrep, Bandit, ESLint, Pylint |
| DAST (Dynamic Analysis)   | Security Vulnerability Scan              | `besman-dynamic_analysis-env.sh`          | `besman-dast-zap-playbook.sh`                                   | OWASP ZAP, Arachni, Nikto, w3af, Burp Suite |
| Dependency Analysis       | Dependency Vulnerability Check         | `besman-dependency_analysis-env.sh`           | `besman-dependency_check-playbook.sh`                          | OWASP Dependency-Check, Retire.js, Synk, WhiteSource         |
| Licensing & Compliance    | License Compliance Audit                | `besman-legal_compliance-env.sh`               | `besman-license_compliance-fossology-playbook.sh`               | FOSSology, LicenseFinder, ScanCode, Toolkit                   |
| Code Quality Analysis     | Code Quality Assessment                 | `besman-code_analysis-env.sh`                   | `besman-code_quality-sonarqube-playbook.sh`                    | SonarQube (Community Edition), PMD, Checkstyle, FindBugs |

**1.2.2 Automotive-Specific Checks**

| Assurance Check Category | Subcategory (Intent) | BeS Env Name | Example Playbook Name | Open-Source Tools |
|---|---|---|---|---|
| Safety Assurance | Functional Safety Assessment | `besman-safety_critical-env.sh` | `besman-safety_assurance-latte-playbook.sh` | Frama-C, CBMC, SPIN, LATTE |
| Security for Autonomous Driving | Adversarial ML & Security Assessment | `besman-security_assessment_env.sh` | `besman-autonomous_driving_security-carla_art-playbook.sh` | CARLA Adversarial Robustness Toolbox (ART), OpenSCENARIO |
| Real-Time Performance | Real-Time Performance Analysis | `besman-safety_critical-env.sh` | `besman-real_time_performance-cyclictest-playbook.sh` | `cyclictest` |
| Data Privacy & Security | Data Privacy Assessment | `besman-security_assessment_env.sh` | `besman-data_privacy-openssl-playbook.sh` | OpenSSL, GPG |
| Interoperability & Compatibility | Protocol Conformance Testing | `besman-network_simulation_env.sh` | `besman-protocol_conformance-cantools-playbook.sh` | Cantools, OpenXC |
| Hardware Integration | HIL Testing | `besman-hardware_integration-env.sh` | `besman-hardware_integration-renode-playbook.sh` | Renode, QEMU |
| Additional Checks | Deep Vulnerability Scan | `besman-symbolic_execution_fuzzing-env.sh` | `besman-fuzzing-afl-playbook.sh` | KLEE (Symbolic Execution), AFL (Fuzzing), Flawfinder, cppcheck |

**1.3 Proof of Attestation**

| Assurance Check Category | BeS Env Name | Example Playbook Name | Open-Source Tools |
|---|---|---|---|
| Attestation | `besman-secure_artifact_signing-env.sh` | `besman-artifact_signing-playbook.sh` | Sigstore, in-toto framework (OpenSSF), The Update Framework (TUF) |

**Note:**  Playbook names are provided in a generic way to emphasize their reusability across different projects. The actual playbook implementation would need to handle project-specific configurations and inputs. 

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






