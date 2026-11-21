# Awesome-Automotive-Aggregation-Vehicle-Data-Scraping

## Top Automated Code Review & Knowledge Graphs Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on AI-Assisted PR Review, Codebase Knowledge Graphs & Self-Hosted Review Automation*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Automated Code Review & Knowledge Graphs**. These tools help teams review pull requests faster and understand codebase structure—covering everything from AI reviewers that post inline comments to local-first knowledge graphs that give coding agents a compressed, queryable map of your entire repository.

**Examples** include CodeRabbit, Qodo, Graphite, Bito, CodeSpy, and code-review-graph (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted code review automation, open-source knowledge graph builders, and community-driven static analysis—ideal for teams seeking data sovereignty and avoiding per-seat or per-credit SaaS pricing that compounds across engineering headcount. The open-source landscape is genuinely functional: **code-review-graph** builds a local-first knowledge graph with risk-scored PR reviews and ~63x median token reduction for AI agents , **CodeSpy** provides a DSPy-powered CLI review pipeline with native GitHub PR annotations , and **SonarQube Community Build** remains the free, open-source standard for static analysis across 21 languages .

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[CodeRabbit](https://www.coderabbit.ai/)**  
  **The most widely adopted AI code review platform with a genuine free tier.** **Free: unlimited public and private repos, PR summarization only** (code reviews via VS Code/CLI) . **Essentials (formerly Pro): $24/dev/mo annual ($30 monthly)** adds PR reviews, Knowledge base, linter/SAST support, analytics, and review fixes . **Team ($48/dev/mo annual)** adds Triage (cross-repo PR queue), Plan, unit test generation, and merge-conflict resolution . **Advanced ($72/dev/mo annual)** adds continuous security review . **Enterprise** adds self-hosting, SSO, RBAC, and audit logging . **OSS projects get Team features free** .

- **[Qodo](https://www.qodo.ai/)**  
  **Agentic PR review with whole-codebase context.** **Pro Team: $30/mo base** with **pooled credits at $0.015/credit**—no per-seat fee, no repository limits, monthly billing with no commitment . **~14 reviews/mo at 2,000 credits; ~114 reviews/mo at 16,000 credits**; credits expire monthly. **14-day free trial** with unlimited reviews; **no permanent free tier** . Enterprise adds SSO, audit logs, BYOK, and on-prem/air-gapped deployment .

- **[Graphite](https://graphite.com/)**  
  **Stacked PR workflow with AI review.** **Hobby: free** (personal repos, limited AI reviews). **Starter: $20/user/mo annual** (all GitHub org repos, Slack). **Team: $40/user/mo annual** adds unlimited AI reviews, customizations, and Merge Queue. **Enterprise: custom** (SAML, audit log, GHES, SLAs) .

- **[Bito](https://bito.ai/)**  
  **AI code reviews priced per seat with LOC-based overage.** **Professional: $20/seat/mo annual ($25 monthly)** includes **5,000 LOC/seat/month**; overage at **$5 per 1,000 LOC** . **Team plan** supports up to 25 seats; Professional/Enterprise unlimited. **Free trial**: 14 days, but **capped at 15 code review executions per user** and **large PRs cannot be manually triggered** .

- **[Reviewpad](https://reviewpad.com/)**  
  Policy-based review automation with AI. A 2026 independent test cited **$89/month** and found it identified **22 issues with ~19%** of expected coverage—positioned as an MVP-stage tool .

- **[Snyk](https://snyk.io/)**  
  **Security-focused PR checks rather than general code review.** **Free: $0/mo** for individuals and small teams. **Team: $25/mo per contributing developer** with higher scan limits and issue-tracker workflow . **Ignite: $1,260/year per developer (~$105/mo)** for organizations under 50 developers wanting enterprise features .

- **[Codacy](https://www.codacy.com/)**  
  **Static analysis with AI auto-fix.** **Free forever: $0** for open-source projects; **Pro: starting ~$18–$21/dev/mo** for up to 30 contributors and 100 private projects . **14-day trial** with full platform access; public repos remain free after trial .

## Open-Source GitHub Projects

- **[code-review-graph](https://github.com/tirth8205/code-review-graph)**  
  **The most complete open-source local-first code knowledge graph for AI agents and PR review.** **28,554 GitHub stars, 2,649 forks** (as of Aug 2026) . **Builds a persistent SQLite graph** of functions, classes, imports, and calls using Tree-sitter—**no external database or cloud service** . **Risk-scored PR reviews via GitHub Action**: posts a sticky comment with overall risk score, top risk-scored changed symbols, affected execution flows, and test gaps; optional `fail-on-risk` merge gate . **Framework-aware parsing** for Laravel (routes/Eloquent), Spring (DI/routes/events), Temporal, and 30+ languages . **~63x median per-question token reduction** for AI agents vs. whole-corpus reading (range 35x–358x) . **MCP server** for Claude Code, Cursor, and Codex; **no source code sent externally** . **Honest caveat**: 528x is the best-case, not the headline; benchmarks are reproducible but represent specific repos . **Best for teams wanting a self-hosted knowledge graph that makes AI agents dramatically more efficient** while adding risk-scored PR review.

- **[CodeSpy](https://pypi.org/project/codespy-ai/)**  
  **DSPy-powered CLI review pipeline with native GitHub PR annotations.** **Posts inline review comments** with severity indicators (Critical/High/Medium/Low) and CWE references for security issues . **Parallel review modules** (Security Auditor, Bug Detector, Documentation Reviewer) with LLM-powered deduplication . **Tree-sitter parsing** for multi-language support; **Ripgrep** for code search. **LiteLLM backend** supports Bedrock, OpenAI, Anthropic, Ollama, and any OpenAI-compatible endpoint . **Cost tracker** reports tokens and spend per review . **Best for teams wanting a scriptable, model-agnostic review pipeline** they can run in CI with native GitHub integration.

- **[SonarQube Community Build](https://github.com/SonarSource/sonarqube)**  
  **The most established free and open-source static analysis platform.** **21 languages** including Java, JavaScript, TypeScript, Python, C#, Go, Ruby, PHP, Rust, Kotlin, and Terraform/Docker/Kubernetes IaC . **Detects bugs, basic vulnerabilities, security hotspots, and hardcoded secrets**; tracks technical debt and code quality history . **CI/CD integration** with GitHub, GitLab, Bitbucket, and Azure DevOps; **SARIF report ingestion** for third-party tools . **50+ community plugins** . **Best for teams wanting a proven, free static analysis foundation** with no seat limits.

### Additional Strong Open-Source Options

- **[okf-generator](https://pypi.org/project/okf-generator/)** — **Map any codebase into an interactive knowledge graph for AI agents, local SLMs, and architectural review.** Tree-sitter parsing for 11 languages and **17 manifest/build formats** (requirements.txt, package.json, Cargo.toml, go.mod, etc.) . **`okf lookup`** queries the graph; **`okf visualize`** renders a D3.js force-directed graph; **MCP server** for agent integration . **Export formats**: GraphML, Neo4j Cypher, Obsidian vault, JSON, SVG . **Best for teams wanting a broad, language-agnostic codebase graph** with multiple export targets—not a PR review tool.

- **[dagayn](https://pypi.org/project/dagayn/)** — **Local-first knowledge graph with configurable embedding backends.** **FTS-only mode** (no model download), **local embedding** via managed BGE-M3 or Qwen3 GGUF sidecars, or **remote embedding** via OpenAI/Google/MiniMax . **`dagayn detect-changes`** and **`visualize`** commands; **MCP server** with workflow-specific tools . **Rust-backed parser** for Markdown, Terraform, Rust, Python, Go, Java, Ruby, C#, PHP, Kotlin, Swift, and more . **Best for teams wanting a graph with flexible embedding options**—including fully offline operation.

- **[gfy](https://pkg.go.dev/github.com/qiangli/gfy)** — **Go-based code knowledge graph CLI with semantic search.** **`gfy query`** supports fuzzy matching and **`--semantic`** embedding-based ranking via Ollama . **`gfy path`** finds shortest paths between nodes; **`gfy view`** opens an interactive graph . **`gfy install`** registers as a Claude Code/Cursor skill and prints MCP config . **Best for Go-centric teams** wanting a lightweight, CLI-first graph tool with semantic search.

- **[RepoLens](https://pypi.org/project/repolens-audit/)** — **AI-powered dual review (security + reliability + architecture) with local-first design.** **`repolens review`** runs full dual review; **`repolens sentinel`** for security-only; **`repolens architecture`** for production-readiness audit . **Plugins** for Semgrep, gitleaks, and OSV (optional, not default install) . **Opt-in local learning index** stays on disk . **Best for teams wanting a multi-perspective audit** rather than a single-lens review.

- **[codeKG](https://github.com/eviking/codeKG)** — **Self-hosted codebase knowledge graph for AI agents.** Indexes Java/Python (and more) into **Neo4j**; serves architectural context via MCP . **Commits a `.codekg/` directory** with `INDEX.md` and module docs into the repo so agents read that first . **Watcher** polls for new commits and re-ingests . **Best for teams already on Neo4j** or wanting a graph persisted in a dedicated database rather than SQLite.

**Frameworks for building custom systems**: Combine **code-review-graph** for a local-first SQLite graph with risk-scored PR review , **CodeSpy** for a model-agnostic CLI review pipeline with native GitHub annotations , and **SonarQube Community Build** for free static analysis across 21 languages —all without per-seat or per-credit SaaS fees.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Automated code review tools post comments to pull requests and may access source code; enforce least-privilege repository scopes, avoid sending proprietary code to external services without review, and validate AI-generated findings before acting on them.
- **Pricing models in this category have hidden traps that compound.** **Bito's overage is $5 per 1,000 LOC**—a 50-developer team with large PRs can easily exceed the 5,000 LOC/seat/month quota, and **unused quota does not roll over** . **Qodo's credits expire monthly**—pick a plan that fits typical usage or you leave credits on the table . **Reviewpad scored poorly in independent testing** (22 issues, ~19% coverage) despite its $89/month price—validate quality before committing . **CodeRabbit's free tier is genuinely useful** for PR summarization, and **OSS projects get Team features free** . **Open-source options require engineering effort**: code-review-graph is powerful but its 528x token reduction is best-case, not typical (~63x median) , and okf-generator/dagayn/gfy are graph builders rather than turnkey PR reviewers . **Validate whether you need a managed AI reviewer (CodeRabbit, Qodo), a security-focused PR check (Snyk), or a self-hosted knowledge graph (code-review-graph)** before committing.

---

**Made for engineering leaders, platform teams, and developers building automated review infrastructure.**  
Let's make automated code review and codebase knowledge graphs more open, auditable, and developer-friendly.
