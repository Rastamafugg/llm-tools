1. **Start from the codebase**
   - Give the model real project context: existing code, docs, APIs, and conventions.

2. **Adapt proven patterns**
   - Prefer extending known-good components and workflows over generating new structures from scratch.

3. **Work in small increments**
   - Make narrow changes, validate them, then expand only after the current slice is correct.

4. **Validate behavior, not just code**
   - Use tests, local runs, staging checks, or manual flows to prove the feature actually works.

5. **Recheck alignment at milestones**
   - Revisit docs, architecture, and shared patterns early and whenever drift appears, then at major feature checkpoints once the workflow is stable.

6. **Separate evidence from guesses**
   - Treat observations, hypotheses, and fixes as different things; do not claim certainty without verification.
