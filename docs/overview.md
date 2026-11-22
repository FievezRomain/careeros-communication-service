# CareerOS Communication Service â€” service overview

## Responsibility

Prepare emails, calendar actions and follow-ups while enforcing explicit approval.

## Data ownership

Message drafts, delivery attempts and provider references.

## Interfaces

- Inputs: Approved communication commands only.
- Outputs: Delivery status events and audit metadata.
- Dependencies: identity and application services plus configured provider adapters.

## Contract rules

- APIs and events are versioned.
- Consumers must be idempotent where retries are possible.
- Correlation identifiers are propagated without logging sensitive payloads.
- Authorization and ownership are checked at the service boundary.

## Non-goals

This service does not absorb responsibilities owned by another CareerOS service. Cross-service workflows are coordinated through explicit contracts rather than shared databases.

## Security and privacy

Persist the minimum data required, record provenance, define retention, redact logs and use synthetic examples in this public repository.