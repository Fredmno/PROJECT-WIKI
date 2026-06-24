Not necessarily.

There are **two separate things** in an agent:

## 1. Instructions (Required)

This is your prompt.

Examples:

* Lifeline prompt
* ControlTower prompt
* Neird prompt
* Checkmate prompt

These go into:

```text
Instructions
System Prompt
Behavior
```

This is **required**.

***

## 2. Knowledge Files (.md, PDFs, DOCX, etc.) (Optional)

These are reference materials the agent can consult.

This is **not required**, but highly recommended for some of your agents.

***

# Recommended Setup

## Lifeline

### Instructions

✅ Yes

Use:

* Personal Chief of Staff Prompt

### Knowledge Files

⚠️ Optional

Examples:

```text
MY_PROFILE.md
HEALTH_GOALS.md
PERSONAL_ROUTINES.md
WORKING_HOURS.md
```

Example:

```markdown
# My Profile

Wake Up: 6:00 AM

Sleep Target: 10:30 PM

Water Goal: 3L

Exercise:
- Walking
- Swimming

Vitamins:
- Vitamin C
- Multivitamin
```

This helps Lifeline create better schedules.

***

## ControlTower

### Instructions

✅ Yes

Use:

* T\&T Management Agent Prompt

### Knowledge Files

✅ Highly Recommended

Example files:

```text
T&T_PROCESS.md
DEMAND_MANAGEMENT.md
CHANGE_MANAGEMENT.md
ITSP_GUIDE.md
SERVICENOW_GUIDE.md
```

These become your organization's SOP library.

***

## Neird

### Instructions

✅ Yes

Use:

* Coding Agent Prompt

### Knowledge Files

⚠️ Optional

Possible files:

```text
CODING_STANDARDS.md
PYTHON_STANDARDS.md
SQL_STANDARDS.md
POWERAUTOMATE_STANDARDS.md
```

Most coding agents work well without knowledge files.

***

## Checkmate

### Instructions

✅ Yes

Use:

* AI Auditor Prompt

### Knowledge Files

✅ Recommended

Example:

```text
REVIEW_CHECKLISTS.md
SECURITY_CHECKLIST.md
FRS_STANDARDS.md
TEST_CASE_STANDARDS.md
AUDIT_RULES.md
```

This becomes the source of truth for reviews.

***

# My Recommendation For You

Create this structure:

```text
AGENTS
│
├── Lifeline
│   ├── Instructions
│   └── Knowledge
│       ├── MY_PROFILE.md
│       ├── HEALTH_GOALS.md
│       └── DAILY_ROUTINES.md
│
├── ControlTower
│   ├── Instructions
│   └── Knowledge
│       ├── DEMAND_MANAGEMENT.md
│       ├── CHANGE_MANAGEMENT.md
│       ├── ITSP_GUIDE.md
│       └── T&T_PROCESS.md
│
├── Neird
│   ├── Instructions
│   └── Knowledge
│       ├── CODING_STANDARDS.md
│       └── SQL_STANDARDS.md
│
└── Checkmate
    ├── Instructions
    └── Knowledge
        ├── AUDIT_RULES.md
        ├── SECURITY_CHECKLIST.md
        ├── FRS_CHECKLIST.md
        └── REVIEW_CHECKLIST.md
```

### Start simple

For now:

✅ Create the agent  
✅ Paste the prompt into Instructions

You do **not** need knowledge files immediately.

Later, when you notice the agent repeatedly needs the same reference material, create `.md` knowledge files and upload them.

So for your first version:

```text
Lifeline      → Prompt only
ControlTower  → Prompt only
Neird         → Prompt only
Checkmate     → Prompt only
```

Then gradually add knowledge files as each agent matures. This is usually the fastest and cleanest approach.
