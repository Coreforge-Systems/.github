[Русский](SECURITY_RU.md) | [English](SECURITY_EN.md)

# Security Policy

Coreforge Systems develops software that may interact with industrial and embedded equipment.

## Reporting a vulnerability

Do **not** open a public issue for a suspected vulnerability. Use GitHub private vulnerability reporting when enabled for the affected repository.

Include when possible:

- affected repository and version;
- affected component;
- technical description;
- reproduction steps;
- potential impact;
- sanitized logs or traces;
- suggested mitigation.

## Scope

Examples include unauthorized device commands, bypass of write restrictions, unsafe replay, authentication bypass, memory corruption from malformed protocol input, leakage of sensitive data into support packages or logs, or insecure update handling.

## Sensitive information

Never include real credentials, private keys, production tokens, customer secrets, or unredacted proprietary device data.

## Industrial safety

Security fixes must not weaken hardware safety mechanisms, safety interlocks, or equipment protections.
