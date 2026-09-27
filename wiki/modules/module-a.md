---
type: Module
title: 'Module A: Internal Production Control'
description: Conformity assessment procedure whereby the manufacturer ensures and
  declares compliance without notified body intervention.
category: module
tags:
- nlf
- module
- module-a
- decision-768-2008-ec
status: draft
generated:
  by: agent:antigravity
  at: '2026-09-27T00:00:00Z'
stale_after: '2027-12-31T00:00:00Z'
sources:
- id: decision-768-2008-ec
  resource: https://eur-lex.europa.eu/eli/dec/2008/768/oj
  title: Decision No 768/2008/EC on a common framework for the marketing of products
  author: European Parliament and Council of the European Union
  last_modified: '2008-07-09T00:00:00Z'
- id: blue-guide-2022
  resource: https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=uriserv%3AOJ.C_.2022.247.01.0001.01.ENG
  title: "Commission Notice \u2014 The 'Blue Guide' on the implementation of EU product\
    \ rules 2022"
  author: European Commission
  last_modified: '2022-06-29T00:00:00Z'
x-conformity-assessment:
  jurisdiction: EU
  authority_level: binding
  instrument_status: in_force
  provision: Annex II, Module A
  checked_at: '2026-09-27T00:00:00Z'
---

# Summary

**Module A (Internal Production Control)** is the baseline self-assessment conformity assessment procedure established under Annex II of Decision No 768/2008/EC[^decision-768-2008-ec] and detailed in the European Commission's Blue Guide[^blue-guide-2022].

Under Module A, the manufacturer independently verifies, ensures, and declares that the products concerned satisfy the essential requirements of the applicable Union harmonization legislation, assuming sole legal responsibility without third-party notified body involvement.

# Procedural Architecture & Workflow

```
+-------------------------------------------------------------+
| 1. Technical Documentation (Annex II Module A Point 2)      |
| - General description, conceptual design, component BOM     |
| - Applied harmonised standards or alternative solutions     |
| - Cybersecurity risk assessment & vulnerability records     |
+-------------------------------------------------------------+
                               |
                               v
+-------------------------------------------------------------+
| 2. Manufacturing Control (Point 3)                          |
| - Ensure manufacturing process & monitoring maintain        |
|   compliance of every manufactured unit with technical docs |
+-------------------------------------------------------------+
                               |
                               v
+-------------------------------------------------------------+
| 3. CE Marking & EU Declaration of Conformity (Point 4)      |
| - Affix CE marking to each individual product or packaging  |
| - Draw up written EU Declaration of Conformity              |
| - Keep docs available for market surveillance for 10 years  |
+-------------------------------------------------------------+
```

# Applicability & Restrictions across EU Cyber Law

- **Cyber Resilience Act (CRA)**: Permitted strictly for **Default Products** with digital elements (Article 32(1)). Prohibited for Important Class I, Important Class II, and Critical products.
- **AI Act (Regulation (EU) 2024/1689)**: Prescribed under Article 43(1) as the default conformity route for high-risk AI systems listed in Annex III, provided harmonized standards or common specifications exist.
- **Radio Equipment Directive (RED 2014/53/EU)**: Permitted when the manufacturer has fully applied harmonized standards covering Article 3(1) and 3(2).

# Related concepts
- [Modules Index](index.md)
- [Module A1: Internal Production Control plus Supervised Testing](module-a1.md)
- [Module B: EU-Type Examination](module-b.md)
- [Decision 768/2008/EC](../law/decision-768-2008-ec.md)
[^decision-768-2008-ec]: European Parliament and Council, Decision No 768/2008/EC, https://eur-lex.europa.eu/eli/dec/2008/768/oj
[^blue-guide-2022]: European Commission, Blue Guide 2022, https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=uriserv%3AOJ.C_.2022.247.01.0001.01.ENG
