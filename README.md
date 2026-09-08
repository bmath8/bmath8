# Brian Mathew

**I build working systems — then I keep them running.** New Jersey. Open to remote, hybrid,
on-site, or relocation, and available to start quickly.

Most of what I know came from operating my own software rather than only writing it. There are
28 scheduled agents executing on my machine right now; when one of them breaks at 3am, I'm the
one who finds out why. That's shaped how I build: test it, document it, put a guardrail in
front of anything destructive, and assume it will fail in a way I didn't predict.

📄 [Portfolio & resume](https://bmath8.vercel.app) · ✉️ [mathew.brian@gmail.com](mailto:mathew.brian@gmail.com) · 💼 [LinkedIn](https://linkedin.com/in/brian-mathew-66235556)

---

### What I've built

| Project | What it is | Status |
|---|---|---|
| **[brian-os](https://github.com/bmath8/brian-os)** | A fleet of 28 scheduled Python agents running unattended on Windows — daily briefs, health checks, self-recovery, two-way Telegram control. Anything that sends, spends, deploys or deletes is draft-only until I approve it. | Running daily · **226 tests passing** |
| **Family Draft Desk** | A real-time snake-draft room for a sixteen-team league across desktop, tablet and phone. Shared clock with reconnect-safe picks, private per-manager state kept out of public state, and commissioner pause, undo and cell repair — because a live draft can't be rolled back by redeploying. | **[Open the public test room ↗](https://family-draft-desk.vercel.app/?demo=1)** · no account · **143 tests passing** |
| **Warranty Tracker** | Local-first warranty and receipt tracker. Automatic expiry math, colour-coded urgency, search and sort, no account and no server. One self-contained HTML file, no build step, no dependencies. | **[Live — try it ↗](https://warranty-tracker-azure.vercel.app)** |
| **[boombox](https://github.com/bmath8/boombox)** | Collaborative music prototype — shared queues and synchronized listening. Durable Postgres state kept deliberately separate from transient WebSocket + Redis Pub/Sub. | Prototype, public source · Jest/RTL |
| **[fam-super-bowl-squares-2026](https://github.com/bmath8/fam-super-bowl-squares-2026)** | A real-time squares pool that real people used during Super Bowl LX. 100 squares, live draw, score-driven winner resolution. | **[Live — try it ↗](https://fam-super-bowl-squares-2026.vercel.app)** |
| **[portfolio](https://github.com/bmath8/portfolio)** | The source for bmath8.vercel.app. Self-hosted fonts, no third-party requests, WCAG AA, and it renders with JavaScript disabled. | **[Live ↗](https://bmath8.vercel.app)** |

### How I test

Testing is the part of this I'd point at first. Across the projects above there are **226**
passing `pytest` cases in brian-os, **143** in `node:test` in Family Draft Desk — unit,
integration, end-to-end and adversarial, including a full 240-pick draft asserted for legal
rosters and unique cells — and Jest/RTL suites in boombox.

Two of those tests exist because something broke. A watchdog in brian-os failed *silently*: it
was alive but had stopped watching, and every dashboard still read green. I traced it to a call
with no timeout, fixed it, and wrote the test that kills the guardian mid-cycle and asserts the
fleet notices within one interval.

I also maintain a verification gate that re-checks every number in my own documentation against
the live machine and **fails the build when the two drift** — which is why the counts above are
worth reading.

### Working with

`Python` · `SQL` · `TypeScript` · `React` / `Next.js` · `Node.js` · `PowerShell` · `Windows` · `pytest` · `Jest/RTL` · `node:test` · `Playwright` · `Docker` · `Postgres/Supabase` · local LLMs via `Ollama`

### What I'm looking for

A full-time role building, testing or supporting software — developer, QA / test automation,
technical support, or operations. Before I wrote software I spent years in customer-facing work
(appliances department lead at Best Buy, then a year driving independently for Uber), and I'd
rather be somewhere those two halves both count.

<sub>Every number on this profile is checkable. The test counts come from real <code>pytest</code> and <code>node:test</code> runs; the agent count comes from a real crontab.</sub>
