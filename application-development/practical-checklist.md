**Practical Checklist**

1. **Before generation**
   - Identify the authoritative project assets for the task.
   - Find an existing template, reference implementation, or analogous feature.
   - Define the exact scope of the requested change.
   - Note any constraints that must remain unchanged.

2. **During generation**
   - Generate from an existing pattern, not from blank space.
   - Keep the change limited to the current requirement.
   - Reuse established interfaces, data shapes, naming, and error-handling patterns.
   - Avoid introducing new structural patterns unless necessary.

3. **During early workflow formation**
   - Revisit templates and standards often.
   - Compare generated code against known-good source when problems recur.
   - Correct drift quickly before it spreads into more files or workflows.

4. **After the workflow stabilizes**
   - Recheck source templates and project docs at milestones, not after every minor edit.
   - Use milestone reviews before integration, after a feature slice, and before final acceptance.
   - Increase review frequency again if errors or inconsistencies start repeating.

5. **For validation**
   - Use a focused test harness or targeted validation path.
   - Confirm the intended workflow or feature behavior under the real scenario.
   - Keep the harness narrow and preserve the scenario unless the scenario is part of the change.

6. **For diagnosis**
   - Separate observed facts from hypotheses.
   - Add the smallest useful instrumentation.
   - Do not rewrite the harness or workflow just to debug unless necessary.

7. **Before completion**
   - Review the change against project standards and existing patterns.
   - Confirm consistency with templates, interfaces, and documentation.
   - Verify the change is still narrowly scoped.
   - Confirm tests or harness results support the claimed outcome.
