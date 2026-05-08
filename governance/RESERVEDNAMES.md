# RESERVEDNAMES.md

Repository Path: `-agentforge-governance/governance/RESERVEDNAMES.md`
GitHub URL: https://github.com/agentforgeframework-cpu/-agentforge-governance/blob/main/governance/RESERVEDNAMES.md
Raw URL: https://raw.githubusercontent.com/agentforgeframework-cpu/-agentforge-governance/refs/heads/main/governance/RESERVEDNAMES.md

Status: DRAFT  
Version: 0.1

---

# Purpose

This document defines reserved operational file names, reserved folder names, and naming conventions within the AgentForge ecosystem.

These conventions exist to:

- reduce operational ambiguity
- improve portability
- improve human readability
- support cross-AI interoperability
- reduce naming collisions
- improve maintainability
- preserve 2 AM engineer usability

Reserved names are operational infrastructure.

They should not be casually repurposed.

---

# Scope

Reserved names govern operational structure within AgentForge kits and governance systems.

They do not attempt to govern unrelated development, testing, sandbox, or external operational environments unless a human intentionally applies AgentForge standards there.

---

# Core Naming Philosophy

Names should:

- reflect what something is and/or does
- prioritize clarity over cleverness
- avoid marketing language
- remain understandable by both technical and non-technical users
- minimize ambiguity

> Vocabulary drift kills ecosystems.

---

# Allowed Characters

AgentForge file and folder names should use only:

- letters A-Z
- letters a-z
- digits 0-9
- underscore `_`
- hyphen `-`
- period `.` for normal file extensions

File and folder names should remain portable across common operating systems, shells, URLs, Git systems, and AI platforms.

Examples:

```text
forecast-tool.md
SETUP_cts-kit.md
cleanup_v2.md
```

---

# Prohibited Characters

The following should not be used in file or folder names:

- spaces
- tabs
- carriage returns
- control characters
- BELL characters
- shell-sensitive characters
- unusual Unicode symbols
- characters that commonly create portability problems

Examples:

```text
BAD > My Tool.md
BAD > setup@tool.md
BAD > cleanup!.md
```

---

# Uppercase vs Lowercase Convention

## Uppercase

UPPERCASE names are reserved for:

- operational infrastructure
- system guidance
- governance files
- lifecycle support files
- operational metadata

Examples:

```text
README.md
LICENSE.md
QUICKSTART_cts-kit.md
SETUP_cts-kit.md
CHANGELOG.md
HELP.md
```

---

## Lowercase

lowercase names are reserved for:

- operational tools
- workflows
- executable procedures
- reusable capability components
- implementation utilities
- machine-readable instructions

Lowercase naming improves portability and reduces ambiguity across platforms and AI systems.

Human instructions and human-oriented support materials belong in `/documents/`, not `/core-tools/`.

Examples:

```text
cleanup.md
analyze.md
forecast.md
validation-runner.md
```

---

# Reserved Operational Files

## README.md

Purpose:
Primary human-readable orientation document.

Reason Reserved:
Common entry point for humans, repositories, folders, and AI-assisted review.

---

## LICENSE.md or LICENSE

Purpose:
Defines operational usage rights and distribution terms.

Reason Reserved:
License information must be easy to find and should not be hidden behind kit-specific naming.

---

## QUICKSTART_<kit>.md

Purpose:
Human-first startup and onboarding guide.

Reason Reserved:
Separates human startup from AI setup.

Example:

```text
QUICKSTART_cts-kit.md
```

---

## SETUP_<kit>.md

Purpose:
AI-readable operational setup and orchestration document.

Reason Reserved:
Provides deterministic loading, explicit references, and operational setup guidance for AI systems.

Example:

```text
SETUP_cts-kit.md
```

---

## KIT_MANIFEST_<kit>.md

Purpose:
Optional machine-oriented operational inventory.

Reason Reserved:
Supports lightweight machine-readable inventory without becoming a package-manager descriptor.

Example:

```text
KIT_MANIFEST_cts-kit.md
```

---

## CHANGELOG.md

Purpose:
Tracks meaningful operational changes over time.

Reason Reserved:
Keeps change history discoverable and consistent.

---

## RELEASE_NOTES.md

Purpose:
Human-readable release summary.

Reason Reserved:
Separates release communication from detailed change history.

---

## HELP.md

Purpose:
Quick operational assistance and support guidance.

Reason Reserved:
Creates a predictable support entry point.

---

## USER_GUIDE.md

Purpose:
Extended operational documentation.

Reason Reserved:
Creates a predictable location for detailed human guidance.

---

# Legacy Compatibility

## LOAD_*.md

Status:
Retired / Transitional

Purpose:
Legacy operational loader format.

Current Standard:
`SETUP_*.md`

Rule:
If a `LOAD_*.md` file exists, it should redirect users and systems to the newer `SETUP_*.md` equivalent.

---

# Reserved Operational Folders

## /core-tools

Purpose:
Primary operational capability components.

Reason Reserved:
Creates a predictable location for machine-readable operational tools, workflows, procedures, implementation utilities, and capability components.

Human instructions and human-oriented support material belong in `/documents/`.

---

## /examples

Purpose:
Operational demonstrations and usage examples.

Reason Reserved:
Separates example usage from validation evidence.

Answers:

> How might this be used?

---

## /validation

Purpose:
Operational validation evidence.

Reason Reserved:
Separates operational behavior evidence from examples, tutorials, and marketing material.

Answers:

> What do we know about operational behavior?

---

## /governance

Purpose:
Local governance extensions specific to the kit.

Reason Reserved:
Provides a predictable location for local governance when central governance must be extended.

Notes:
- central governance inheritance is assumed by default
- local governance exists only when additional governance is needed

---

## /lessons

Purpose:
Educational or instructional materials related to operational use.

Reason Reserved:
Separates learning material from core operational tools.

---

## /media

Purpose:
Images, video, diagrams, audio, and visual artifacts.

Reason Reserved:
Separates visual and media support files from operational text and source materials.

---

## /data

Purpose:
Structured operational data.

Reason Reserved:
Separates data assets from tools, documents, and examples.

---

## /documents

Purpose:
Human-oriented supporting documents and rich artifacts.

Reason Reserved:
Separates human support material from machine-readable operational tools.

---

## /contact

Purpose:
Contact, attribution, or support information.

Reason Reserved:
Creates a predictable location for human support and attribution details.

---

## /appendix

Purpose:
Supplementary material not central to operational flow.

Reason Reserved:
Keeps supporting material available without cluttering primary operational paths.

---

# Text File Reference Standard

All text-based AgentForge files should include both:

- repository-relative path
- full GitHub web URL

Reason:
The repository-relative path supports local clone use, offline review, and structural understanding.

The full GitHub URL supports browser access, external reference, and AI retrieval.

Example:

```text
Repository Path: `-agentforge-governance/governance/RESERVEDNAMES.md`
GitHub URL: https://github.com/agentforgeframework-cpu/-agentforge-governance/blob/main/governance/RESERVEDNAMES.md
```

---

# Naming Enforcement Philosophy

AgentForge naming governance exists to:

- reduce friction
- reduce ambiguity
- improve portability
- improve maintainability

It does not exist to create unnecessary bureaucracy.

If operational reality reveals problems:

> Fix what is broken.

---

# Development & Test Environment

- Platform: ChatGPT (Web)
- Model: GPT-5.5
- Date: 2026-05-08

Notes:
- Initial reserved names standard for AgentForge governance stabilization.
