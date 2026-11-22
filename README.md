# CareerOS Communication Service

Prepare emails, calendar actions and follow-ups while enforcing explicit approval.

## Scope

- **Owns:** Message drafts, delivery attempts and provider references.
- **Inputs:** Approved communication commands only.
- **Outputs:** Delivery status events and audit metadata.
- **Dependencies:** identity and application services plus configured provider adapters.

## Safety baseline

This public repository must never contain secrets, real resumes, real applications or personal data. External communication and application submission always require explicit user approval.

## Documentation

See [docs/overview.md](docs/overview.md) and the central [CareerOS workspace](https://github.com/FievezRomain/careeros-workspace).

## Status

Architecture and security baseline. Functional implementation will be added incrementally with tests and versioned contracts.

## License

Apache-2.0.