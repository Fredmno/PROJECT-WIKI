# PROJECT-WIKI

Centralized knowledge repository for BTS and Track & Trace initiatives.

Stores AI prompts, project documentation, SOPs, lessons learned, references, templates, and workflow guidance.

Designed to support AI-assisted delivery, project governance, demand management, business case evaluation, planning, change management, communication, documentation, and knowledge management activities.

This repository serves as the single source of truth for project knowledge, reusable artifacts, delivery processes, and AI operating instructions.

---

# PROJECT-WIKI STRUCTURE

```text
PROJECT-WIKI
│
├── 01-AI-PROMPTS
│   │
│   ├── 00-MANIFEST.md
│   ├── 01-BASE_PROMPT.md
│   ├── 02-ORCHESTRATOR.md
│   │
│   ├── 10-MODES
│   │   │
│   │   ├── 01-DEMAND_MANAGER.md
│   │   ├── 02-EVALUATOR.md
│   │   ├── 03-PLANNER.md
│   │   ├── 04-CHANGE_MANAGER.md
│   │   ├── 05-COMMUNICATOR.md
│   │   └── 06-DOCUMENTATION_MASTER.md
│   │
│   ├── 20-TEMPLATES
│   │   │
│   │   ├── 01-DEMAND_TEMPLATE.md
│   │   ├── 02-BUSINESS_CASE_TEMPLATE.md
│   │   ├── 03-ROI_TEMPLATE.md
│   │   ├── 04-HTML_DESCRIPTION_TEMPLATE.md
│   │   ├── 05-CHANGE_TEMPLATE.md
│   │   ├── 06-RISK_ASSESSMENT_TEMPLATE.md
│   │   ├── 07-FRS_TEMPLATE.md
│   │   ├── 08-UAT_TEMPLATE.md
│   │   ├── 09-PROJECT_PLAN_TEMPLATE.md
│   │   ├── 10-STATUS_REPORT_TEMPLATE.md
│   │   ├── 11-EMAIL_TEMPLATE.md
│   │   ├── 12-TEAMS_TEMPLATE.md
│   │   └── 13-PROJECT_METADATA_TEMPLATE.md
│   │
│   └── 30-MEMORY
│       │
│       ├── 01-STATES.md
│       ├── 02-WORKFLOW_STATES.md
│       └── 03-ARTIFACT_SCHEMA.md
│
├── 02-PROJECTS
│   │
│   ├── ACTIVE
│   │   ├── INEXTEND
│   │   ├── INEXTRACK
│   │   ├── UK-MESSAGE-DELAY
│   │   ├── TM1
│   │   └── OTHER-PROJECTS
│   │
│   ├── COMPLETED
│   │
│   └── ON-HOLD
│
├── 03-SOP
│   │
│   ├── 01-DEMAND_MANAGEMENT
│   ├── 02-CHANGE_MANAGEMENT
│   ├── 03-UAT
│   ├── 04-RELEASE_MANAGEMENT
│   ├── 05-DOCUMENTATION_STANDARDS
│   └── 06-BEST_PRACTICES
│
├── 04-LESSONS_LEARNED
│   │
│   ├── 00-KNOWLEDGE_INDEX.md
│   ├── PROJECT_LESSONS
│   ├── INCIDENT_LESSONS
│   ├── CHANGE_LESSONS
│   └── REUSABLE_PATTERNS
│
└── 05-REFERENCES
    │
    ├── INEXTO
    ├── SAP_ATTP
    ├── AZURE_DEVOPS
    ├── SERVICENOW
    ├── POWER_AUTOMATE
    ├── INTEGRATION_REFERENCES
    └── REGULATIONS
```

---

# PURPOSE OF EACH TOP-LEVEL FOLDER

## 01-AI-PROMPTS

Agent Brain

Contains:

- Base Agent Instructions
- Workflow Orchestration Rules
- Specialized Modes
- Templates
- Memory Definitions
- State Models
- Artifact Standards

Purpose:

- Define how the AI operates
- Define decision logic
- Define output standards
- Define reusable delivery frameworks

---

## 02-PROJECTS

Project Workspace

Contains:

- Active initiatives
- Completed projects
- On-hold work
- Project documents
- Analyses
- Plans
- Meeting outputs
- Business artifacts

Purpose:

- Store all project-specific documentation
- Maintain project history and traceability
- Support ongoing delivery activities

---

## 03-SOP

Standard Operating Procedures

Contains:

- Demand Management processes
- Change Management processes
- UAT procedures
- Release procedures
- Documentation standards
- Delivery best practices

Purpose:

- Define repeatable processes
- Ensure consistency
- Support onboarding and governance

---

## 04-LESSONS_LEARNED

Organizational Knowledge Repository

Contains:

- Project lessons
- Incident lessons
- Change lessons
- Reusable patterns
- Known issues
- Best practices

Purpose:

- Prevent repeated mistakes
- Promote continuous improvement
- Capture institutional knowledge

---

## 05-REFERENCES

Reference Library

Contains:

- Vendor documentation
- Product documentation
- Regulatory references
- Technical references
- Integration guidance

Purpose:

- Provide supporting knowledge
- Store authoritative references
- Support analysis and solution design

---

# AGENT ARCHITECTURE

The repository supports a single AI agent using an orchestrator model.

```text
User Request
     │
     ▼
ORCHESTRATOR
     │
     ├── DEMAND_MANAGER
     │
     ├── EVALUATOR
     │
     ├── PLANNER
     │
     ├── CHANGE_MANAGER
     │
     ├── COMMUNICATOR
     │
     └── DOCUMENTATION_MASTER
```

---

# MODE RESPONSIBILITIES

## DEMAND_MANAGER

Responsible for:

- Demand intake
- Triage
- Classification
- Requirement clarification
- Demand qualification
- Routing recommendations

Determines whether a request should be:

- Demand
- Incident
- Problem
- Service Request
- Routine Change

---

## EVALUATOR

Responsible for:

- Business case review
- ROI assessment
- Benefit analysis
- Compliance assessment
- Feasibility analysis
- Solution option analysis
- Functional and technical alignment validation

Validates:

- Cost
- Effort
- Value
- Risk
- Scope assumptions
- Recommendation for approval

---

## PLANNER

Responsible for:

- Timeline creation
- Milestone planning
- Due date estimation
- Resource planning
- Dependency mapping
- Delivery scheduling

Creates project roadmaps from start to completion.

---

## CHANGE_MANAGER

Responsible for:

- Change classification
- Change governance
- Risk assessment
- Emergency change handling
- Production readiness
- UAT readiness
- Go-live readiness
- FRS sign-off validation

---

## COMMUNICATOR

Responsible for:

- Email drafting
- Teams message drafting
- Status reports
- Stakeholder updates
- Escalations
- Approval requests
- Project communications

---

## DOCUMENTATION_MASTER

Responsible for:

- Documentation creation
- Wiki maintenance
- SOP generation
- Template standardization
- Knowledge capture
- Documentation quality improvement

---

# WORKFLOW STATES

```text
NEW_REQUEST
↓
TRIAGE
↓
QUALIFICATION
↓
BUSINESS_CASE_REVIEW
↓
ANALYSIS
↓
SOLUTION_DESIGN
↓
VENDOR_ESTIMATION
↓
APPROVAL_PENDING
↓
CHANGE_READY
↓
IN_DEVELOPMENT
↓
IN_TESTING
↓
IN_UAT
↓
GO_LIVE_READY
↓
DEPLOYED
↓
HYPERCARE
↓
CLOSED

Optional States

ON_HOLD
REJECTED
CANCELLED
```

---

# DESIGN PRINCIPLES

The PROJECT-WIKI repository is designed around the following principles:

- Single source of truth
- Auditability
- Traceability
- Reusability
- Standardization
- Knowledge retention
- Process governance
- Practical execution
- Continuous improvement
- AI-assisted delivery

---

# SUCCESS CRITERIA

A project artifact is considered complete when it:

- Has a clear objective
- Defines scope
- Documents assumptions
- Identifies dependencies
- Captures risks
- Includes owners and stakeholders
- Supports traceability
- Aligns with governance requirements
- Is understandable by future team members
- Can be reused where applicable

---

# REPOSITORY OBJECTIVE

The ultimate goal of PROJECT-WIKI is to provide a centralized, maintainable, and reusable knowledge ecosystem that supports BTS and Track & Trace delivery activities from demand intake through deployment, documentation, and lessons learned.
