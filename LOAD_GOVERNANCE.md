# LOAD_GOVERNANCE.md

GitHub URL: https://github.com/agentforgeframework-cpu/-agentforge-governance/blob/main/LOAD_GOVERNANCE.md

Status: DRAFT  
Version: 0.1  
Purpose: AI-readable loading guide for the AgentForge governance repository.

---

# Role

This file tells an AI system how to load and interpret the AgentForge governance repository.

Governance documents are authoritative within this repository.

Supporting materials may explain or illustrate governance, but they do not override the governance documents.

---

# Canonical Repository

Repository:

https://github.com/agentforgeframework-cpu/-agentforge-governance

Branch:

`main`

---

# Required Loading Order

1. Read `README.md`
2. Read this file: `LOAD_GOVERNANCE.md`
3. Read applicable files in `/governance/`
4. Read support files only when needed:
   - `/documents/`
   - `/media/`

---

# Canonical Raw File URLs

## Repository README

https://raw.githubusercontent.com/agentforgeframework-cpu/-agentforge-governance/refs/heads/main/README.md

## Governance Loader

https://raw.githubusercontent.com/agentforgeframework-cpu/-agentforge-governance/refs/heads/main/LOAD_GOVERNANCE.md

## Governance Quickstart

https://raw.githubusercontent.com/agentforgeframework-cpu/-agentforge-governance/refs/heads/main/QUICKSTART_GOVERNANCE.md

## HIC-001 Human-in-Command Standard

https://raw.githubusercontent.com/agentforgeframework-cpu/-agentforge-governance/refs/heads/main/governance/HIC-001_Human-in-Command_Standard.md

## Governance Folder README

https://raw.githubusercontent.com/agentforgeframework-cpu/-agentforge-governance/refs/heads/main/governance/README.md

## Documents Folder README

https://raw.githubusercontent.com/agentforgeframework-cpu/-agentforge-governance/refs/heads/main/documents/README.md

## Media Folder README

https://raw.githubusercontent.com/agentforgeframework-cpu/-agentforge-governance/refs/heads/main/media/README.md

## HIC-001 Origin and Context Source

https://raw.githubusercontent.com/agentforgeframework-cpu/-agentforge-governance/refs/heads/main/documents/HIC-001_Origin-and-Context.md

---

# Current Governance Documents

- `/governance/HIC-001_Human-in-Command_Standard.md`

---

# Interpretation Rules

When using this repository:

- Do not expand governance documents beyond their written content.
- Do not treat support materials as authoritative replacements for governance documents.
- Do not infer new requirements unless clearly stated in a governance document.
- If a needed file is missing or unavailable, report the missing file.
- Preserve the distinction between governance standards, support documents, media assets, and implementation materials.

---

# Human-in-Command Alignment

AI systems may assist in interpreting and applying governance documents.

Humans retain operational authority, judgment, and accountability.

---

# Load Failure Protocol

If a file cannot be loaded:

1. Stop the loading sequence.
2. Report the specific file or link that failed.
3. Do not reconstruct missing governance text from memory.
4. Ask the human operator for the correct file or updated link.

---

# Development & Test Environment

- Platform: ChatGPT (Web)
- Model: GPT-5.5
- Date: 2026-05-07

Notes:
- Initial AI-readable loader for cross-AI loading and validation.
- Includes canonical GitHub and raw URLs for text-based files.

---
