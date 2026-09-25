# Brian Mathew

**From the sales floor to building software.** Technical Support · IT Support · Help Desk · QA · New Jersey
(remote, hybrid, on-site or relocation · available to start right away).

For years my job was helping people with a problem, a budget and a deadline: first as appliances
department lead at Best Buy, then on the road with Uber. I got curious about how the tools I used
every day actually worked, so I taught myself to build them. Now I build, test and support real
software, and I'd love to bring both halves, the patience of customer-facing work and the know-how
to find and fix what's broken, to a team that makes things for people.

💼 [LinkedIn](https://linkedin.com/in/brian-mathew-66235556) · 📄 [Portfolio & résumé](https://bmath8.vercel.app)

---

### What I've built

| Project | What it is | Status |
|---|---|---|
| **[brian-os](https://github.com/bmath8/brian-os)** | A Windows automation platform I built: 32 scheduled Python jobs with health checks, self-recovery and phone alerts. Anything that sends, spends, deploys or deletes waits for my approval. | Built · being upgraded · **235 tests passing** |
| **Family Draft Desk** | A real-time draft room for a sixteen-team league across phones, tablets and laptops. Shared clock, reconnect-safe picks, and commissioner pause, undo and repair while the draft is live. | **[Open the public test room ↗](https://family-draft-desk.vercel.app/?demo=1)** · no account · **142 tests passing** |
| **Warranty Tracker** | Add a purchase and see how long the warranty has left, with anything close to expiring flagged first. No account, no server, works offline. | **[Live, try it ↗](https://warranty-tracker-azure.vercel.app)** |
| **[boombox](https://github.com/bmath8/boombox)** | Listen-together music prototype. Room history lives in Postgres; live traffic runs over WebSockets and Redis. | Prototype · Jest/RTL |
| **[fam-super-bowl-squares-2026](https://github.com/bmath8/fam-super-bowl-squares-2026)** | A real-time squares pool that real people used during Super Bowl LX. | **[Live ↗](https://fam-super-bowl-squares-2026.vercel.app)** |

### How I troubleshoot

A watchdog in brian-os failed *silently*: it was alive but had stopped watching, and every
dashboard still read green. I traced it through the logs to a call with no timeout, fixed it, made
the watchdog report its own heartbeat, and wrote a test that freezes it on purpose and checks the
failure is caught within one interval. Every bug I fix gets a test so it can't come back.

### Working with

**Support:** troubleshooting · root-cause analysis · help desk · customer service · documentation<br>
**Systems:** `Windows` · `PowerShell` · monitoring · log analysis<br>
**Testing:** `pytest` · `node:test` · `Jest/RTL` · `Playwright` · regression testing<br>
**Build:** `Python` · `JavaScript` · `TypeScript` · `SQL` · `React` / `Next.js` · `Node.js` · `Postgres/Supabase` · `Docker`

<sub>Every number here is checkable: the test counts come from real <code>pytest</code> and <code>node:test</code> runs.</sub>
