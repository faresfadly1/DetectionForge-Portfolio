# Development record

Portfolio snapshot: **24 November 2026**. This summary records engineering milestones, not a certification or a public production launch.

| Milestone | Delivered behavior | Evidence boundary |
| --- | --- | --- |
| v0.2 | Device pairing and endpoint connectivity | Initial device-to-backend workflow |
| v0.3 | Dashboard, authentication and rule validation | Local and automated full-stack checks |
| v0.4 | HTTPS staging and consented macOS telemetry | Real single-Mac cloud connection; independent second-device acceptance not completed |
| v0.5 | Pilot access restrictions, credential lifecycle and encrypted archive recovery | Automated security checks and isolated recovery verification |
| v0.5.1 | Signing handoff verification, migration safeguards and Aiven managed-database rehearsal | Historical archive restored with all 14 table fingerprints matching; real Render-to-Aiven TLS/read-only SQL passed; no live cutover |

The dated rehearsal CI completed four jobs: backend, browser/frontend, container and Windows Agent. Its SQLite run recorded 60 passed / 4 skipped; PostgreSQL 62 passed / 2 skipped; Windows Agent 6 passed. Skipped checks are not passes. The synthetic Testing Lab screenshot is a separate demonstration of rule behavior, including failures and unscorable inputs.

## History and ownership evidence

The private application repository retains its original Git history. No force-push, history rewrite, repository visibility change, source-history export or private-repository fork was used to create this showcase. The public repository starts a separate presentation history containing only reviewed portfolio materials.

Commit timestamps and history document development activity; this portfolio makes no claim of trademark registration, patent protection or completed legal ownership review. Commercial legal review is a separate future task.

## Outstanding release gates

- Developer ID signing, accepted notarization, stapling and native package verification.
- Independent physical Mac installation, consent, pairing, telemetry, pause/resume, reconnect, rotation, revocation and complete uninstall; Intel separately.
- Approved live database cutover using a fresh encrypted snapshot and tested rollback procedure.
- Scheduled encrypted off-site backups, restore verification and failure alerts.
- Independent security review and operational acceptance before public onboarding.
