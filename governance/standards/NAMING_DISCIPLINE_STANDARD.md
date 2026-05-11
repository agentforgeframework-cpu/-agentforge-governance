# AgentForge Naming Discipline Standard

Status: DRAFT  
Version: 0.1  
Authority: HIC-001_Human-in-Command_Standard.md

---

# Purpose

This standard defines practical naming discipline for the AgentForge ecosystem.

The goal is to reduce:
- operational confusion
- portability failures
- governance ambiguity
- vocabulary drift
- maintenance friction
- unnecessary renaming churn

This standard is intended to remain:
- lightweight
- understandable
- portable
- operational
- maintainable
- “2 AM engineer” friendly

---

# Core Principle

> Names should reflect what something IS and/or DOES.

---

# Operational Naming Philosophy

Names should:
- describe function
- support maintainability
- remain understandable under operational stress
- favor clarity over cleverness
- favor stability over novelty
- remain portable across systems and tools

Avoid:
- marketing-style naming
- unnecessary abstraction
- semantic inflation
- forced cleverness
- unnecessary acronym creation
- vocabulary drift

If a simpler name works:

> prefer the simpler name.

---

# Scope

This naming discipline applies only to official AgentForge ecosystems and repositories.

External projects are free to:
- follow these standards
- adapt them
- ignore them

---

# Human Authority

AI systems may suggest names.

Humans retain naming authority.

Final naming decisions remain under:

`agentforgeframework-cpu/-agentforge-governance/governance/HIC-001_Human-in-Command_Standard.md`

---

# Semantic Stability Doctrine

Operational terminology should remain stable whenever practical.

Avoid:
- unnecessary renaming
- synonym proliferation
- terminology fragmentation
- multiple names for the same concept

Prefer:
- strengthening definitions
- improving documentation
- operational clarification

New terminology must justify its existence.

Vocabulary drift damages ecosystems.

---

# Reserved System Names

Examples:
- README.md
- LICENSE.md
- CHANGELOG.md
- RELEASE_NOTES.md
- HELP.md
- USER_GUIDE.md
- QUICKSTART_*.md
- SETUP_*.md
- KIT_MANIFEST_*.md

Retired names are not reserved for active use.

Explicitly retired:
- LOAD_*.md
- QUICKSTART.md
- SETUP.md

Additional reserved names may be defined in:

`agentforgeframework-cpu/-agentforge-governance/governance/standards/RESERVEDNAMES.md`

---

# Filename Classes

## Class 1 — System / Operational Files

Case:
UPPERCASE.

Purpose:
System-level, operational, onboarding, lifecycle, support, and repository-control files.

Examples:
- README.md
- LICENSE.md
- CHANGELOG.md
- RELEASE_NOTES.md
- HELP.md
- USER_GUIDE.md
- QUICKSTART_<kit>.md
- SETUP_<kit>.md
- KIT_MANIFEST_<kit>.md

Notes:
- `README.md` is the standard folder-local orientation filename.
- `README_*.md` is not the standard because it is clumsy and conflicts with a widely understood convention.
- The file's repository-relative path should be documented inside the file.

## Class 2 — User-Facing Tool Modules

Case:
lowercase.

Purpose:
Operational tools, command modules, reusable capability components, and functional procedures intended to be loaded, invoked, or used as tooling.

Examples:
- cleanup.md
- deepdive.md
- visualbrief.md
- intake.md
- math.md
- diag.md
- override.md
- rules.md
- chatexport.md

Notes:
- Existing MixedCase tool module filenames should be treated as rename candidates when remediation is operationally safe.
- Do not create a separate low-level command-module case class. Low-level command modules are user-facing tool modules for naming purposes.

## Class 3 — Essays

Case:
CamelCase title-style naming

Purpose:
Essays preserve reasoning, tradeoffs, operational lessons, interpretation, disagreement, and historical context without becoming governance.

Examples:
- What-Essays-Are.md
- Visible-Disagreement-Is-Healthy.md
- Why-Human-In-Command-Matters.md
- AI-Involvement-vs-Integration.md

Notes:
- Essays are not governance.
- Governance preserves authority. Essays preserve thought.

---

# Reserved Operational Folder Names

Examples:
- /core-tools
- /examples
- /validation
- /governance
- /lessons
- /media
- /data
- /documents
- /contact
- /appendix

Folder naming generally prefers plural collection-style naming.

Reason:
- supports future growth
- avoids rename churn
- preserves path stability

---

# Filename Recognition Doctrine

AgentForge uses case to support fast recognition and operational survivability.

- UPPERCASE names identify system / operational files.
- lowercase names identify user-facing tool modules.
- CamelCase title-style filenames identify essays.

Do not create file names that differ only by case.

Examples to avoid:
- README.md
- readme.md

---

# Character Restrictions

Preferred allowed characters:
- letters
- digits
- underscore (_)
- hyphen (-)
- period (.) for extensions

Avoid:
- spaces
- tabs
- control characters
- unusual special characters
- shell-sensitive characters

---

# Hyphen vs Underscore Philosophy

Both hyphen (-) and underscore (_) are permitted.

Guidance:
- remain internally consistent within a component
- prioritize readability
- prioritize operational clarity

---

# Case Sensitivity Doctrine

Avoid names that differ only by case.

Examples to avoid:
- README.md
- readme.md

---

# Root vs Local Naming

Root-level operational files should use standardized naming.

Internal operational tools may use local kit-specific naming.

Global uniqueness is not required.

Operational clarity IS required.

---

# Local Extensions

Kits and repositories may define:
- local reserved names
- local operational conventions
- local organizational structures

Provided they do not conflict with:
- HIC-001
- RESERVEDNAMES.md
- official protected operational names

---

# Portability-Oriented Naming

Naming should remain:
- shell-safe
- Git-safe
- AI-readable
- cross-platform practical
- operationally maintainable

---

# Acronym Discipline

Acronyms are acceptable when they:
- materially reduce friction
- are repeatedly used operationally
- remain understandable

Examples:
- CTS
- AFD
- HIC

Avoid:
- excessive acronym stacking
- unreadable shorthand
- unnecessary acronym creation

---

# Namespace Collision Philosophy

Seek uniqueness where practical.

Collisions matter when they create:
- operational confusion
- maintenance risk
- governance ambiguity
- portability problems

If a naming conflict becomes operationally harmful:

> fix it.

---

# Historical Compatibility Philosophy

Older names may remain historically visible in documentation, changelogs, archives, or release history when needed for understanding.

Active operational scaffolds should not preserve retired filenames merely for compatibility when the human has approved removal.

Current retired active-use names:
- LOAD_*.md
- QUICKSTART.md
- SETUP.md

Modernization is permitted when a name is:
- broken
- misleading
- unclear
- operationally harmful
- causing standards propagation failure

Avoid:
- unnecessary rename churn
- cosmetic refactoring
- disruption without operational benefit

---

# Naming Correction Philosophy

If a name is found to be:
- broken
- misleading
- unclear
- operationally harmful

…fix it.

Operational correction is preferred over bureaucratic enforcement.

Avoid:
- naming purity wars
- committee-driven naming politics
- unnecessary governance overhead
- style-policing behavior

---

# Enforcement Philosophy

Naming discipline is maintained through:
- operational review
- practical correction
- governance guidance
- human judgment

Not through:
- centralized naming approval systems
- punitive enforcement
- excessive process overhead

Human judgment remains authoritative under:

`agentforgeframework-cpu/-agentforge-governance/governance/HIC-001_Human-in-Command_Standard.md`

---

# RESERVEDNAMES.md Relationship

`agentforgeframework-cpu/-agentforge-governance/governance/standards/RESERVEDNAMES.md`

serves as the operational anchor for protected naming governance.

Authority derives from:

`agentforgeframework-cpu/-agentforge-governance/governance/HIC-001_Human-in-Command_Standard.md`

---

# Final Principle

> Naming discipline exists to support operational clarity, portability, maintainability, and ecosystem stability.

Build names that humans can understand.

Especially at 2 AM.

---

# Suggested Repository Placement

Recommended Location:

`agentforgeframework-cpu/-agentforge-governance/governance/standards/NAMING_DISCIPLINE_STANDARD.md`

---

# Development & Test Environment

- Platform: ChatGPT (Web)
- Model: GPT-5.5
- Date: 2026-05-11

Notes:
- Updated during file-alignment remediation to clarify filename classes, retire LOAD_*.md and QUICKSTART.md from active use, and record the README.md folder-local exception.
