# CONV-GOV-0001-CONVERSATION_KNOWLEDGE_NAMING_STANDARD

Date: 2026-06-23

## Purpose

Define a standard naming convention and storage strategy for preserving valuable conversations, frameworks, prompts, SOPs, governance rules, and agent designs as reusable knowledge assets.

---

## Recommended Naming Convention

Use a predictable identifier that makes the purpose of each conversation immediately visible.

### Simple Format

```text
CONV0001-LIFELINE_AGENT_ARCHITECTURE
CONV0002-CONTROLTOWER_KNOWLEDGE_STRUCTURE
CONV0003-CHECKMATE_REVIEW_FRAMEWORK
CONV0004-AGENT_GOVERNANCE_STANDARDS
```

### Date-Based Format

```text
CONV20260623-0001-LIFELINE_AGENT_ARCHITECTURE
CONV20260623-0002-LIFEOS_KNOWLEDGE_STRATEGY
CONV20260623-0003-COPILOT_AGENT_LIMITATIONS
```

---

## Why This System Works

### Traceability

A file name should immediately communicate:

- What was discussed
- Which agent it relates to
- Why it was created

Example:

```text
CONV0021-CHECKMATE_AUDIT_RULES.md
```

Interpretation:

```text
Agent: Checkmate
Subject: Audit Rules
Type: Preserved Knowledge
```

This is significantly easier to manage than:

```text
notes_final_v2_new_latest.md
```

---

### Knowledge Base Growth

Over time, conversations become a structured knowledge repository.

Example:

```text
AGENTS
│
├── Lifeline
├── ControlTower
├── Neird
└── Checkmate

CONVERSATIONS
│
├── CONV0001-LIFELINE_AGENT_ARCHITECTURE.md
├── CONV0002-LIFELINE_HEALTH_ROUTINES.md
├── CONV0003-CONTROLTOWER_DEPLOYMENT.md
├── CONV0004-CHECKMATE_AUDIT_RULES.md
└── ...
```

This creates a long-term organizational memory system.

---

## Knowledge-Worthy Conversations

Not every conversation should be preserved.

### Temporary Conversations

```text
How do I do X?
```

### Knowledge Conversations

```text
CONV0042-LIFELINE_HEALTH_FRAMEWORK
```

Preserve conversations when they become:

- Frameworks
- Standards
- Prompts
- SOPs
- Checklists
- Reusable processes
- Governance rules
- Agent designs
- Architecture decisions
- Knowledge-management practices

---

## Standard Preservation Rule

Whenever a conversation becomes reusable knowledge:

```text
CONV####-[SUBJECT]
```

Store it as:

```text
Markdown (.md)
```

Reason:

- Portable
- Searchable
- Version-control friendly
- Works well with Copilot, SharePoint, GitHub, and knowledge bases

---

## Scalable Category Structure

As the knowledge base grows, use category prefixes.

### Life OS

```text
CONV-LIFE-0001-DAILY_PLANNING_FRAMEWORK
CONV-LIFE-0007-ENERGY_MANAGEMENT
```

### T&T Governance

```text
CONV-TT-0001-DEMAND_MANAGEMENT_RULES
CONV-TT-0018-CHANGE_CLASSIFICATION
```

### Coding Agent

```text
CONV-CODE-0001-NEIRD_OPERATING_MODEL
CONV-CODE-0014-SECURE_CODING_STANDARD
```

### Audit Agent

```text
CONV-AUDIT-0001-CHECKMATE_REVIEW_STANDARD
CONV-AUDIT-0005-HALLUCINATION_DETECTION
```

Benefits:

- Easier filtering
- Easier indexing
- Cleaner libraries
- Better long-term scalability

---

## Recommended Preservation Workflow

When a discussion should become knowledge:

### Request

```text
Generate as:
CONV-LIFE-0001-LIFELINE_AGENT_ARCHITECTURE
```

Or:

```text
Save as conversation knowledge
```

### Output Template

```markdown
# CONV-LIFE-0001-LIFELINE_AGENT_ARCHITECTURE

Date: YYYY-MM-DD

## Purpose

...

## Discussion

...

## Decisions

...

## Recommendations

...

## Next Actions

...
```

---

## Recommended Agent Ecosystem

```text
Lifeline
→ Personal Chief of Staff / Life OS

ControlTower
→ T&T Demand, Change, Documentation Governance

Neird
→ Workflow Coding Agent

Checkmate
→ AI Auditor & Quality Assurance Agent
```

Each agent develops its own structured body of knowledge over time using the same CONV naming framework.

---

## Decisions

- Use Markdown as the standard preservation format.
- Preserve reusable conversations as knowledge artifacts.
- Use structured CONV identifiers.
- Categorize by domain when scale increases.
- Store conversations separately from agent operating manuals.
- Maintain traceability between agents and conversations.

---

## Recommendations

1. Adopt the CONV naming convention immediately.
2. Create a dedicated Conversations library.
3. Use category prefixes (LIFE, TT, CODE, AUDIT).
4. Store knowledge-worthy discussions as Markdown.
5. Preserve decisions and rationale, not raw transcripts.
6. Keep agent operating manuals separate from conversation archives.

---

## Next Actions

- Create a SharePoint or OneDrive Conversations folder.
- Create agent-specific folders for Lifeline, ControlTower, Neird, and Checkmate.
- Begin numbering preserved conversations sequentially.
- Use this standard as the official conversation-to-knowledge conversion process.
