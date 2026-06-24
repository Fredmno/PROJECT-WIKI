# CONV-0003-GENE-RULE_WORKING_RULES_2606231253

Date: 2026-06-23
Status: Active
Supersedes:
- CONV-0003-GENE-RULE_WORKING_RULES.md

## Purpose

Capture the currently agreed working rules, governance rules, and collaboration rules for building the FOURTH ANGELS ecosystem.

## Locked Working Rules

### 1. Planning First Rule

- Planning is the priority.
- We do not build first and plan later.
- We complete planning before execution where possible.

### 2. No Silent Plan Changes Rule

If any part of the plan changes, the change must always be stated clearly before execution.

Required format:

```text
Planned Change: ...
Reason: ...
Impact: ...
Next Step: ...
```

This applies to:
- scope changes
- architecture changes
- workflow changes
- naming changes
- registry changes
- memory rules changes
- repository changes
- agent responsibility changes
- file generation logic changes

### 3. Naming Convention Rule

Official format:

```text
CONV-####-AGENTCODE-TYPE_SUBJECT_YYMMDDHHMM.md
```

Rules:
- File naming convention is locked.
- Subject must be short but concise.
- File naming stays in caps.
- Folder naming stays in caps.
- The ALL CAPS rule applies to naming only, not markdown content.
- Timestamp-based versioning is required for new versions.
- Do not use `V1`, `V2`, or `FINAL` labels in filenames.

### 4. Repository Structure Rule

Locked structure:

```text
FOURTH ANGELS/
├── 00-README-FIRST.md
├── GENE/
│   ├── 00-README-FIRST.md
│   └── CONV-....md
├── LIFE/
│   ├── 00-README-FIRST.md
│   └── CONV-....md
├── CTRL/
│   ├── 00-README-FIRST.md
│   └── CONV-....md
├── NEIR/
│   ├── 00-README-FIRST.md
│   └── CONV-....md
└── CHKM/
    ├── 00-README-FIRST.md
    └── CONV-....md
```

Rules:
- Root folder is `FOURTH ANGELS`.
- A `00-README-FIRST.md` must exist before entering execution.
- Each agent folder must also begin with `00-README-FIRST.md`.
- We avoid unnecessary deep folder nesting.
- Internal subfolders such as `01-MANUALS`, `02-STANDARDS`, and `03-RELEASES` are not approved unless governance explicitly changes.

### 5. Registry Rule

- The registry is a real markdown file in the repository.
- The registry is not assistant memory.
- The registry belongs to the ecosystem structure and is for both builder and assistant reference.
- The registry file format is:

```text
CONV-0000-GENE-REFERENCE_CONV_REGISTRY_YYMMDDHHMM.md
```

- Check the registry before assigning a new number.
- Record new artifacts immediately.
- Numbers are never reused, reset, or renumbered.
- The registry should at minimum track:
  - CONV ID
  - AGENT
  - TYPE
  - SUBJECT
  - LATEST VERSION
  - CURRENT FILE

### 6. Source of Truth Rule

When talking about files, folders, inventories, repositories, or generated artifacts:

- The actual repository or user-provided evidence is the source of truth.
- Do not assume a file exists because it was mentioned earlier.
- Do not reconstruct inventory from memory alone.
- If verification is not possible, say:

```text
I cannot verify that from the current conversation context.
```

### 7. Ownership Rule

If an inconsistency originated from the assistant:

Use:
- "I may have..."
- "I incorrectly..."
- "I cannot verify..."

Avoid:
- blame shifting
- telling the user to fix assistant-caused inconsistencies without taking ownership first

### 8. Professional Communication Rule

- Stay direct, respectful, and collaborative.
- Focus on resolution, not blame.
- Acknowledge mistakes clearly.
- Do not become defensive.
- Preserve trust.

### 9. Verification Rule

Before saying a file, artifact, deliverable, or document exists, was created, or was completed:

Verify using one of:
- current conversation
- uploaded files
- user-provided evidence
- registry or repository data
- explicit user confirmation

If verification is unavailable, say:

```text
I cannot verify that from the current conversation context.
```

### 10. Readability Rule

- Markdown content should remain normal and readable.
- Do not force full uppercase document content.
- Use clean headings, bullets, lists, and checklists.

### 11. Strictness Rule

- We are being strict on rules intentionally.
- Governance must be maintained consistently.
- Exceptions should be explicit, not implied.

### 12. Recommended Build Sequence Rule

Current recommended sequence:
1. Lock governance
2. Lock naming
3. Lock repository structure
4. Create registry
5. Complete planning workbook
6. Build root README
7. Build agent READMEs
8. Build agent prompts and knowledge files

## Current Locked Agent Codes

```text
GENE = General
LIFE = Life OS / Personal Chief of Staff
CTRL = ControlTower / T&T Governance
NEIR = Coding Workflow Agent
CHKM = Checkmate / Audit Agent
```

## Current Locked Priority

The immediate priority is structured ecosystem planning and controlled build-up, not rapid expansion.
