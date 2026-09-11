<p align="center">
  <img src="https://raw.githubusercontent.com/lxlynx/lxlynx/main/assets/header.svg" alt="Alexander Cardoza — AI Toolchain Engineer" width="880"/>
</p>
<p align="center">
  <img src="https://raw.githubusercontent.com/lxlynx/lxlynx/main/assets/now.svg" alt="now" width="720"/>
</p>
<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white" height="22"/>
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white" height="22"/>
  <img src="https://img.shields.io/badge/Cloudflare-F38020?style=flat&logo=cloudflare&logoColor=white" height="22"/>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white" height="22"/>
  <img src="https://img.shields.io/badge/Neovim-57A143?style=flat&logo=neovim&logoColor=white" height="22"/>
  <img src="https://img.shields.io/badge/lxlynx.com-1F2328?style=flat&logo=readme&logoColor=white" height="22"/>
</p>

---

Founder of LynxFlow. I build developer tooling and write about the parts that break in production.

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

**[resume](https://github.com/lxlynx/resume)**
A one-file Markdown resume template for engineers, with no build step and no personal
contact details baked into the template.

**[eval-harness](https://github.com/lxlynx/eval-harness)**
A stdlib-only Python script that scores LLM outputs against multiple metrics —
exact match, substring containment, token overlap, and custom callables. Run it
before you commit a prompt change, not after the invoice arrives. The thing I
reach for when "vibes-based eval" stops being defensible.

**[model-router](https://github.com/lxlynx/model-router)**
A rule-based routing layer that picks a model and endpoint by task type, cost
ceiling, and context length. No embeddings, no learned weights, no dashboard.
First matching rule wins, and you can read the entire routing logic in one
screen. Built because every team running more than one model reinvents this
badly, and I wanted the version I could explain at 3am.

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

## 📊 Activity

<p align="center">
  <img height="160" src="https://gh-profile-stats.zli39uclan.workers.dev/stats?username=lxlynx&hide_border=true"/>
  <img height="160" src="https://gh-profile-stats.zli39uclan.workers.dev/top-langs?username=lxlynx&hide_border=true"/>
</p>
<p align="center">
  <img width="720" src="https://gh-profile-stats.zli39uclan.workers.dev/activity?username=lxlynx&hide_border=true"/>
</p>

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
