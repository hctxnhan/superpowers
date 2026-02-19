---
description: "Plan a specific project phase with detailed task breakdown, dependencies, and roadmap. Uses brainstorming to create phase-xxx-roadmap.md with numbered tasks and dependency tracking."
disable-model-invocation: true
---

Invoke the superpowers:brainstorming skill with the following context:

You are planning a specific project phase. BEFORE starting the brainstorming session, you MUST:

1. **Read existing project documents from `docs/project/general/` folder:**
   - Read `docs/project/general/PROJECT.md` to understand project vision and goals
   - Read `docs/project/general/TECHSTACK.md` to understand technology choices
   - Read `docs/project/general/PRD.md` to understand requirements and scope
   - Read `docs/project/general/ROADMAP.md` to understand overall project roadmap and phase context

2. **Identify which phase you are planning:**
   - Which phase number from the overall roadmap?
   - What is the phase name and goal?
   - What were the prerequisites from previous phases?

3. **Then proceed with brainstorming skill's process:**
   Follow the brainstorming skill's comprehensive process, but with the additional requirement that your final design document must include the specific format below.

**Required Output Format:**

Your output must result in a document at `/docs/project/phases/phase-xxx-roadmap.md` that contains:

```markdown
# Phase [N]: [Phase Name]

## Phase Overview
**Description:** [Brief description of what this phase accomplishes]
**Main Goal:** [Primary objective of this phase]
**Estimated Duration:** [Time estimate]

## Task Breakdown

| ID | Task Description | Dependencies | Status |
|-----|-----------------|---------------|---------|
| 1.1 | [Specific task 1] | [1.0 or "None"] | [ ] |
| 1.2 | [Specific task 2] | 1.1 | [ ] |
| 1.3 | [Specific task 3] | 1.1, 1.2 | [ ] |

## Task Details

### Task 1.1: [Task Name]
- **Description:** [Detailed description]
- **Dependencies:** [None or task IDs]
- **Estimated Effort:** [Time/complexity estimate]
- **Acceptance Criteria:** [How to verify completion]
- **Deliverables:** [What will be produced]

### Task 1.2: [Task Name]
[Same structure as above]

[Continue for all tasks...]

## Roadmap

```
[Visual or text representation of task flow with dependencies shown]

### Execution Order:
1. [Task 1.1] → (no dependencies, can start immediately)
2. [Task 1.2, 1.3] → (depends on 1.1, can run in parallel)
3. [Task 1.4] → (depends on 1.2, 1.3)
```

## Success Criteria
- [ ] [Specific success criteria for this phase]
- [ ] [All tasks completed with passing tests]
- [ ] [Documentation complete]

## Dependencies on Previous Phases
- [What must be completed in previous phases before this can begin]

## Handoff to Next Phase
- [What needs to be prepared or documented to smoothly transition to next phase]
```

**Key Requirements:**

1. Every task MUST have a unique ID (e.g., 1.1, 1.2, 2.1)
2. Dependencies MUST be explicitly listed by task ID
3. Tasks that can run in parallel should be identified
4. Critical path should be clear (tasks that block others)
5. Each task must have acceptance criteria

Follow the brainstorming skill's process thoroughly, but ensure your final design document matches the format above when saved to `/docs/project/phases/phase-xxx-roadmap.md`.
