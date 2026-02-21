<h1 align="center">Ren</h1>

<p align="center">
  Software • Cybersecurity • AI Developer — network infrastructure, security tooling, and LLM-powered automation
</p>

<p align="center">
  loving my girl
</p>

---

## What I Build

- **AI + Cybersecurity**: LLM API integration, multi-stage analysis pipelines, security review assistants, automated reporting & remediation
- **Security Engineering**: recon + API discovery, pentesting-oriented tooling (educational), exploit concepts, detection-minded engineering
- **Network Infrastructure**: reverse proxies, client-server systems, production networking services
- **Developer Tooling**: CLI/GUI utilities, workflow automation, version-control experiments

---

## Featured Projects

| Project | What it does | Stack | Link |
|--------|---------------|-------|------|
| **SentinAI (Security Review Assistant)** | AI-assisted secure code review: heuristic hotspot detection + cross-file context indexing + DeepWiki-style project semantics, with **multi-layer LLM (Qwen → DeepSeek)** to converge on actionable findings + fixes (+ optional PoC generation) | Python, Flask, FastAPI, LLM APIs | *not public yet* |
| **Simple-Ai-agent** | Lightweight AI agent scaffold focused on **LLM API connectivity** and tool-ready automation workflows (a base for assistants, pipelines, and security-oriented agents) | LLM APIs, Automation | https://github.com/v7ren/Simple-Ai-agent |
| **Logeral (Clerk-style Auth Platform)** | Full auth provider: **Next.js dashboard + Flask core auth backend**. Create apps, issue **pk_/sk_** keys, support **BYOK or Hosted OAuth**, sessions, scoped apps, and an SDK-style client integration | Next.js, TypeScript, Flask, SQLite, OAuth | *not public yet* |
| **Certion-ReverseProxy** | Production-grade reverse proxy for the Certion platform with modern architecture | TypeScript, Node.js, Networking | https://github.com/v7ren/Certion-ReverseProxy |
| **api-endpoint-discoverer** | Multi-phase API endpoint discovery & detection for security testing and research | Python, API Analysis | https://github.com/v7ren/api-endpoint-discoverer |
| **vmc2** | Modular reverse shell framework for security research and educational purposes | Python, Networking | https://github.com/v7ren/vmc2 |
| **verctrl** | Lightweight version control CLI + PyQt6 GUI | Python, PyQt6 | https://github.com/v7ren/verctrl |

---

## Technical Expertise & Current Focus

| Domain | Technologies | Level | Notes |
|-------|--------------|-------|------|
| **LLM Engineering** | LLM APIs, streaming, structured JSON outputs, cost/token control, multi-stage pipelines | **Experienced** | Security-focused agents + automation |
| **AI + Security** | hybrid analysis (heuristics + indexing + LLM), report generation, remediation guidance, optional PoC workflows | **Experienced** | SentinAI |
| **Network Infrastructure** | TypeScript, reverse proxies, client-server architecture | **Advanced** | Certion-ReverseProxy |
| **Security Research** | Python, reverse shells, API discovery, pentesting workflow | **Intermediate** | vmc2, api-endpoint-discoverer |
| **Developer Tooling** | Python, CLI, PyQt6 GUI, Git/workflows | **Intermediate** | verctrl |
| **Backend Development** | Python/TypeScript, API design, service architecture | **Intermediate** | auth + security services |

---

## Highlight: SentinAI (SentinAI Security Review Assistant)

SentinAI is an **AI-assisted secure code review system** designed to behave less like “rule spam” and more like a security engineer:

- **Understands the project first** (components, entrypoints, dependencies, data flow)
- **Finds high-risk hotspots cheaply** (keywords/regex/symbol indexing)
- **Uses LLMs for context-aware verification** (reduce false positives, add CWE/confidence/impact/remediation)
- **Optional PoC generation** for validating findings in a safe test environment

**Architecture (Gateway + Worker):**
- `main4.py` — Flask API gateway/orchestrator (uploads, scan_id, SSE streaming, history DB, docs/PoC endpoints)
- `nodev17.py` — FastAPI worker (tiered scans, symbol/call graph lite index, DeepWiki build, PoC enrich)
- `LLMindexer.py` — DeepWiki-like semantic indexer (project IR + multi-chapter markdown)

**Tiered scanning model (cheap → expensive):**
- **Tier 1 (Qwen/DeepInfra)**: high-recall prescan
- **Tier 2 (DeepSeek)**: context validation + CWE/confidence/impact
- **Tier 3 (DeepSeek + streaming)**: consultant-grade report (JSON repair for stream truncation)
- **Tier 4 (optional)**: PoC generator bound to stable `fingerprint`

---

## Highlight: Logeral (Clerk-style Auth)

**Logeral-server**: Next.js platform UI + Flask auth backend. Create applications, issue **pk_/sk_** keys, support **BYOK** or **Hosted OAuth**, sessions, and per-app user DB scoping.

**Logeral client/SDK**: Next.js client + `logeral-auth` package (hooks, components, server utils, middleware) for protecting routes with cookie-based sessions.

- Server: *not public yet*
- Client/SDK: *not public yet*

---

## Contact

| Platform | Link |
|---------|------|
| GitHub | https://github.com/v7ren |
| Discord | https://discordapp.com/users/957578507649683457 |
| Instagram | https://instagram.com/v7r.envy |

---

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=v7ren&show_icons=true&theme=radical" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=v7ren&layout=compact&theme=radical" />
</p>

---

*All security-related projects are for educational and research purposes only. I do not support illegal or unauthorized activity.*
