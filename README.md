# Brian Mathew

**From the sales floor to building software.** Customer Success · Support · IT · QA · New Jersey
(remote, hybrid, on-site or relocation · available to start right away).

I got my first job at 16, working concessions and as an usher at AMC Theatres. Grocery stores, clothing
stores and Best Buy followed, where I led the appliances department. The common thread was always people:
listening, handling rejection, and working out what someone actually needed.

That work made me curious about sales and marketing, and then about the tools themselves. AI gave me
a way to start turning ideas into things I could try, and I kept going until they worked properly.
Today that is two live apps anyone can open and a Windows automation system, backed by 460+ passing
tests.

I build around everyday problems and interests: tracking warranties, a family fantasy draft,
organizing a job search, listening to music with friends. I want what I build to make someone's day a
little easier. I'm looking for a team where I can bring the customer-facing experience and the
curiosity, do useful work, and keep growing technically.

💼 [LinkedIn](https://linkedin.com/in/brian-mathew-66235556) · 📄 [Portfolio & résumé](https://bmath8.vercel.app)

---

### What I've built

| Project | What it is | Status |
|---|---|---|
| **[brian-os](https://github.com/bmath8/brian-os)** | A Windows automation system I built: 30+ scheduled Python jobs with health checks, self-recovery and phone alerts. Anything that sends, spends, deploys or deletes waits for my approval. | Built · being upgraded · **235 tests passing** |
| **Family Draft Desk** | A real-time draft room for a sixteen-team league across phones, tablets and laptops. Shared clock, reconnect-safe picks, and commissioner pause, undo and repair while the draft is live. | **[Open the public test room ↗](https://family-draft-desk.vercel.app/?demo=1)** · no account · **142 tests passing** |
| **Warranty Tracker** | Add a purchase and see how long the warranty has left, with anything close to expiring flagged first. No account, no server, and no data leaves the device. | **[Live, try it ↗](https://warranty-tracker-azure.vercel.app)** |
| **[boombox](https://github.com/bmath8/boombox)** | Listen-together music prototype. Room history lives in Postgres; live traffic runs over WebSockets and Redis. | Prototype · Jest/RTL |
| **[fam-super-bowl-squares-2026](https://github.com/bmath8/fam-super-bowl-squares-2026)** | A real-time squares pool that ran a live event: a family pool during Super Bowl LX. | **[Live ↗](https://fam-super-bowl-squares-2026.vercel.app)** |

### How I troubleshoot

The process guardian in brian-os failed *silently*: it aborted on every run for days while its exit
codes still read success, and 160 orphaned processes built up until the disk was down to 0.4 GB
free. I traced it to a helper that used a name PowerShell reserves, renamed it, and gave the
guardian a heartbeat that the watchdog checks. Three tests went into the suite; one runs the real
guardian and fails on any error output
([the tests](https://github.com/bmath8/brian-os/blob/main/tests/test_powershell.py)).
Every bug I fix gets a test so it can't come back.

### Working with

**Support:** troubleshooting · root-cause analysis · help desk · customer service · documentation<br>
**Systems:** `Windows` · `PowerShell` · monitoring · log analysis<br>
**Testing:** `pytest` · `node:test` · `Jest/RTL` · `Playwright` · regression testing<br>
**Build:** `Python` · `JavaScript` · `TypeScript` · `SQL` · `React` / `Next.js` · `Node.js` · `Postgres/Supabase` · `Docker`

<sub>Every number here is checkable: the test counts come from real <code>pytest</code> and <code>node:test</code> runs.</sub>
