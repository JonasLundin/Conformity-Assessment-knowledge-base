---
type: Scheme
title: 'EUCC: European Common Criteria Cybersecurity Certification Scheme'
description: Union candidate cybersecurity certification scheme based on Common Criteria
  (ISO/IEC 15408) for ICT products.
category: scheme
tags:
- scheme
- cybersecurity-act
- eucc
- certification
status: draft
generated:
  by: agent:antigravity
  at: '2026-09-27T00:00:00Z'
stale_after: '2027-12-31T00:00:00Z'
sources:
- id: csa-regulation
  resource: http://data.europa.eu/eli/reg/2019/881/oj
  title: Regulation (EU) 2019/881 on ENISA and on information and communications technology
    cybersecurity certification (Cybersecurity Act)
  author: European Parliament and Council of the European Union
  last_modified: '2019-04-17T00:00:00Z'
x-conformity-assessment:
  jurisdiction: EU
  authority_level: guidance
  instrument_status: in_force
  provision: Cybersecurity Act Title III
  checked_at: '2026-09-27T00:00:00Z'
---

# Summary

The **European Common Criteria Cybersecurity Certification Scheme (EUCC)** is the first official European cybersecurity certification scheme adopted under **Regulation (EU) 2019/881 (Cybersecurity Act)** via Commission Implementing Regulation (EU) 2024/482[^csa-regulation].

EUCC establishes a harmonized, Union-wide certification framework for ICT products, replacing disparate national schemes (such as the SOG-IS agreement) with certificates recognized across all EU Member States.

# Technical Architecture & Evaluation Levels

```
+-------------------------------------------------------------+
|                      EUCC Scheme Levels                     |
|                                                             |
|   +--------------------------+  +------------------------+  |
|   |   Assurance Level:       |  |  Assurance Level:      |  |
|   |      SUBSTANTIAL         |  |         HIGH           |  |
|   |  - AVA_VAN.1 / AVA_VAN.2 |  | - AVA_VAN.4 / AVA_VAN.5|  |
|   |  - Basic penetration     |  | - Advanced resistance  |  |
|   |    resistance            |  |   against state actors |  |
|   +--------------------------+  +------------------------+  |
|                                                             |
+-------------------------------------------------------------+
```

### Key Operational Characteristics
- **Evaluation Standard**: Based on Common Criteria v3.1 / ISO/IEC 15408 and Common Evaluation Methodology (CEM / ISO/IEC 18045).
- **Vulnerability Handling & Patch Management**: Incorporates mandatory requirements for manufacturers to maintain active CVD programs and manage patch updates for certified products.
- **Interoperability with CRA**: EUCC certificates at assurance level 'substantial' or 'high' confer a direct presumption of conformity for products with digital elements under Article 27 of the Cyber Resilience Act.

# Related concepts
- [ISO/IEC 17065 Standard](../standards/iso-iec-17065.md)
- [ISO/IEC 17025 Standard](../standards/iso-iec-17025.md)
- [Certificate Issuance Procedure](../procedures/certificate-issuance.md)
- [Cybersecurity Act Regulation](../law/regulation-eu-2019-881.md)
[^csa-regulation]: European Parliament and Council, Cybersecurity Act, http://data.europa.eu/eli/reg/2019/881/oj
