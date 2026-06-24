# DOCUMENTATION STANDARDS SOP

## Metadata

Type: SOP
Title: Documentation Standards SOP
Owner: BTS T&T
Status: ACTIVE
Workflow State: N/A
Version: v1.0
Created:
Last Updated:
Tags: #documentation #governance #standards #knowledge #audit

---

# Purpose

This SOP defines the documentation standards used within the PROJECT-WIKI repository.

The objective is to ensure that documentation is:

- consistent
- traceable
- auditable
- reusable
- maintainable
- easy to understand
- AI-friendly

This SOP establishes minimum requirements for all project, governance, knowledge, and operational documentation.

---

# Scope

This SOP applies to:

- project documentation
- demand documentation
- business cases
- functional analysis
- technical analysis
- project plans
- change records
- UAT documents
- lessons learned
- SOPs
- templates
- reference documents
- knowledge articles

---

# Documentation Principles

## Clarity

Documentation should be understandable by:

- project teams
- business users
- technical teams
- auditors
- future team members

Avoid:

- ambiguous language
- undocumented assumptions
- unclear ownership

---

## Consistency

Documentation should follow:

- standard naming conventions
- standard metadata
- standard structure
- standard terminology

---

## Traceability

Documentation should always show:

- owner
- related project
- related demand
- related change
- workflow state
- approval status where applicable

---

## Reusability

Documentation should be written so it can:

- support future projects
- serve as a reference
- become an SOP
- become a template
- become a lesson learned

---

## Auditability

Key decisions, assumptions, risks, and approvals should be documented.

Documentation should support:

- reviews
- audits
- project history reconstruction

---

# Repository Classification

All documents should be classified into one of the following categories.

---

## PROJECT

Examples:

- Business Case
- Analysis
- Project Plan
- Change Summary
- UAT Package

Location:

```text
02-PROJECTS
```

---

## SOP

Examples:

- Demand Management SOP
- Change Management SOP
- UAT SOP

Location:

```text
03-SOP
```

---

## LESSON_LEARNED

Examples:

- Project lessons
- Deployment lessons
- Incident lessons

Location:

```text
04-LESSONS_LEARNED
```

---

## REFERENCE

Examples:

- Vendor documentation
- Regulatory guidance
- Technical manuals

Location:

```text
05-REFERENCES
```

---

## TEMPLATE

Examples:

- Demand Template
- FRS Template
- Status Report Template

Location:

```text
01-AI-PROMPTS/20-TEMPLATES
```

---

# Mandatory Metadata Standard

All formal artifacts should begin with the following metadata block.

```md
Type:
Title:
Owner:
Status:
Project:
Related Demand:
Related Change:
Related ADO / Ticket:
Workflow State:
Version:
Created:
Last Updated:
Source:
Tags:
```

---

# Status Definitions

Allowed Status Values:

```text
DRAFT
IN_REVIEW
APPROVED
ACTIVE
COMPLETED
SUPERSEDED
ARCHIVED
REJECTED
CANCELLED
```

Refer to:

```text
01-STATES.md
```

for detailed definitions.

---

# Workflow State Definitions

Allowed Workflow States:

```text
NEW_REQUEST
TRIAGE
QUALIFICATION
BUSINESS_CASE_REVIEW
ANALYSIS
SOLUTION_DESIGN
VENDOR_ESTIMATION
APPROVAL_PENDING
CHANGE_READY
IN_DEVELOPMENT
IN_TESTING
IN_UAT
GO_LIVE_READY
DEPLOYED
HYPERCARE
CLOSED
```

Refer to:

```text
02-WORKFLOW_STATES.md
```

for detailed definitions.

---

# Standard Document Structure

Unless a template defines otherwise, documentation should follow:

```md
# Title

## Purpose

## Background

## Scope

## Assumptions

## Details / Analysis

## Risks

## Recommendations

## Next Actions

## Linked Artifacts
```

---

# Naming Convention Standard

## File Naming Format

```text
NN-FILE_NAME.md
```

Examples:

```text
00-INDEX.md
01-BUSINESS_CASE.md
02-FUNCTIONAL_ANALYSIS.md
03-TECHNICAL_ANALYSIS.md
04-CHANGE_SUMMARY.md
05-UAT_RESULTS.md
```

---

## Naming Rules

Use:

- descriptive names
- uppercase words where appropriate
- underscores instead of spaces

Avoid:

- special characters
- overly long names
- vague names

---

# Versioning Standard

## Draft Versions

```text
v0.1
v0.2
v0.3
```

---

## Approved Versions

```text
v1.0
v1.1
v1.2
```

---

## Major Revisions

```text
v2.0
v3.0
```

---

# Traceability Requirements

Where applicable, documents should be linked.

Standard traceability path:

```text
Demand
    ↓
Business Case
    ↓
Functional Analysis
    ↓
Technical Analysis
    ↓
Change
    ↓
UAT
    ↓
Deployment
    ↓
Closure
```

---

# Linked Artifacts Section

Use:

```md
## Linked Artifacts

Demand:
-

Business Case:
-

FRS:
-

Change:
-

UAT:
-

Deployment:
-
```

---

# Documentation Quality Requirements

Every document should address:

## Purpose

Why does the document exist?

---

## Ownership

Who owns the document?

---

## Scope

What is covered?

---

## Assumptions

What assumptions exist?

---

## Risks

What risks are known?

---

## Actions

What should happen next?

---

## References

What supporting documentation exists?

---

# Assumption Documentation Standard

If assumptions exist:

Use:

```md
## Assumptions

-
-
-
```

Assumptions should never be presented as facts.

---

# Risk Documentation Standard

If risks exist:

Use:

```md
## Risks

Risk:
Impact:
Likelihood:
Mitigation:
Owner:
```

---

# Approval Documentation Standard

For reviewable documents:

Use:

```md
## Approval Status

Business Approval:
Technical Approval:
Governance Approval:
Status:
Comments:
```

---

# Meeting Documentation Standard

Minimum sections:

```md
Meeting Purpose

Participants

Discussion Summary

Decisions

Actions

Owners

Due Dates
```

---

# Lessons Learned Standard

Minimum sections:

```md
Situation

What Happened

Impact

Root Cause

What Worked

What Did Not Work

Recommendations

Reusable Pattern
```

---

# SOP Standard

Minimum sections:

```md
Purpose

Scope

Roles and Responsibilities

Process

Inputs

Outputs

Exceptions

Related Artifacts
```

---

# Review Requirements

Documents should be reviewed for:

```text
[ ] Clarity
[ ] Completeness
[ ] Consistency
[ ] Traceability
[ ] Ownership
[ ] Reusability
[ ] Governance Compliance
```

---

# Common Documentation Issues

Avoid:

## Missing Ownership

Documents without owners.

---

## Missing Assumptions

Hidden assumptions.

---

## Missing Risks

Undocumented risks.

---

## Missing Links

No related artifact references.

---

## Duplicate Documentation

Creating multiple conflicting versions.

---

## Unclear Status

No indication of maturity.

---

# AI Documentation Rules

When generating content, the AI should:

- follow repository templates
- add metadata where appropriate
- recommend missing sections
- improve readability
- improve traceability
- identify governance gaps
- maintain consistency with repository standards

---

# Knowledge Preservation Rules

If documentation contains valuable reusable knowledge:

Promote to:

```text
LESSONS_LEARNED
```

or

```text
SOP
```

or

```text
TEMPLATE
```

where appropriate.

---

# Documentation Completion Checklist

```text
[ ] Metadata completed
[ ] Purpose documented
[ ] Scope documented
[ ] Assumptions documented
[ ] Risks documented
[ ] Linked artifacts documented
[ ] Status assigned
[ ] Version assigned
[ ] Owner assigned
[ ] Next actions documented
```

---

# Required Artifacts

This SOP supports:

- DEMAND_TEMPLATE.md
- BUSINESS_CASE_TEMPLATE.md
- ROI_TEMPLATE.md
- FRS_TEMPLATE.md
- CHANGE_TEMPLATE.md
- UAT_TEMPLATE.md
- PROJECT_PLAN_TEMPLATE.md
- STATUS_REPORT_TEMPLATE.md

---

# Related Artifacts

- ARTIFACT_SCHEMA.md
- STATES.md
- WORKFLOW_STATES.md
- DOCUMENTATION_MASTER.md

---

# Revision History

| Version | Date | Author | Description |
|----------|----------|----------|----------|
| v1.0 | | | Initial Version |