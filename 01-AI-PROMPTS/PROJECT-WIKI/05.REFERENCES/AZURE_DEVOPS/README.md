\# AZURE DEVOPS REFERENCE LIBRARY



\## Metadata



Type: REFERENCE

Title: Azure DevOps Reference Library

Owner: BTS T\&T

Status: ACTIVE

Version: v1.0

Created:

Last Updated:

Tags: #azuredevops #ado #agile #projectmanagement #backlog #planning



\---



\# Purpose



This folder contains Azure DevOps (ADO) documentation, governance standards, templates, workflows, and best practices used across BTS and Track \& Trace initiatives.



The objective is to provide a centralized source of truth for:



\- Demand Management

\- Agile Delivery

\- Work Item Management

\- Backlog Management

\- Sprint Planning

\- Project Tracking

\- Reporting

\- Governance

\- Delivery Lifecycle Management



\---



\# Scope



This repository supports:



\- Demand Intake

\- Project Planning

\- Feature Tracking

\- Change Delivery

\- UAT Management

\- Release Planning

\- Team Coordination

\- Reporting and Dashboards



\---



\# Folder Structure



```text

AZURE\_DEVOPS

│

├── WORK\_ITEM\_TYPES

├── BOARDS

├── BACKLOG\_MANAGEMENT

├── EPICS\_FEATURES\_STORIES

├── REPORTING

├── GOVERNANCE

├── DASHBOARDS

├── AUTOMATION

├── BEST\_PRACTICES

└── TRAINING

```



\---



\# Folder Descriptions



\## WORK\_ITEM\_TYPES



Store documentation related to:



\- Epics

\- Features

\- User Stories

\- Tasks

\- Bugs

\- Risks

\- Issues



Examples:



```text

Epic Guidelines

Feature Standards

User Story Templates

Bug Workflow

```



\---



\## BOARDS



Store board management documentation.



Examples:



```text

Kanban Board Setup

Board Configuration

Workflow Design

Column Definitions

```



\---



\## BACKLOG\_MANAGEMENT



Store backlog management standards.



Examples:



```text

Backlog Grooming Guide

Prioritization Framework

Backlog Review Process

```



\---



\## EPICS\_FEATURES\_STORIES



Store hierarchy guidance.



Examples:



```text

Epic Structure Standards

Feature Breakdown Rules

Story Writing Guidelines

Task Breakdown Examples

```



\---



\## REPORTING



Store reporting references.



Examples:



```text

Sprint Reports

Velocity Reports

Delivery Dashboards

Progress Tracking Guides

```



\---



\## GOVERNANCE



Store governance rules.



Examples:



```text

ADO Usage Standards

Workflow Governance

Approval Requirements

Traceability Standards

```



\---



\## DASHBOARDS



Store dashboard documentation.



Examples:



```text

Executive Dashboard

Project Dashboard

KPI Dashboard

Operational Dashboard

```



\---



\## AUTOMATION



Store automation references.



Examples:



```text

ADO Automation

Service Hooks

Power Automate Integrations

Work Item Automation

Notification Rules

```



\---



\## BEST\_PRACTICES



Store reusable guidance.



Examples:



```text

Work Item Naming

Sprint Planning Practices

Backlog Refinement Best Practices

Reporting Standards

```



\---



\## TRAINING



Store training materials.



Examples:



```text

ADO Onboarding Guide

Sprint Planning Workshop

Board Usage Training

Dashboard Tutorial

```



\---



\# Recommended Work Item Hierarchy



```text

Epic

&#x20;   ↓

Feature

&#x20;   ↓

User Story

&#x20;   ↓

Task

```



\---



\# Epic Guidelines



An Epic should:



\- represent a major business objective

\- contain multiple features

\- provide strategic value

\- span multiple work streams



Examples:



```text

UK Message Delay Initiative

Inextend Rollout

Warehouse Integration Program

```



\---



\# Feature Guidelines



A Feature should:



\- deliver a significant capability

\- support an Epic

\- contain multiple stories



Examples:



```text

Message Retry Logic

Invoice Integration

Reporting Enhancement

```



\---



\# User Story Guidelines



A User Story should:



\- describe a user need

\- be testable

\- provide measurable value



Format:



```text

As a <user>

I want <capability>

So that <business outcome>

```



\---



\# Task Guidelines



Tasks should:



\- be executable

\- be assignable

\- have clear ownership

\- support a user story



\---



\# Backlog Management Rules



\## Prioritization Factors



Consider:



\- business value

\- compliance impact

\- operational risk

\- technical dependency

\- strategic alignment



\---



\## Backlog Grooming Frequency



Recommended:



\### Active Projects



Weekly



\### Long-Term Initiatives



Bi-weekly



\### Portfolio Review



Monthly



\---



\# Reporting Standards



Recommended reports:



\## Delivery Status



Track:



\- completed work

\- work in progress

\- blocked work



\---



\## Velocity



Track:



\- completed story points

\- sprint trends



\---



\## Risk Dashboard



Track:



\- open risks

\- high-risk items

\- mitigation activities



\---



\## Project Dashboard



Track:



\- milestones

\- deployment dates

\- overall health



\---



\# Traceability Standards



Recommended traceability:



```text

Demand

&#x20;   ↓

Epic

&#x20;   ↓

Feature

&#x20;   ↓

User Story

&#x20;   ↓

Task

&#x20;   ↓

Change

&#x20;   ↓

Deployment

```



\---



\# ADO Governance Rules



All work items should contain:



```text

Title

Description

Business Value

Owner

Status

Priority

Due Date

Linked Artifacts

```



\---



\# Naming Standards



Examples:



```text

\[UK] Message Delay Enhancement



\[INEXTEND] New Warehouse Integration



\[SAP ATTP] Reporting Improvement

```



\---



\# Suggested Tags



```text

\#ado

\#azuredevops

\#epic

\#feature

\#userstory

\#task

\#agile

\#backlog

\#sprint

\#reporting

```



\---



\# Common Usage Scenarios



\## Demand Management



Use for:



\- demand tracking

\- request intake

\- prioritization



\---



\## Project Management



Use for:



\- milestone tracking

\- delivery planning

\- dependency management



\---



\## UAT Management



Use for:



\- test planning

\- defect tracking

\- sign-off management



\---



\## Change Management



Use for:



\- implementation tracking

\- deployment coordination

\- release visibility



\---



\# Knowledge Promotion Rules



If reusable approaches are discovered:



```text

ADO Experience

&#x20;       ↓

Lesson Learned

&#x20;       ↓

Reusable Pattern

&#x20;       ↓

SOP Improvement

```



\---



\# Review Schedule



\## Quarterly Review



Verify:



```text

\[ ] Governance standards current

\[ ] Dashboards still relevant

\[ ] Automation documentation updated

\[ ] Templates current

```



\---



\## Annual Review



Verify:



```text

\[ ] Obsolete practices removed

\[ ] New features documented

\[ ] Training refreshed

```



\---



\# Related Repository Areas



```text

01-AI-PROMPTS

02-PROJECTS

03-SOP

04-LESSONS\_LEARNED

```



ADO references support project execution and governance throughout the delivery lifecycle.



\---



\# Success Criteria



The Azure DevOps Reference Library is successful when:



\- work is consistently structured

\- traceability improves

\- backlog quality increases

\- reporting becomes standardized

\- onboarding becomes easier

\- delivery governance improves



\---



\# Revision History



| Version | Date | Author | Description |

|----------|----------|----------|----------|

| v1.0 | | | Initial Version |

