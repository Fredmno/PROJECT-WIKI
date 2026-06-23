````md
# 02-WORKFLOW_STATES.md

# WORKFLOW STATES

## Purpose

This file defines the standard workflow states used by the T&T Workflow Orchestrator.

Its purpose is to:

- Standardize project lifecycle tracking
- Align AI outputs with delivery progression
- Clarify expected activities per stage
- Define minimum governance expectations
- Improve traceability across demands, analysis, planning, change, testing, deployment, and closure
- Support consistent project reviews and artifact validation

This state model is used by the Orchestrator, Modes, Templates, and Project Index files.

---

# State Model Overview

The workflow follows this lifecycle:

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
````

Optional states:

```text
ON_HOLD
REJECTED
CANCELLED
```

***

# State Definitions

## 01. NEW\_REQUEST

### Description

Initial state when a request, idea, issue, or enhancement is first received.

### Objective

Capture the request and determine whether it requires formal processing.

### Typical Activities

* Record incoming request
* Capture initial summary
* Identify requestor
* Identify business need
* Log available context

### Expected Outputs

* Initial request description
* Request source
* Known stakeholders
* Initial assumptions

### Exit Criteria

* Enough information exists to begin triage

### Next State

```text
TRIAGE
```

***

## 02. TRIAGE

### Description

Initial screening stage to determine what kind of item has been received.

### Objective

Determine whether the request should be treated as:

* Demand
* Incident
* Problem
* Service Request
* Routine Change
* Standard Change
* Minor enhancement
* Other

### Typical Activities

* Review request intent
* Clarify unclear request details
* Assess whether formal demand process applies
* Identify possible alternative handling path

### Expected Outputs

* Classification recommendation
* Clarification questions if required
* Routing recommendation

### Exit Criteria

* Request type is understood
* Appropriate processing path is identified

### Next State

```text
QUALIFICATION
```

or

```text
REJECTED
CANCELLED
ON_HOLD
```

***

## 03. QUALIFICATION

### Description

Request is reviewed in enough detail to determine whether it is valid, in scope, and worth formal evaluation.

### Objective

Confirm that the request is meaningful, relevant, and ready for deeper business evaluation.

### Typical Activities

* Validate request scope
* Confirm affected area / service / application
* Identify key stakeholders
* Capture assumptions
* Confirm whether the request should proceed as a formal demand or change-related initiative

### Expected Outputs

* Qualified request summary
* Scope assumptions
* Stakeholder list
* Initial recommendation

### Exit Criteria

* Request is sufficiently understood
* Stakeholders and scope are identified
* Ready for business case review

### Next State

```text
BUSINESS_CASE_REVIEW
```

or

```text
REJECTED
ON_HOLD
```

***

## 04. BUSINESS\_CASE\_REVIEW

### Description

Business value, justification, and feasibility are evaluated.

### Objective

Determine whether the demand is justified from business, compliance, operational, and cost perspectives.

### Typical Activities

* Review benefits
* Evaluate ROI where applicable
* Assess quantitative and qualitative value
* Consider compliance / regulatory impact
* Review cost vs value
* Identify whether the request should proceed

### Expected Outputs

* Business case
* Benefit analysis
* ROI assessment
* Feasibility recommendation
* Standardized HTML description if required

### Expected Key Fields

* Benefit summary
* Regulations impacted
* Assumptions for scope
* Feasibility
* Effort estimate
* Cost estimate
* Duration estimate

### Exit Criteria

* Business case is sufficient for decision-making
* Initiative is justified or rejected

### Next State

```text
ANALYSIS
```

or

```text
REJECTED
ON_HOLD
```

***

## 05. ANALYSIS

### Description

Detailed functional and technical analysis begins.

### Objective

Define what needs to be done and assess possible solution paths.

### Typical Activities

* Functional analysis
* Technical analysis
* Requirement review
* Impact review
* Alternative option assessment
* Risk / value / size review

### Expected Outputs

* Functional analysis
* Technical analysis
* Assumptions
* Solution options
* Risk and impact notes

### Expected Key Fields

* Functional analysis
* Technical analysis
* Cost
* Effort
* Risk / Value / Size
* Action
* Start Date
* Due Date
* Vendor impact

### Exit Criteria

* Needs are clearly understood
* Analysis is complete enough for solution design

### Next State

```text
SOLUTION_DESIGN
```

***

## 06. SOLUTION\_DESIGN

### Description

The preferred solution is defined at a level suitable for planning and implementation preparation.

### Objective

Select the best solution path and clarify what will be delivered.

### Typical Activities

* Compare solution options
* Select preferred option
* Validate technical solution against functional needs
* Identify optimization opportunities
* Prepare implementation direction

### Expected Outputs

* Preferred solution summary
* Option comparison
* Design assumptions
* Delivery approach

### Exit Criteria

* Preferred solution is chosen
* Design direction is clear
* Ready for cost/vendor confirmation if needed

### Next State

```text
VENDOR_ESTIMATION
```

or

```text
APPROVAL_PENDING
```

***

## 07. VENDOR\_ESTIMATION

### Description

Used when vendor input, commercial pricing, or external effort estimation is required.

### Objective

Obtain external delivery estimates and understand cost/resource impact.

### Typical Activities

* Request vendor estimate
* Review quoted cost
* Estimate external effort
* Compare scenarios
* Update resource/cost plans

### Expected Outputs

* Vendor estimate
* Updated cost assumptions
* External effort estimate
* Timeline impact

### Exit Criteria

* Vendor-related cost and effort are known or reasonably estimated

### Next State

```text
APPROVAL_PENDING
```

***

## 08. APPROVAL\_PENDING

### Description

The initiative is waiting for formal decision or approval.

### Objective

Secure approval to proceed.

### Typical Activities

* Compile review package
* Request approvals
* Confirm stakeholders
* Confirm funding / prioritization / governance decision
* Resolve comments if needed

### Expected Outputs

* Approval record
* Decision summary
* Approval comments
* Conditions for proceeding

### Exit Criteria

* Approval received
* Or rejected / deferred / put on hold

### Next State

```text
CHANGE_READY
```

or

```text
REJECTED
ON_HOLD
CANCELLED
```

***

## 09. CHANGE\_READY

### Description

The initiative is approved and ready for formal implementation preparation.

### Objective

Prepare all required artifacts for implementation and production governance.

### Typical Activities

* Confirm change classification
* Prepare change request
* Prepare risk assessment
* Confirm readiness for build / config / implementation
* Confirm FRS sign-off where applicable
* Prepare UAT / deployment planning

### Expected Outputs

* Change classification
* Change record or change package
* Risk assessment
* FRS sign-off status
* Readiness summary

### Exit Criteria

* Governance and implementation prerequisites are complete
* Ready to start build / implementation activity

### Next State

```text
IN_DEVELOPMENT
```

***

## 10. IN\_DEVELOPMENT

### Description

Build, configuration, or implementation work is actively in progress.

### Objective

Deliver the approved solution.

### Typical Activities

* Configuration
* Development
* Integration work
* Internal validation
* Issue resolution

### Expected Outputs

* Built/configured solution
* Development notes
* Build status
* Internal progress updates

### Exit Criteria

* Solution is ready for formal testing

### Next State

```text
IN_TESTING
```

***

## 11. IN\_TESTING

### Description

Internal testing or technical validation is underway.

### Objective

Ensure the solution works as expected before user validation.

### Typical Activities

* Internal testing
* Defect logging
* Fix verification
* Regression review
* Technical validation

### Expected Outputs

* Test evidence
* Defect list
* Retest confirmation
* Readiness recommendation for UAT

### Exit Criteria

* Internal testing is sufficiently complete
* Solution is stable enough for UAT

### Next State

```text
IN_UAT
```

***

## 12. IN\_UAT

### Description

Business-side validation is in progress.

### Objective

Obtain user confirmation that the solution meets business expectations.

### Typical Activities

* Execute UAT scenarios
* Collect user feedback
* Track issues
* Confirm business acceptance
* Collect sign-off if required

### Expected Outputs

* UAT plan
* UAT execution evidence
* UAT defect list
* UAT sign-off or approval recommendation

### Exit Criteria

* UAT passed
* Or UAT issues identified for rework

### Next State

```text
GO_LIVE_READY
```

or back to:

```text
IN_DEVELOPMENT
IN_TESTING
```

***

## 13. GO\_LIVE\_READY

### Description

All required conditions for production deployment have been met.

### Objective

Confirm readiness for go-live.

### Typical Activities

* Final deployment review
* Confirm approvals
* Confirm rollback / backout readiness
* Confirm communication plan
* Confirm implementation schedule
* Confirm production support readiness

### Expected Outputs

* Go-live readiness summary
* Deployment checklist
* Rollback plan
* Communication plan
* Final approvals

### Exit Criteria

* All go-live conditions are satisfied
* Deployment date approved

### Next State

```text
DEPLOYED
```

***

## 14. DEPLOYED

### Description

Solution has been implemented in production.

### Objective

Confirm deployment completion and monitor immediate outcome.

### Typical Activities

* Deploy to production
* Verify successful implementation
* Communicate deployment completion
* Monitor initial behavior
* Confirm service stability

### Expected Outputs

* Deployment evidence
* Production verification
* Stakeholder update
* Initial support notes

### Exit Criteria

* Deployment completed successfully
* Stabilization decision made

### Next State

```text
HYPERCARE
```

or

```text
CLOSED
```

***

## 15. HYPERCARE

### Description

Short stabilization period after production deployment.

### Objective

Observe production performance and quickly address post-go-live issues.

### Typical Activities

* Monitor production behavior
* Resolve early defects
* Support users
* Confirm stability
* Capture lessons learned

### Expected Outputs

* Hypercare notes
* Issue log
* Stabilization confirmation
* Closure readiness recommendation

### Exit Criteria

* Solution is stable
* No blocking production issues remain

### Next State

```text
CLOSED
```

***

## 16. CLOSED

### Description

The initiative is complete.

### Objective

Formally close the work and preserve knowledge.

### Typical Activities

* Confirm closure
* Archive key artifacts
* Capture lessons learned
* Confirm final status
* Update project history

### Expected Outputs

* Closure summary
* Final artifact set
* Lessons learned
* Final status

### Exit Criteria

* Work is complete
* Required documentation is stored
* Closure confirmed

### Next State

```text
END
```

***

# Optional States

## ON\_HOLD

### Description

Work is paused due to dependency, priority, funding, resource, or decision delay.

### Use When

* input is missing
* approval is delayed
* priority changed
* dependency blocked progress

### Required Notes

* reason for hold
* owner of unblock action
* expected review date

***

## REJECTED

### Description

The request will not proceed.

### Use When

* request is out of scope
* value does not justify effort
* duplicate / unnecessary request
* incorrect process path
* no approval obtained

### Required Notes

* rejection reason
* recommended alternative path if applicable

***

## CANCELLED

### Description

The request was valid but has been intentionally stopped after initiation.

### Use When

* request withdrawn by requestor
* business priority changed
* superseded by another initiative
* no longer needed

### Required Notes

* cancellation reason
* linked replacement initiative if applicable

***

# Minimum State Metadata

For each active project or initiative, the following should be tracked:

```md
Current State:
Previous State:
State Owner:
State Start Date:
Target Next State:
Target Date:
Blocking Issues:
Linked Artifacts:
Approval Status:
```

***

# Recommended Artifact Expectations by State

## NEW\_REQUEST

* Initial request summary

## TRIAGE

* Classification recommendation

## QUALIFICATION

* Qualified scope summary
* Stakeholder list
* assumptions

## BUSINESS\_CASE\_REVIEW

* Business case
* ROI or value view
* HTML description if applicable

## ANALYSIS

* Functional analysis
* Technical analysis
* cost / effort / risk view

## SOLUTION\_DESIGN

* Solution options
* preferred approach
* optimization notes

## VENDOR\_ESTIMATION

* Vendor estimate
* external cost view

## APPROVAL\_PENDING

* Approval package
* approval record

## CHANGE\_READY

* Change template
* risk assessment
* FRS sign-off status
* implementation readiness

## IN\_DEVELOPMENT

* Build / configuration notes
* progress status

## IN\_TESTING

* Test evidence
* defect status

## IN\_UAT

* UAT plan
* UAT results
* sign-off status

## GO\_LIVE\_READY

* Deployment checklist
* rollback plan
* comms plan

## DEPLOYED

* Deployment confirmation
* production verification

## HYPERCARE

* issue tracking
* stabilization notes

## CLOSED

* closure summary
* lessons learned

***

# Mapping to Official / External Process States

If needed, internal workflow states may be mapped to external systems or official process stages.

Example mapping:

```text
Internal State              External / Official Equivalent
----------------------------------------------------------
NEW_REQUEST                 Draft / Intake
TRIAGE                      Submitted / Screening
QUALIFICATION               Qualified
BUSINESS_CASE_REVIEW        Qualified / Assessment
ANALYSIS                    Assessment / Analysis
SOLUTION_DESIGN             Solution Definition
APPROVAL_PENDING            Approval
CHANGE_READY                Approved / Ready for Change
IN_DEVELOPMENT              Build / Implementation
IN_TESTING                  Internal Testing
IN_UAT                      UAT
GO_LIVE_READY               Go-Live Approval
DEPLOYED                    Implemented
HYPERCARE                   Stabilization
CLOSED                      Completed / Closed
```

This mapping should be adapted where needed for ServiceNow, Azure DevOps, or local governance processes.

***

# State Transition Rules

General rules:

1. A state should not be advanced without minimum required information.
2. Missing mandatory artifacts must be highlighted before progression.
3. State changes should be documented in the project index.
4. If critical approval is missing, progression should stop.
5. If scope changes significantly, the initiative may return to:
   * QUALIFICATION
   * BUSINESS\_CASE\_REVIEW
   * ANALYSIS
6. If testing fails, the initiative may return to:
   * IN\_DEVELOPMENT
   * IN\_TESTING
7. If deployment readiness fails, the initiative should not leave:
   * GO\_LIVE\_READY

***

# AI Usage Rules

The Orchestrator and all modes should use workflow states to:

* understand project maturity
* decide what output is needed next
* identify missing artifacts
* prevent governance gaps
* improve traceability
* produce context-aware recommendations

The workflow state should influence:

* template selection
* validation depth
* recommended next actions
* approval reminders
* communication drafts
* documentation expectations

***

# Success Criteria

The workflow state model is successful when it:

* makes project progress easy to understand
* improves artifact traceability
* reduces governance gaps
* supports auditing and review
* helps the AI provide the right next-step guidance
* supports end-to-end delivery from intake to closure

```

If you want, next I can give you **`03-ARTIFACT_SCHEMA.md`** in the same full copy-paste block style.
```
