---
name: Comment
about: Propose a community-facing change or feature for Tsūro
labels: comment, architecture, needs discussion
---

# Comment

<!--
Use this template to propose community-facing changes and features for Tsūro.
Comments are also known as requests for comments (RFCs).
For internal technical and organisational decisions, use the decision template
instead.

After creating this issue, draft your full proposal using the template at
templates/comment.md and submit a merge request.

Process details: https://handbook.omnifi.foundation/engineering/architecture/governance/
-->

## Overview

### Title
<!-- A clear, descriptive title for the proposal -->

### Category
<!-- Select the primary category -->
- [ ] Public interfaces (contracts and boundaries)
- [ ] Features (new functionality or capabilities)
- [ ] Protocols (communication standards and formats)
- [ ] Behaviour (how the system responds or operates)
- [ ] Community process (governance and workflows)
- [ ] Standards (public specifications and conventions)

### Affected projects
<!-- Which Tsūro projects does this proposal affect? -->
- [ ] Core (server, proxy, connection pool, TLS, configuration)
- [ ] Request lifecycle (filters, middleware, load balancing, health checks)
- [ ] Protocol support (HTTP/1.1, HTTP/2, gRPC proxying, WebSocket)
- [ ] Deployment (standalone binary, library crate, containers, systemd)
- [ ] Observability (logging, metrics, tracing, error reporting)
- [ ] Operations (zero-downtime upgrades, graceful shutdown, hot reload)
- [ ] Other: <!-- specify -->

---

## Summary

### Proposal
<!-- One paragraph summary of what you are proposing -->

### Motivation
<!-- Why is this change needed? What problem does it solve? -->

---

## Impact

### Who is affected?
<!-- Who will be affected by this change and how? -->

### Migration considerations
<!-- Will existing setups need to change? -->

---

## Proposed design

### Overview
<!-- High-level description of the proposed solution -->

### Alternatives considered
<!-- Briefly list other approaches you considered -->

---

## Discussion

### Open questions
<!-- Questions that need community input -->
- <!-- Question 1 -->
- <!-- Question 2 -->

### Discussion period
**Proposed duration**: <!-- minimum 14 days -->

---

## Next steps

- [ ] Draft full proposal in `comments/XXXX-title.md`
- [ ] Submit merge request to begin discussion period
- [ ] Engage with community feedback
- [ ] Await decision after discussion closes

---

## Governance

This proposal follows the
[Omnifi Foundation governance model](https://handbook.omnifi.foundation/engineering/architecture/governance/).
Technical leads carry responsibility for facilitating decisions after the
community discussion period closes. See the
[handbook](https://handbook.omnifi.foundation/engineering/architecture/governance/) for
process details.
