---
type: Module
title: 'Module H: Full Quality Assurance'
description: Comprehensive conformity assessment based on full quality assurance covering
  design, manufacturing, final inspection, and testing.
category: module
tags:
- nlf
- module
- module-h
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
  provision: Annex II, Module H
  checked_at: '2026-09-27T00:00:00Z'
---

# Summary

**Module H (Full Quality Assurance)** is the most comprehensive single-module conformity assessment procedure under Annex II of Decision No 768/2008/EC[^decision-768-2008-ec][^blue-guide-2022].

Module H covers both the **design phase** and the **production phase** through a notified body audit of the manufacturer's total quality management system. It eliminates the need for a separate Module B type examination, providing maximum flexibility for manufacturers with continuous development and deployment cycles (such as software updates).

# Requirements for Full Quality Assurance

### 1. Quality System Scope (Point 3)
The manufacturer must operate an approved quality system covering:
- **Design Control**: Design specifications, cybersecurity threat modeling, secure coding standards, and design verification methods.
- **Manufacturing & Build Controls**: Continuous integration pipelines, reproducible build environments, and component inventory controls.
- **Testing & Quality Assurance**: Static analysis (SAST), software composition analysis (SCA), dynamic testing (DAST), and regression suites.

### 2. Notified Body Audit & Surveillance
- **Initial Assessment**: Complete audit of design offices and manufacturing/build facilities.
- **Periodic Surveillance**: Continuous verification of quality records, design changes, and vulnerability handling workflows.
- **Unannounced Visits**: The notified body may perform unannounced inspections and run independent verification tests.

# Strategic Importance in the Cyber Resilience Act
Under CRA Article 32(3), manufacturers of Important Class II products (e.g. firewalls, hypervisors, tamper-resistant microprocessors) can choose Module H as an alternative to Module B+C, allowing agile software development without submitting every release for external type re-certification.

# Related concepts
- [Modules Index](index.md)
- [Module H1: Full Quality Assurance plus Design Examination](module-h1.md)
- [Module B: EU-Type Examination](module-b.md)
- [Module D: Production Quality Assurance](module-d.md)
[^decision-768-2008-ec]: European Parliament and Council, Decision No 768/2008/EC, https://eur-lex.europa.eu/eli/dec/2008/768/oj
[^blue-guide-2022]: European Commission, Blue Guide 2022, https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=uriserv%3AOJ.C_.2022.247.01.0001.01.ENG
