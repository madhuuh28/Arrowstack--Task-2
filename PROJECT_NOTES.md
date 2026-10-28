# Project Notes

## Objective
Demonstrate an AI-assisted first-pass review workflow for Python code.

## Workflow
1. User pastes code into the GUI.
2. The app checks that code is non-empty and no longer than 20,000 characters.
3. Code is sent to Gemini with review instructions.
4. JSON output is parsed and checked for required fields.
5. Results are displayed and can be saved as a JSON report.

## Output fields
`summary`, `issues`, `optimization_suggestions`, `improved_code`, `tests_to_run`.

## Validation checklist
- Empty input is rejected.
- Oversized input is rejected.
- Successful response contains required JSON fields.
- Invalid API key produces an error.
- `.env` is excluded from Git.
- Submitted code is never executed.

## Limitations
AI output can be wrong or incomplete. No static-analysis engine or sandboxed code execution is included. API availability and quotas depend on the Gemini account.
