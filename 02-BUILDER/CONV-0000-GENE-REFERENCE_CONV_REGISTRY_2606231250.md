# CONV-0000-GENE-REFERENCE_CONV_REGISTRY_2606231250

Date: 2026-06-23
Status: Active
Type: REFERENCE
Agent Code: GENE
Trace No: 0000

## Purpose

Provide the master registry for CONV numbering and latest-version lookup in the FOURTH ANGELS ecosystem.

## Registry Rules

- This registry is a real markdown file in the repository.
- This registry is part of the ecosystem structure.
- This registry is the source of truth for CONV numbering and latest-version lookup.
- This registry must be updated whenever a new CONV file is created.
- This registry must be updated whenever a newer timestamp version is created for an existing CONV ID.
- Numbers are global across the ecosystem.
- Numbers are never reused.
- Numbers are never reset.
- Numbers are never renumbered.

## Current Registry

| CONV ID | AGENT | TYPE | SUBJECT | LATEST VERSION | CURRENT FILE |
|---------|-------|------|---------|----------------|--------------|
| 0000 | GENE | REFERENCE | CONV_REGISTRY | 2606231250 | CONV-0000-GENE-REFERENCE_CONV_REGISTRY_2606231250.md |
| 0001 | GENE | GOV | NAMING_STANDARD | 2606231251 | CONV-0001-GENE-GOV_NAMING_STANDARD_2606231251.md |
| 0002 | GENE | PLAN | ECOSYSTEM_WORKBOOK | 2606231252 | CONV-0002-GENE-PLAN_ECOSYSTEM_WORKBOOK_2606231252.md |
| 0003 | GENE | RULE | WORKING_RULES | 2606231253 | CONV-0003-GENE-RULE_WORKING_RULES_2606231253.md |
| 0004 | CHKM | PROMPT | CHECKMATE | 2606231254 | CONV-0004-CHKM-PROMPT_CHECKMATE_2606231254.md |

## Registry Maintenance Procedure

Before assigning a new number:
1. Open the latest registry file.
2. Identify the highest used CONV ID.
3. Assign the next available number.
4. Create the new file using the locked naming format.
5. Update the registry with the new entry.
6. If the file is a newer version of an existing CONV ID, update only the `LATEST VERSION` and `CURRENT FILE` fields.

## Notes

- The registry does not need full status tracking yet.
- The timestamp identifies the latest version for each CONV ID.
- Historical files remain valid records even after newer versions exist.
