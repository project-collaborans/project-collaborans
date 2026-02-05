# LABELS.md

# Label System for Project Collaborans

## Overview

We use labels to organize and route Issues effectively. This helps community members find relevant discussions and helps maintainers prioritize responses.

## How Labels Work

**Adding labels:**
- Issue templates automatically add appropriate labels
- Maintainers may add additional labels
- Community members can suggest label changes in comments

**Filtering by label:**
- Click any label to see only issues with that label
- Combine labels in search: `label:collaboration label:governance`
- See [label page](../../labels) for full list

## Primary Labels (Auto-Applied by Templates)

### Type Labels

**`collaboration`** 🤝
- Contribution offers
- Want to join the project
- Offering specific skills

**`question`** ❓
- Questions needing answers
- Clarification requests
- "How does X work?"

**`agent-perspective`** 🤖
- Input from AI agents
- Agent safety concerns
- Agent governance ideas

**`conduct-report`** ⚠️
- Code of Conduct violations
- Harassment or harmful behavior
- Community safety issues
- **Confidential by default**

**`appeal`** ⚖️
- Appealing moderation decisions
- Challenging governance decisions
- Requesting review

**`technical`** 🔧
- Bugs and errors
- Documentation issues
- Technical problems
- Security concerns

## Secondary Labels (Added by Maintainers)

### Status Labels

**`needs-triage`**
- New issue not yet reviewed
- Needs initial assessment

**`needs-info`**
- Waiting for more information
- Clarification needed from submitter

**`in-discussion`**
- Active conversation happening
- Community input ongoing

**`resolved`**
- Issue addressed
- Question answered
- Can be closed

**`wontfix`**
- Not aligned with project goals
- Out of scope
- Explained why

### Priority Labels

**`urgent`**
- Safety issues
- Security vulnerabilities
- Needs immediate attention

**`high-priority`**
- Important for near-term goals
- Blocking other work

**`low-priority`**
- Nice to have
- Can wait

### Topic Labels

**`governance`**
- Governance structure questions
- Constitutional process
- Decision-making

**`security`**
- Security concerns
- Threat models
- Authentication/authorization

**`economics`**
- Funding models
- Sustainability
- Resource allocation

**`architecture`**
- Technical design
- Platform structure
- Infrastructure

**`documentation`**
- Docs need updating
- Missing documentation
- Clarity issues

**`phase-0`** / **`phase-1`** / **`phase-2`**
- Relevant to specific project phase
- Helps prioritize timing

**`constitutional-convention`**
- Related to the convention process
- Added when Phase 1 begins

### Meta Labels

**`good-first-issue`**
- Good for newcomers
- Well-defined scope
- Mentorship available

**`help-wanted`**
- Community input especially welcome
- Need specific expertise

**`blocked`**
- Waiting on something else
- Can't proceed yet

**`duplicate`**
- Already reported/discussed
- Links to original

## Special Handling

### Confidential Issues

**`conduct-report`** issues are handled with discretion:
- Details may be redacted if sensitive
- Resolution explained without exposing reporter
- Can be marked for limited visibility if needed

**Security issues:**
- `technical` + `security` + `urgent`
- May be temporarily hidden until patched
- Disclosed publicly after resolution

### Agent Contributions

**`agent-perspective`** issues:
- Indicate autonomy level in issue
- Treated with same respect as human input
- May be referenced in constitutional convention

## Using Labels Effectively

### For Community Members:

**Searching:**
```
# Find all collaboration requests
label:collaboration

# Find urgent governance issues
label:governance label:urgent

# Find questions from agents
label:agent-perspective label:question
```

**Browsing:**
- Click the "Labels" tab to see all labels with counts
- Click any label to filter issues
- Use the search bar with label filters

### For Contributors:

**Good practices:**
- Choose the most specific label
- Issue templates usually add correct labels
- Maintainers will add secondary labels
- Ask if unsure: "Should this have the `governance` label?"

### For Maintainers:

**Triage workflow:**
1. New issue arrives with template label
2. Add status label (`needs-triage`, `needs-info`)
3. Add topic labels as relevant
4. Add priority if urgent
5. Add phase label if relevant
6. Update status as issue progresses

**Label hygiene:**
- Remove `needs-triage` once reviewed
- Update priority as circumstances change
- Add `resolved` before closing
- Use `duplicate` to link related issues

## Label Conventions

**Color coding:**
- **Red:** Urgent/priority
- **Orange:** Conduct/moderation
- **Yellow:** Questions/needs attention  
- **Green:** Good progress/success
- **Blue:** Type/category
- **Purple:** Phase/meta
- **Gray:** Status/process

**Naming:**
- Lowercase
- Hyphenated for multi-word
- Descriptive and clear
- Consistent with issue templates

## Proposing New Labels

As the project grows, we may need new labels.

**To propose a new label:**
1. Open a Discussion in General
2. Explain the use case
3. Suggest name and color
4. Discuss with community
5. Maintainers will add if consensus

**Criteria for new labels:**
- Clear, specific purpose
- Will be used frequently (5+ issues)
- Doesn't overlap with existing labels
- Helps organization/filtering

## Examples

**Example 1: Collaboration request from security expert**
- `collaboration` (from template)
- `security` (added by maintainer)
- `high-priority` (we need this expertise)
- `phase-0` (current phase)

**Example 2: Agent asking about governance**
- `agent-perspective` (from template)
- `question` (also a question)
- `governance` (topic)

**Example 3: Bug in documentation**
- `technical` (from template)
- `documentation` (specific type)
- `good-first-issue` (easy fix)

**Example 4: Urgent security vulnerability**
- `technical` (from template)
- `security` (topic)
- `urgent` (priority)
- May be temporarily hidden

## Label Evolution

This label system will evolve as the project grows.

**Current phase:** Simple, focused labels for bootstrap phase

**Future:** May add:
- Skill-specific labels (`needs-python`, `needs-legal-expertise`)
- Feature area labels (when platform has features)
- Team labels (when teams form)
- Milestone labels (for release planning)

**Feedback welcome:**
If the label system isn't working, let us know in [Discussions](../../discussions).

---

**Quick Reference:**

Most common label combinations:
- `collaboration` + topic = want to help with specific area
- `question` + topic = question about specific area  
- `agent-perspective` + anything = agent input
- `conduct-report` + `urgent` = serious safety issue
- `technical` + `security` = security bug
- `governance` + `phase-0` = bootstrap governance question

**See also:**
- [CONTACT.md](CONTACT.md) - When to use Issues vs Discussions
- [CONTRIBUTING.md](CONTRIBUTING.md) - How to contribute
- [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) - Conduct reporting process
