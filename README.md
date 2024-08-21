# OSSVerse (Open Source Market place)

OSSVerse is an open source Marketplace. It is conceptualized as an eco system project comprising of multiple platforms. It is an adaptation of ONDC and Beckn protocol for open source software service delivery . OSSVerse leverages BeSecure(BeS) for delivering open source software security assurance services . OSSVerse aims to establish an open network of OASPs for businesses that will offer trustworthy and reliable open source software assurance services.

## Why an Open source Marketplace..

### State of open source in enterprise.

The widespread adoption of OSS (open source software) across industries has brought immense innovation but also unique security challenges. 
One of the barriers to OSS adoption is the lack of Trust.
Many organizations lack internal expertise to effectively assure and remediate open-source models, creating a demand for external services such as Open-source Assurance Service Providers (OASP).
Organizations require  timely support for open-source models, datasets, and projects. 

#### Consideration while adopting an Open source first Strategy
- Supply chain & Security Risks​
- Limited Control and support​
- Forking Costs​
- Incomplete Security​, Uncertain Reliability​
- Fragmented Knowledge​

## Solution to the problem
A Trustworthy Marketplace for Open-Source Assurance Service Providers (OASP) backed by a thriving open-source security community. Affordable and timely access to vendor neutral security services for organizations producing and consuming open-source. OASP led open source assurance service delivery would give full control over their  open source components

![Marketplace](./docs/images/marketplace.png)

## Key benefits to the enterprise client
OSS Consumers:
- Trustworthy Marketplace
- Access Affordable & prompt Vendor-Neutral Security Services
- Timely Support
- Full Control

OSS Producers:
- Enhanced Trust and Credibility
- Marketability
- Compliance and Standards
- Competitive Advantage
- Quality Assurance
- Legal Protection

## Key Stakeholders
1. Open Source Model Producers (Individuals & Organizations)
    - Create and share open source models
2. Open Source Model Consumers (Organizations)
    - Consume and request for assurance services of open source models 
3. Open Source Model Distributors (Platforms & Organizations)
    - Distribute the sharing of open-source models along with the proof of attestation of models OASP
4. Open Source Marketplace operator/consortia
    - Deploys people resources to maintain and operate marketplace and responsible for  the governance marketplace
5. Open Source Assurance Service Provider (OASP)
    - Provide Validation, Verification, Attestation & Support Service
    - Set up dedicated remediated pipelines for organizations
    - Validate models, create model cards & ensure quality/security
6. Security Experts & Freelancers
    - Offering open-source security assessments and support services

# FAQs on Registering and Evaluating OASPs in OSSVerse, TAVOSS Certification Process

## How do I register the first OASP when there are no OASPs registered?

Any organization or business interested in becoming an Open Source Assurance Provider (OASP) can initiate the registration process to join the OSSVerse open network. However, actual participation as an OASP is contingent upon the issuance of an OASP license. The process of registration effectively refers to the application for an OASP license. OSSVerse facilitates the issuance of OASP licenses for specific Projects of Interest (PoI) or Models of Interest (MoI) or their categories through dedicated OASP License Issuance Services. Initially, this service is provided directly by OSSVerse but may later be delegated to other ecosystem partners within the OSSVerse network who specialize in OASP license issuance and renewals.
To encourage organizations that have developed their own Open Source Software (OSS) projects to become OASPs for the OSS they have curated or seeded, OSSVerse highlights the potential monetary benefits. These benefits include remuneration for providing OSS security assurance and other support services. Additionally, OSSVerse incentivizes these organizations to engage in Assessment & Attestation services for technology PoIs and MoIs similar to their own, enhancing the verification and validation process within the network.

## How is the evaluation done when there are no OASPs with the capability to assess, despite having many registered OASPs?

In situations where the registered OASPs do not possess the skills or Projects of Interest (PoI) or Models of Interest (MoI) matching those required by a prospective OASP, the selection process becomes more open. The opportunity to curate a new BeSecure (BeS) Environment & BeS Playbook and to obtain an OASP license will be awarded to the entity that can do so at the lowest cost. It is essential for the OASP to indicate their openness to projects or models outside their current PoI and MoI and to apply for an OASP License for the new PoI or MoI as part of their service request. The additional costs associated with obtaining an OASP license can either be included in the service request or covered by the aspiring OASP. This approach ensures that even when existing OASPs lack certain capabilities, there remains a pathway for new and capable entities to join the OSSVerse as OASPs, thereby maintaining the network's growth and diversity.

## What happens when an OASP is not available with a POI and applies for OASP?

When an OASP without a Projects of Interest (POI) applies for an Open Source Assurance Provider (OASP) status, they must first publish an Open Source Assurance Report (OSAR) and obtain a TAVOSS Certificate issued by OSSVerse. The TAVOSS Certificate serves as proof of attestation by one or more OASPs, based on the OSAR report. For new projects or categories, BeSEnvironment & BeSPlaybooks need to be curated and published onto the marketplace BeSEnv & BeS Playbook Repos. The client, if aspiring to become an OASP, will receive the license in addition to the TAVOSS certificate, contingent on the attested report.

## Can Assurance Levels be tied to the quorum of Assessment?

Yes, Assurance Levels can potentially be tied to the quorum of Assessment. For instance, a client may opt for Assurance Level 1-2, which could be certified by a single OASP. For Assurance Level 3, a quorum of 3 OASPs would be required. However, the decision to tie assurance levels to the quorum has been postponed for future consideration. The certificate issued by OSSVerse is a proof of attestation by an OASP and does not directly reflect the quality of the Open Source Software (OSS). It indicates that the OASP has validated the BeS Environment & BeSPlaybooks for the project.

## What happens if an OSAR is unsatisfactory?

An unsatisfactory OSAR can result from either inadequate assessment or inherent problems within the project. In the case of inadequate assessment, neither a license nor a TAVOSS certificate will be issued. If the issue lies with inherent problems in the project, a license may still be granted, but not the TAVOSS certificate. This differentiation ensures that only projects meeting certain standards receive full certification.

## What is the process for issuing a TAVOSS Certification?

The issuance of a TAVOSS Certification is the final step in the process, conducted by the OSSVerse Certification service. This step comes after establishing the validity of all proofs submitted by OASPs, either individually or as part of a quorum (i.e., multi-party attestation). The certification is a testament that the OASP has validated the BeS Environment & BeSPlaybooks for the project, and that the execution and verification of the playbooks in the OSAR have been satisfactorily completed.

# FAQ: Understanding OSAR and Its Connection to Certificates and Attestation

## What is an OSAR?

An Open Source Assessment Report (OSAR) is the output produced by executing the BeSPlaybook. It serves as a detailed document that outlines the findings and outcomes of the assessment process.

## How does an OSAR differ from a certificate?

An OSAR is a comprehensive assessment report, while a certificate, specifically a TAVOSS Certificate, is an official recognition issued by OSSVerse. The certificate is awarded after validating the proof of attestation, which is derived from the OSAR, thereby certifying that the assessment meets certain predefined standards.

## What role does an OSAR play in the certification process?

The OSAR is crucial in the certification process as it provides the necessary evidence from which a proof of attestation is generated. This proof of attestation is then validated by the OSSVerse certification service, leading to the issuance of a TAVOSS Certificate.

## How is a TAVOSS Certificate issued based on an OSAR?

A TAVOSS Certificate is issued by OSSVerse once the proof of attestation, which is based on the evidence provided by the OSAR, is validated. This ensures that the assessment adheres to the standards set by OSSVerse.

## Are there any plans to evolve the format of the OSAR?

Yes, there are future plans to make the OSAR's output format compliant with an open attestation standard, such as the CycloneDX Attestation standard. This initiative aims to standardize the format for broader acceptance and interoperability.
