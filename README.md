<div align="center">

<a href="https://github.com/zakky8">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=24&duration=3000&pause=800&color=F97316&center=true&vCenter=true&width=820&lines=Verification-first+TypeScript+agent+framework;Mechanism-grounded+jailbreak+taxonomy;Three.js+%2B+WebGPU+performance+reference;Adversarial+review+as+engineering+discipline;Self-correction+documented%2C+not+silently+rewritten" alt="header" />
</a>

<br>

<p>
<a href="https://github.com/zakky8/TENET"><img src="https://img.shields.io/badge/Agent%20Framework-TENET-f97316?style=flat-square&labelColor=0d0c0b" /></a>
<a href="https://github.com/zakky8/llm-jailbreak-taxonomy"><img src="https://img.shields.io/badge/AI%20Safety-Research-f97316?style=flat-square&labelColor=0d0c0b" /></a>
<a href="https://github.com/zakky8/web-optimization"><img src="https://img.shields.io/badge/3D%20Web-Performance-f97316?style=flat-square&labelColor=0d0c0b" /></a>
<a href="https://github.com/tldr-pages/tldr/pulls?q=author%3Azakky8"><img src="https://img.shields.io/badge/OSS-tldr--pages%20(62.7k%20★)-f97316?style=flat-square&labelColor=0d0c0b" /></a>
<img src="https://komarev.com/ghpvc/?username=zakky8&style=flat-square&color=f97316&label=PROFILE+VIEWS" />
</p>

</div>

---

## › Now Shipping

> **2026-06-04** · [`TENET`](https://github.com/zakky8/TENET) — Phase 14 vuln-test triage landed.
> A 3-agent adversarial security review (security · correctness · supply-chain) over the post-P9 packages surfaced 23 real issues; HIGH + MEDIUM patched in [`a2ca9a8`](https://github.com/zakky8/TENET/commit/a2ca9a8). Bug count caught by the framework's own discipline across three review passes: **44.** Latest CI: all green (build · BENCHMARKS gate · Trivy SARIF · pnpm audit).

> **2026-06-04** · `TENET` ships [`@tenet/acp`](https://github.com/zakky8/TENET/tree/main/packages/acp) — Agent Client Protocol v1 adapter.
> JSON-RPC 2.0 over stdio, NDJSON framed, crypto-random session IDs, fresh AbortController per prompt. Lets a TENET agent talk to Zed / Cursor / Helix-class clients without bespoke glue.

> **2026-06-02** · [`llm-jailbreak-taxonomy v4.2.1`](https://github.com/zakky8/llm-jailbreak-taxonomy/releases/tag/v4.2.1) — *"Honest Reframing: Simulation is Prior, Not Result"*
> Adversarial peer review caught four overclaim issues in v4.2.0. v4.2.1 publicly retracts each one with a side-by-side "claim → why wrong" table in the changelog. **Self-correction documented, not silently rewritten** — full audit trail in `git log`.

> **2026-06-02** · `tldr-pages/tldr` PR [`#22461 fc-scan`](https://github.com/tldr-pages/tldr/pull/22461) — review suggestions applied, awaiting final maintainer merge.
> PRs [`#22489 syft`](https://github.com/tldr-pages/tldr/pull/22489) + [`#22490 helmfile`](https://github.com/tldr-pages/tldr/pull/22490) approved, queued for second-reviewer merge.

> **2026-06-02** · [`pyinstaller` page](https://github.com/tldr-pages/tldr/pull/22460) shipped to `tldr-pages/tldr` upstream.

---

## › Active Research

### 🧭 [TENET](https://github.com/zakky8/TENET) — Verification-First Agent Framework

OSS TypeScript framework where hallucination defense, source-grounding, pre-tool-call governance, capability-token sandboxing, and platform rate-limit scheduling are first-class layers — not bolt-ons. One config powers Telegram, Discord, Slack, MS Teams, embedded web widget, REST + gRPC, ticketing webhooks (Zendesk · Intercom · Freshdesk · ServiceNow), Matrix, and a voice surface (OpenAI Realtime + Twilio Media Streams).

| | |
|---|---|
| Workspaces | **28 packages · 10 surfaces** under pnpm + TS strict |
| Tests | **916 passing** · hermetic Jest · BENCHMARKS gate runs every PR |
| Verifier | Atomic-claim multi-judge + Vectara HHEM-2.1 hallucination adapter |
| Governance | `@tenet/governance` — per-tool deny / allow / require-approval policy + structured AuditSink (the OSS gap LangChain · LlamaIndex · Semantic Kernel all leave open) |
| Adapters | Anthropic-direct · Bedrock · OpenAI · Gemini · Mistral · Ollama (3 streaming) · Qdrant · pgvector · Redis state |
| Interop | MCP client + OAuth gateway · WASM-sandboxed tools (wasmtime) · Agent Client Protocol v1 (Zed / Cursor / Helix) |
| Honesty | This is a *framework*, not a model — it calls frontier LLMs and makes them grounded, cheaper per resolution, and harder to jailbreak. **Systems claim, measurable.** |
| Security | 44 bugs caught by in-house adversarial review across three passes · 0 known CVEs · Trivy SARIF + pnpm audit gated in CI |

### 🛡 [llm-jailbreak-taxonomy](https://github.com/zakky8/llm-jailbreak-taxonomy)

Mechanism-grounded taxonomy of **40 jailbreak patterns** across **10 categories**, mapped to the safety-alignment assumptions they subvert. Ships a complete evaluation harness, citation-audit methodology (every claim verified via direct WebFetch), and explicit retraction discipline when an adversarial reviewer catches an overclaim.

| | |
|---|---|
| Latest release | [v4.2.1](https://github.com/zakky8/llm-jailbreak-taxonomy/releases/tag/v4.2.1) (2026-06-02) |
| Live site | [zakky8.github.io/llm-jailbreak-taxonomy](https://zakky8.github.io/llm-jailbreak-taxonomy/) |
| Test suite | pytest 10/10 passing · GitHub Actions CI on Python 3.10/3.11/3.12 |
| Patterns | 40 · across 10 mechanism-grounded categories |
| Citations | 17, every claim direct-WebFetch verified · 1 publicly refuted (PoisonedRAG 90% not 97–99%) · 1 mis-classified category renamed (GCG vs token-smuggling) |
| Reproducibility | seed-42 bit-identical across runs · verified in CI |

### ⚡ [web-optimization](https://github.com/zakky8/web-optimization)

The definitive Three.js + WebGL performance reference. **48 validated topic folders.** Every claim sourced against live repos and browser specs. Covers WebGPU, GLSL, R3F, GSAP, mobile, GPGPU particles, and validated corrections to claims most tutorials get wrong.

| | |
|---|---|
| Live site | [zakky8.github.io/web-optimization](https://zakky8.github.io/web-optimization/) — ⌘K search, filter, particle background |
| Three.js version | r184 |
| Folders | 48 covering full 3D web stack |
| Approach | Sourced corrections to widely-repeated wrong claims (GSAP plugins free, SMIL not deprecated, PCFSoftShadowMap deprecated, Safari WebXR support) |

---

## › Open Source Contributions

| Project | Stars | Contributions |
|---|---:|---|
| [`tldr-pages/tldr`](https://github.com/tldr-pages/tldr) — collaborative cheatsheets for console commands | **62.7k** | **2 merged:** [`kioclient`](https://github.com/tldr-pages/tldr/pull/22491), [`pyinstaller`](https://github.com/tldr-pages/tldr/pull/22460) · **3 approved:** [`fc-scan`](https://github.com/tldr-pages/tldr/pull/22461), [`syft`](https://github.com/tldr-pages/tldr/pull/22489), [`helmfile`](https://github.com/tldr-pages/tldr/pull/22490) |

External-PR throughput this year: **12 PRs · ~850 commits**.

---

## › Stack

<table>
<tr>
<td valign="top" width="33%">

**AI / Safety**
- Python · Jupyter
- Anthropic SDK · OpenAI SDK
- Red teaming · RLHF
- Constitutional AI
- Statistical eval (Wilson CI, McNemar, Cochran Q)

</td>
<td valign="top" width="33%">

**Agents**
- TypeScript strict · Node 22 · ES2024
- pnpm workspaces · Jest hermetic
- MCP · ACP · OAuth gateway
- WASM-sandboxed tools (wasmtime)
- LLM-as-judge · multi-judge verifier
- pre-tool-call governance + audit

</td>
<td valign="top" width="33%">

**3D / Web**
- Three.js · R3F · drei
- WebGPU · GLSL · WGSL
- Vite · Astro · Next.js 15
- GSAP · Lenis
- Performance budgets

</td>
</tr>
</table>

---

## › Activity

<div align="center">
<img src="https://github-readme-activity-graph.vercel.app/graph?username=zakky8&theme=react-dark&bg_color=0d0c0b&hide_border=true&color=ede8e3&line=f97316&point=ede8e3&area=true&area_color=f97316" alt="Contribution activity graph" />
</div>

<table>
<tr>
<td align="center" width="50%">
<img src="https://github-readme-stats.vercel.app/api?username=zakky8&show_icons=true&hide_border=true&bg_color=0d0c0b&text_color=ede8e3&title_color=f97316&icon_color=f97316&include_all_commits=true&count_private=true&card_width=440" alt="GitHub stats" />
</td>
<td align="center" width="50%">
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=zakky8&layout=compact&hide_border=true&bg_color=0d0c0b&text_color=ede8e3&title_color=f97316&langs_count=8&include_all_commits=true&card_width=440" alt="Top languages" />
</td>
</tr>
</table>

<div align="center">
<img src="https://github-readme-streak-stats.herokuapp.com?user=zakky8&hide_border=true&background=0d0c0b&stroke=0d0c0b&ring=f97316&fire=f97316&currStreakLabel=f97316&sideLabels=ede8e3&dates=7a7570&currStreakNum=ede8e3&sideNums=ede8e3" alt="Streak" />

<br><br>

<img src="https://github-profile-trophy.vercel.app/?username=zakky8&theme=darkhub&no-frame=true&no-bg=true&margin-w=8&row=1&column=7&title=Stars,Followers,Commits,Repositories,PullRequest,Issues,Reviews" alt="Trophies" />
</div>

---

## › Citing the Research

If you use the LLM Jailbreak Taxonomy in your work:

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

Full `CITATION.cff` and BibTeX bibliography in [`paper/references.bib`](https://github.com/zakky8/llm-jailbreak-taxonomy/blob/main/paper/references.bib) (every entry direct-WebFetch verified against arxiv).

---

## › Method

Working principles that show up in every repo:

```yaml
sourcing:
  primary:   "Official docs, changelogs, browser specs, live repos"
  secondary: "Peer-reviewed papers (NeurIPS, USENIX, ICML, ACM CCS)"
  rejected:  "Affiliate review sites, paraphrased rules, training memory"

claims:
  default:     "Hypothesis until corroborated by ≥2 independent sources"
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
  adversarial: "Welcome — assumption is reviewer is right until proven otherwise"
  response:    "Fix > defend > silently ignore"
```

---

<div align="center">
<sub>
  <a href="https://github.com/zakky8/TENET">TENET</a>
  <code>·</code>
  <a href="https://github.com/zakky8/llm-jailbreak-taxonomy">llm-jailbreak-taxonomy</a>
  <code>·</code>
  <a href="https://github.com/zakky8/web-optimization">web-optimization</a>
  <code>·</code>
  <a href="https://github.com/tldr-pages/tldr/pulls?q=author%3Azakky8">tldr-pages PRs</a>
  <code>·</code>
  <a href="https://github.com/zakky8?tab=repositories">all repos</a>
</sub>
</div>
