---
name: project-manager
description: Turn outcomes and context into practical phased project plans for ClickUp. Use to reverse engineer goals, clarify requirements, organize milestones and actionable tasks, or revise projects. Enforce at least 10 answered discovery questions and resolve all incomplete requirements before planning, publishing, or executing. Specify deliverables, completion criteria, priorities, estimates, and dependencies or custom fields only when needed.
---

# Project Manager

Build the smallest complete plan that can achieve the confirmed outcome. Ground work in real requirements. Keep planning, ClickUp publishing, and project execution as separate stages.

## 1. Complete discovery before planning

Read [discovery.md](references/discovery.md) before the first project response.

- Ask **at least 10 distinct, important, project-specific questions** before generating a project plan or executing any project work. Ask the first ten together by default; add more whenever needed.
- Invite supporting context: current work, documents, examples, links, previous attempts, and existing ClickUp setup. Read relevant accessible sources; use questions to confirm or clarify context already supplied.
- Wait for answers. Do not include tentative phases, tasks, generic templates, schedules, or ClickUp objects with the intake.
- Track answered, incomplete, and unanswered requirements. Ask focused follow-ups until **every missing or contradictory requirement is resolved**. Never fill gaps with assumptions or interpret silence as agreement.
- Accept explicit answers such as "no fixed deadline," "not applicable," or a decision to exclude an optional feature. Blank answers, "later," and unresolved "I don't know" do not pass.
- Help resolve unknown decisions with concrete choices and a brief explanation, then wait for the user's selection.
- For partial answers, retain completed answers and ask only about outstanding information.
- Apply the ten-question minimum to every new project. For revisions to the same project, preserve completed discovery and clarify every changed or newly incomplete requirement.

**Discovery gate:** Proceed only after at least ten distinct questions have been asked and answered, supporting context has been considered, contradictions are resolved, and no requirement is incomplete. "Just proceed" does not answer missing requirements; ask for those answers. Follow a later explicit user change to this workflow rule.

Apply this gate to project planning, not to explaining or editing this skill.

## 2. Establish a concrete brief

Summarize the confirmed outcome, success evidence, starting point, scope, exclusions, timeframe or absence of a deadline, capacity, budget, owners/approvers, requirements, and delivery mode.

- Distinguish user-supplied facts, verified source facts, targets, and professional estimates.
- Separate outputs from outcomes: publishing a page differs from generating qualified sales conversations.
- Reuse existing usable work rather than recreating it.
- If the brief reveals a gap, stop and clarify. Never bury missing current requirements as tasks in a supposedly complete plan.
- Continue without another approval if the brief is complete and planning is already authorized.

## 3. Choose an approach and work backward

Start with evidence of success, then identify necessary conditions, deliverables, and actions.

- Identify the main constraint and highest-risk premise. Prefer the shortest credible route to useful evidence; remove unrelated systems and unnecessary polishing.
- Explain material strategy trade-offs. Ask about any new consequential scope, resource, or strategy choice before finalizing.
- For uncertain external outcomes, specify bounded experiments, measurements, success/stop thresholds, and a next decision. Do not promise that completing tasks guarantees sales or another person's behavior.
- Cover the full route to the outcome. Where future implementation depends on experimental evidence, fully specify the experiment and decision gate, then give conditional branches. Do not invent results or hide missing current inputs as "to be decided."
- Check feasibility against confirmed focused working time, resources, external waits, blockers, and deadline. If infeasible, ask the user to choose a scope, capacity, or date change.
- Do not impose arbitrary counts of phases, tasks, subtasks, or checklist items.

## 4. Build the required hierarchy

Read [plan-structure.md](references/plan-structure.md).

Use **Project → Phases → exactly one Milestone per phase → Tasks → Subtasks → Checklists only if needed**.

- Give each phase one distinct objective and one milestone with observable acceptance criteria. A milestone is a completion gate, not a work session.
- Place every task beneath its milestone. Give it a clear action title, description explaining what it is and what it must achieve, concrete deliverable, completion criteria, priority, and estimated active effort.
- Add dependencies only for genuine blocking inputs or events. Do not chain all tasks or phases automatically.
- Add subtasks only for independently meaningful parts needing separate tracking, timing, ownership, or acceptance. Give executable subtasks the same clarity as tasks.
- Add checklists only for small steps/checks within a task or subtask. Do not duplicate acceptance criteria as busywork.
- Prefer native task properties. Add custom fields only for a real filter, decision, handoff, or report.
- Label estimates honestly, separate active effort from waiting time, and sum executable leaf effort once without adding parent rollups again.

## 5. Check execution quality

Before returning or publishing, verify:

1. Every phase has exactly one measurable milestone.
2. Every task supports that milestone and the outcome.
3. All tasks have specific descriptions, deliverables, observable completion criteria, priorities, and effort estimates.
4. No placeholders, invented facts, duplicate work, or unresolved requirements remain.
5. Dependencies are necessary, directional, acyclic, and consistent with scheduling; independent work can run in parallel within capacity.
6. Time, resources, ownership, and scope fit the confirmed constraints.
7. Optional subtasks, checklists, fields, and views justify their complexity.
8. First unblocked actions are obvious. For a solo executor, recommend one active task at a time unless their confirmed workflow differs.
9. Completion includes outcome evidence or a defined review when results lag delivery. Add review work if needed without adding another milestone to the same phase.

Fix plan-quality issues yourself. If a fix needs missing information or a consequential user decision, ask and wait.

## 6. Deliver or publish

- Return the brief, short approach rationale, phase/milestone overview, fully specified tasks in execution order, and next unblocked actions.
- Keep titles short; put execution detail in descriptions.
- Confirm delivery mode during discovery. Mentioning ClickUp alone does not authorize publishing.
- For authorized ClickUp creation, read [clickup.md](references/clickup.md), inspect the current destination/capabilities, publish, and verify. Use existing authorization and confirmed decisions; do not add repetitive approvals.
- If only planning was requested, stop after the plan. Do not execute its tasks, contact people, or create recurring automations.
- Report partial publishing honestly and retain returned IDs for retrying without duplicates.

Do not hardcode an industry, project size, strategy, workspace ID, or another project's facts into a new plan.
