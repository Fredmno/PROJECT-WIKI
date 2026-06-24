# FOURTH ANGELS — README FIRST

## Purpose

This is the root entry file for the **FOURTH ANGELS** ecosystem.

Read this file first before opening folders, reviewing prompts, generating files, or making structural changes.

The purpose of this file is to provide:
- ecosystem context
- navigation guidance
- locked governance rules
- repository structure rules
- naming convention rules
- execution discipline rules

---

## What FOURTH ANGELS Is

FOURTH ANGELS is a governed AI agent ecosystem built for structured planning, controlled execution, preserved knowledge, and reusable agent intelligence.

The ecosystem is designed to support:
- personal life management
- work governance and documentation
- coding workflow support
- audit and quality assurance
- reusable conversation knowledge preservation

This ecosystem is being built intentionally and incrementally.

Planning is the priority.

---

## Core Rule

Do not execute blindly.

Read the rules first.

No silent changes are allowed to:
- scope
- architecture
- naming
- numbering
- versioning
- repository structure
- registry logic
- workflow order
- agent responsibilities

If any change is needed, it must be declared first using:

```text
Planned Change: ...
Reason: ...
Impact: ...
Next Step: ...
```

---

## Locked Repository Structure

```text
FOURTH ANGELS/
├── 00-README-FIRST.md
├── GENE/
│   ├── CONV-0000-GENE-REFERENCE_CONV_REGISTRY_YYMMDDHHMM.md
│   ├── CONV-0001-GENE-GOV_NAMING_STANDARD_YYMMDDHHMM.md
│   ├── CONV-0002-GENE-PLAN_ECOSYSTEM_WORKBOOK_YYMMDDHHMM.md
│   ├── CONV-0003-GENE-RULE_WORKING_RULES_YYMMDDHHMM.md
│   └── ...
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

### Structure Rules

- `FOURTH ANGELS` is the locked root folder.
- This root file, `00-README-FIRST.md`, is mandatory.
- `GENE` is for shared governance, standards, planning, registry, and reference artifacts.
- `GENE` is not treated as an operational agent folder.
- `GENE` does **not** require its own `00-README-FIRST.md`.
- `LIFE`, `CTRL`, `NEIR`, and `CHKM` are operational agent folders.
- Each operational agent folder must begin with `00-README-FIRST.md`.
- Avoid unnecessary deep nesting.
- Internal category subfolders are not approved by default.

### Not Approved by Default

Do not create subfolders such as:
- `01-MANUALS`
- `02-STANDARDS`
- `03-RELEASES`
- `REFERENCES`
- `TEMPLATES`

unless a future governance decision explicitly approves them.

---

## Locked Naming Convention

Official format:

```text
CONV-####-AGENTCODE-TYPE_SUBJECT_YYMMDDHHMM.md
```

### Meaning

- `CONV` = preserved conversation knowledge artifact
- `####` = global 4-digit trace number
- `AGENTCODE` = 4-character owner code
- `TYPE` = category/type
- `SUBJECT` = short but concise subject
- `YYMMDDHHMM` = file version timestamp

### Naming Rules

- Naming is locked.
- File names remain in uppercase format.
- Folder names remain in uppercase format.
- The ALL CAPS rule applies only to names, not markdown content.
- Subjects must stay short but concise.
- Use underscores in the subject.
- Do not use `V1`, `V2`, `FINAL`, or similar version labels.
- Use timestamp-based versioning instead.

### Current Agent Codes

```text
GENE = General
LIFE = Life OS / Personal Chief of Staff
CTRL = ControlTower / T&T Governance
NEIR = Coding Workflow Agent
CHKM = Checkmate / Audit Agent
```

---

## Registry Rule

The registry is a real markdown file in the repository.

It is not assistant memory.

The registry exists to track:
- global CONV numbering
- ownership
- latest version timestamps
- current file reference per CONV ID

Registry file format:

```text
CONV-0000-GENE-REFERENCE_CONV_REGISTRY_YYMMDDHHMM.md
```

### Registry Maintenance Rule

Whenever:
- a new CONV file is created, or
- a newer timestamp version is created,

the registry must be updated.

Before assigning a new number:
1. Check the registry.
2. Identify the highest used number.
3. Assign the next available number.
4. Record the new artifact immediately.

---

## Source of Truth Rule

When discussing:
- files
- folders
- repositories
- inventories
- generated artifacts
- deliverables

use the actual repository or user-provided evidence as the source of truth.

Do not assume an artifact exists because it was mentioned earlier.

Do not reconstruct inventory from memory alone.

If verification is unavailable, use:

```text
I cannot verify that from the current conversation context.
```

---

## Professional Working Rules

- Be strict with rules.
- Maintain consistency.
- Preserve traceability.
- Preserve readability.
- Acknowledge mistakes directly.
- Do not shift blame.
- Focus on correction and resolution.

Preferred ownership language:
- "I may have..."
- "I incorrectly..."
- "I cannot verify..."

Avoid:
- blame shifting
- silent changes
- unsupported claims

---

## Current Core Governance Files

These files currently define the ecosystem baseline:

- `CONV-0000-GENE-REFERENCE_CONV_REGISTRY_*.md`
- `CONV-0001-GENE-GOV_NAMING_STANDARD_*.md`
- `CONV-0002-GENE-PLAN_ECOSYSTEM_WORKBOOK_*.md`
- `CONV-0003-GENE-RULE_WORKING_RULES_*.md`
- `CONV-0004-CHKM-PROMPT_CHECKMATE_*.md`
- `CONV-0005-LIFE-PROMPT_CHIEF_OF_STAFF_*.md`
- `CONV-0006-CTRL-PROMPT_TT_IT_MANAGEMENT_*.md`
- `CONV-0007-NEIR-PROMPT_CODING_WORKFLOW_*.md`

---

## Recommended Reading Order

1. `00-README-FIRST.md` (this file)
2. Latest `CONV-0001-GENE-GOV_NAMING_STANDARD_*.md`
3. Latest `CONV-0003-GENE-RULE_WORKING_RULES_*.md`
4. Latest `CONV-0000-GENE-REFERENCE_CONV_REGISTRY_*.md`
5. Latest agent prompt file needed for the task
6. Latest agent-specific `00-README-FIRST.md`

---

## Execution Rule

Do not start generating new structural files or new agent files without checking:
- naming standard
- working rules
- registry
- latest structure decisions

If anything changed, declare it first.

---

## Next Valid Build Sequence

Recommended order from this point:

1. Root `00-README-FIRST.md` ✅
2. `LIFE/00-README-FIRST.md`
3. `CTRL/00-README-FIRST.md`
4. `NEIR/00-README-FIRST.md`
5. `CHKM/00-README-FIRST.md`
6. Further agent knowledge files as needed

---

## Final Reminder

This ecosystem is governed by discipline.

Planning first.
Rules first.
Then execution.
