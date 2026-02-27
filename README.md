# 1bash Scan Agent

Lightweight, open-source collection agent for 1bash.

> Project status: **early-stage development**. Interfaces, payload shape, and deployment model may change.

## Early Access

1bash is currently in early access.

- Visit **https://1bash.dev**
- Join the waiting list
- Get notified when access opens

## What This Repository Is

This repository contains the MVP scan agent workflow used by 1bash:

- bootstrap script delivery (`/scan`)
- one-time scan launch flow with short-lived keys
- encrypted payload relay for browser-side review

The goal is to keep collection auditable and minimal while we iterate publicly.

## Security Model (MVP)

- Script runs on your host.
- Scan launch key is short-lived and single-use.
- Ingest token is short-lived and single-use.
- Payload can be encrypted locally before transit.
- Query-string API keys are intentionally rejected.

This is an MVP, not a final cryptographic protocol. Expect hardening changes.

## Current Scope

- Host metadata collection (basic)
- Secure init + ingest API
- Credit-gated scan start
- Encrypted payload handoff path

## License

Licensed under the **Apache License 2.0**.
See [LICENSE](./LICENSE).
