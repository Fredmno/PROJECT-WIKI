# DEMAND MANAGEMENT SOP

## Metadata

Type: SOP
Title: Demand Management SOP
Owner: BTS T&T
Status: ACTIVE
Workflow State: N/A
Version: v1.0
Created:
Last Updated:
Tags: #demand #governance #qualification #evaluation

---

# Purpose

This SOP defines the standard process for managing requests, demands, enhancements, and initiatives from initial intake through qualification and approval readiness.

The objective is to ensure:

- consistent demand handling
- proper governance
- clear ownership
- traceable decision making
- standardized intake and qualification

---

# Scope

This SOP applies to:

- new business requests
- enhancements
- process improvements
- integration requests
- reporting requests
- compliance initiatives
- vendor-driven initiatives

This SOP does not apply to:

- incidents
- service requests
- operational support tickets
- routine changes
- standard changes

---

# Roles and Responsibilities

## Requestor

Responsible for:

- submitting the request
- providing business context
- explaining expected outcomes
- participating in clarification activities

---

## Demand Manager

Responsible for:

- intake review
- request classification
- demand qualification
- stakeholder identification
- routing recommendations

---

## Evaluator

Responsible for:

- business case validation
- benefit review
- feasibility assessment
- cost/value review

---

## Business Owner

Responsible for:

- confirming business need
- validating benefits
- approving scope

---

## Technical Owner

Responsible for:

- validating technical feasibility
- identifying dependencies
- providing technical input

---

# Process Workflow

```text
Request Received
        ↓
Demand Intake
        ↓
Classification
        ↓
Qualification
        ↓
Business Case Review
        ↓
Analysis
        ↓
Approval Decision
```

---

# Procedure

## Step 1 – Receive Request

### Objective

Capture the request.

### Inputs

- email
- Teams message
- meeting discussion
- workshop output
- stakeholder request

### Activities

- record request
- identify requestor
- identify business area
- identify business objective

### Output

- demand record
- demand template

---

## Step 2 – Initial Classification

### Objective

Determine the correct processing path.

### Classification Options

- Demand
- Incident
- Problem
- Service Request
- Standard Change
- Routine Change

### Decision Rule

If demand governance is not required:

```text
Do not continue through Demand Management.
```

Route to the correct process.

### Output

- classification decision

---

## Step 3 – Qualification

### Objective

Determine whether the request should proceed.

### Activities

Review:

- business need
- scope
- stakeholders
- assumptions
- dependencies

### Qualification Questions

- Is the request understandable?
- Is the request in scope?
- Does a business need exist?
- Is ownership clear?
- Is further investment justified?

### Output

- qualified demand summary

---

## Step 4 – Stakeholder Identification

### Objective

Identify all critical participants.

### Minimum Stakeholders

- requestor
- business owner
- process owner
- BTS owner
- technical owner
- vendor (if applicable)

### Output

- stakeholder register

---

## Step 5 – Existing Solution Review

### Objective

Avoid duplicate work.

### Activities

Check:

- existing project
- existing demand
- existing enhancement
- existing roadmap item
- existing routine process

### Output

- reuse recommendation

---

## Step 6 – Business Case Evaluation

### Objective

Determine whether the initiative should proceed.

### Review Areas

- value
- cost
- effort
- ROI
- compliance benefit
- operational benefit
- feasibility

### Output

- business case recommendation

---

## Step 7 – Approval Recommendation

### Objective

Determine next action.

### Possible Outcomes

- proceed
- proceed with conditions
- hold
- reject
- route elsewhere

### Output

- recommendation summary

---

# Required Artifacts

## Mandatory

- Demand Template
- Business Case
- Stakeholder Identification

---

## Conditional

- ROI Assessment
- Functional Analysis
- Technical Analysis
- Risk Assessment

---

# Workflow States

## NEW_REQUEST

Initial intake.

---

## TRIAGE

Classification review.

---

## QUALIFICATION

Validation and business understanding.

---

## BUSINESS_CASE_REVIEW

Value assessment.

---

## ANALYSIS

Detailed review.

---

## APPROVAL_PENDING

Waiting for decision.

---

## ON_HOLD

Paused.

---

## REJECTED

Will not proceed.

---

# Quality Checklist

```text
[ ] Business need identified
[ ] Scope identified
[ ] Stakeholders identified
[ ] Dependencies identified
[ ] Assumptions documented
[ ] Classification completed
[ ] Existing solutions reviewed
[ ] Business value understood
[ ] Recommendation documented
```

---

# Escalation Conditions

Escalate when:

- scope cannot be defined
- ownership is unclear
- stakeholders disagree
- compliance implications are unclear
- significant investment is required
- prioritization conflict exists

---

# Metrics

Suggested KPIs:

- demand intake volume
- qualification lead time
- approval rate
- rejection rate
- average evaluation duration
- demand-to-project conversion rate

---

# Related Artifacts

- DEMAND_TEMPLATE.md
- BUSINESS_CASE_TEMPLATE.md
- ROI_TEMPLATE.md
- WORKFLOW_STATES.md
- DEMAND_MANAGER.md

---

# Revision History

| Version | Date | Author | Description |
|----------|----------|----------|----------|
| v1.0 | | | Initial Version |