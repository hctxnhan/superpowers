---
description: Execute a planned project phase with task progress tracking and status updates
disable-model-invocation: true
---

Invoke the superpowers:executing-plans skill and follow it exactly as presented to you.

## Phase Execution Context

Before starting execution, ensure you have:

1. **Located the phase roadmap file** at `/docs/project/phases/phase-xxx-roadmap.md` (where `xxx` is the phase number)
2. **Reviewed the task breakdown** to understand all tasks, their dependencies, and acceptance criteria
3. **Understood the execution order** from the Roadmap section to identify which tasks can run in parallel

## Task Status Tracking

As you complete each task during phase execution:

1. **Update the Task Breakdown table** in the phase roadmap file:
   - Change the Status column from `[ ]` (unchecked) to `[x]` (checked) when a task is complete
   - Format: `[x]` for completed, `[ ]` for pending

2. **Mark task details as complete** in the Task Details section:
   - Add ✅ prefix to completed task headers
   - Example: `### Task 1.1: [Task Name] ✅`

3. **Commit progress** after completing task groups:
   - Commit message format: `phase-[N]: Complete tasks [1.1, 1.2, 1.3]`
   - Include brief summary of what was accomplished

## Execution Flow

1. Follow the execution order from the phase roadmap
2. Execute tasks respecting their dependencies
3. Update status in the roadmap file after each completed task
4. Create review checkpoints between major task groups
5. Verify all success criteria are met before marking phase as complete

## Phase Completion

When all tasks are done:

1. Verify all Success Criteria checkboxes are marked `[x]`
2. Ensure all task statuses show `[x]` in the Task Breakdown table
3. Add a Phase Completion Note at the end of the roadmap documenting:
   - Actual duration vs estimated
   - Any blockers or deviations
   - Lessons learned
   - Readiness for next phase handoff
