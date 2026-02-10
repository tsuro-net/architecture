# Architecture decision record

<!--
Use this template to propose technical and organisational decisions for Tsūro.
For community-facing changes and feature proposals, use the request for comments
template instead.

After creating this issue, draft your full proposal using the template at
templates/adr.md and submit a merge request.

Process details: https://handbook.omnifi.foundation/engineering/architecture/adrs/
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

- [ ] Draft full proposal in `adrs/XXXX-title.md`
- [ ] Submit merge request for review
- [ ] Address feedback from technical leads
- [ ] Update status after decision

---

## Governance

This decision follows the
[Omnifi Foundation governance model](https://handbook.omnifi.foundation/engineering/architecture/governance/).
Technical leads carry responsibility for shepherding proposals through the
process. See the
[handbook](https://handbook.omnifi.foundation/engineering/architecture/adrs/) for
process details.

/label ~"adr" ~"architecture" ~"technical"
