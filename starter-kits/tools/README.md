# AgentForge Tool Kit Starter

Repository Path: `-agentforge-governance/starter-kits/tools/README.md`
GitHub URL: https://github.com/agentforgeframework-cpu/-agentforge-governance/blob/main/starter-kits/tools/README.md
Raw URL: https://raw.githubusercontent.com/agentforgeframework-cpu/-agentforge-governance/refs/heads/main/starter-kits/tools/README.md

Status: DRAFT  
Version: 0.1

---

# Purpose

This starter kit provides a lightweight canonical structure for creating an AgentForge Tool Kit.

It is designed to be copied, renamed, and adapted by a human for a defined kind of AI-assisted operational work.

---

# What This Starter Kit Demonstrates

This starter kit demonstrates:

- required kit structure
- README → QUICKSTART_<kit> → SETUP_<kit> doctrine
- `/core-tools` operational boundary
- `/examples` demonstration boundary
- optional folder behavior
- governance inheritance by default
- text-file path and URL traceability

---

# Starter Structure

```text
/tool-kit
├── README.md
├── LICENSE.md
├── QUICKSTART_tool-kit.md
├── SETUP_tool-kit.md
├── KIT_MANIFEST_tool-kit.md
├── /core-tools
│   └── README.md
├── /examples
│   └── README.md
└── /documents
    └── README.md
```

`KIT_MANIFEST_tool-kit.md` is included as an optional example.

A copied kit may remove it if no machine-oriented manifest is needed.

---

# Required Customization

When adapting this starter kit:

Follow the current filename standards:

- `SETUP_<kit>.md` for AI-readable setup
- `QUICKSTART_<kit>.md` for human-first onboarding
- lowercase filenames for user-facing tool modules
- no `LOAD_*.md` files
- no plain `QUICKSTART.md` files

1. Rename `tool-kit` to the actual kit name.
2. Rename `QUICKSTART_tool-kit.md` to match the kit name.
3. Rename `SETUP_tool-kit.md` to match the kit name.
4. Rename `KIT_MANIFEST_tool-kit.md` if used.
5. Update all repository paths and GitHub URLs.
6. Replace placeholder purpose and usage text.
7. Add real operational tools under `/core-tools/`.
8. Add real examples under `/examples/`.

---

# Operational Requirement

A kit may be small.

It may contain only one operational tool.

But:

> It has to do something.

---

# Governance

Governance inheritance is assumed by default.

A local `/governance/` folder should be added only when kit-specific governance extensions are needed.

---

# Development & Test Environment

- Platform: ChatGPT (Web)
- Model: GPT-5.5
- Date: 2026-05-11

Notes:
- Updated during file-alignment remediation to clarify current setup and quickstart filename standards.
