# Plan structure

| Level | Purpose | Required content |
|---|---|---|
| Project | Achieve the outcome | Brief, success evidence, scope, constraints |
| Phase | Organize a meaningful stage | Objective and exactly one milestone |
| Milestone | Verify the phase result | Observable state, acceptance criteria, evidence |
| Task | Produce a useful result | Description, outcome, deliverable, completion criteria, priority, effort |
| Subtask, only when needed | Track a meaningful component | Same clarity as executable tasks |
| Checklist, only when needed | Capture small steps/checks | Short observable actions |

Do not estimate a milestone as extra work. Do not add several milestones to one phase. Split distinct gates into separate phases only when the work warrants it.

## Task specification

Use the following authoring pattern, populated with actual project content. Never return unfilled template instructions as the plan.

- **ID/title:** Stable short ID and action verb plus concrete object/result.
- **Description:** What the work is, relevant inputs/context, what it must achieve, and minimum useful execution guidance.
- **Deliverable:** Actual artifact, decision, verified state, or completed action, with an evidence location.
- **Complete when:** Observable pass/fail criteria. Avoid "professional," "optimized," or "high quality" without a test.
- **Priority:** Urgent, High, Normal, or Low according to consequence and sequencing.
- **Estimated effort:** Active minutes/hours. Use a range when uncertainty matters and explain material uncertainty. Label any selected scheduling estimate.
- **Owner:** A confirmed person/role when relevant, never an invented collaborator.
- **Dependency, only when needed:** Genuine blocker using stable task IDs, or an explicit external input/event.
- **Timing, only when needed:** Confirmed dates or a feasible proposed schedule. Separate waiting time from effort; never invent a deadline.
- **Subtasks/checklist:** Include only when useful.

Store required information in descriptions when the publishing surface lacks native fields. Do not turn every description heading into a custom column.

## Priority and estimates

Use Urgent for a confirmed immediate deadline or consequential blocker; High for the main constraint or essential enabling work; Normal for necessary routine delivery; Low for optional work the user deliberately retained. Remove irrelevant optional work.

Split work with independently trackable outputs, owners, timing, or acceptance tests. Match detail to the executor's needs; do not enforce universal 30-minute tasks. Use checkpoints where work cannot sensibly be split.

Sum executable leaf estimates once. Parent rollups are summaries. Include coordination/review effort only as real specified work. Check focused time and working days, not just calendar duration.

## Output order

1. Brief: confirmed outcome, success test, scope, constraints.
2. Approach: short rationale, main risk, material trade-off.
3. Overview table: phase, its one milestone, completion evidence, leaf effort estimate.
4. Phase sections: milestone gate, fully specified tasks, optional lower levels.
5. Execution: next unblocked actions, review trigger, next decision if relevant.

Keep the whole route visible. When future work depends on experiment results, describe the concrete decision rule and conditional branches without inventing results.

## Custom fields

Prefer native status, assignee, priority, start/due date, effort, and dependencies. Add a custom field only for a repeatable operational question that native properties/descriptions do not serve adequately.

For each needed field, specify name, type, options, scope, and purpose. For example, a channel dropdown can support channel filtering; an evidence URL can support review. Do not automatically add outcome, phase, milestone, or effort fields when hierarchy/native properties suffice. Distinguish proposed configuration from fields actually created.
