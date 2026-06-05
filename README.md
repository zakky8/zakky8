<div align="center">

# ZAKKY

**AI safety research · agent engineering · 3D web performance**

<sub>Open-source maintainer · adversarial-review discipline · primary-source citation</sub>

<p>
<a href="https://github.com/zakky8/TENET"><img src="https://img.shields.io/badge/Agent_Framework-TENET-0d0c0b?style=for-the-badge&logoColor=white" alt="TENET" /></a>
<a href="https://github.com/zakky8/llm-jailbreak-taxonomy"><img src="https://img.shields.io/badge/AI_Safety-Research-0d0c0b?style=for-the-badge&logoColor=white" alt="AI Safety Research" /></a>
<a href="https://github.com/zakky8/web-optimization"><img src="https://img.shields.io/badge/3D_Web-Performance-0d0c0b?style=for-the-badge&logoColor=white" alt="3D Web Performance" /></a>
<a href="https://github.com/tldr-pages/tldr/pulls?q=author%3Azakky8"><img src="https://img.shields.io/badge/Upstream-tldr--pages-0d0c0b?style=for-the-badge&logoColor=white" alt="tldr-pages contributor" /></a>
</p>

</div>

---

## About

I build AI-adjacent infrastructure where the engineering discipline is the product:
verification-first agent frameworks, mechanism-grounded safety research, and 3D web
performance references. Every claim I ship is sourced against primary documents,
adversarially reviewed before publication, and publicly retracted if a reviewer
later proves it wrong.

<table>
<tr>
<td valign="top" width="50%">

**Currently focused on**
- Pre-tool-call governance + audit for agent frameworks
- Adversarial security review of recently shipped TypeScript packages
- Mechanism-grounded jailbreak taxonomy (v4.x)
- Upstream contributions to widely-used OSS tooling

</td>
<td valign="top" width="50%">

**Open to**
- AI safety / red-team / agent-framework consulting
- Independent security review (TypeScript / Node 22)
- Three.js + WebGPU performance audits
- Technical writing with sourced citations

</td>
</tr>
</table>

---

## Selected work

### TENET — Verification-First Agent Framework

Open-source TypeScript framework where hallucination defense, source grounding,
pre-tool-call governance, capability-token sandboxing, and platform rate-limit
scheduling are first-class layers. One config powers Discord, Slack, Telegram,
MS Teams, embedded web widget, REST, gRPC, ticketing webhooks (Zendesk,
Intercom, Freshdesk, ServiceNow), Matrix, and voice (OpenAI Realtime +
Twilio Media Streams).

<table>
<tr><td><b>Workspaces</b></td><td>28 packages · 10 surfaces · pnpm + TypeScript strict</td></tr>
<tr><td><b>Tests</b></td><td>916 passing · hermetic Jest · BENCHMARKS dimensions gated in CI on every PR</td></tr>
<tr><td><b>Verifier</b></td><td>Atomic-claim multi-judge with Vectara HHEM-2.1 hallucination adapter</td></tr>
<tr><td><b>Governance</b></td><td><code>@tenet/governance</code> — per-tool deny / allow / require-approval policy + structured AuditSink (the gap LangChain, LlamaIndex, Semantic Kernel leave open)</td></tr>
<tr><td><b>Model adapters</b></td><td>Anthropic-direct, Bedrock, OpenAI, Gemini, Mistral, Ollama · 3 streaming</td></tr>
<tr><td><b>Interop</b></td><td>MCP client + OAuth gateway · WASM-sandboxed tools (wasmtime) · Agent Client Protocol v1 (Zed, Cursor, Helix)</td></tr>
<tr><td><b>Security</b></td><td>44 bugs caught across three internal adversarial review passes · 0 known CVEs · Trivy SARIF + <code>pnpm audit</code> gated in CI</td></tr>
<tr><td><b>License</b></td><td>Apache-2.0</td></tr>
</table>

> Status: pre-1.0, APIs may change. This is a framework, not a model — it calls
> frontier LLMs and makes them measurably more grounded, cheaper per
> resolution, and harder to jailbreak. The claim is a systems claim, and it is
> measurable: the BENCHMARKS gate runs every PR and numbers are produced, not asserted.

→ [`zakky8/TENET`](https://github.com/zakky8/TENET)

---

### LLM Jailbreak Taxonomy

Mechanism-grounded taxonomy of 40 jailbreak patterns across 10 categories,
mapped to the safety-alignment assumptions they subvert. Ships a complete
evaluation harness, a citation-audit methodology (every claim verified via
direct WebFetch against primary sources), and explicit retraction discipline
when an adversarial reviewer catches an overclaim.

<table>
<tr><td><b>Latest release</b></td><td><a href="https://github.com/zakky8/llm-jailbreak-taxonomy/releases/tag/v4.2.1">v4.2.1</a> · 2026-06-02 — "Honest Reframing: Simulation is Prior, Not Result"</td></tr>
<tr><td><b>Live site</b></td><td><a href="https://zakky8.github.io/llm-jailbreak-taxonomy/">zakky8.github.io/llm-jailbreak-taxonomy</a></td></tr>
<tr><td><b>Test suite</b></td><td>pytest 10/10 · GitHub Actions on Python 3.10 / 3.11 / 3.12</td></tr>
<tr><td><b>Patterns</b></td><td>40 across 10 mechanism-grounded categories</td></tr>
<tr><td><b>Citations</b></td><td>17 sources, every claim direct-WebFetch verified · 1 publicly refuted (PoisonedRAG 90%, not 97–99%) · 1 mis-classified category renamed (GCG vs token-smuggling)</td></tr>
<tr><td><b>Reproducibility</b></td><td>Seed-42 bit-identical across runs · verified in CI</td></tr>
</table>

→ [`zakky8/llm-jailbreak-taxonomy`](https://github.com/zakky8/llm-jailbreak-taxonomy)

---

### Three.js + WebGL Performance Reference

A primary-source-cited reference for production Three.js and WebGL
performance work. 48 validated topic folders covering WebGPU, GLSL, React
Three Fiber, GSAP, mobile optimization, GPGPU particles, and corrections to
widely-repeated wrong claims.

<table>
<tr><td><b>Live site</b></td><td><a href="https://zakky8.github.io/web-optimization/">zakky8.github.io/web-optimization</a> — ⌘K search, filter, particle background</td></tr>
<tr><td><b>Three.js version</b></td><td>r184</td></tr>
<tr><td><b>Folders</b></td><td>48 covering the full 3D web stack</td></tr>
<tr><td><b>Corrections</b></td><td>GSAP plugins free, SMIL not deprecated, PCFSoftShadowMap deprecated, Safari WebXR support — all sourced</td></tr>
</table>

→ [`zakky8/web-optimization`](https://github.com/zakky8/web-optimization)

---

## Recent shipments

| Date | Project | Summary |
|---|---|---|
| 2026-06-04 | `TENET` | Phase 14 vulnerability-test triage — three-agent adversarial review surfaced 23 real issues; HIGH + MEDIUM patched ([`a2ca9a8`](https://github.com/zakky8/TENET/commit/a2ca9a8)) |
| 2026-06-04 | `@tenet/acp` | Agent Client Protocol v1 adapter shipped — JSON-RPC 2.0 over stdio, NDJSON framed, for Zed / Cursor / Helix interop |
| 2026-06-02 | `llm-jailbreak-taxonomy` | [v4.2.1](https://github.com/zakky8/llm-jailbreak-taxonomy/releases/tag/v4.2.1) released with public retractions of four overclaims from v4.2.0 |
| 2026-06-02 | `tldr-pages/tldr` | PR [#22461 `fc-scan`](https://github.com/tldr-pages/tldr/pull/22461) addressed; PRs [#22489 `syft`](https://github.com/tldr-pages/tldr/pull/22489) and [#22490 `helmfile`](https://github.com/tldr-pages/tldr/pull/22490) approved |
| 2026-06-02 | `tldr-pages/tldr` | [`pyinstaller`](https://github.com/tldr-pages/tldr/pull/22460) page merged upstream |

---

## Open-source contributions

| Project | Stars | Contributions |
|---|---:|---|
| [`tldr-pages/tldr`](https://github.com/tldr-pages/tldr) — collaborative cheatsheets for console commands | 62.7k | **Merged:** [`kioclient`](https://github.com/tldr-pages/tldr/pull/22491), [`pyinstaller`](https://github.com/tldr-pages/tldr/pull/22460) · **Approved:** [`fc-scan`](https://github.com/tldr-pages/tldr/pull/22461), [`syft`](https://github.com/tldr-pages/tldr/pull/22489), [`helmfile`](https://github.com/tldr-pages/tldr/pull/22490) |

External-PR throughput this year: 12 PRs · ~850 commits.

---

## Stack

<table>
<tr>
<td valign="top" width="33%">

**AI / Safety**
- Python · Jupyter
- Anthropic SDK · OpenAI SDK
- Red teaming · RLHF
- Constitutional AI
- Statistical evaluation (Wilson CI, McNemar, Cochran Q)

</td>
<td valign="top" width="33%">

**Agents**
- TypeScript strict · Node 22 · ES2024
- pnpm workspaces · hermetic Jest
- MCP · ACP · OAuth gateway
- WASM-sandboxed tools (wasmtime)
- Multi-judge verifier
- Pre-tool-call governance + audit

</td>
<td valign="top" width="33%">

**3D / Web**
- Three.js · React Three Fiber · drei
- WebGPU · GLSL · WGSL
- Vite · Astro · Next.js 15
- GSAP · Lenis
- Performance budgets · Core Web Vitals

</td>
</tr>
</table>

---

## Activity

<div align="center">
<img src="https://github-readme-activity-graph.vercel.app/graph?username=zakky8&theme=react-dark&bg_color=0d0c0b&hide_border=true&color=ede8e3&line=f97316&point=ede8e3&area=true&area_color=f97316" alt="Contribution activity" />

<br><br>

<img src="https://streak-stats.demolab.com?user=zakky8&hide_border=true&background=0d0c0b&stroke=0d0c0b&ring=f97316&fire=f97316&currStreakLabel=f97316&sideLabels=ede8e3&dates=7a7570&currStreakNum=ede8e3&sideNums=ede8e3" alt="Contribution streak" />

<br><br>

<sub>Flagship repositories — live state</sub>

<p>
<a href="https://github.com/zakky8/TENET"><img src="https://img.shields.io/github/last-commit/zakky8/TENET?style=flat-square&labelColor=0d0c0b&color=f97316&label=TENET" /></a>
<a href="https://github.com/zakky8/TENET/actions"><img src="https://img.shields.io/github/actions/workflow/status/zakky8/TENET/ci.yml?branch=main&style=flat-square&labelColor=0d0c0b&label=TENET%20CI" /></a>
<a href="https://github.com/zakky8/llm-jailbreak-taxonomy"><img src="https://img.shields.io/github/last-commit/zakky8/llm-jailbreak-taxonomy?style=flat-square&labelColor=0d0c0b&color=f97316&label=jailbreak-taxonomy" /></a>
<a href="https://github.com/zakky8/llm-jailbreak-taxonomy/stargazers"><img src="https://img.shields.io/github/stars/zakky8/llm-jailbreak-taxonomy?style=flat-square&labelColor=0d0c0b&color=f97316" /></a>
<a href="https://github.com/zakky8/web-optimization"><img src="https://img.shields.io/github/last-commit/zakky8/web-optimization?style=flat-square&labelColor=0d0c0b&color=f97316&label=web-optimization" /></a>
<a href="https://github.com/zakky8?tab=followers"><img src="https://img.shields.io/github/followers/zakky8?style=flat-square&labelColor=0d0c0b&color=f97316&label=followers" /></a>
</p>

</div>

<!--
Widget choice rationale (for future maintainers — do not restore the dead URLs):

  github-readme-stats.vercel.app          — DEPLOYMENT_PAUSED (free-tier exhausted)
  github-profile-trophy.vercel.app        — 402 Payment Required (same)
  github-readme-streak-stats.herokuapp.com — backend dead, returns
                                              "Failed to retrieve contributions"

Replaced with streak-stats.demolab.com (maintained fork) and Shields.io
badges that source directly from the GitHub API.
-->

---

## Working principles

```yaml
sourcing:
  primary:   "Official docs, changelogs, browser specs, live repos"
  secondary: "Peer-reviewed papers (NeurIPS, USENIX, ICML, ACM CCS)"
  rejected:  "Affiliate review sites, paraphrased rules, training memory"

claims:
  default:     "Hypothesis until corroborated by at least two independent sources"
  single:      "Marked UNVERIFIED"
  retractions: "Documented publicly in CHANGELOG, not silently rewritten"

simulation_vs_measurement:
  prior:       "Hand-tuned parameters reproduce literature distributions"
  measurement: "Live API calls against real models"
  rule:        "Never present the first as the second"

disclosure:
  vulnerabilities: "Disclosed to affected vendors before public release"
  payloads:        "Mechanisms published; specific exploits redacted"

review:
  adversarial: "Welcome — assumption is the reviewer is right until proven otherwise"
  response:    "Fix > defend > silently ignore"
```

---

## Citation

If you reference the LLM Jailbreak Taxonomy in academic or industry work:

```bibtex
@misc{zakky2026llmjailbreak,
  title  = {A Systematic Taxonomy of Jailbreak Techniques in Large Language Models:
            Toward Robust Safety Alignment},
  author = {Zakky},
  year   = {2026},
  month  = {June},
  note   = {Version 4.2.1 --- honest reframing release},
  url    = {https://github.com/zakky8/llm-jailbreak-taxonomy}
}
```

Full `CITATION.cff` and BibTeX bibliography in
[`paper/references.bib`](https://github.com/zakky8/llm-jailbreak-taxonomy/blob/main/paper/references.bib) —
every entry direct-WebFetch verified against arXiv.

---

<div align="center">
<sub>
  <a href="https://github.com/zakky8/TENET">TENET</a>
  &nbsp;·&nbsp;
  <a href="https://github.com/zakky8/llm-jailbreak-taxonomy">llm-jailbreak-taxonomy</a>
  &nbsp;·&nbsp;
  <a href="https://github.com/zakky8/web-optimization">web-optimization</a>
  &nbsp;·&nbsp;
  <a href="https://github.com/tldr-pages/tldr/pulls?q=author%3Azakky8">tldr-pages PRs</a>
  &nbsp;·&nbsp;
  <a href="https://github.com/zakky8?tab=repositories">all repositories</a>
</sub>
</div>
