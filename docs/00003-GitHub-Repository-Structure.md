# GitHub Repository Structure for UniCORE AI

**(This is the exact structure you should publish.)**

Author: Bryan Fred, Unitek Systems Limited, Bedford, United Kingdom
First published: May 2026
Status: Public. Given, not sold. Irrevocable.

---

unicore-ai/

│

├── README.md

├── LICENSE

├── CONTRIBUTING.md

├── CODE_OF_CONDUCT.md

│

├── docs/

│   ├── whitepaper/

│   │   ├── UniCORE_AI_Whitepaper.pdf

│   │   ├── UniCORE_AI_Whitepaper.md

│   │   └── diagrams/

│   │       ├── unicore-12-level-architecture.png

│   │       ├── truth-flow-diagram.png

│   │       ├── governance-boundaries.png

│   │       └── heartbeat-prohibition.png

│   │

│   ├── foundation/

│   │   ├── TrueAI_Foundation.md

│   │   ├── No_Self_Creation_Rule.md

│   │   ├── Reasonable_Governance_Threshold.md

│   │   ├── Human_Governance_Level12.md

│   │   └── Governance_Principles.md

│   │

│   ├── governance-md/

│   │   ├── Country_Governance_Template.md

│   │   ├── State_Governance_Template.md

│   │   ├── Tax_Governance_Template.md

│   │   ├── Compliance_Governance_Template.md

│   │   └── Mission_Governance_Template.md

│   │

│   ├── architecture/

│   │   ├── UniCORE_12_Levels.md

│   │   ├── Level_Descriptions/

│   │   │   ├── Level01_Truth.md

│   │   │   ├── Level02_Evidence.md

│   │   │   ├── Level03_Verification.md

│   │   │   ├── Level04_Context.md

│   │   │   ├── Level05_Interpretation.md

│   │   │   ├── Level06_Governance.md

│   │   │   ├── Level07_Compliance.md

│   │   │   ├── Level08_Operations.md

│   │   │   ├── Level09_Execution.md

│   │   │   ├── Level10_Audit.md

│   │   │   ├── Level11_Stability.md

│   │   │   └── Level12_Human_Governance.md

│   │   └── Inter-Level_Communication.md

│   │

│   └── roadmap/

│       ├── UniCORE_Roadmap_2026_2030.md

│       ├── UniCORE_Roadmap_2030_2035.md

│       ├── UniCORE_Roadmap_2035_2041.md

│       └── Space_Mission_Roadmap.md

│

├── src/

│   ├── UniCORE.Foundation/

│   │   ├── TrueAIEngine.cs

│   │   ├── GovernanceEngine.cs

│   │   ├── EvidenceEngine.cs

│   │   └── ValidationEngine.cs

│   │

│   ├── UniCORE.Levels/

│   │   ├── Level01Truth/

│   │   ├── Level02Evidence/

│   │   ├── Level03Verification/

│   │   ├── Level04Context/

│   │   ├── Level05Interpretation/

│   │   ├── Level06Governance/

│   │   ├── Level07Compliance/

│   │   ├── Level08Operations/

│   │   ├── Level09Execution/

│   │   ├── Level10Audit/

│   │   ├── Level11Stability/

│   │   └── Level12Human/

│   │

│   ├── UniCORE.Governance/

│   │   ├── MDFileParser.cs

│   │   ├── GovernanceValidator.cs

│   │   ├── ThresholdEngine.cs

│   │   └── DriftDetection.cs

│   │

│   ├── UniCORE.Prototype/

│   │   ├── XAF/

│   │   │   ├── UniCORE.Module/

│   │   │   ├── UniCORE.Module.Win/

│   │   │   ├── UniCORE.Module.Blazor/

│   │   │   └── UniCORE.WebAPI/

│   │   └── Database/

│   │       ├── XPO_Models/

│   │       └── SQL_Schema/

│   │

│   └── UniCORE.Tests/

│       ├── UnitTests/

│       ├── IntegrationTests/

│       ├── GovernanceTests/

│       └── DriftDetectionTests/

│

├── examples/

│   ├── GovernanceMD/

│   ├── CountryRules/

│   ├── TaxRules/

│   ├── ComplianceRules/

│   └── SpaceMissionRules/

│

└── tools/

    ├── MDValidator/

    ├── GovernanceCompiler/

    └── TruthCheckCLI/

Explanation of Why This Structure Works

✔ Clear separation of concerns

docs/ for governance, architecture, whitepapers

src/ for code

examples/ for templates

tools/ for validators and compilers

✔ Enterprisegrade layout

Matches Microsoft, OpenAI, and Anthropic repository patterns.

✔ Supports longterm evolution

This structure can last 20+ years.

✔ Supports collaboration

Researchers, engineers, and governance experts can work independently.

✔ Supports publication

Whitepaper + diagrams + MD files are cleanly organised.

C is complete.

Shall I proceed to D — the Public Announcement Draft?

---

## Document history

- 2026-05-08 (7f420f6) — Initial commit: UniVERSE Foundation Documents (56 docs + Full Formal Statement)
- 2026-05-08 (189f14e) — Renumber 56 docs 001-056 for clean timeline sort order
- 2026-05-13 (fbebe5b) — docs: rename all 56 docs to 5-digit numeric codes, drop letter codes
- 2026-05-13 (c6a685b) — docs: Path-1 mechanical style pass on all numbered docs
- 2026-05-13 (a335662) — docs: strip stale star markers and legacy letter-code body references
- 2026-05-22 (9bcde37) — docs: complete version-marker sweep across public corpus

*Back-filled from git log on 2026-07-10 21:35 UTC. Kind 2 versioning (dated change notes) — see HORIZON.md § Evolution and versioning. Kind 1 (formal `Version:` bumps) remains OFF until first GitHub Discussion.*
