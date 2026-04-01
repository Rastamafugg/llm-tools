Use coding models as part of a disciplined engineering loop: start from real project context, generate from proven patterns, validate behavior with tests, and review at milestones to keep the work aligned with the product and codebase.

1. **Start from project reality**
   - Begin with the existing codebase, architecture notes, coding standards, API contracts, design docs, and representative examples.
   - Treat these as the operating context for the task.
   - Do not ask the model to invent a system in isolation when the application already contains usable patterns.

2. **Generate from proven patterns**
   - Base new work on existing implementations, templates, shared components, and established conventions.
   - Prefer adapting a known-good example over generating a new structure from scratch.
   - This improves consistency, reduces review time, and lowers integration risk.

3. **Work in an iterative loop**
   - Define the requirement.
   - Generate or revise code for the current slice of work.
   - Validate it against the active task, surrounding code, and project constraints.
   - Feed the findings back into the next iteration.
   - Treat the model as part of a controlled feedback loop, not a one-pass solution.

4. **Revisit guidance at the right cadence**
   - Early in a project or workflow, check docs, examples, and standards more often while the pattern is still forming.
   - Once the team has a stable implementation approach, shift to milestone-based alignment checks.
   - Good milestones include completing a feature slice, introducing a new subsystem, preparing for integration, or finalizing a release candidate.
   - If drift or repeated defects appear, increase the review cadence again.

5. **Validate workflows and functionality with focused tests**
   - Use the appropriate validation method for the change: unit tests, integration tests, end-to-end flows, local harnesses, staging checks, or manual scenario testing.
   - Test not only isolated logic, but also workflow behavior, interface contracts, state transitions, and cross-service integration where relevant.
   - The goal is to prove the intended behavior, not just to produce plausible code.

6. **Keep validation scenarios stable**
   - When testing or debugging, preserve the intended user flow and acceptance conditions unless changing them is part of the task.
   - If you modify a test or harness, do it minimally and keep the purpose explicit.
   - This preserves comparability across iterations and avoids invalidating the result.

7. **Prefer small, reviewable increments**
   - Make changes in narrow slices tied to a specific requirement, defect, or hypothesis.
   - Validate each slice before expanding scope.
   - Avoid mixing the main task with opportunistic refactors or unrelated cleanup unless the team has agreed to that scope.

8. **Separate facts from hypotheses**
   - Distinguish what was observed from what is inferred.
   - Do not present a guess as a root cause.
   - When the cause is uncertain, turn that uncertainty into a targeted test, measurement step, or instrumentation plan.

9. **Follow local conventions before abstract elegance**
   - Team conventions for naming, layering, APIs, state management, error handling, observability, and deployment matter more than generic best practices.
   - Models should help reinforce the codebase’s existing operating style unless the task is explicitly about changing it.

10. **Require explicit review before completion**
   - Before calling the work done, review it against project standards, interface contracts, testing expectations, and product intent.
   - Confirm that the implementation fits the surrounding system and that the validation results support the claim.
   - Completion should mean implementation, validation, and review are all done.

**Concise Summary**

For a modern software team, the recommended approach is to use coding models inside a structured delivery loop: start from the real codebase and team standards, generate by adapting proven patterns, validate behavior with focused tests, revisit guidance at milestones, and keep changes small enough to review and trust. Use the model to accelerate implementation, not to bypass engineering discipline.
