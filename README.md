# Conformity Assessment Knowledge Base

An English-language [Open Knowledge Format (OKF)](https://github.com/GoogleCloudPlatform/knowledge-catalog/blob/main/okf/SPEC.md) bundle covering conformity assessment in the EU: the New Legislative Framework, the conformity assessment modules of Decision 768/2008/EC, accreditation under Regulation (EC) No 765/2008, notification and notified bodies, market surveillance, cybersecurity certification schemes under the Cybersecurity Act, and how sector laws such as the Cyber Resilience Act and the AI Act use them.

The bundle will contain concise original summaries with provision-level citations to primary sources. It does not reproduce full legal instruments, rules, guidance documents, or standards.

Current release: **none yet** (`VERSION` 0.0.0)

> **Scaffold:** the manifest, section structure, validator and registers are in place. No concepts have been ingested yet; every section index describes what will go there.

> **General orientation only:** once populated, do not rely on this knowledge base for decisions that determine, demonstrate, or materially affect legal or regulatory compliance. Verify the current primary sources and obtain qualified professional advice before making module-selection, accreditation, notification, certification, market-access, or other compliance-impacting decisions.

## Use With Meerkat

[Meerkat](https://github.com/zegit-zoo/meerkat) can serve the bundle as CLI, MCP, or HTTP without conversion:

```sh
mk --kb-dir . search "module B type examination"
mk --kb-dir . show modules/module-b
mk --kb-dir . list --category law
mk --kb-dir . mcp serve
mk --kb-dir . http serve --port 4004
```

Run these commands from the repository root. The knowledge bundle itself is under `wiki/`; Meerkat's `--kb-dir` reads that content-repository layout. The paths above are the planned concept IDs and resolve once ingestion has reached them.

The Markdown remains usable without Meerkat or any other tool.

## Coverage

The intended corpus includes:

- Regulation (EC) No 765/2008, Decision 768/2008/EC, Regulation (EU) 2019/1020, Regulation (EU) No 1025/2012, the Cybersecurity Act and the EUCC implementing regulation;
- the 16 conformity assessment modules and their sector variants;
- accreditation, notification, NANDO, surveillance and certificate lifecycle procedures;
- the ISO/CASCO standards as identifiers and scope;
- the Blue Guide, EA and coordination-group guidance;
- notifying and accreditation authorities for the 27 Member States and EEA status;
- how the CRA, the AI Act and other sector laws use the framework.

Coverage is measured in `coverage.yaml`. Each gate names a glob over `wiki/`, the expected number of concepts where the corpus is finite, and the count actually present. A missing official source is recorded as a research gap rather than filled by inference.

## Structure

`kb.yaml` declares the bundle's slug, extension key (`x-conformity-assessment`), categories and sections. Every section has an `index.md` describing what belongs there.

| Section | Contents |
|---|---|
| [`law/`](wiki/law/index.md) | Horizontal instruments of the New Legislative Framework and the sector laws that build on them. |
| [`modules/`](wiki/modules/index.md) | The conformity assessment modules of Decision 768/2008/EC Annex II, one page per module, with the sector variants that reference them. |
| [`procedures/`](wiki/procedures/index.md) | How bodies become and stay competent, and how assessment and certificates work. |
| [`roles/`](wiki/roles/index.md) | Manufacturer, authorised representative, importer, distributor, conformity assessment body, notified body, notifying authority, national accreditation body, EA, market surveillance authority, the Commission. |
| [`standards/`](wiki/standards/index.md) | The ISO/CASCO toolbox and its European adoptions, recorded as identifiers, scope and links. |
| [`schemes/`](wiki/schemes/index.md) | Certification schemes that sit beside notified-body assessment. |
| [`guidance/`](wiki/guidance/index.md) | Official non-binding guidance. |
| [`jurisdictions/`](wiki/jurisdictions/index.md) | Each Member State's notifying authorities and national accreditation body, with the sector designations that matter for cybersecurity and AI. |
| [`timeline/`](wiki/timeline/index.md) | The 2008 framework, Regulation (EU) 2019/1020 application, the Cybersecurity Act, EUCC, the CRA Chapter IV date, the AI Act and Machinery Regulation notified-body dates. |
| [`glossary/`](wiki/glossary/index.md) | Terms defined in Regulation (EC) No 765/2008, Decision 768/2008/EC, Regulation (EU) 2019/1020 and ISO/IEC 17000. |

## Source And Publication Policy

- Binding claims cite OJEU, ELI, EUR-Lex, an official national gazette, or the Commission's NANDO database for notification status.
- Official guidance is labelled non-binding.
- A standard provides presumption of conformity only when its reference is cited in the OJEU for the requirements concerned.
- Publicly accessible drafts are linked, not copied.
- Sector laws are summarised only for their conformity-assessment provisions; the CRA and AI Act bundles in this series hold the rest.
- Notification status of a body is cited from NANDO with the date checked; the bundle does not list individual bodies as concepts.
- Agent-generated content stays `status: draft` until a human verifies it against the cited source.
- Superseded material is retained and marked rather than silently deleted.

This repository is not legal advice, is not a conformity assessment, does not certify any product or organisation, and must not be used as the basis for compliance-impacting decisions.

## Validate

```sh
python3 -m pip install -r requirements-dev.txt
python3 -m unittest tools/test_validate.py
python3 tools/validate.py wiki
```

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). Corrections with exact primary-source citations are welcome. Do not submit copied standards text, private compliance evidence, or confidential information.

## Related Knowledge Bases

- [CRA-knowledge-base](https://github.com/JonasLundin/CRA-knowledge-base): Regulation (EU) 2024/2847, the Cyber Resilience Act
- [NIS2-knowledge-base](https://github.com/JonasLundin/NIS2-knowledge-base): Directive (EU) 2022/2555 and its national transpositions
- [CVD-knowledge-base](https://github.com/JonasLundin/CVD-knowledge-base): coordinated vulnerability disclosure, the CVE Program, CSAF, VEX and scoring
- [AI-Act-knowledge-base](https://github.com/JonasLundin/AI-Act-knowledge-base): Regulation (EU) 2024/1689 as amended
- [Software-Supply-Chain-knowledge-base](https://github.com/JonasLundin/Software-Supply-Chain-knowledge-base): SBOM formats, attestation, provenance and VEX
- [NIST-CSF-knowledge-base](https://github.com/JonasLundin/NIST-CSF-knowledge-base): NIST Cybersecurity Framework 2.0
- [knowledge-base-template](https://github.com/JonasLundin/knowledge-base-template): the shared template every bundle in the series is built from

## Licence

Original summaries, structure, and metadata are licensed under [CC BY 4.0](LICENSE). Source documents, rules, specifications and standards retain their own terms; see [NOTICE](NOTICE).

This project is independent and is not affiliated with or endorsed by the European Commission, ENISA, the European co-operation for Accreditation, any national accreditation body or notifying authority, any notified body, ISO, IEC, CEN, CENELEC, Google Cloud, or Meerkat. Repository: https://github.com/JonasLundin/Conformity-Assessment-knowledge-base
