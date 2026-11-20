# ClickUp delivery

## Authorization and destination

Do not write during discovery. Complete requirements and the plan first. Use confirmed delivery mode, names, destination, and authorization. Do not ask again for decisions already supplied.

For an import artifact, check current official import documentation before promising support for hierarchy, milestones, dependencies, or custom fields. A CSV header alone does not prove import support. Preserve the full readable plan and disclose manual steps.

## Inspect current capabilities

- Discover available tools. Resolve workspace, space/folder/list, existing content, statuses, task types, and assignees through tools; never guess IDs.
- Before converting relative dates for a tool call, use clickup_get_user and compute from its returned time/timezone. Clarify conflicts with the stated timezone.
- Read live schemas. If no dedicated tool fits, inspect clickup_get_operators before clickup_execute_operator; never invent operators or payloads.
- Read existing custom-field definitions before setting values. Reuse suitable fields/options. Inspect the operator catalog for field creation, checklist handling, milestone types, and other capabilities without dedicated tools.

## Preserve the hierarchy honestly

Preferred mapping, subject to verified workspace support:

| Concept | ClickUp representation |
|---|---|
| Project | Project folder in the confirmed space |
| Phase | Ordered list in the folder |
| One milestone | Parent item using an existing Milestone task type if it supports children |
| Task | Child item under that milestone |
| Subtask | Nested child item if the required nesting is supported |
| Checklist | Native checklist if supported; otherwise explicit Markdown checks in the description |

Explain that the conceptual Task level may appear as a subtask in ClickUp. Confirm mapping and names as part of the intake/complete plan rather than asking about each item individually.

Do not assume milestone parents, nested subtasks, new folders/lists, or checklists are supported. If the mapping is unsupported, propose a concrete alternative and ask before publishing. For example, one clearly labeled standard parent task as the phase gate may preserve nesting if native Milestone items cannot. Never silently flatten the user's hierarchy or claim standard tasks are native milestones.

If the user needs a single existing list, resolve the representation of phases and milestone parents before publishing rather than imposing folders/lists.

## Create and verify

1. Inspect destination content for duplicates. Keep stable plan IDs in descriptions and a plan-ID to created-ID map.
2. Create only confirmed containers; preserve existing content/configuration.
3. Create milestone parents, then tasks and optional descendants in parent-first order.
4. Set full descriptions, deliverables, acceptance criteria, priority, and effort. The currently described dedicated create-task tool takes time_estimate as minutes expressed as a string; recheck its current schema. Other surfaces may use other units.
5. Use verified custom-field IDs/options only. If workspace-required fields need missing inputs, ask; do not invent values to bypass them.
6. Add genuine dependencies after task IDs exist. In clickup_add_task_dependency, B waiting on A means task_id=B, depends_on=A, type=waiting_on; recheck the current schema.
7. Read back created hierarchy and task properties. Verify object counts, one milestone per phase, parent IDs, descriptions, native properties, dependency edges, custom-field values, and nonduplicated effort totals. Inspect every created object as needed; do not equate an attempted call with success.
8. Report results with inline links using actual returned URLs: [Task name](returned URL). Distinguish completed, unsupported, and incomplete work.

On partial failure, retain IDs, inspect actual state, and resume missing operations without duplication. Do not delete existing work, overwrite unrelated tasks, send chat messages, or begin execution merely to finish publishing.
