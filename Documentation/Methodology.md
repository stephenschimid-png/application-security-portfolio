# Application Security Testing Methodology

Use this workflow only for systems you own or are explicitly authorized to assess.

## 1. Confirm scope

- Identify the approved application, environment, accounts, and testing window.
- Confirm which actions and data are in scope.
- Stop if the target or authorization is unclear.

## 2. Understand the application

- Map the relevant pages, API endpoints, roles, and data flows.
- Note the expected behavior before testing.
- Use test accounts and data where possible.

## 3. Test one issue at a time

- Form a specific security question.
- Change one relevant input or condition at a time.
- Compare the result with the expected access-control or validation behavior.
- Avoid unnecessary data access or changes.

## 4. Record evidence

For each confirmed finding, record:

- A concise title and severity rationale
- The affected endpoint or component
- Preconditions and reproduction steps
- Expected and observed behavior
- Sanitized evidence that supports the result
- Demonstrated impact
- A practical remediation

## 5. Validate and report

- Repeat the steps to confirm the behavior is consistent.
- Remove credentials, tokens, personal data, and unrelated system details.
- Separate confirmed findings from hypotheses and work in progress.
- Retest after remediation when authorized.

## 6. Clean up

- Restore lab data or configuration changed during testing when practical.
- Store reports and evidence only in the intended portfolio repository.
