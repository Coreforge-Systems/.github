# Contributing to Coreforge Systems

## Engineering principles

- Reliability before convenience.
- Explicit state and error handling.
- No hidden blocking I/O in GUI code.
- Clear architectural boundaries.
- Testability without physical hardware where possible.
- Read-only behavior by default for diagnostics.
- No unsafe retries for non-idempotent device commands.
- No secrets or customer-sensitive data in commits, logs, fixtures, or tests.

## Workflow

1. Create a focused branch from `main`.
2. Keep each change limited to one logical purpose.
3. Add or update tests where behavior changes.
4. Run formatting, static analysis, build, and tests locally.
5. Open a pull request using the organization template.
6. Do not merge while required checks are failing.

### Branch naming

```text
feature/
fix/
refactor/
test/
docs/
build/
ci/
chore/
```

Examples:

```text
feature/device-identification
fix/frame-decoder-overflow
refactor/operation-scheduler
test/protocol-timeout
docs/demo-protocol-v1
```

## Commit messages

```text
feat: add device identification request
fix: reject oversized protocol frames
refactor: isolate operation timeout handling
test: add delayed response integration case
docs: document support package schema
```

## C++ requirements

- Prefer RAII and clear ownership.
- Avoid raw owning pointers.
- Keep public APIs minimal.
- Avoid unnecessary global state.
- Treat compiler warnings as defects.
- Do not block Qt GUI threads.
- Document thread affinity and ownership for `QObject`-based components.

## Testing

Device communication changes should cover both success and failure paths where applicable: timeout, disconnect, malformed input, unsupported operations, invalid parameters, cancellation, and late responses.

## Security

Do not commit passwords, API tokens, private keys, customer protocols covered by NDA, production credentials, personal data, or unredacted diagnostic packages.
