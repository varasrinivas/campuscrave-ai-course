# CampusCrave — Code With AI

**The student's guide to building software in the agent era.** A 44-episode course, plus
an orientation and a capstone, built around one small app and two real repositories.

## Start here

Get this repository onto your machine, then open **`index.html`** from your own disk:

```bash
git clone https://github.com/varasrinivas/campuscrave-ai-course
cd campuscrave-ai-course
```

Then double-click `index.html`, or open it with `File → Open` in any browser. That's the
whole player — one file, no build step, no install, nothing to run. It opens on Episode 0.

> **Don't try to watch it from the GitHub page.** Clicking `index.html` up there shows you
> the source code, not the course. It has to be a local file.

Everything in the player is inside that file — no build, no server, nothing fetched while
you read. The one exception is the typefaces, which come from Google Fonts: offline the
course works exactly the same and simply falls back to your system fonts.

## The two repositories

The course is not a tutorial with snippets. You work in two real codebases that ship in
their honest day-one state: the demo went great, and several things are quietly wrong.

```bash
git clone https://github.com/varasrinivas/campuscrave-api
git clone https://github.com/varasrinivas/campuscrave-web
```

**Clone them — a downloaded zip will not do.** Twenty-seven episodes read these
repositories' own history, starting with `git checkout day-1` in Episode 1.

Setup (Java 21, Node 20+, git, an editor, optionally a terminal agent) is Episode 0's
seven-item checklist. Do that first.

## What's in here

| File | What it is |
|---|---|
| `index.html` | The player — all 45 episodes and the capstone brief |
| `CAPSTONE.md` | The capstone brief and its grading rubric |
| `RADAR.md` | The tool landscape appendix — the only page designed to go out of date |

## How the course works

Every episode is four beats: a cold open that dramatises something real in the
repositories, the teach, a decision to make, and a lab. Every lab has three paths —
🟡 Claude Code, 🔵 GitHub Copilot, ⚪ free tier — and **every one of them is completable
at ₹0.** No lab depends on a paid tool.

Each lab ends with a **Verify** step that no AI can do for you. That is the point of the
course.

## A note on the bugs

The repositories contain planted defects. They are deliberate, they are documented in the
course, and they are solved on screen — but not in the episode you first meet them in.
Resist looking ahead; the discovery is the lesson, and Episode 32 exists to prove that a
bug you couldn't find on day one takes about twenty minutes by the end.

## Reading the radar

`RADAR.md` names current tools and is checked per cohort. Three of the seven tools on it
changed name or ownership during the six weeks the course was written — that errata table
is at the top of the file, and it is the course's own argument in miniature: learn the
map, not the street names.

## Licence / use

Ask before running this with a cohort you charge for.
