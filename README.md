# Alexander Cardoza

Founder of LynxFlow. I build developer tooling and write about the parts that break in production.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare-F38020?style=flat&logo=cloudflare&logoColor=white)
[![lxlynx.com](https://img.shields.io/badge/lxlynx.com-1F2328?style=flat&logo=readme&logoColor=white)](https://lxlynx.com)

---

## About

I run LynxFlow, a small studio working on tooling for LLM-backed products. Most of what
I do sits in the unglamorous layer underneath the demo: retries, rate limits, cost
accounting, and the scripts that stop a fleet of small services from quietly drifting
apart.

I write Python and TypeScript, deploy most things to Cloudflare's edge, and have a
standing bias toward systems I can debug at three in the morning with a terminal and a
log file. If a tool needs a dashboard to explain itself, I usually don't keep it.

Working hours are UTC+8, which mostly means I answer email before the rest of the
internet wakes up.

## Currently working on

- **AI toolchain.** Evaluation harnesses, prompt and model versioning, and making the
  cost of an LLM pipeline visible before the invoice arrives rather than after.
- **Growth engineering.** The engineering half of acquisition and retention:
  instrumentation, lifecycle mechanics, and experiments that survive someone checking
  the math afterwards.
- **Security engineering.** Secret handling, dependency and supply-chain review, and the
  small set of controls a five-person team can realistically maintain.

## Selected work

**[ops-toolkit](https://github.com/lxlynx/ops-toolkit)**
Dependency-free scripts I got tired of rewriting on every new machine: size-based log
rotation, a health check across every git repository on disk, and a reconciler for
diffing two JSON exports.

**[blog](https://github.com/lxlynx/blog)**
Source for lxlynx.com. Plain Jekyll, no build pipeline, no trackers, no popups.

**[LynxFlow](https://lxlynx.com)**
The studio itself. Tooling and architecture work for teams small enough that one bad
abstraction genuinely hurts.

## What I reach for

| Layer | Usually |
| --- | --- |
| Services | Python (FastAPI), TypeScript (Hono, Node) |
| Edge and storage | Cloudflare Workers, D1, R2, KV |
| Data | SQLite, Postgres, DuckDB for anything ad hoc |
| Ops | Bash, systemd, Docker, GitHub Actions |
| Daily driver | Neovim, tmux, ripgrep, jq |

Nothing here is a religious position. It is the set of things I have debugged often
enough to predict how they fail.

## How I work

- Small, boring, reversible changes. The interesting part of a system should be the
  problem it solves, not its deployment story.
- Instrument before optimising. If I cannot see it in a log or a counter, I assume it
  is broken and I am simply not being told yet.
- Write the runbook while the context is still in my head, not the week after, when it
  becomes fiction.

## Writing

I keep a blog at **[lxlynx.com](https://lxlynx.com)**. Recurring subjects:

- Post-mortems from tooling that failed in ways I did not predict
- What growth work looks like when engineers own the instrumentation
- Practical security for teams without a security team

Posts go out when I have something worth saying, which is less often than any content
calendar would like.

## Contact

- Blog — [lxlynx.com](https://lxlynx.com)
- Email — `hello@lxlynx.com`
- Happy to talk about: interesting bugs, tooling collaborations, reviewing early
  architecture before it calcifies

Slower to reply about anything that starts with "quick call?".

---

<sub>Code in these repositories is MIT unless a repository says otherwise. Opinions are
load-bearing and subject to revision.</sub>
