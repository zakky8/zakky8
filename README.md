<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d0c0b,100:F97316&height=140&section=header" width="100%" alt="header" />

<div align="center">

# ZAKKY

**AI safety · agent engineering · 3D web performance**

</div>

<div align="center">

<a href="https://github.com/zakky8/TENET"><img src="https://img.shields.io/badge/-TENET-0d0c0b?style=for-the-badge" /></a>
<a href="https://github.com/zakky8/llm-jailbreak-taxonomy"><img src="https://img.shields.io/badge/-AI_Safety-0d0c0b?style=for-the-badge" /></a>
<a href="https://github.com/zakky8/web-optimization"><img src="https://img.shields.io/badge/-3D_Web-0d0c0b?style=for-the-badge" /></a>
<a href="https://github.com/tldr-pages/tldr/pulls?q=author%3Azakky8"><img src="https://img.shields.io/badge/-tldr--pages-0d0c0b?style=for-the-badge" /></a>

</div>

<br>

<table>
<tr>
<td valign="top" width="50%">

### 🛠 Currently building

Pre-tool-call governance + structured audit for OSS agent frameworks. Adversarial security review of every TypeScript package I ship. A mechanism-grounded jailbreak taxonomy that publicly retracts overclaims instead of silently rewriting them.

</td>
<td valign="top" width="50%">

### 📬 Available for

AI safety / red-team consulting · independent security review for TypeScript + Node 22 · Three.js + WebGPU performance audits · technical writing with sourced citations.

</td>
</tr>
</table>

---

## Featured projects

<table>
<tr>
<td width="33%" valign="top">

<div align="center">
<a href="https://github.com/zakky8/TENET">
<img src="https://img.shields.io/badge/TENET-Agent_Framework-f97316?style=for-the-badge&labelColor=0d0c0b" />
</a>
</div>

Verification-first TypeScript agent framework. Hallucination defense, source grounding, pre-tool-call governance, capability-token sandboxing, and platform rate-limit scheduling as first-class layers — not bolt-ons.

- **28 packages · 10 surfaces** (Discord, Slack, Telegram, Teams, web, REST, gRPC, ticketing, Matrix, voice)
- **916 tests passing** · BENCHMARKS dimensions gated in CI on every PR
- Verifier: atomic-claim multi-judge with Vectara HHEM-2.1 adapter
- Interop: MCP + OAuth gateway · WASM sandbox (wasmtime) · Agent Client Protocol v1 (Zed / Cursor / Helix)
- **44 bugs caught** across three internal adversarial review passes · 0 known CVEs
- Apache-2.0

<sub><a href="https://github.com/zakky8/TENET"><b>→ zakky8/TENET</b></a></sub>

</td>
<td width="33%" valign="top">

<div align="center">
<a href="https://github.com/zakky8/llm-jailbreak-taxonomy">
<img src="https://img.shields.io/badge/Taxonomy-AI_Safety-f97316?style=for-the-badge&labelColor=0d0c0b" />
</a>
</div>

Mechanism-grounded taxonomy of 40 LLM jailbreak patterns across 10 categories, mapped to the safety-alignment assumptions they subvert.

- Latest: [**v4.2.1**](https://github.com/zakky8/llm-jailbreak-taxonomy/releases/tag/v4.2.1) — *"Honest Reframing: Simulation is Prior"*
- Live site: [zakky8.github.io/llm-jailbreak-taxonomy](https://zakky8.github.io/llm-jailbreak-taxonomy/)
- pytest **10/10** · Python 3.10 / 3.11 / 3.12 on GitHub Actions
- 17 citations, every one direct-WebFetch verified · 1 publicly refuted (PoisonedRAG 90%, not 97–99%)
- Seed-42 bit-identical across runs · verified in CI
- Adversarial peer review caught four overclaims in v4.2.0 — all retracted in v4.2.1 with side-by-side "claim → why wrong"

<sub><a href="https://github.com/zakky8/llm-jailbreak-taxonomy"><b>→ zakky8/llm-jailbreak-taxonomy</b></a></sub>

</td>
<td width="33%" valign="top">

<div align="center">
<a href="https://github.com/zakky8/web-optimization">
<img src="https://img.shields.io/badge/Three.js-Performance-f97316?style=for-the-badge&labelColor=0d0c0b" />
</a>
</div>

The Three.js + WebGL performance reference I wish I'd had: 48 validated topic folders, every claim sourced against live repos and browser specs.

- Live site: [zakky8.github.io/web-optimization](https://zakky8.github.io/web-optimization/) — ⌘K search, filter, particle background
- Three.js **r184**
- Covers WebGPU, GLSL, R3F, GSAP, mobile, GPGPU particles, Core Web Vitals for 3D
- Sourced corrections to widely-repeated wrong claims: GSAP plugins free, SMIL not deprecated, PCFSoftShadowMap deprecated, Safari WebXR support

<sub><a href="https://github.com/zakky8/web-optimization"><b>→ zakky8/web-optimization</b></a></sub>

</td>
</tr>
</table>

---

## Stack

<div align="center">

<img src="https://skillicons.dev/icons?i=ts,py,nodejs,rust,react,nextjs,threejs,docker,kubernetes,aws,gcp,linux,bash,git,github,vscode&perline=8" alt="Stack" />

<br><br>

<sub>**AI / Safety** · Anthropic SDK · OpenAI SDK · Constitutional AI · RLHF · red-teaming · Wilson CI · McNemar · Cochran Q</sub>
<br>
<sub>**Agents** · TypeScript strict · ES2024 · pnpm workspaces · MCP · ACP · OAuth gateway · wasmtime sandbox · multi-judge verifier · pre-tool-call governance + audit</sub>
<br>
<sub>**3D / Web** · Three.js · React Three Fiber · drei · WebGPU · WGSL · GLSL · GSAP · Lenis · Vite · Astro · Next.js 15 · Core Web Vitals</sub>

</div>

---

## Recent shipments

| Date | Project | Summary |
|---|---|---|
| 2026-06-04 | `TENET` | Phase 14 vulnerability-test triage — three-agent adversarial review surfaced 23 real issues; HIGH + MEDIUM patched ([`a2ca9a8`](https://github.com/zakky8/TENET/commit/a2ca9a8)) |
| 2026-06-04 | `@tenet/acp` | Agent Client Protocol v1 adapter — JSON-RPC 2.0 over stdio, NDJSON framed, for Zed / Cursor / Helix interop |
| 2026-06-02 | `llm-jailbreak-taxonomy` | [v4.2.1](https://github.com/zakky8/llm-jailbreak-taxonomy/releases/tag/v4.2.1) released with public retractions of four overclaims |
| 2026-06-02 | `tldr-pages/tldr` | [`pyinstaller`](https://github.com/tldr-pages/tldr/pull/22460) merged upstream · `fc-scan` / `syft` / `helmfile` PRs approved |

<sub>External-PR throughput this year: **12 PRs · ~850 commits**</sub>

---

## Activity

<div align="center">

<img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=zakky8&theme=github_dark" alt="Profile summary" />

<br>

<img src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=zakky8&theme=github_dark&exclude=html,css" alt="Repos per language" width="48%" />
<img src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=zakky8&theme=github_dark&exclude=html,css" alt="Most-commit language" width="48%" />

<br>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=zakky8&theme=react-dark&bg_color=0d0c0b&hide_border=true&color=ede8e3&line=f97316&point=ede8e3&area=true&area_color=f97316" alt="Contribution activity" />

<br>

<img src="https://streak-stats.demolab.com?user=zakky8&hide_border=true&background=0d0c0b&stroke=0d0c0b&ring=f97316&fire=f97316&currStreakLabel=f97316&sideLabels=ede8e3&dates=7a7570&currStreakNum=ede8e3&sideNums=ede8e3" alt="Streak" />

</div>

---

## Working principles

> Sources: primary documents first (official docs, browser specs, live repos); peer-reviewed papers second. Affiliate review sites, paraphrased rules, and training-data memory are rejected outright.
>
> Claims: hypothesis until corroborated by ≥2 independent sources. A single source is marked `UNVERIFIED`. Retractions are documented publicly in the CHANGELOG — never silently rewritten.
>
> Simulation vs measurement: hand-tuned parameters that reproduce literature distributions are a *prior*, never presented as *measurement*. Live API calls against real models are the only valid measurement.
>
> Review: adversarial review is welcome. The assumption is the reviewer is right until proven otherwise. Response order: fix → defend → silently ignore (last is never acceptable).

---

<div align="center">

<a href="https://github.com/zakky8"><img src="https://img.shields.io/github/followers/zakky8?style=for-the-badge&labelColor=0d0c0b&color=f97316&label=Followers" /></a>
<a href="https://github.com/zakky8?tab=repositories"><img src="https://img.shields.io/badge/-All_repositories-0d0c0b?style=for-the-badge" /></a>

<br><br>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:F97316,100:0d0c0b&height=120&section=footer" width="100%" alt="footer" />

</div>

<!--
Widget choice rationale — do not restore the following dead URLs:
  github-readme-stats.vercel.app           → DEPLOYMENT_PAUSED (free-tier exhausted)
  github-profile-trophy.vercel.app         → 402 Payment Required
  github-readme-streak-stats.herokuapp.com → backend dead ("Failed to retrieve contributions")
  github-contributor-stats.vercel.app      → 402 Payment Required

Currently live alternatives in use:
  capsule-render.vercel.app                — gradient banner header / footer
  skillicons.dev                           — tech-stack icon row
  github-profile-summary-cards.vercel.app  — repo language cards (replacement for readme-stats)
  streak-stats.demolab.com                 — maintained streak-stats fork
  github-readme-activity-graph.vercel.app  — contribution graph
  shields.io                               — followers + all-repos badge
-->
