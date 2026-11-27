# Broken Object Level Authorization (BOLA)

**Status:** In progress — not confirmed
**Environment:** OWASP crAPI training application
**Authorization:** Intended for the locally deployed training environment only

## Summary

This report is a work-in-progress record for investigating whether an API operation enforces authorization for each object it accesses. No vulnerability is claimed until the behavior has been reproduced and documented in the authorized training environment.

## Objective

Determine whether a user can access or modify an object they are not authorized to access by changing an object identifier in an API request.

## Scope and prerequisites

- Target only the OWASP crAPI instance deployed for this exercise.
- Use test accounts and data created for the lab.
- Do not test a public or third-party system.

## Test record

Complete this section after testing:

- **Date:**
- **crAPI version or deployment:**
- **Endpoint and HTTP method:**
- **Test accounts and object ownership:**
- **Expected access-control behavior:**
- **Observed behavior:**
- **Reproduction steps:**
  1.
  2.
  3.

## Evidence

Add sanitized screenshots or request/response excerpts to `evidence/`. Remove authorization tokens, cookies, passwords, and personal data before saving evidence.

## Impact

Describe only the impact demonstrated in the authorized lab. Do not infer access to data or actions that were not tested.

## Root cause

Record the authorization check that was missing or ineffective, if confirmed.

## Remediation

Enforce object-level authorization on the server for every request that reads or changes an object. Derive the caller’s identity from trusted authentication context, check ownership or an explicit permission before returning or changing the object, and add tests that verify access is denied across users.

## References

- OWASP crAPI project: https://github.com/OWASP/crAPI
- OWASP API Security guidance: https://owasp.org/www-project-api-security/
