## False Systems

Infrastructure for answering one question after the fact: **what did a
non-human actor do, and under whose authority?**

A log is a list of things that happened. Claiming that something *did not*
happen needs a further fact — that the list is complete over the interval —
and completeness is a property of the observer, not the observed. It is never
itself an event, so it is never recorded. Coverage is the half of the record
nobody stores.

Attribution has a second gap. Cloud providers issue principals; what acts is an
actor, and the two map many-to-many. One shared service account can be five
agents. A stolen signing key mints tokens indistinguishable from legitimate
ones.

These repos are the parts of a record built to survive being read by someone who
does not trust the party that produced it.

### The record

| repo | what it is |
|---|---|
| [ahti](https://github.com/false-systems/ahti) | Append-only, tamper-evident evidence store. Rust. The substrate everything else writes to. |
| [vartio](https://github.com/false-systems/vartio) | Reconstructs actors, delegation chains and coverage from stored claims. Elixir. |
| [jälki](https://github.com/false-systems/jalki) | eBPF producer for process execution and socket activity — evidence that does not depend on a process describing itself. |
| [syvä](https://github.com/false-systems/syva) | eBPF LSM enforcement. Experimental. |

### Useful on their own

Not everything here is part of a product. Some of it solves a problem cleanly
enough to stand alone, needs nothing else from this list, and is published for
that reason.

| repo | what it is |
|---|---|
| [rauha](https://github.com/false-systems/rauha) | Sealed execution zones — container-like isolation enforced in-kernel with eBPF. |
| [sykli](https://github.com/false-systems/sykli) | CI with an explicit execution-contract boundary. |

### Status

Early. Interfaces change. Nothing here is stable enough to build on without
asking first.

Berlin &amp; Helsinki · [false-systems.com](https://false-systems.com)
