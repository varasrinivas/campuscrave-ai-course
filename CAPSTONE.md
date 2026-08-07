# CAPSTONE — brief, rubric and grading guidance

Season 1's final assessment. The student builds **a small app of their own** and takes
it through all seven phases. It is graded on **evidence of how the work was done**, not
on whether the app is impressive.

This file is for whoever grades it. The student-facing brief lives in the player
(`index.html` → `renderCapstone()`), reachable from EP44's final CTA and from EP44's
Stretch, which tells students to open it and choose an idea.

---

## 1. The brief, in one paragraph

Pick something small and real — a thing you or somebody you know would actually use
once. Take it through **decide · design · spell it out · slice · build · check · ship
and run**. Keep the artifacts you have been keeping all season. Hand in the repository
*and* the evidence. Nobody planted the bugs this time; they are yours, which means the
reproduction step is the one that matters most.

### Scope guardrails (state these loudly — over-scoping is the #1 failure)
- **Smaller than CampusCrave.** One screen, one or two entities, one interesting rule.
- **One week of evenings**, not a term project.
- **₹0.** Same constraint as every lab in the season — free tiers, local running, hosting optional.
- **Any stack.** The course taught Spring Boot + React; the method is the assessed part.
- A student who ships less app and more evidence scores **higher** than the reverse.
  Say this before they start, or half of them will build a clone of something.

---

## 2. The one grading rule

Every dimension is scored on the same three levels:

| Level | Meaning |
|---|---|
| **Absent** | The artifact isn't there. |
| **Present** | The artifact exists and is accurate. |
| **Load-bearing** | The artifact **visibly changed a decision** — you can point at the thing that would otherwise have happened. |

**Only load-bearing scores full marks.** This is the whole rubric, and it comes straight
out of the season: EP13 asked *"did the answer change, or did you write documentation?"*,
EP41 said documentation goes quietly wrong when nothing depends on it, and EP37 said a
test that stays green when you break the code is a comment that takes eight seconds to run.

A beautifully formatted spec that never altered the build is **Present**, not
load-bearing. A scruffy three-line note that made somebody cut a feature is
**load-bearing**. Grade the influence, not the presentation.

---

## 3. The nine dimensions

Seven phases plus two cross-cutting. Equal weight; the two cross-cutting ones are not
bonus marks.

### D1 · Decide
**Assessed:** is there a problem statement naming a real person and a way to know it's solved?
**Evidence:** acceptance criteria; every number in them sourced (measured, decided by a named
person, or labelled `GUESS`).
- *Present:* criteria exist and are checkable.
- *Load-bearing:* at least one criterion **changed the scope** — something got cut, added or redefined because of it.
- *Weak signals:* "users want a better experience"; numbers with no owner (EP27's rule).

### D2 · Design
**Assessed:** were at least two designs considered?
**Evidence:** a four-line decision record — chose · rejected · why · **what would change our minds**.
- *Load-bearing:* the rejected option is described well enough that a reader could argue for it.
- *Weak signals:* one design plus a justification written afterwards. That's a rationalisation, and it reads like one.

### D3 · Spell it out
**Assessed:** is there a spec that is actually the source of truth?
**Evidence:** the spec, and its history.
- *Load-bearing:* the file's history shows it **changed before the behaviour did**, at least once (EP29's rule).
- *Weak signals:* a spec written after the code and never touched again.

### D4 · Slice
**Assessed:** was the work cut into pieces with finish lines?
**Evidence:** the slice list, each with a one-line done-test, ordered.
- *Load-bearing:* the ordering is **risk-first** and they can say what would have invalidated the rest (EP30).
- *Weak signals:* slices that are chapters of a plan rather than shippable pieces; any done-test containing "and".

### D5 · Build
**Assessed:** is the history legible and revertable?
**Evidence:** `git log`.
- *Load-bearing:* messages name **behaviour, not files**, and at least one change is revertable on its own (EP31, EP38).
- *Weak signals:* "fix stuff" ×n; one commit for everything.

### D6 · Check
**Assessed:** do the tests mean anything?
**Evidence:** the suite plus a **survivors list** — mutations tried, and which the tests failed to catch (EP37).
- *Load-bearing:* a mutation survived, and they **changed a test because of it**.
- *Weak signals:* coverage percentages; generated tests that assert current behaviour.

### D7 · Ship and run
**Assessed:** does it run somewhere that isn't only their editor?
**Evidence:** a build artifact **and** the configuration list — what it needs from outside the repo. Actual hosting is optional (₹0 constraint).
- *Load-bearing:* configuration is genuinely external — **no secrets in the repo**, and it fails loudly when a value is missing (EP40).
- *Weak signals:* a committed `.env`; "it works locally".

### D8 · Verification you can show
**Assessed:** can they prove something works rather than assert it?
**Evidence:** at least one **red → green** record (the failure observed, then absent), and at least one check **only a human could run**.
- *Load-bearing:* the red came first and is documented.
- *Weak signals:* screenshots of passing tests; "I tested it thoroughly".

### D9 · Honesty
**Assessed:** can they describe how the work was actually done?
**Evidence:** `ai-notes.md` kept **as they went**, the one-pager (delegate · never delegate · verify · worked example), and **one number they'd defend with its conditions attached** (EP43, EP44).
- *Load-bearing:* the notes record at least one place a tool was **wrong or unhelpful**, and what they did about it.
- *Weak signals:* a disclosure written the night before submission; "AI helped with some parts"; and equally, over-claiming — a tool credited with a decision the student made.

---

## 4. Grading guidance

- **Read the evidence before running the app.** The app biases you; that is the failure this rubric exists to correct.
- **Ask one live question per submission**, chosen from their own artifacts: *"why did you reject the other design?"*, *"which mutation survived?"*, *"what would change your mind about that number?"* A load-bearing artifact survives the question. A decorative one doesn't, instantly, and kindly.
- **Do not reward volume.** Forty generated tests, a forty-page spec and a forty-file repo are all signals to look harder, not to score higher (EP43: production was never the constraint).
- **A broken app with excellent evidence is a pass.** A polished app with no evidence is not. Say so in advance; it changes what students spend their week on, which is the entire point of grading process.

### Common failure modes seen in the season's own episodes
| Failure | Where the course already named it |
|---|---|
| Artifacts written afterwards to satisfy the rubric | EP29 — spec-after-code isn't a source of truth |
| Coverage as proof | EP37 — seven honest tests, eight live defects |
| A tidy history that hides the work | EP38 — squashing eleven commits into "Week 5 changes" |
| Confident numbers with no owner | EP27 — every number needs a human source |
| Concealment or over-claiming in disclosure | EP44 — checkpoint 4 of 4 |

---

## 5. What the student hands in

1. The repository (code + history).
2. **The evidence folder** — spec, decision records, slice list, survivors list, verification notes, postmortem if anything went wrong.
3. `ai-notes.md`.
4. The one-pager, ninety seconds spoken.
5. One number they would defend, with its conditions.

Five things. Four of them are not code, which is the message.
