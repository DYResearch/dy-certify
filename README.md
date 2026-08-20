<div align="center">

# dy-certify

### A signed schedulability certificate an auditor can re-run.

[![Status](https://img.shields.io/badge/status-design-e8b04b?style=flat-square&labelColor=0e141d)](#what-is-not-here-yet)
[![Licence](https://img.shields.io/badge/Apache--2.0%20OR%20MIT-475569?style=flat-square&labelColor=0e141d)](#licence)
[![DY Research](https://img.shields.io/badge/DY%20Research-5b8def?style=flat-square&labelColor=0e141d)](https://github.com/DYResearch)

</div>

---

## Why this exists

DO-178C, IEC 61508 and ISO 26262 all require evidence that deadlines are
met. The evidence is produced today by proprietary tools priced per seat, and
reproducing their result means trusting their binary. The standard asks for
proof and the industry supplies a receipt.

A certificate here is a file: the task set, the derivation step by step, the
tool version, and a hash over all of it. An auditor runs the same tool on the
same input and gets the same bytes, or the certificate is void.

## What is not here yet

Nothing is implemented. This repository exists so the design can be argued
with before it is built, and so the name is not claimed by something that does
less.

The hard part is not the signature. It is deciding what a derivation must
contain to be checkable by somebody who was not there — and that is a question
about what an auditor needs, not about cryptography.

## Related

[`dy-wcet`](https://github.com/DYResearch/dy-wcet) is the piece that works
today: response-time analysis for fixed-priority task sets, in integer
arithmetic that refuses rather than rounds.

## Licence

Apache-2.0 OR MIT, at your option.

---

<div align="center">

**DY Research** — Denis Yermakou

[github.com/DYResearch](https://github.com/DYResearch) · [connect@axonos.org](mailto:connect@axonos.org)

© 2026 Denis Yermakou

</div>
