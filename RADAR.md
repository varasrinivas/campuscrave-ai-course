# LANDSCAPE RADAR — appendix

**Checked: 5 August 2026.** Refresh this page per cohort; it is the only part of the
course designed to go out of date. Episode 3 teaches the *map*; this page holds the
*names*, precisely so that when the names move, nothing in the season has to be rewritten.

**Deliberately excluded:** prices, plan names, benchmark scores and rankings. Episode 3's
rule was *"not fandom, and not benchmarks"* and CLAUDE.md forbids printing pricing. Where a
free tier matters, this page says whether one exists for individuals — never the numbers,
which change faster than anything else here.

---

## Read this first — the errata that proves the point

CampusCrave Season 1 was written across about six weeks. In that time, **three of the seven
tools on its own radar changed name or ownership:**

| Was | Now | When |
|---|---|---|
| **Windsurf** (Codeium → Cognition) | rebranded **Devin Desktop** | 2 June 2026, by over-the-air update |
| **Gemini CLI** | transitioning to **Antigravity CLI**; free access for individual accounts stopped | 18 June 2026 |
| **Amazon Q Developer CLI** | renamed **Kiro CLI** | 2026 |

Nothing in the season broke, and that is the entire argument. The tool names live in
**Episode 3 only** — verified by grep — and **no lab in any of the 44 episodes depends on
any of these products**, so the course's ₹0 promise is unaffected. Episode 36's seven
transferable habits were unaffected too, because they were never about software.

If you teach this course and a student says "but Windsurf is called something else now" —
that is the lesson landing early. Show them this table.

---

## How to use these cards

- **Two tools deep, not six shallow** (Episode 3). These cards exist so you can hold a
  conversation about a tool you don't use — not so you can use it.
- The map that matters is still the one from Episode 3: **where it lives** (in the line ·
  in the editor · in the terminal · in the cloud) × **how much it does per ask**.
- Anything below marked *status* is the volatile part. The *what it's for* line is the
  part that has held.

---

## The cards

### Cursor
- **What it is:** a full editor built around AI, forked from VS Code.
- **Where it lives:** replaces your editor.
- **Good at:** agent work with the whole project in view; the most mature of the IDE-first tools.
- **Not:** portable — you adopt the editor, not just the assistant.
- **Status (Aug 2026):** independent, heavily funded, still the default recommendation for solo developers who want an IDE-native agent.

### Windsurf → **Devin Desktop**
- **What it is:** the IDE formerly known as Windsurf, now Cognition's desktop surface for its autonomous agent, Devin.
- **Where it lives:** replaces your editor; long-running agents run *inside* it rather than in a separate tab.
- **Good at:** handing work to an agent that keeps going, without leaving the editor.
- **Not:** the standalone product the season describes — the roadmap now follows Devin.
- **Status (Aug 2026):** acquired by Cognition (announced Dec 2025); **rebranded to Devin Desktop on 2 June 2026**. Expect the name "Windsurf" to disappear from documentation.

### Cline
- **What it is:** an open-source agent that runs as an extension inside your existing editor.
- **Where it lives:** alongside your setup — you keep your editor.
- **Good at:** transparency; you watch every step, and you bring your own model key.
- **Not:** a managed product with a support contract.
- **Status (Aug 2026):** actively developed, pushing frequently, free to install (you pay for whatever model you point it at). Supports local models.

### Codex (OpenAI)
- **What it is:** OpenAI's coding agent, most used as a CLI.
- **Where it lives:** terminal, and in CI.
- **Good at:** scripted and pipeline work — the terminal-first shape, like Claude Code.
- **Not:** an editor.
- **Status (Aug 2026):** active and widely deployed; commonly paired with an IDE tool rather than replacing one.

### Gemini CLI → **Antigravity CLI**
- **What it is:** Google's terminal coding agent.
- **Where it lives:** terminal.
- **Good at:** it was, for a year, the most generous free terminal agent available to a student.
- **Not:** that any more — **on 18 June 2026 it stopped serving individual free and consumer-tier accounts**; organisational licences kept access, and the product is being transitioned to **Antigravity CLI**.
- **Status (Aug 2026):** ⚠ **the single most important change for anyone teaching at ₹0.** If a previous cohort was pointed here for a free terminal agent, point the next one elsewhere and check the free options below before term starts.

### Aider
- **What it is:** the original open-source terminal pair-programmer.
- **Where it lives:** terminal.
- **Good at:** **git-native work** — it commits as it goes, with real messages, and its undo story is the best of the group. Episode 38 would approve.
- **Not:** the fastest-moving project in this list any more.
- **Status (Aug 2026):** still available and still free; development cadence has slowed relative to the newer agents. Supports local models.

### Kiro
- **What it is:** AWS's spec-first coding tool — you describe what you want, it produces a spec, then implements from it.
- **Where it lives:** its own IDE, plus a CLI.
- **Good at:** the workflow Episode 29 teaches. If you want students to *see* spec-driven development as a product rather than a discipline, this is the demo.
- **Not:** editor-agnostic.
- **Status (Aug 2026):** active; **the former Amazon Q Developer CLI is now Kiro CLI**, so older AWS documentation and tutorials use the old name. Free tier for individuals exists.

---

## New names since the season was shot

Listed without claims, deliberately — they will churn too. Mentioned only so nobody is
blindsided by a name in an interview: **Antigravity** (Google), **OpenCode**, **Goose**,
**Kilo Code**, **Zed**, **Grok Build**.

If you refresh this page, resist expanding this list into cards. Episode 3's "six tools,
three families" structure is what makes the landscape teachable; a list of eighteen is
just noise wearing a lanyard.

---

## Free options for a ₹0 cohort — check before term starts

The season promises every lab is completable at ₹0, and no lab depends on a specific
product. Still, verify the current state of these before teaching:

- **Free to install, bring your own model key:** Cline, Aider, Goose, OpenCode, Kilo Code.
  (Cost then depends on the model, and local models via Ollama or similar are an option
  for Cline and Aider.)
- **Free tiers attached to a product:** GitHub Copilot, Cursor, Kiro all offer one for
  individuals. Limits change constantly — check, don't assume, and never print the numbers
  in course material.
- **Chat surfaces** remain the reliable free path, which is why every Free path in this
  season is written to work with a chat box and a keyboard.

---

## What hasn't changed

Episode 36's seven, unaffected by every rename above: the four-part prompt · aiming the
context window · reading a plan before it acts · one job per window · reading the diff ·
proving red before green · one slice, one commit.

That list has now survived three product renames and one acquisition **during the writing
of the course that teaches it.** Say that to a cohort on day one.

---

## Refreshing this page

1. Re-check each card's **status** line only. The *what it's for* lines have been stable.
2. Search for renames and acquisitions first — that is what actually moves.
3. Do not add benchmark scores, rankings or prices. They date faster than the names and
   they teach nothing (Episode 3: *"not fandom, and not benchmarks"*).
4. Update the **checked** date at the top, and add any rename to the errata table rather
   than silently correcting it. The table is more useful than a clean page.

### Sources for the 5 August 2026 check
- [Cognition's acquisition of Windsurf — Cognition](https://cognition.com/blog/windsurf)
- [Windsurf Is Now Devin Desktop (June 2026) — AIToolTier](https://aitooltier.com/tools/windsurf)
- [CLI coding agents compared — hidekazu-konishi.com](https://hidekazu-konishi.com/entry/cli_coding_agents_comparison.html)
- [The 2026 Guide to Coding CLI Tools — Tembo](https://www.tembo.io/blog/coding-cli-tools-comparison)
- [AI Coding IDE Landscape, May 2026 — Digital Applied](https://www.digitalapplied.com/blog/ai-coding-ide-landscape-may-2026-10-tools)
- [Agentic CLI tools compared — AIMultiple](https://aimultiple.com/agentic-cli)
