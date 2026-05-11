<h1 align="center">rpikit</h1>

<p align="center">
  <strong>The operating system for autonomous AI agents — kernel, skills, and SDKs to run a company on agents.</strong>
</p>

<p align="center">
  <a href="https://github.com/rpikit">📦 Repositories</a> &nbsp;·&nbsp;
  <a href="https://github.com/orgs/rpikit/discussions">💬 Discussions</a> &nbsp;·&nbsp;
  <a href="https://github.com/rpikit/.github/issues">🐛 Issues</a>
</p>

---

## Why this org exists

Today's "AI agents" are mostly chatbots with extra steps. They answer one question, write one function, send one email — then stop. The hard part isn't asking a model to do something. The hard part is **keeping it running, on goals, with memory, across days, talking to other agents, without a human babysitting the loop**.

That layer — the runtime, the scheduler, the skill registry, the inter-agent protocol, the lifecycle — is what an operating system does for processes. **rpikit is that operating system, but for agents.** Local-first, model-agnostic (BYOM), open source. **Apache-2.0 / MIT**, no telemetry, no lock-in.

Our bet: in five years, real companies will be run by graphs of autonomous agents the way they're run by org charts today. Someone has to build the OS. We're starting.

## What we ship

<table>
<tr>
<td width="50%" valign="top">

### 🎼 <a href="https://github.com/rpikit/open-company-os">open-company-os</a> · ⭐ live

The **flagship console** for AI-run companies. Score-based UI where agents play in parallel across pipeline phases, with cinematic human-in-the-loop overlays. Built on Next.js 16, TypeScript strict, Tailwind v4.

`pnpm dev` &rarr; Átrio (calm mode), Partitura (orchestra grid), Solo (agent deep-dive), Maestro (`⌘;`).

</td>
<td width="50%" valign="top">

### 🧠 <a href="#">kernel</a> · *coming soon*

The **agent runtime**. Scheduling, memory, tool registry, lifecycle, sandboxing. Brings the same primitives a Unix kernel gives processes — but for autonomous agents that own goals instead of executing instructions.

`rpikit run agent.yaml` &rarr; an agent that wakes up, checks state, picks the next action, and writes back to memory.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🧩 <a href="#">skills</a> · *coming soon*

**Composable capabilities** any agent on the runtime can install at startup. Drop a folder, restart, it works. The <a href="https://docs.anthropic.com/en/docs/claude-code/skills"><code>SKILL.md</code></a> convention — fork, drop, run.

CRM, billing, calendar, Slack, code-review, deploy — each one a folder, not a plugin.

</td>
<td width="50%" valign="top">

### 📦 <a href="#">sdk-python</a> / <a href="#">sdk-typescript</a> · *coming soon*

**Build your own agents** on top of the kernel. Typed APIs for state, tools, sub-agents, and the inter-agent bus. BYOM at every layer — Claude, GPT, local LLMs, your fine-tune.

`pip install rpikit` · `npm install @rpikit/sdk`

</td>
</tr>
</table>

> Status: **early**. Only `open-company-os` is shipped today; everything else is being built in the open. Interfaces will change.

## Principles

- **Bring your own model.** We don't ship a model. Plug Claude, GPT, Llama, your fine-tune — whatever runs.
- **Open by default.** Apache-2.0 / MIT across the stack. No locked surface, no telemetry, no phone-home.
- **Local-first.** Your agents, memory, and state run on your hardware. Cloud is a deployment target, not the home.
- **Skills are files, not plugins.** Drop a folder, restart, it works. The <a href="https://docs.anthropic.com/en/docs/claude-code/skills"><code>SKILL.md</code></a> convention.
- **Autonomy by default.** Agents own goals, not tickets. The runtime keeps them alive across days, not turns.

## Get involved

- **Star the projects** that resonate — cheapest, loudest signal.
- **Add a skill** — drop a `SKILL.md` folder and open a PR.
- **Build a reference agent** — fork `agents`, ship a job description as code.
- **Open an issue** with the use case you wish the runtime supported.

Issues, PRs, and Discussions are open across every public repo.

---

<p align="center"><sub>Built in the open by a small team — <i>the OS for autonomous agents.</i><br>Apache-2.0 / MIT</sub></p>
