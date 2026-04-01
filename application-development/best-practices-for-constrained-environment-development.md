Use the model inside a controlled development loop anchored by project assets, validated through focused testing, and reviewed for consistency at the right cadence.

1. **Start from authoritative project assets**
   - Begin with existing source templates, reference implementations, architecture notes, coding standards, workflow instructions, and established module patterns.
   - Treat these as the baseline contract for structure, naming, interfaces, error handling, state transitions, and review expectations.
   - Do not let the model invent patterns when working project-specific ones already exist.

2. **Generate from known-good patterns, not from scratch**
   - Use template source and prior working code as the base for new code generation.
   - Have the model adapt an established pattern to the new requirement rather than freehand a novel structure.
   - This keeps new work consistent with the application and reduces variance across features.

3. **Use an iterative generation loop**
   - Start from templates and instructions.
   - Generate or revise code for the current requirement.
   - Validate the result against the active task, existing code patterns, and project constraints.
   - Feed corrections and findings back into the next iteration.
   - Treat development as a controlled loop, not a one-shot generation step.

4. **Revisit templates and documentation at the right frequency**
   - Early in a project, or while a workflow is still unstable, revisit templates and documentation more often.
   - If issues keep appearing, use those source materials to recalibrate the model’s output and reestablish the correct pattern.
   - Once a reliable workflow emerges, shift to milestone-based alignment reviews rather than checking after every draft or edit.
   - Good checkpoints include completion of a feature slice, introduction of a new workflow, preparation for integration, or final review.
   - If drift, repeated defects, or inconsistencies reappear, increase the review cadence again until stability returns.

5. **Use test harnesses to validate workflows and functionality**
   - Use focused test harnesses to validate not only bug fixes, but also proposed workflows, feature behavior, integration boundaries, and application state transitions.
   - A harness should prove that the intended behavior works under the target scenario, not merely that the code compiles or appears plausible.
   - Keep harnesses narrow and purpose-built so they test the behavior under investigation without unnecessary structural change.

6. **Preserve the intended scenario during validation**
   - When validating a new workflow or diagnosing a defect, keep the scenario stable unless the scenario itself is what is being redesigned.
   - Preserve execution order, prompts, inputs, pauses, interaction model, and acceptance conditions unless a change to those items is explicitly part of the task.
   - If you modify a harness, do so minimally and state what must remain unchanged.

7. **Prefer small, reviewable increments**
   - Make narrowly scoped changes tied to a specific requirement, defect, or hypothesis.
   - Validate each increment before widening the scope.
   - Avoid bundling cleanup, unrelated refactors, or speculative improvements into the same change.

8. **Separate observed facts from hypotheses**
   - Distinguish clearly between what was observed in code, test output, or user reports and what is only inferred.
   - Do not claim root cause without evidence.
   - When uncertainty remains, convert it into a targeted check, small instrumentation step, or focused test.

9. **Use project-specific rules over general assumptions**
   - General programming knowledge is useful, but local project rules take priority.
   - If the project has established conventions for interfaces, data contracts, error handling, diagnostics, or module coordination, follow those conventions unless the task explicitly changes them.
   - Consistency with the application is usually more valuable than abstract elegance.

10. **Require explicit QA before calling work complete**
   - After edits, perform a deliberate review against project standards, template patterns, interface contracts, and test expectations.
   - Confirm that the final result still aligns with the established workflow and application design.
   - Treat completion as an outcome of implementation plus validation plus review.

**Concise Summary**

Use the model in a disciplined software-development loop: start from existing templates and project documentation, generate by adapting known-good patterns, validate workflows and features with focused test harnesses, and revisit source guidance frequently while the workflow is forming, then at project milestones once the process stabilizes. Keep changes narrow, distinguish facts from hypotheses, and require explicit review before declaring the work complete.
