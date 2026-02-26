<p align="center">
  <strong>Awesome Vibecoding</strong>
  <br/>
  <em>The complete guide to building software with AI. Tools, workflows, prompts, and real projects.</em>
</p>

<p align="center">
  <a href="https://awesome.re"><img src="https://awesome.re/badge-flat2.svg" alt="Awesome" /></a>
  <img src="https://img.shields.io/github/stars/DukeDeSouth/awesome-vibecoding?style=social" alt="Stars" />
  <img src="https://img.shields.io/github/last-commit/DukeDeSouth/awesome-vibecoding" alt="Last Commit" />
</p>

---

> **Vibe coding** — describe what you want, AI writes the code, you iterate. Coined by [Andrej Karpathy](https://x.com/karpathy/status/1886192184808149383) (Feb 2025). By 2026, 72% of developers use AI coding tools daily.

Not just a list of tools — this is the **complete playbook**: what to use, how to use it, real workflows, real prompts, and real projects people shipped.

## Contents

- [The Stack](#the-stack) — What to install today
- [AI-Native IDEs](#ai-native-ides)
- [Browser Builders](#browser-builders)
- [Terminal Agents](#terminal-agents)
- [Code Completion](#code-completion)
- [Design to Code](#design-to-code)
- [Workflows](#workflows) — How people actually work
- [Prompts & Techniques](#prompts--techniques) — Copy-paste and go
- [Shipped Projects](#shipped-projects) — Real things built with vibecoding
- [Learning](#learning)
- [Communities](#communities)

---

## The Stack

What you need to start vibecoding today. Pick one from each row:

| Layer | Best Free | Best Paid | Why |
|-------|-----------|-----------|-----|
| **IDE** | [Cursor](https://cursor.com) (free tier) | [Cursor Pro](https://cursor.com) ($20/mo) | Inline AI edits, chat, multi-file |
| **Model** | Claude Sonnet 4.5 | Claude Opus 4.5 | Best at code generation as of Feb 2026 |
| **Terminal** | [Claude Code](https://github.com/anthropics/claude-code) | [Codex CLI](https://github.com/openai/codex) | AI agents in your terminal |
| **Browser** | [Bolt.new](https://bolt.new) | [Lovable](https://lovable.dev) | Full apps from prompts |
| **Version Control** | Git | Git | Non-negotiable |

---

## AI-Native IDEs

Full development environments built around AI from the ground up.

| Tool | Pricing | Best For | Key Feature |
|------|---------|----------|-------------|
| [Cursor](https://cursor.com) | Free / $20 / $40 | Everything | Tab completion + chat + multi-file edits |
| [Windsurf](https://codeium.com/windsurf) | Free / $15 | Beginners | Cascade flow, gentle learning curve |
| [Zed](https://zed.dev) | Free | Speed | Fastest editor, built-in AI |
| [Void](https://voideditor.com) | Free (OSS) | Privacy | Open-source, local models |
| [PearAI](https://trypear.ai) | Free (OSS) | Customization | Fork-friendly, extensible |

## Browser Builders

Build full-stack apps from a text prompt. No local setup.

| Tool | Pricing | Best For | Ships To |
|------|---------|----------|----------|
| [Bolt.new](https://bolt.new) | Free / $20 | Full-stack web apps | Netlify |
| [Lovable](https://lovable.dev) | Free / $20 | Polished UIs | Supabase + Netlify |
| [v0](https://v0.dev) | Free / $20 | React components | Vercel |
| [Replit Agent](https://replit.com) | Free / $25 | Quick prototypes | Replit hosting |
| [Firebase Genkit](https://firebase.google.com/products/genkit) | Free | Backend logic | Google Cloud |

## Terminal Agents

AI coding agents that run in your terminal.

| Tool | Pricing | Language | Key Feature |
|------|---------|----------|-------------|
| [Claude Code](https://github.com/anthropics/claude-code) | API costs | Python | Agentic coding, file edits |
| [Codex CLI](https://github.com/openai/codex) | API costs | TypeScript | GPT-powered terminal agent |
| [Aider](https://github.com/paul-gauthier/aider) | API costs | Python | Git-aware pair programming |
| [Mentat](https://github.com/AbanteAI/mentat) | API costs | Python | Understands your whole codebase |
| [GPT Engineer](https://github.com/gpt-engineer-org/gpt-engineer) | API costs | Python | Generates entire codebases |

## Code Completion

Autocomplete on steroids. Works inside any editor.

| Tool | Pricing | Editor Support |
|------|---------|---------------|
| [GitHub Copilot](https://github.com/features/copilot) | Free / $10 | VS Code, JetBrains, Vim |
| [Supermaven](https://supermaven.com) | Free / $10 | VS Code, JetBrains |
| [Codeium](https://codeium.com) | Free | VS Code, JetBrains, Vim, Emacs |
| [Tabby](https://github.com/TabbyML/tabby) | Free (OSS) | VS Code, JetBrains (self-hosted) |
| [Continue](https://github.com/continuedev/continue) | Free (OSS) | VS Code, JetBrains |

## Design to Code

Turn designs, screenshots, or mockups into working code.

| Tool | Input | Output |
|------|-------|--------|
| [v0](https://v0.dev) | Text prompt / image | React + Tailwind |
| [Lovable](https://lovable.dev) | Text / Figma | Full-stack app |
| [Screenshot to Code](https://github.com/abi/screenshot-to-code) | Screenshot | HTML / React / Vue |
| [tldraw Make Real](https://makereal.tldraw.com) | Hand-drawn sketch | Working app |

---

## Workflows

How people actually use these tools day-to-day.

### The Basic Loop

```
1. Describe what you want (be specific)
2. AI generates code
3. Run it
4. See what's wrong
5. Tell AI what to fix
6. Repeat until done
```

### The Pro Workflow

```
1. Plan in markdown first (features, architecture, tech stack)
2. Give the plan to AI as context
3. Build feature by feature, not all at once
4. Commit after each working feature
5. Use AI for tests after implementation
6. Review AI code before shipping (it makes mistakes)
```

### The "Ship Fast" Workflow

```
1. Use browser builder (Bolt/Lovable) for UI + basic backend
2. Export to GitHub
3. Open in Cursor for refinement
4. Deploy to Vercel/Railway
5. Total time: hours, not weeks
```

### Rules for Better Results

- **Be specific.** "Add a login page with email/password, Google OAuth, and a forgot password flow" > "add auth"
- **Give context.** Paste your schema, your API, your existing code.
- **One thing at a time.** Don't ask for 5 features in one prompt.
- **Use .cursorrules / AGENTS.md.** Project-specific instructions make AI 10x better.
- **Commit often.** AI breaks things. Git is your undo button.

---

## Prompts & Techniques

Copy-paste these into your AI IDE.

### Project Kickoff Prompt

```
I'm building [PRODUCT] — a [one-line description].

Tech stack: Next.js 15, TypeScript, Tailwind CSS, Prisma, PostgreSQL.

Start by creating:
1. Project structure with app router
2. Database schema for [core entities]
3. Basic layout with navigation
4. Home page with [key feature]

Use TypeScript strict mode. Functional components only. 
No comments that just describe what code does.
```

### Bug Fix Prompt

```
This code throws [ERROR]. 

File: [paste file]
Error: [paste error]

Fix the bug. Don't change anything else. Explain what was wrong.
```

### Refactor Prompt

```
Refactor this file. Goals:
- Extract reusable logic into hooks/utils
- Remove duplication
- Improve type safety
- Keep the same behavior

[paste file]
```

---

## Shipped Projects

Real products built primarily with vibecoding.

| Project | What | Built With | Time | Link |
|---------|------|-----------|------|------|
| [Rybbit](https://rybbit.io) | Google Analytics alternative | Next.js + ClickHouse | ~2 weeks | [GitHub](https://github.com/rybbit-io/rybbit) |
| [OpenStatus](https://openstatus.dev) | Uptime monitoring | Next.js + Turso | ~1 week | [GitHub](https://github.com/openstatusHQ/openstatus) |
| [Dub.co](https://dub.co) | Link management | Next.js + PlanetScale | Ongoing | [GitHub](https://github.com/dubinc/dub) |
| [Cal.com](https://cal.com) | Scheduling | Next.js + Prisma | Ongoing | [GitHub](https://github.com/calcom/cal.com) |
| [OpenLoom](https://github.com/DukeDeSouth/OpenLoom) | Self-hosted Loom alternative | Next.js + ffmpeg + Whisper | ~1 week | [GitHub](https://github.com/DukeDeSouth/OpenLoom) |
| [portwatch](https://github.com/DukeDeSouth/portwatch) | Port & process viewer with risk assessment | TypeScript + Ink | ~1 day | [npm](https://www.npmjs.com/package/portwatch) |
| [vps-harden](https://github.com/DukeDeSouth/vps-harden) | VPS hardening wizard — SSH, firewall, fail2ban | TypeScript + node-ssh | ~1 day | [npm](https://www.npmjs.com/package/vps-harden) |

> **Submit your project!** Built something with vibecoding? [Open a PR.](CONTRIBUTING.md)

---

## Learning

| Resource | Format | Level |
|----------|--------|-------|
| [Vibe Coding with GitHub Copilot](https://docs.github.com/en/copilot/tutorials/vibe-coding) | Tutorial | Beginner |
| [Cursor Documentation](https://docs.cursor.com) | Docs | All |
| [Build with AI (YouTube)](https://www.youtube.com/@buildwithai) | Video | Beginner |
| [Vibecoding Workflow Guide](https://vibecoding.app/blog/vibe-coding-workflow-examples) | Blog | Intermediate |

## Communities

| Community | Platform | Focus |
|-----------|----------|-------|
| [r/vibecoding](https://reddit.com/r/vibecoding) | Reddit | General |
| [r/cursor](https://reddit.com/r/cursor) | Reddit | Cursor IDE |
| [Cursor Forum](https://forum.cursor.com) | Forum | Cursor IDE |
| [AI Coding Discord](https://discord.gg/ai-coding) | Discord | General |

---

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). PRs welcome — especially for:
- New tools with 100+ stars
- Real projects shipped with vibecoding
- Workflows and prompts that actually work

## License

[CC0 1.0](LICENSE) — Public Domain.
