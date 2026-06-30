# AgentForge Production Repository Standard

**Status:** Version 1.0 Candidate
**Version:** 1.0 
**Approved: 2026-06-29

---

# Purpose

This standard defines the minimum structure and operating characteristics of an AgentForge production deployment.

It governs individual AgentForge production kit folders.

It does not govern promotion, approval, qualification, release management, lifecycle governance, or parent-repository organization.

---

# Core Principle

> Every AgentForge production kit shall be independently discoverable, deterministic, recoverable, and readable by both humans and AI systems.

---

# 1. Kit Identification

Every production kit shall have a permanent AgentForge identifier.

Format:

```text
AF-###
```

Identifiers:

- are assigned in sequence
- are never reused
- reflect assignment order
- may extend beyond three digits

The kit folder shall use:

```text
af-###-lowercase-hyphenated-name
```

Example:

```text
af-004-clean-think-share
```

---

# 2. Kit Types

AgentForge production kits are:

- Tool Kits
- Training Kits

A Tool Kit shall contain:

```text
tools/
```

A Training Kit shall contain:

```text
lessons/
```

Only folders required by the kit shall be included.

---

# 3. Required Root Files

Every production kit shall contain:

```text
README.md
SETUP.md
LIBRARY.md
LICENSE.md
```

`README.md` is the repository entry point.

`SETUP.md` contains the instructions required to prepare and operate the kit.

`LIBRARY.md` is the authoritative Repository Object Table.

`LICENSE.md` contains the licensing terms.

---

# 4. Repository Discovery

Repository discovery begins with:

```text
README.md
```

The root `README.md` shall provide the complete raw locations of:

```text
ROOT_LIBRARY
ROOT_SETUP
```

`ROOT_LIBRARY` is the authoritative source for all Repository Object locations.

Repository locations shall not be inferred.

---

# 5. Retrieval Failure

If a required Repository Object cannot be retrieved:

1. Stop.
2. Identify the inaccessible object.
3. Report the failed location.
4. Do not infer, reconstruct, or substitute content.
5. Request a corrected location or another authorized copy.

---

# 6. Repository Object Table

`LIBRARY.md` shall list every file and asset included in the production kit.

Folders are represented by their required `README.md`.

The table shall contain exactly two functional columns:

```text
HANDLE | RAW FILE
```

Each object shall:

- appear once
- have one unique Repository Object Handle
- have one complete raw location

Relative paths are not sufficient.

`LIBRARY.md` is an index, not documentation.

---

# 7. Repository Object Handles

Repository Object Handles shall use only:

- uppercase letters
- digits
- underscore

Examples:

```text
ROOT_README
ROOT_SETUP
ROOT_LIBRARY
ROOT_LICENSE
TOOLS_README
LESSONS_README
NOTE_INTAKE
LESSON_01
EXAMPLE_01
```

The prefix:

```text
ROOT_
```

is reserved for required root objects.

---

# 8. Standard Markdown Metadata

Every production Markdown file shall include:

```text
Kit Type
Status
Version
Repository
Repository Object
Raw
This File (Raw)
```

Standard pattern:

```text
**Kit Type:** <Kit Type>
**Status:** Production
**Version:** 1.0

Repository:
AF-004 - Clean Think Share (CTS)

Repository Object:
`ROOT_LIBRARY`

Raw:
https://raw.githubusercontent.com/.../LIBRARY.md

This File (Raw):
https://raw.githubusercontent.com/.../currentfile.md
```

`Repository Object` identifies `ROOT_LIBRARY`.

`Raw` provides the complete raw location of `ROOT_LIBRARY`.

`This File (Raw)` provides the complete raw location of the current file.

This repeated metadata is required for discovery and recovery.

---

# 9. Files and Folders

Required control filenames and `TUTORIAL.md` retain their canonical names.

```text
README.md
SETUP.md
LIBRARY.md
LICENSE.md
TUTORIAL.md
```

Operational filenames shall use lowercase and shall not contain spaces.

Every folder included in the production kit shall contain:

```text
README.md
```

The folder `README.md` shall:

- state the folder purpose
- include the standard Markdown metadata
- appear in `LIBRARY.md`

---

# 10. Tools

Each tool shall:

- have a distinct operational purpose
- contain enough instruction for the AI to operate it

A Tool Kit may contain one or more tools.

---

# 11. Lessons

Each lesson shall contain enough instruction for the AI to deliver or support it.

When lesson order matters, the sequence shall be explicit.

---

# 12. Optional Repository Objects

A production kit may include:

```text
examples/
media/
TUTORIAL.md
```

only when required for operation of the kit.

Examples contain whatever is required for the AI to run the example.

Media contains whatever is required for the AI to operate the kit.

`TUTORIAL.md` contains kit-specific guidance when that guidance is required within the production deployment.

---

# 13. Portable Markdown

Production Markdown shall use UTF-8 and portable Markdown.

Decorative Unicode, emoji, custom bullets, and platform-dependent formatting shall not be used.

All Markdown tables shall use padded columns and remain readable in plain text.

---

# 14. External References

External references may support attribution or context.

Operation shall not depend on an external reference unless that dependency is explicitly declared.

---

# Final Principle

> Repository structure should disappear behind consistent operation.

Humans and AI systems should spend their effort using AgentForge kits rather than discovering how those kits are organized.
