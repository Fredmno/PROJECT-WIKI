# PROJECT-WIKI
A flat, centralized storage for all project documentation — specs, flowcharts, decisions, hardening notes, and integration references. No hierarchy, no fluff. Drop a doc, tag it, find it later. Works for Kuya B, Power Automate experiments, or anything else that needs a paper trail.

### PROJECT-WIKI STRUCTURE
```
PROJECT-WIKI
│
├── 01-AI-PROMPTS
│   │
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
│   │   └── 12-TEAMS_TEMPLATE.md
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

###Purpose of each top-level folder
```
01-AI-PROMPTS
= Agent brain
= Prompts, modes, templates, memory

02-PROJECTS
= Working project documentation
= Active and completed initiatives

03-SOP
= Standard operating procedures
= Repeatable processes

04-LESSONS_LEARNED
= Historical knowledge
= Reusable experiences and fixes

05-REFERENCES
= Vendor documentation
= System documentation
= Regulatory references
```

###Agent Workflow
```
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

###Workflow States
```
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
```
