# PhD Research Engine

A unified toolchain for academic assignments and job search — works on laptop and mobile.

## What This Is

A **multi-agent system** built on Claude Code that handles:

- **PhD/Master's level academic work** (theory, code, statistics)
- **Industry job search** (resumes, interviews, career strategy)

All accessible from:

| Platform | Tool |
|-----------|------|
| **Laptop/Terminal** | Claude Code agents (`@cs-theory`, `@datasci-code`, `@datasci-stats`, `@job-search`) |
| **Phone/Browser** | Web app at <your-github-pages-url> |

---

## Agents (Terminal)

| Agent | Description | Example |
|-------|-------------|---------|
| `@cs-theory` | Hard proofs, algorithm analysis, ML theory | `@cs-theory Prove the convergence of SGD with momentum` |
| `@datasci-code` | PyTorch/JAX, data pipelines, reproducibility | `@datasci-code Write a JAX model for transformer attention` |
| `@datasci-stats` | Causality, experiment design, hypothesis tests | `@datasci-stats Design an experiment to test feature importance in XGBoost` |
| `@assignment` | General academic task, auto-detects level | `@assignment Explain bias-variance tradeoff` |
| `@job-search` | Resumes, interviews, career strategy | `@job-search Optimize my resume for a ML Engineer role` |

---

## Mobile Web App

**One URL works on your phone.** Access via GitHub Pages.

### Features
- Switch between **PhD**, **Masters**, **Customer**, and **Job Search** modes
- Clean, mobile-responsive interface
- Your API key is stored in browser memory (never sent to servers)

### Setup
1. Clone this repo
2. Go to **Settings → Pages → Source**
3. Set **Branch: main** | **Folder: /web-app/public**

---

## Getting Started

### 1. Get your Claude API Key
1. Visit <https://console.anthropic.com/>
2. Create a project and API key
3. Copy the key (starts with `sk-ant-...`)

### 2. Use in Terminal
```bash
# Example: PhD-level theory
@cs-theory What is the generalization bound for PAC learning with VC dimension d?
```

### 3. Use on Mobile
1. Save the GitHub Pages URL to your home screen
2. Enter your API key once
3. Select mode, type task, press "Process Task"

---

## Deployment

```bash
git push origin main   # Updates terminal agents + web app
```

GitHub automatically builds the web app → available in ~60s.

---

## Security

- **Terminal:** Runs locally
- **Web app:** Browser stores API key only in memory (cleared on close)

---

## Support

Built by Claude. Questions? Ask in issues.