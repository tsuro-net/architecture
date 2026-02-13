# Tsūro Architecture

Welcome! This repository is where architectural decisions for
[Tsūro](https://gitlab.com/tsuro.net) are proposed, discussed, and
recorded.

## What is Tsūro?

Tsūro is an open source, high-performance HTTP server and proxy framework built
in Rust. It provides connection pooling, TLS termination, HTTP/1.1 and HTTP/2
support, zero-downtime upgrades, and a programmable request lifecycle. Tsūro can
be consumed as a library crate for embedding into other services or run as a
standalone binary for production deployments.

## What this repository is for

This repository tracks architectural decisions using two complementary
approaches:

- **Decisions** capture internal technical and organisational choices — how Tsūro is built, structured, and maintained.

- **Comments** handle community-facing proposals — changes
  to public interfaces, features, behaviour, and integration patterns that
  affect how people use Tsūro.

These terms map to well-established practices — decisions are also known as
architecture decision records (ADRs), and comments are also known as requests
for comments (RFCs). We use plainer language to lower the barrier to
contribution.

Both approaches are open to everyone. You don’t need to be a maintainer or a
regular contributor to submit a proposal. If you have an idea or see something
that could be improved, you're welcome here.

## How the process works

1. **Create an issue** using one of the issue templates (decision or comment) to signal
   your intent and invite early feedback.
2. **Draft a proposal** using the document templates in `templates/`.
3. **Submit a merge request** with your proposal in `decisions/` or `comments/`.
4. **Discuss** — for decisions, technical leads review over 7–14 days. For comments,
   the community discusses for a minimum of 14 days.
5. **Decision** — once consensus is reached, the proposal is merged and becomes
   part of the project's record.

The full process, including how consensus works, how disagreements are resolved,
and what happens with urgent decisions, is documented in the
[Omnifi Foundation handbook](https://handbook.omnifi.foundation/engineering/architecture/).

## Projects in scope

Proposals in this repository may affect any part of the Tsūro ecosystem:

**Core**
- `tsuro-server` — HTTP server, listener management, graceful shutdown
- `tsuro-proxy` — reverse proxy, upstream connection pooling, load balancing
- `tsuro-tls` — TLS termination, certificate management, rustls integration
- `tsuro-config` — configuration loading, validation, hot reload

**Request lifecycle**
- Filters, middleware, request and response transformation
- Load balancing algorithms and health checks
- Authentication, rate limiting, and access control hooks

**Protocol support**
- HTTP/1.1 and HTTP/2 serving and proxying
- gRPC proxying, including streaming
- WebSocket transparent proxying

**Deployment**
- Standalone binary
- Library crate for embedding
- Container images
- systemd integration

**Observability**
- Structured logging, metrics, and tracing
- OpenTelemetry integration
- Error reporting and diagnostics

**Operations**
- Zero-downtime upgrades and socket handoff
- Graceful shutdown and drain
- Hot configuration reload

If your proposal spans multiple areas, note all affected projects in your
proposal so the right people can weigh in.

## Governance

Tsūro is governed by the [Omnifi Foundation](https://omnifi.foundation), a
community-driven organisation that stewards open source projects. The
architecture decision process — how proposals are written, reviewed, and
decided — is defined in the
[Omnifi Foundation handbook](https://handbook.omnifi.foundation/engineering/architecture/)
and applies equally to all contributors.

[Eolian Ab](https://eolian.group) is a contributing organisation that develops
Tsūro. All code is contributed to the foundation and governed through this open
process.

Decisions are made through consensus. Technical leads facilitate the process but
don't dictate outcomes. Every voice carries weight, and dissenting perspectives
are documented and valued. See the
[governance model](https://handbook.omnifi.foundation/engineering/architecture/governance/)
for full details.

## Getting started

New to the project? Here's how to get oriented:

1. **Browse existing proposals** in `decisions/` and `comments/` to see what's been
   decided and how proposals are structured.
2. **Check open merge requests** for proposals currently under discussion.
3. **Read the handbook** for
   [detailed process guidance](https://handbook.omnifi.foundation/engineering/architecture/).
4. **Open an issue** if you have questions — there are no bad questions.

## Repository structure

```
├── README.md              You are here
├── CONTRIBUTING.md        How to submit proposals
├── templates/
│   ├── decision.md        Decision template
│   └── comment.md         Comment template
├── decisions/             Accepted decisions
├── comments/              Accepted comments
└── .gitlab/
    └── issue_templates/
        ├── decision.md    Issue template for proposing a decision
        └── comment.md     Issue template for proposing a comment
```

## Code of conduct

All participation is subject to the
[Omnifi Foundation code of conduct](https://handbook.omnifi.foundation/CODE_OF_CONDUCT/).
We're committed to a welcoming, respectful, and inclusive environment.

## License

CC BY-SA 4.0 — see LICENSE for details.
