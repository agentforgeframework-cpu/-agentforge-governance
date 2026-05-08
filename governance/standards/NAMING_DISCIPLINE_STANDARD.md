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
- LOAD_*.md
- KIT_MANIFEST_*.md

Additional reserved names may be defined in:

`agentforgeframework-cpu/-agentforge-governance/governance/standards/RESERVEDNAMES.md`

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

# Uppercase vs Lowercase Doctrine

Operational infrastructure and system-level files should use uppercase naming.

Examples:
- README.md
- HELP.md
- CHANGELOG.md
- QUICKSTART_cts-kit.md
- SETUP_cts-kit.md

Operational tools and functional components should generally use lowercase naming.

Examples:
- cleanup.md
- visualbrief.md
- forecast.md
- intake.md

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

Older names may remain grandfathered when practical.

Modernization is permitted.

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
- Date: 2026-05-08

Notes:
- Initial stabilization draft based on operational patterns already established across the AgentForge ecosystem.
