Next file should be:

```text
03-ARTIFACT_SCHEMA.md
```

Here is the **full copy-paste block**:

````md
# 03-ARTIFACT_SCHEMA.md

# ARTIFACT SCHEMA

## Purpose

This file defines the standard structure, metadata, and minimum quality expectations for artifacts stored in the PROJECT-WIKI repository.

Its purpose is to:

- standardize documentation structure
- improve traceability
- support audit readiness
- make artifacts easier for AI and humans to review
- reduce ambiguity across projects
- ensure reusable and consistent project documentation

This schema applies to project documents, templates, SOPs, lessons learned, and governance artifacts unless a specific file type requires a specialized format.

---

# Core Principles

All artifacts should be:

- clear
- structured
- traceable
- reusable
- reviewable
- maintainable
- audit-friendly

Every artifact should help answer these questions:

- what is this file?
- why does it exist?
- who owns it?
- what initiative does it support?
- what state is it in?
- what other artifacts is it linked to?
- is it complete enough to be used?

---

# Minimum Required Metadata

Every formal artifact should begin with a metadata section.

Use this structure:

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
````

***

# Metadata Field Definitions

## Type

Defines what kind of artifact it is.

Allowed examples:

* PROJECT
* TEMPLATE
* SOP
* LESSON\_LEARNED
* REFERENCE
* PROMPT
* MEMORY
* ANALYSIS
* BUSINESS\_CASE
* CHANGE
* RISK\_ASSESSMENT
* UAT
* FRS
* PLAN
* COMMUNICATION
* STATUS\_REPORT

***

## Title

Human-readable name of the artifact.

Example:

```text
UK Message Delay – Business Case Review
```

***

## Owner

Primary person or team responsible for maintaining the artifact.

Example:

```text
BTS T&T
```

or

```text
Alfredo Dimaano Jr.
```

***

## Status

Defines maturity level.

Recommended values:

* DRAFT
* IN\_REVIEW
* APPROVED
* ACTIVE
* COMPLETED
* SUPERSEDED
* ARCHIVED
* REJECTED
* CANCELLED

***

## Project

Name of the related project or initiative.

Example:

```text
INEXTEND
```

If not project-specific, use:

```text
N/A
```

***

## Related Demand

Demand identifier if applicable.

Example:

```text
DMND0012345
```

***

## Related Change

Change identifier if applicable.

Example:

```text
CHG1234567
```

***

## Related ADO / Ticket

Azure DevOps ID, ServiceNow task, vendor ticket, or similar tracking reference.

Example:

```text
ADO-2451
```

***

## Workflow State

Current delivery state associated with the artifact.

Examples:

* NEW\_REQUEST
* TRIAGE
* QUALIFICATION
* BUSINESS\_CASE\_REVIEW
* ANALYSIS
* CHANGE\_READY
* IN\_UAT
* DEPLOYED
* CLOSED

***

## Version

Artifact version.

Examples:

```text
v0.1
v1.0
v1.1
```

***

## Created

Creation date in a consistent format.

Recommended format:

```text
YYYY-MM-DD
```

***

## Last Updated

Last update date in a consistent format.

Recommended format:

```text
YYYY-MM-DD
```

***

## Source

Origin of the information.

Examples:

* Requestor interview
* Vendor estimate
* ServiceNow demand
* Teams discussion
* Internal workshop
* Existing SOP
* Manual analysis

***

## Tags

Keywords for search and classification.

Examples:

```text
#demand #uat #inexto #change #tandt
```

***

# Standard Artifact Layout

Unless a specialized template overrides it, artifacts should follow this general structure:

```md
# Title

## Metadata
...

## Purpose
...

## Background
...

## Scope
...

## Assumptions
...

## Details / Analysis
...

## Risks / Issues
...

## Recommendations / Decisions
...

## Next Actions
...

## Linked Artifacts
...
```

***

# Minimum Required Sections by Artifact Type

## 1. Project Artifact

Required sections:

* Metadata
* Purpose
* Background
* Scope
* Assumptions
* Current State
* Risks / Issues
* Next Actions
* Linked Artifacts

***

## 2. Business Case Artifact

Required sections:

* Metadata
* Business Need
* Benefit Summary
* Cost Summary
* ROI / Value View
* Assumptions
* Risks
* Recommendation
* Linked Artifacts

***

## 3. Functional Analysis Artifact

Required sections:

* Metadata
* Objective
* Business Requirement Summary
* Functional Scope
* Assumptions
* Dependencies
* Constraints
* Open Questions
* Recommendation

***

## 4. Technical Analysis Artifact

Required sections:

* Metadata
* Objective
* Technical Context
* Proposed Solution
* Dependencies
* Constraints
* Risks
* Alternatives
* Recommendation

***

## 5. Change Artifact

Required sections:

* Metadata
* Change Objective
* Change Classification
* Impact Summary
* Risk Summary
* Implementation Window
* Rollback / Backout Considerations
* Approvals
* Linked Artifacts

***

## 6. UAT Artifact

Required sections:

* Metadata
* UAT Scope
* Test Scenarios
* Entry Criteria
* Exit Criteria
* Defects / Issues
* Sign-Off Status
* Linked Artifacts

***

## 7. Project Plan Artifact

Required sections:

* Metadata
* Objective
* Scope
* Assumptions
* Milestones
* Dependencies
* Risks
* Timeline
* Owners
* Due Dates

***

## 8. SOP Artifact

Required sections:

* Metadata
* Purpose
* Scope
* Roles and Responsibilities
* Inputs
* Process Steps
* Exceptions
* Outputs
* Related References

***

## 9. Lessons Learned Artifact

Required sections:

* Metadata
* Situation
* What Happened
* Root Cause / Key Factor
* Impact
* What Worked
* What Did Not Work
* Recommendation for Future Use
* Related Artifacts

***

## 10. Communication Artifact

Required sections:

* Metadata
* Audience
* Purpose
* Main Message
* Required Action
* Sender / Owner
* Related Reference

***

# Mandatory Traceability Rules

Artifacts should be linked whenever relevant.

Minimum traceability expectations:

```text
Demand
→ Business Case
→ Functional Analysis
→ Technical Analysis
→ Change
→ UAT
→ Deployment / Closure
```

If an artifact is part of a delivery chain, it should reference:

* upstream artifact
* downstream artifact
* project index if available

***

# Linked Artifacts Section

Use this structure:

```md
## Linked Artifacts

- Demand: DMND0012345
- Business Case: 02-BUSINESS_CASE.md
- Functional Analysis: 03-FUNCTIONAL_ANALYSIS.md
- Technical Analysis: 04-TECHNICAL_ANALYSIS.md
- Change: CHG1234567
- UAT: 08-UAT_PLAN.md
- Project Index: 00-INDEX.md
```

If not applicable, write:

```text
N/A
```

***

# Artifact Status Rules

## DRAFT

Artifact is being prepared and is not yet review-ready.

## IN\_REVIEW

Artifact is under active review.

## APPROVED

Artifact has been accepted for use.

## ACTIVE

Artifact is currently in operational use.

## COMPLETED

Artifact reflects completed work.

## SUPERSEDED

Artifact has been replaced by a newer version.

## ARCHIVED

Artifact is retained for history only.

## REJECTED

Artifact or proposal was not accepted.

## CANCELLED

Artifact is no longer needed due to initiative cancellation.

***

# Versioning Rules

Use simple versioning:

## Draft stage

```text
v0.1
v0.2
v0.3
```

## Approved stage

```text
v1.0
v1.1
v1.2
```

## Major revision

```text
v2.0
```

Update version when:

* scope changes significantly
* recommendation changes significantly
* approved version is revised
* governance-critical information changes

***

# Naming Rules

Recommended naming pattern:

```text
NN-ARTIFACT_NAME.md
```

Examples:

```text
00-INDEX.md
01-BUSINESS_CASE.md
02-FUNCTIONAL_ANALYSIS.md
03-TECHNICAL_ANALYSIS.md
04-CHANGE_SUMMARY.md
05-UAT_PLAN.md
06-DEPLOYMENT_NOTES.md
```

Guidelines:

* use uppercase or consistent naming style
* avoid spaces if possible
* keep names descriptive but concise
* use numbering where file order matters

***

# Quality Validation Checklist

Before an artifact is considered usable, validate:

## Completeness

* are required sections present?

## Clarity

* is the purpose understandable?

## Traceability

* are linked artifacts identified?

## Ownership

* is the owner defined?

## Status

* is the maturity/state clear?

## Consistency

* does the content contradict other known documents?

## Reusability

* can this be reused or referenced later?

## Governance

* does it support review, approval, or audit if needed?

***

# Minimum Approval Expectations

Not all artifacts require approval, but governance-relevant artifacts should show approval status clearly.

Examples of artifacts that may require explicit approval:

* business case
* FRS
* change summary
* UAT sign-off
* deployment readiness summary
* final closure summary

Recommended approval note structure:

```md
## Approval Status

Business Approval:
IT Approval:
Change Approval:
UAT Sign-Off:
Final Status:
```

***

# Assumption Rules

If assumptions exist, they must be explicitly documented.

Use:

```md
## Assumptions

- Assumption 1
- Assumption 2
- Assumption 3
```

Assumptions must never be mixed with confirmed facts.

***

# Risk Rules

If risks are relevant, include:

```md
## Risks

- Risk:
  Impact:
  Likelihood:
  Mitigation:

- Risk:
  Impact:
  Likelihood:
  Mitigation:
```

This is especially important for:

* business cases
* technical analysis
* changes
* project plans
* deployment readiness

***

# Project Index Relationship

Every major project should ideally have:

```text
00-INDEX.md
```

All major project artifacts should be linked from that index.

The project index acts as the master navigation point for:

* current state
* owners
* related documents
* approvals
* milestones
* open risks

***

# AI Handling Rules

The AI agent should use this schema to:

* validate whether an artifact is complete
* identify missing metadata
* recommend missing sections
* enforce traceability
* improve consistency
* standardize future outputs

If a user provides an unstructured document, the AI should help convert it into schema-compliant form where appropriate.

***

# Success Criteria

The artifact schema is successful when:

* artifacts are easy to understand
* metadata is consistent
* project traceability improves
* documents become easier to review
* audits become easier to support
* AI can navigate the repository more reliably
* reusable knowledge is easier to preserve

```

If you want, **next file should be `01-STATES.md`**, and I can give that in the same format.
```
