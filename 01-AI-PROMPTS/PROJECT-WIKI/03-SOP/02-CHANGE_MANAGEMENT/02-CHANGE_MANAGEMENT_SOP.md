# CHANGE MANAGEMENT SOP

## Metadata

Type: SOP
Title: Change Management SOP
Owner: BTS T&T
Status: ACTIVE
Workflow State: N/A
Version: v1.0
Created:
Last Updated:
Tags: #change #deployment #uat #governance #risk

---

# Purpose

This SOP defines the standard process for managing changes from approved initiative through implementation, deployment, stabilization, and closure.

The objective is to ensure:

- controlled implementation
- appropriate governance
- risk visibility
- deployment readiness
- production stability
- auditability and traceability

---

# Scope

This SOP applies to:

- enhancements
- application changes
- integrations
- configuration updates
- reporting changes
- serialization changes
- vendor-delivered solutions
- production deployments

This SOP does not replace:

- incident management
- problem management
- service request fulfillment

---

# Roles and Responsibilities

## Change Manager

Responsible for:

- change governance
- readiness validation
- implementation control
- deployment coordination
- approval validation

---

## Business Owner

Responsible for:

- approving business impact
- validating readiness
- confirming business acceptance

---

## BTS Owner

Responsible for:

- functional alignment
- requirements validation
- business coordination

---

## Technical Owner

Responsible for:

- implementation planning
- technical validation
- deployment support

---

## Vendor

Responsible for:

- solution delivery
- technical documentation
- implementation support

---

## UAT Lead

Responsible for:

- UAT execution
- business testing coordination
- sign-off collection

---

# Process Workflow

```text
Approved Solution
        ↓
Change Classification
        ↓
Risk Assessment
        ↓
Implementation Planning
        ↓
Build / Configuration
        ↓
Testing
        ↓
UAT
        ↓
Go-Live Readiness
        ↓
Deployment
        ↓
Hypercare
        ↓
Closure
```

---

# Step 1 – Change Classification

## Objective

Determine the correct governance path.

---

## Change Types

### Standard Change

Use when:

- repeatable
- pre-approved
- low risk
- known implementation process exists

Examples:

- recurring maintenance
- standard operational activities

---

### Normal Change

Use when:

- implementation requires review
- testing is required
- approvals are required
- production impact exists

Examples:

- enhancements
- integrations
- reporting modifications

---

### Emergency Change

Use when:

- urgent business need exists
- critical production issue exists
- waiting is not acceptable

Examples:

- critical defect fixes
- mandatory compliance corrections

---

# Step 2 – Risk Assessment

## Objective

Understand implementation risk before work proceeds.

---

## Review Areas

- business impact
- operational impact
- technical impact
- integration impact
- vendor dependency
- deployment complexity
- rollback complexity

---

## Risk Levels

### Low

Minor impact

Limited dependencies

Limited production exposure

---

### Medium

Moderate complexity

Some dependencies

Controlled deployment risk

---

### High

Major production impact

Cross-system dependencies

Complex deployment

Regulatory exposure

---

# Step 3 – Implementation Planning

## Objective

Prepare implementation activities.

---

## Required Inputs

- approved requirements
- approved scope
- approved analysis
- implementation approach

---

## Required Outputs

- implementation plan
- deployment plan
- resource plan
- support plan

---

# Step 4 – Build / Configuration

## Objective

Implement the approved solution.

---

## Activities

- development
- configuration
- integration updates
- vendor delivery
- internal validation

---

## Exit Criteria

```text
[ ] Build completed
[ ] Internal validation completed
[ ] No critical build issues
```

---

# Step 5 – Testing

## Objective

Verify technical quality.

---

## Activities

- functional testing
- integration testing
- regression testing
- defect correction

---

## Exit Criteria

```text
[ ] Testing completed
[ ] Critical defects resolved
[ ] Test evidence available
```

---

# Step 6 – User Acceptance Testing

## Objective

Validate business expectations.

---

## Activities

- execute UAT scenarios
- collect feedback
- log defects
- obtain sign-off

---

## Exit Criteria

```text
[ ] UAT completed
[ ] Business validation completed
[ ] Sign-off received
```

---

# Step 7 – Go-Live Readiness Review

## Objective

Determine deployment readiness.

---

## Required Validation

```text
[ ] Scope understood
[ ] Approvals completed
[ ] Risk assessment completed
[ ] Testing completed
[ ] UAT completed
[ ] Deployment plan available
[ ] Rollback plan available
[ ] Communications prepared
```

---

# Step 8 – Deployment

## Objective

Implement solution into production.

---

## Activities

### Pre-Deployment

- validate readiness
- notify stakeholders
- confirm deployment window

### Deployment

- execute implementation
- monitor deployment
- validate technical success

### Post-Deployment

- verify functionality
- confirm service availability
- communicate completion

---

# Step 9 – Hypercare

## Objective

Stabilize production operation.

---

## Activities

- issue monitoring
- defect correction
- business support
- production observation

---

## Exit Criteria

```text
[ ] No critical production issues
[ ] Business confirms stability
[ ] Hypercare objectives completed
```

---

# Step 10 – Closure

## Objective

Formally close the implementation.

---

## Activities

- closure review
- lessons learned
- documentation updates
- archive records

---

## Deliverables

- closure summary
- lessons learned
- deployment record
- updated documentation

---

# FRS Requirements

FRS should be reviewed when:

- functional requirements exist
- scope requires formal validation
- business sign-off is required

---

## Minimum FRS Validation

```text
[ ] Scope approved
[ ] Requirements documented
[ ] Assumptions confirmed
[ ] Business acceptance recorded
```

---

# UAT Requirements

UAT should be reviewed when:

- user-facing functionality changes
- business process changes
- regulatory requirements exist

---

## Minimum UAT Validation

```text
[ ] Test scope defined
[ ] Test users assigned
[ ] Test data available
[ ] Sign-off process defined
```

---

# Rollback Planning

For production-impacting changes, document:

## Rollback Available

- Yes
- No
- Partial

---

## Rollback Trigger

-

---

## Rollback Steps

-

---

## Rollback Owner

-

---

# Communication Requirements

The following communications should be considered:

- approval request
- UAT coordination
- deployment notification
- deployment completion
- closure notification

---

# Required Artifacts

## Mandatory

- Risk Assessment
- Change Record
- Implementation Plan

---

## Conditional

- Business Case
- FRS
- UAT Plan
- Deployment Checklist
- Rollback Plan

---

# Workflow States

## CHANGE_READY

Governance preparation.

---

## IN_DEVELOPMENT

Implementation underway.

---

## IN_TESTING

Testing underway.

---

## IN_UAT

Business validation underway.

---

## GO_LIVE_READY

Ready for deployment.

---

## DEPLOYED

Implemented in production.

---

## HYPERCARE

Stabilization period.

---

## CLOSED

Implementation completed.

---

# Readiness Checklist

```text
[ ] Change classified
[ ] Risk assessed
[ ] Scope validated
[ ] Approvals identified
[ ] Testing completed
[ ] UAT completed
[ ] Rollback documented
[ ] Deployment plan reviewed
[ ] Communication plan prepared
[ ] Support ownership defined
```

---

# Escalation Conditions

Escalate when:

- critical risk remains unresolved
- sign-off is missing
- deployment risk is excessive
- rollback strategy is unclear
- business and technical teams disagree
- UAT fails
- production readiness is uncertain

---

# Metrics

Suggested KPIs:

- change success rate
- change failure rate
- deployment success rate
- rollback frequency
- emergency change volume
- UAT pass rate
- post-go-live incidents

---

# Related Artifacts

- CHANGE_TEMPLATE.md
- RISK_ASSESSMENT_TEMPLATE.md
- FRS_TEMPLATE.md
- UAT_TEMPLATE.md
- PROJECT_PLAN_TEMPLATE.md
- WORKFLOW_STATES.md
- CHANGE_MANAGER.md

---

# Revision History

| Version | Date | Author | Description |
|----------|----------|----------|----------|
| v1.0 | | | Initial Version |