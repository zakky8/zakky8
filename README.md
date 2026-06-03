<div align="center">

<a href="https://github.com/zakky8">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=24&duration=3000&pause=800&color=F97316&center=true&vCenter=true&width=720&lines=AI+safety+%2B+agent+engineering;Mechanism-grounded+jailbreak+taxonomy;3D+web+performance+reference" alt="header" />
</a>

<br>

<p>
<a href="https://github.com/zakky8/llm-jailbreak-taxonomy"><img src="https://img.shields.io/badge/AI%20Safety-Research-f97316?style=flat-square&labelColor=0d0c0b" /></a>
<a href="https://github.com/zakky8/web-optimization"><img src="https://img.shields.io/badge/3D%20Web-Performance-f97316?style=flat-square&labelColor=0d0c0b" /></a>
<a href="https://github.com/tldr-pages/tldr/pulls?q=author%3Azakky8"><img src="https://img.shields.io/badge/OSS-tldr--pages-f97316?style=flat-square&labelColor=0d0c0b" /></a>
<img src="https://komarev.com/ghpvc/?username=zakky8&style=flat-square&color=f97316&label=PROFILE+VIEWS" />
</p>

</div>

---

## › Active Work

### 🛡 [llm-jailbreak-taxonomy](https://github.com/zakky8/llm-jailbreak-taxonomy) · v4.2.1
Mechanism-grounded taxonomy of **40 jailbreak patterns** across **10 categories**, mapped to the safety-alignment assumptions they subvert. Ships a complete evaluation harness, citation-audit methodology (every claim verified via direct WebFetch), and explicit retraction discipline.

> v4.2.1 publicly retracted four overclaims from v4.2.0 after adversarial review caught circular-simulation issues. The simulation is now correctly framed as a parameterized risk model awaiting empirical validation via live API execution — not as findings. Self-correction documented in `CHANGELOG.md`.

```
40 patterns · 10 categories · 17 citations all WebFetch-verified
Engineering: PEP 621 · Dockerfile · CI Python 3.10/3.11/3.12 · 10/10 pytest
Live site: zakky8.github.io/llm-jailbreak-taxonomy
```

### ⚡ [web-optimization](https://github.com/zakky8/web-optimization)
The definitive Three.js + WebGL performance reference. **48 validated topic folders.** Every claim sourced against live repos and browser specs. Covers WebGPU, GLSL, R3F, GSAP, mobile, GPGPU particles, and validated corrections to claims most tutorials get wrong.

[**zakky8.github.io/web-optimization**](https://zakky8.github.io/web-optimization/) · ⌘K search, filter, particle background.

```
48 folders · 200+ markdown files · three.js r184 · MIT
```

---

## › Open Source Contributions

External PRs to projects beyond my own:

| Project | Stars | Contributions |
|---|---:|---|
| [`tldr-pages/tldr`](https://github.com/tldr-pages/tldr) — collaborative man-page-style cheatsheets | 52k+ | [`kioclient` merged](https://github.com/tldr-pages/tldr/pull/22491) · [`pyinstaller` merged](https://github.com/tldr-pages/tldr/pull/22460) · [`fc-scan`](https://github.com/tldr-pages/tldr/pull/22461), [`syft`](https://github.com/tldr-pages/tldr/pull/22489), [`helmfile`](https://github.com/tldr-pages/tldr/pull/22490) approved/awaiting merge |

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

</td>
<td valign="top" width="33%">

**Agents**
- TypeScript · Rust
- Discord · Telegram
- RAG · vector DBs
- Tool-use orchestration

</td>
<td valign="top" width="33%">

**3D / Web**
- Three.js · R3F · drei
- WebGPU · GLSL · WGSL
- Vite · Astro · Next.js 15
- GSAP · Lenis

</td>
</tr>
</table>

---

## › Public Repositories

| Repository | Focus | Status |
|---|---|---|
| [`llm-jailbreak-taxonomy`](https://github.com/zakky8/llm-jailbreak-taxonomy) | 40-pattern AI safety taxonomy + evaluation harness | v4.2.1 active |
| [`web-optimization`](https://github.com/zakky8/web-optimization) | Three.js + WebGL performance reference, 48 folders | Active |
| [`Constitutional-ai-pipeline`](https://github.com/zakky8/Constitutional-ai-pipeline) | RLHF + constitutional AI experiments | Archived patterns |
| [`Support-Ticket-Classifier`](https://github.com/zakky8/Support-Ticket-Classifier) | ML classification pipeline | Reference |
| [`Auto-Moderation`](https://github.com/zakky8/Auto-Moderation) | Content moderation system | Reference |
| [`openclaw`](https://github.com/zakky8/openclaw) | Personal AI assistant (TypeScript) | Experimental |

---

## › Stats

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
</div>

<br>

<div align="center">
<img src="https://github-profile-trophy.vercel.app/?username=zakky8&theme=darkhub&no-frame=true&no-bg=true&margin-w=8&row=1&column=7&title=Stars,Followers,Commits,Repositories,PullRequest,Issues,Reviews" alt="Trophies" />
</div>

---

## › Method

Working principles that show up in every repo:

```yaml
sourcing:
  primary:   "Official docs, changelogs, browser specs, live repos"
  secondary: "Peer-reviewed papers (NeurIPS, USENIX, ICML, ACM CCS)"
  rejected:  "Affiliate review sites, paraphrased rules, training memory"

claims:
  default:    "Hypothesis until corroborated by ≥2 independent sources"
  single:     "Marked UNVERIFIED"
  retractions: "Documented publicly in CHANGELOG, not silently rewritten"

simulation_vs_measurement:
  prior:        "Hand-tuned parameters reproduce literature distributions"
  measurement:  "Live API calls against real models"
  rule:         "Never present the first as the second"

disclosure:
  vulnerabilities: "Disclosed to affected vendors before public release"
  payloads:        "Mechanisms published; specific exploits redacted"
```

---

<div align="center">
<sub>
  <a href="https://github.com/zakky8/llm-jailbreak-taxonomy">llm-jailbreak-taxonomy</a>
  <code>·</code>
  <a href="https://github.com/zakky8/web-optimization">web-optimization</a>
  <code>·</code>
  <a href="https://github.com/tldr-pages/tldr/pulls?q=author%3Azakky8">tldr-pages contributions</a>
  <code>·</code>
  <a href="https://github.com/zakky8?tab=repositories">all repos</a>
</sub>
</div>
