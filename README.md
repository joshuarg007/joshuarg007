# Joshua R. Gutierrez

Full stack engineer working across Python, FastAPI, TypeScript, React, PostgreSQL, and AWS. I have been building professionally since 2013, starting in Laravel and PHP and working in Python and React now.

I split my time between three things: shipping production SaaS, building technical SEO tooling, and applied machine learning research on how neural networks forget.

Based in New Mexico. I work at [Axion Deep Labs](https://axiondeep.com).

- Research profile: [ORCID 0009-0008-2595-9484](https://orcid.org/0009-0008-2595-9484)
- Longer bio: [axiondeepdigital.com/team/joshua-gutierrez](https://www.axiondeepdigital.com/team/joshua-gutierrez)

---

## Stack

| Area | Tools |
| --- | --- |
| Languages | Python, TypeScript, JavaScript, SQL, Kotlin |
| Backend | FastAPI, SQLAlchemy, Alembic, Node.js, REST APIs |
| Frontend | React, Next.js, Vite, Tailwind CSS, Three.js |
| Data | PostgreSQL, SQLite, Redis |
| Infrastructure | Docker, AWS (SES, SNS, Lambda, S3, Route 53, Amplify), Nginx, GitHub Actions |
| Machine learning | PyTorch, persistent homology, continual learning, topological data analysis |
| Security | JWT, OAuth 2.0, AES-256 at rest, SSRF-safe fetching, webhook signature verification |

---

## Products

**[Made4Founders](https://made4founders.com)**
A command center for people running small companies. Task and deadline tracking, document management, an encrypted credential vault, cap table and investor updates, and social publishing that adapts one post across platforms.
`FastAPI` `React` `TypeScript` `PostgreSQL` `Docker`

**[Site2CRM](https://site2crm.io)**
Website to CRM lead capture with AI lead scoring, a chat widget, and a WordPress plugin. Turns form fills and conversations into scored, routed leads.
`FastAPI` `React` `PostgreSQL`

**[DeepAudit](https://axiondeepdigital.com/free-seo-audit)**
A free technical SEO audit tool that runs 60+ checks against a real browser render rather than parsing raw HTML, which is the only way to see what Googlebot sees on a JavaScript-heavy site.
`Puppeteer` `Chromium` `AWS Lambda` `Next.js`

---

## Research

Two open source research programs, plus a line of empirical web studies published as preprints. Compute runs on the NMSU Discovery cluster.

**[PERSIST](https://github.com/Axion-Deep-Labs/persist-topological-forgetting)** asks whether the topology of a loss landscape predicts how well a model resists catastrophic forgetting.

The method computes persistent homology over loss landscape slices and tests whether those topological features predict forgetting, and how much a mitigation strategy such as EWC will help, before you retrain.

Scope so far is 57 configurations across CIFAR-100, CUB-200-2011, and NWPU-RESISC45, spanning 19 architectures from 0.3M to 44.7M parameters, plus a scale validation on ImageNet-100. The strongest result is that H0, the count of connected components, tracks how much a model benefits from EWC regularization, replicating on two of the three datasets. At ImageNet scale H1 becomes the dominant signal instead, which is the kind of thing you only find by running it. A follow-on study extends the same framework to grokking, where the signal so far is borderline and looks like it lives in a late-grokking subpopulation rather than in grokking onset generally.

A preprint is in preparation. The repository holds the full pipeline, configs, and analysis.

`PyTorch` `Ripser` `SLURM` `NumPy` `SciPy`

**[EMERGE](https://github.com/Axion-Deep-Labs/emerge-icl)** asks when in-context learning emerges in transformers trained from scratch, and how the task diversity threshold that triggers it scales with model capacity.

The setting is in-context noisy linear regression, which has exact baselines on both sides: ridge regression for genuine in-context behavior, and dMMSE for memorized in-weights behavior. That makes emergence measurable rather than eyeballed. Open source from the first commit, with every dataset synthetic from seeded RNGs and every model trained from scratch, so the whole program is reproducible by anyone with a GPU.

The research plan is pre-registered and frozen before results, with amendments tracked in a separate experiment log. The Phase 0 pilot is complete at 28 of 28 cells and analysis is underway.

`PyTorch` `SLURM` `NumPy`

### Published studies

Empirical web research, sole author, with an open dataset and methodology published alongside each paper.

- **[AI Crawler Visibility and JavaScript Rendering Gaps in Small Business Websites](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6915818)** (n=368). A quarter of the sites measured put at least one answer critical element behind JavaScript that non-rendering AI crawlers never execute. Managed server rendered platforms were roughly seven times less affected. Descriptive, with an [open dataset](https://www.axiondeepdigital.com/research/ai-visibility-2026/dataset.csv) that reproduces every figure.
- **[State of Small Business Websites 2026](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6719299)** (n=292). Automated Core Web Vitals and accessibility auditing of small business sites. 96.9% of the sites measured fail at least one Core Web Vital on mobile.
- **[The State of AI-Readiness on Business Websites](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=7057078)**. Crawl based measurement of how legibly business websites identify themselves to machines: identity markup, structured data, named people, and llms.txt adoption, broken out by vertical.

`Playwright` `Puppeteer` `pandas` `SciPy`

## Open source

- **[QUANTA](https://github.com/joshuarg007/quanta)** Quantum computing education platform. Drag and drop circuit builder, Bloch sphere visualization, and a guided curriculum. `FastAPI` `Qiskit` `React`
- **[Forma](https://github.com/joshuarg007/forma)** Full stack React app platform pairing a visual builder with a schema-driven backend runtime. `FastAPI` `SQLAlchemy` `Next.js`
- **[axiondeep](https://github.com/joshuarg007/axiondeep)** Frontend for Axion Deep Labs. `TypeScript` `React`

---

## Education

- **MS, Artificial Intelligence and Data Science**, CSU Global. Expected December 2026, in progress.
- **BS, Computer Science**, Colorado State University. Completed May 2025.

---

## Elsewhere

[LinkedIn](https://linkedin.com/in/joshua-gutierrez-b198117a) · [ORCID](https://orcid.org/0009-0008-2595-9484) · [CoderLegion](https://coderlegion.com/user/Joshua+R.+Gutierrez) · [Email](mailto:joshuarg007@gmail.com)
