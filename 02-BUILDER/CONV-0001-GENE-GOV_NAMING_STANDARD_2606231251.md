# CONV-0001-GENE-GOV_NAMING_STANDARD_2606231251

Date: 2026-06-23
Status: Approved
Supersedes:
- CONV-GENE-0001-GOV_NAMING_STANDARD.md
- CONV-0001-GENE-GOV_NAMING_STANDARD.md

## Purpose

Define the official, non-negotiable naming convention for preserved conversation knowledge artifacts in the FOURTH ANGELS ecosystem.

## Official File Naming Format

```text
CONV-####-AGENTCODE-TYPE_SUBJECT_YYMMDDHHMM.md
```

## Meaning

- `CONV` = preserved conversation knowledge artifact
- `####` = global 4-digit trace number
- `AGENTCODE` = 4-character agent code
- `TYPE` = artifact type/category
- `SUBJECT` = short but concise subject
- `YYMMDDHHMM` = version timestamp in user-local time
- `.md` = markdown format

## Examples

```text
CONV-0000-GENE-REFERENCE_CONV_REGISTRY_2606231250.md
CONV-0001-GENE-GOV_NAMING_STANDARD_2606231251.md
CONV-0002-GENE-PLAN_ECOSYSTEM_WORKBOOK_2606231252.md
CONV-0003-GENE-RULE_WORKING_RULES_2606231253.md
CONV-0004-CHKM-PROMPT_CHECKMATE_2606231254.md
```

## Naming Rules

- File naming convention is locked.
- File and folder names remain in uppercase format.
- The ALL CAPS rule applies to naming only, not to markdown document content.
- Subjects must be short but concise.
- Prefer 2–5 words in the subject when possible.
- Use underscores inside the subject.
- Avoid unnecessary wording in the subject.
- Do not silently change the naming convention.
- New versions must use a new timestamp suffix.
- Existing files must not be renamed just to change status.

## Agent Codes

```text
GENE = General
LIFE = Life OS / Personal Chief of Staff
CTRL = ControlTower / T&T Governance
NEIR = Coding Workflow Agent
CHKM = Checkmate / Audit Agent
```

## Allowed Types

```text
ARCH
PLAN
GOV
RULE
SOP
PROMPT
FRAMEWORK
LESSON
REFL
TEMPLATE
CHECKLIST
GUIDE
REFERENCE
DECISION
```

## Numbering Rule

### Global Sequence

The 4-digit trace number is global across the entire ecosystem.

Rules:

- Numbers are never reused.
- Numbers are never reset.
- Numbers are never renumbered.
- Every approved knowledge artifact receives the next available number.
- Deleted, archived, or superseded files keep their original number in history.

## Versioning Rule

The timestamp suffix identifies a specific file version.

Example:

```text
CONV-0004-CHKM-PROMPT_CHECKMATE_2606231254.md
```

Interpretation:
- `0004` = artifact lineage
- `CHKM` = owning agent
- `PROMPT` = type
- `CHECKMATE` = subject
- `2606231254` = specific version timestamp

### Versioning Principles

- Files are immutable snapshots.
- New versions create new files with new timestamps.
- Old files remain as historical records.
- The latest approved timestamp is the current version for that CONV ID.
- Do not use `V1`, `V2`, `FINAL`, or similar labels in file names.

## Registry Rule

Maintain a master registry file:

```text
CONV-0000-GENE-REFERENCE_CONV_REGISTRY_YYMMDDHHMM.md
```

### Registry Purpose

The registry exists to:
1. Prevent duplicate CONV numbers
2. Track artifact ownership
3. Track latest version timestamps
4. Act as the ecosystem source of truth for numbering and latest-version lookup

### Minimum Registry Fields

- CONV ID
- AGENT
- TYPE
- SUBJECT
- LATEST VERSION
- CURRENT FILE

Before assigning a new number:
1. Check the registry.
2. Identify the highest used number.
3. Assign the next available number.
4. Record the new artifact immediately.

## Repository Structure Rule

Approved root structure:

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

- `FOURTH ANGELS/` is the locked root folder.
- Each agent has its own folder.
- Each folder must begin with `00-README-FIRST.md`.
- `00-README-FIRST.md` is exempt from CONV naming because it is an instruction file, not a preserved conversation artifact.
- Deep folder nesting should be avoided unless governance explicitly requires it later.
- Internal subfolders such as `01-MANUALS`, `02-STANDARDS`, and `03-RELEASES` are not approved by default.

## Content Rule

Markdown content should use normal professional readability.

Examples:
- Normal headings
- Normal sentences
- Normal bullets
- Normal markdown structure

The ALL CAPS rule does **not** apply to the internal content of the document.

## Governance Rule

If the naming convention, repository structure, numbering logic, registry logic, or file format rule changes, the change must be stated before execution using:

```text
Planned Change: ...
Reason: ...
Impact: ...
Next Step: ...
```

## Final Decision

This naming standard is approved and locked unless a future governance decision explicitly supersedes it.
