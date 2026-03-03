# False Systems

> Infrastructure built for AI agents, not retrofitted for them.

---

Every major company is deploying AI agents to manage infrastructure and developer workflows. But all the tools those agents rely on were built for humans — dashboards to look at, logs to read, YAML to write.

Agents can use them. They can't understand them.

False Systems builds the infrastructure layer that AI agents actually need: context-aware, causally-aware, designed from the schema up for LLM consumption. Not a wrapper around legacy observability. A new foundation.

---

## The Shift

The infrastructure stack we have — Terraform, Helm, Kubernetes YAML, CI configs — exists because humans needed readable abstractions over APIs. If the agent is the one managing infrastructure, that translation layer is dead weight.

What agents need instead:

- **APIs to act on** — already exist
- **Context to make good decisions** — this is what's missing
- **Guardrails so they don't destroy production** — this is the human's actual job now

The engineer's role is shifting from *operator* to *policy maker*. We're building the tooling for that world.

---

## What We're Building

**False Protocol** — An open standard for AI-native infrastructure events. Every occurrence carries semantic fields (`what_failed`, `why_it_matters`, `causal_chain`, `confidence`) designed for LLM consumption. The industry builds AI on top of observability data. We built observability data for AI from the start.

**KRETO** — A local daemon with memory and context. Persistent, structured, causally-weighted knowledge that agents can query before acting. Not stateless API calls. Institutional memory at the edge.

**AHTI** — Causality correlation engine. Traces the causal chain from code change to production event across all tools in the system.

**SYKLI** — CI as code, not YAML. Pipelines that express intent, emit False Protocol events, and give agents the context to understand what happened and why.

---

## The Architecture Principle

Every tool in this system was designed to answer one question an agent might ask.

Not "show me a dashboard." Not "here are your logs." *Why did this happen, what was the chain of events, what should happen next, and how confident are we.*

That requires events with semantics embedded at the source — not inferred after the fact by an LLM squinting at unstructured text.

---

## Status

Active development. Berlin-based. Solo founder.

CD Foundation Ambassador · Helm Committee · Berlin DevOps Meetup
