# Decision

<!--
Use this template to propose technical and organisational decisions for Tsūro.
Decisions are also known as architecture decision records (ADRs).
For community-facing changes, use the comment template instead.

After creating this issue, draft your full proposal using the template at
templates/decision.md and submit a merge request.

Process details: https://handbook.omnifi.foundation/engineering/architecture/governance/
-->

## Overview

### Title
<!-- A clear, descriptive title for the decision -->

### Affected projects
<!-- Which Tsūro projects does this decision affect? -->
- [ ] Core (server, proxy, connection pool, TLS, configuration)
- [ ] Request lifecycle (filters, middleware, load balancing, health checks)
- [ ] Protocol support (HTTP/1.1, HTTP/2, gRPC proxying, WebSocket)
- [ ] Deployment (standalone binary, library crate, containers, systemd)
- [ ] Observability (logging, metrics, tracing, error reporting)
- [ ] Operations (zero-downtime upgrades, graceful shutdown, hot reload)
- [ ] Other: <!-- specify -->

---

## Problem statement

### Current situation
<!-- Describe the technical or organisational situation requiring this decision -->

### Decision drivers
<!-- What factors are influencing this decision? -->
- <!-- Driver 1 -->
- <!-- Driver 2 -->
- <!-- Driver 3 -->

---

## Proposed decision

### Chosen approach
<!-- State the proposed decision clearly -->

### Rationale
<!-- Why is this approach being proposed? -->

### Alternatives considered
<!-- Briefly list other approaches you considered -->

---

## Impact summary

### Technical impact
<!-- How does this affect the codebase and architecture? -->

### Contributor impact
<!-- How does this affect how people contribute to the project? -->

---

## Next steps

- [ ] Draft full proposal in `decisions/XXXX-title.md`
- [ ] Submit merge request for review
- [ ] Address feedback from technical leads
- [ ] Update status after decision

---

## Governance

This decision follows the
[Omnifi Foundation governance model](https://handbook.omnifi.foundation/engineering/architecture/governance/).
Technical leads carry responsibility for shepherding proposals through the
process. See the
[handbook](https://handbook.omnifi.foundation/engineering/architecture/governance/) for
process details.

/label ~"decision" ~"architecture"
