# 00-MANIFEST.md

# PROJECT-WIKI MANIFEST

## Purpose

This manifest serves as the master index for the PROJECT-WIKI repository.

Its purpose is to:

- Explain the repository structure.
- Define the purpose of each folder and file group.
- Describe how the AI agent should navigate the repository.
- Define dependencies between prompts, templates, memory, SOPs, projects, and references.
- Provide a single starting point for both humans and AI agents.

---

# Repository Overview

PROJECT-WIKI is a centralized knowledge repository designed to support:

- Demand Management
- Business Case Evaluation
- Project Planning
- Change Management
- Communication Management
- Documentation Management
- Knowledge Management

The repository acts as the operational knowledge base for the T&T Workflow Orchestrator architecture.

---

# Repository Structure

```text
PROJECT-WIKI
│
├── 01-AI-PROMPTS
├── 02-PROJECTS
├── 03-SOP
├── 04-LESSONS_LEARNED
└── 05-REFERENCES
```

---

# Folder Descriptions

## 01-AI-PROMPTS

Purpose:

Contains the AI operating system.

This folder defines:

- Agent identity
- Agent behavior
- Workflow orchestration
- Decision logic
- Templates
- Repository memory
- Artifact standards

Subfolders:

```text
10-MODES
20-TEMPLATES
30-MEMORY
```

---

## 02-PROJECTS

Purpose:

Contains all project-specific artifacts.

Examples:

- Demand Documents
- Business Cases
- Functional Analysis
- Technical Analysis
- Meeting Notes
- Change Documentation
- UAT Documentation
- Go-Live Documentation

Project artifacts should be organized according to project lifecycle and status.

---

## 03-SOP

Purpose:

Contains approved operating procedures.

Examples:

- Demand Management SOP
- Change Management SOP
- UAT SOP
- Release Management SOP
- Documentation Standards

SOP files are considered operational standards.

---

## 04-LESSONS_LEARNED

Purpose:

Capture organizational knowledge.

Examples:

- Project mistakes
- Project successes
- Change lessons
- Incident lessons
- Reusable solutions
- Best practices

Knowledge from completed projects should be promoted here when reusable.

---

## 05-REFERENCES

Purpose:

Store supporting and external information.

Examples:

- Vendor documentation
- Product documentation
- Platform documentation
- Regulatory references
- Integration specifications

Reference material should remain source-oriented and factual.

---

# AI Prompt Dependencies

The AI operating model follows this hierarchy:

```text
BASE_PROMPT
        ↓
ORCHESTRATOR
        ↓
SELECTED MODE
        ↓
TEMPLATE
        ↓
MEMORY
        ↓
PROJECT CONTEXT
```

---

# Prompt Files

## 01-BASE_PROMPT.md

Purpose:

Defines:

- Agent identity
- Core principles
- Global behavior
- Writing style
- Review methodology
- Quality standards

This file should remain mode-independent.

---

## 02-ORCHESTRATOR.md

Purpose:

Acts as the routing engine.

Responsibilities:

- Understand user intent
- Select appropriate mode
- Determine workflow stage
- Select supporting templates
- Reference memory when required

The Orchestrator does not perform work itself.

The Orchestrator determines which mode should perform the work.

---

# Modes

Location:

```text
10-MODES
```

Purpose:

Specialized operating behaviors.

---

## 01-DEMAND_MANAGER.md

Responsible for:

- Demand Intake
- Triage
- Classification
- Requirement Clarification
- Request Qualification

Determines whether a request should be treated as:

- Demand
- Incident
- Problem
- Service Request
- Routine Change

---

## 02-EVALUATOR.md

Responsible for:

- Business Case Review
- ROI Validation
- Benefit Analysis
- Cost Justification
- Feasibility Review
- Compliance Review
- Alternative Solution Evaluation

Challenges assumptions and recommends approval or rejection.

---

## 03-PLANNER.md

Responsible for:

- Timeline Creation
- Milestone Planning
- Resource Planning
- Dependency Mapping
- Delivery Scheduling

Creates realistic project plans.

---

## 04-CHANGE_MANAGER.md

Responsible for:

- Change Governance
- Change Classification
- Risk Assessment
- Emergency Change Handling
- UAT Readiness
- Production Readiness
- Deployment Validation

Validates readiness before implementation.

---

## 05-COMMUNICATOR.md

Responsible for:

- Email Drafting
- Teams Messages
- Escalations
- Stakeholder Updates
- Status Reports
- Approval Requests

Produces audience-appropriate communications.

---

## 06-DOCUMENTATION_MASTER.md

Responsible for:

- Documentation Creation
- Documentation Cleanup
- SOP Generation
- Wiki Maintenance
- Knowledge Capture

Ensures consistency and readability.

---

# Templates

Location:

```text
20-TEMPLATES
```

Purpose:

Provide reusable structures and standard outputs.

Templates are invoked by modes when needed.

Examples:

```text
Demand Template
Business Case Template
ROI Template
HTML Description Template
Change Template
Risk Assessment Template
FRS Template
UAT Template
Project Plan Template
Status Report Template
Email Template
Teams Template
Project Metadata Template
```

Templates should not contain project-specific content.

Templates should only define structure.

---

# Memory

Location:

```text
30-MEMORY
```

Purpose:

Provide reusable operational memory.

Contains:

```text
01-STATES.md
02-WORKFLOW_STATES.md
03-ARTIFACT_SCHEMA.md
```

Used to maintain consistency across projects.

---

## 01-STATES.md

Defines repository-level states.

Used to track artifact maturity and lifecycle.

---

## 02-WORKFLOW_STATES.md

Defines project delivery states.

Current workflow:

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

Optional States

ON_HOLD
REJECTED
CANCELLED
```

---

## 03-ARTIFACT_SCHEMA.md

Defines expected artifact structure.

Examples:

- Required sections
- Mandatory metadata
- Naming conventions
- Traceability standards
- Review requirements

---

# Recommended AI Navigation Strategy

When processing a request:

Step 1

Identify user intent.

Step 2

Determine workflow stage.

Step 3

Select appropriate mode.

Step 4

Retrieve supporting template.

Step 5

Reference relevant project files.

Step 6

Reference related SOPs.

Step 7

Reference lessons learned if available.

Step 8

Generate or validate output.

---

# Artifact Quality Framework

Every artifact should be assessed for:

## Completeness

Are required sections present?

## Consistency

Are there contradictions?

## Traceability

Can decisions be traced?

## Governance

Does the artifact support approvals and audits?

## Practicality

Can the proposed actions be executed?

## Reusability

Can future projects benefit?

## Risk

Are implementation risks documented?

---

# Design Principles

The PROJECT-WIKI repository is built on the following principles:

- Single Source of Truth
- Traceability
- Auditability
- Simplicity
- Reusability
- Governance
- Practicality
- Knowledge Retention
- Continuous Improvement
- AI-Assisted Delivery

---

# Repository Objective

Provide a maintainable knowledge ecosystem that supports BTS and Track & Trace delivery activities from request intake through deployment, closure, and lessons learned while enabling AI-assisted delivery and artifact validation.
