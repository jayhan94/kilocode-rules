# kilocode-rules

Opinionated configuration for [Kilo Code](https://kilocode.ai/) — a local AI coding agent in VS Code. This repo contains system prompts and rule files that shape how Kilo Code interacts with your codebase.

---

## ⚠️ Disclaimers

* This setup is **opinionated**. If you're looking for stable or beginner-friendly templates, start here - [rules_template](https://github.com/Bhartendu-Kumar/rules_template).
* Want to use a similar setup with **Roo Code** or **Cline**? That link works for those too.
* Designed for **solo dev workflows**, not teams.
* Changes often; no stability guaranteed.

---

## ⚙️ What This Repo Contains

- `rules/` & `rules-*` – structured prompts for behavior control
- `system-prompt-*` – main system instructions
- Bun-based runtime setup
- Minimal dependencies, zero TypeScript scaffolding

This repo assumes you know what you're doing. Defaults are heavily customized and may break at any time.

---

## 🧠 Prompt Entry Point

The default entry point for large or multi-step prompts is **Orchestrator**, which is included by default in Kilo Code.

You may define your own prompt flow strategies as needed — this repo stays unopinionated about modes.

---

## 📦 How to Use These Rules

1. Clone into your project root:

```bash
cd your-project-root
git clone https://github.com/shanefully-done/kilocode-rules.git
````

2. Rename the directory so Kilo Code can detect it:

```bash
mv kilocode-rules .kilocode
```

3. Kilo Code will automatically detect `.kilocode` and apply the rules.

Note: To enable Memory Bank, switch to Architect mode and run "initialize memory bank". For details, see the Memory Bank docs: https://kilocode.ai/docs/advanced-usage/memory-bank

---

## 🙏 Credits

* Base prompt structure and configuration largely forked from [`shanefully-done/kilocode-rules`](https://github.com/shanefully-done/kilocode-rules)

---

## 🧪 Tips

* Keep prompts minimal and specific.
* Use **Orchestrator** for complex flows — or define your own logic.
* Disable conflicting VS Code extensions (like Copilot) for clean integration.
