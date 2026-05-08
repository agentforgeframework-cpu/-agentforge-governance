# KIT_STANDARD.md

Repository Path: `-agentforge-governance/governance/KIT_STANDARD.md`
GitHub URL: https://github.com/agentforgeframework-cpu/-agentforge-governance/blob/main/governance/KIT_STANDARD.md
Raw URL: https://raw.githubusercontent.com/agentforgeframework-cpu/-agentforge-governance/refs/heads/main/governance/KIT_STANDARD.md

Status: DRAFT  
Version: 0.1

---

# Purpose

This document defines the canonical lightweight structure and operational expectations for AgentForge Kits.

---

# Canonical Definition

> An AgentForge Kit is a governed operational collection assembled to help humans accomplish a defined kind of AI-assisted work.

A kit is assembled around purpose.

It contains curated components organized to support real operational use.

---

# Core Principles

## Kits Equip Humans

Kits equip humans.

They do not replace humans.

---

## Capability Drives Structure

> Capability drives structure, not the other way around.

A kit should contain the structure required to support its operational capability.

Structure should not be added merely because it is available.

---

## Kits Are Curated

Kits are curated operational collections.

They are not uncontrolled accumulations of files, prompts, tools, or examples.

---

## Preparedness Is Part of Capability

A kit should be organized so that a human can understand, use, maintain, and recover it under realistic operational conditions.

---

# Canonical Kit Flow

AgentForge Kits follow this operational guidance sequence:

```text
README.md
→ QUICKSTART_<kit>.md
→ SETUP_<kit>.md
```

There is no plain `QUICKSTART.md` or plain `SETUP.md` standard for kits.

The kit-specific suffix is required for clarity and portability.

---

# Minimum Required Structure

A minimal AgentForge Tool Kit should normally include:

```text
/kit-name
├── README.md
├── LICENSE.md
├── QUICKSTART_<kit>.md
├── SETUP_<kit>.md
├── /core-tools
│   └── README.md
└── /examples
    └── README.md
```

A minimal kit may contain only one operational tool.

Critical condition:

> It has to do something.

Operational usefulness matters more than size, complexity, or file count.

---

# Optional Structure

Additional folders may be added when operationally justified:

```text
/validation
/governance
/lessons
/media
/data
/documents
/contact
/appendix
/<source-language>
```

Structure must justify its operational cost.

---

# Folder Expectations

Every folder should contain a `README.md` file.

Folder README files should explain:

- what belongs in the folder
- what does not belong in the folder
- expected file inventory when useful
- operational purpose

---

# /core-tools Boundary

`/core-tools` contains machine-readable operational capability components.

This may include:

- operational tools
- workflows
- procedures
- executable code
- templates intended for machine use
- structured machine-readable instructions
- implementation utilities

Human instructions and human-oriented support material belong in `/documents/`.

---

# /documents Boundary

`/documents` contains human-oriented support material.

This may include:

- guides
- explanations
- background documents
- printable references
- user-facing support documents
- rich artifacts intended for human review

---

# /examples Boundary

`/examples` answers:

> How might this be used?

Examples should demonstrate operational use.

Examples are not validation evidence by default.

---

# /validation Boundary

`/validation` answers:

> What do we know about operational behavior?

Validation exists to improve operational confidence.

Validation does not certify anything.

---

# Governance Inheritance

AgentForge governance inheritance is automatic by default.

Local `/governance/` folders exist only when additional kit-specific governance is needed.

Central governance remains authoritative unless explicitly extended locally.

---

# Production Evidence

The minimum operational evidence required before a human may reasonably promote a kit to Production is self-contained in the design of each kit and approved by the human designing it.

Production requires human approval.

---

# Portability Expectations

AgentForge Kits prioritize:

1. human portability
2. AI portability
3. practical cross-platform use where reasonably possible

AgentForge does not promise:

- deterministic universal portability
- identical cross-platform behavior
- platform independence

---

# Naming Expectations

Follow `RESERVEDNAMES.md` for reserved operational names and naming conventions.

General convention:

- UPPERCASE = operational infrastructure
- lowercase = operational tools/components

---

# Manifest Philosophy

`KIT_MANIFEST_<kit>.md` is optional.

README files provide human operational inventory.

Manifest files provide optional machine operational inventory.

A manifest should remain:

- lightweight
- optional
- machine-oriented
- operationally justified

It should not become:

- a giant metadata system
- a bureaucracy engine
- a package manager descriptor

---

# Lifecycle

Common lifecycle stages include:

- Concept
- Alpha
- Prototype
- Beta
- Stabilized
- Production
- Archived

Stages may be skipped when reasonable.

Governance should not slow work unnecessarily.

---

# Maintenance Principle

If something is found to be broken:

> Fix it.

---

# Development & Test Environment

- Platform: ChatGPT (Web)
- Model: GPT-5.5
- Date: 2026-05-08

Notes:
- Initial canonical AgentForge Kit standard draft.
