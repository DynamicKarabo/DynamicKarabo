# My AI-Assisted Development Workflow

> A 5-layer system for building applications efficiently without writing code yourself.
> Built through trial and error. Optimised for token efficiency, context persistence, and clean output.

---

## The Core Philosophy

Most people one-shot projects — paste a vague idea into an LLM and hope for the best.
This workflow treats LLMs as **mechanical execution tools**, not oracles.
Each layer has one job. Nothing overlaps. The system compounds over time.

---

## The Stack

| Layer | Tool | Job |
|-------|------|-----|
| 1 | Claude | Architecture & planning |
| 2 | NotebookLM | Persistent project brain |
| 3 | MATHA | Context bridge & session memory |
| 4 | DeepSeek V3.2 / MiMo V2 Flash | Code writing |
| 5 | Cursor | Environment — run, test, git |

---

## Layer 1 — Claude (Architecture)

**When:** Once per project, or at the start of every major feature.

**What happens here:**
- Define the system architecture
- Plan the tech stack
- Think through business logic, edge cases, and constraints
- Identify what the system must and must not do

**Output:** A structured architecture document — the source of truth for everything downstream.

**Key rule:** This is the thinking layer. Claude does the heavy reasoning here so no other layer has to.

---

## Layer 2 — NotebookLM (The Brain)

**When:** After architecture is defined. Active throughout the entire project.

**What happens here:**
- Upload the architecture document
- Have deep conversations about the system to internalise the logic
- Draft structured prompts for the coding layer using this template:

```
TASK:        [What needs to be built — 2-3 sentences max]
STACK:       [Relevant technologies and frameworks]
CONSTRAINTS: [What not to do / patterns to follow]
CONTEXT:     [Only what's directly relevant to this task]
DONE WHEN:   [Clear, specific acceptance criteria]
```

**Output:** A structured, prescriptive prompt — not too long, not too short. No ambiguity for the LLM to fill in itself.

**Key rule:** NotebookLM holds the project context so the coding LLM doesn't have to reason about it. The reasoning has already been done here.

---

## Layer 3 — MATHA (Context Bridge)

**When:** Before and after every coding session.

**What happens here:**

MATHA is a local MCP server that gives the coding LLM persistent project memory across sessions.

### Before every session — `matha before`

Runs **Eight Gates** before any code is written:

| Gate | Purpose |
|------|---------|
| 01 UNDERSTAND | Why does this change exist? |
| 02 BOUND | What are the non-negotiable rules? |
| 03 ORIENT | What exists? What is stable, frozen, volatile? |
| 04 SURFACE DANGER | Any prior failures in this area? |
| 05 CONTRACT | What must be true after? Written before code. |
| 06 COST CHECK | What model tier? What token budget? |
| 07 BUILD | AI is now allowed to generate code. |
| 08 WRITE BACK | What was learned? Captured. Never lost. |

> Gate 07 does not open until Gates 01–05 are complete.

Produces a **session brief** — copy-paste ready, structured, warm with prior context.

### After every session — `matha after`

- Captures what was learned
- Records any corrections or assumption changes
- Updates the brain so the next session starts with full context
- Every correction is captured once — never explained twice

### Installation

```bash
npm install -g @10kdevs/matha
matha init
matha init --from requirements.md   # if you have an existing spec doc
```

### Auto-wiring (set once, works forever)

Add this rule to your IDE's AI settings:

```
At the start of every conversation, call matha_brief() before writing any code.
Review all rules, danger zones, and prior decisions.
Flag any hasCritical:true results before proceeding.
After completing work, call matha_record_decision() for any assumption
that changed during the session.
```

**Output:** A structured, context-rich session brief that feeds directly into the coding layer.

**Key rule:** MATHA closes the gap between NotebookLM's spec and the coding LLM's context. The brain never resets.

---

## Layer 4 — DeepSeek V3.2 / MiMo V2 Flash (Code Writer)

**When:** During active coding sessions, fed by MATHA's session brief.

**What happens here:**
- Receives a structured brief — not an essay, not a vague one-liner
- Implements code based on clear, prescriptive instructions
- Operates in **chat mode** (not reasoner) — the reasoning was done upstream
- Only switches to reasoner mode when debugging complex or unexpected failures

**Models:**

| Model | Use case | Cost (per 1M output) |
|-------|----------|----------------------|
| DeepSeek V3.2 chat | Primary code writer | R7.07 |
| MiMo V2 Flash | Alternative — faster, cheaper, strong on SWE-bench | R5.04 |

**Key rule:** This layer is purely mechanical execution. The spec is clear, the context is loaded, the LLM just writes. No gap-filling. No hallucinating business logic.

---

## Layer 5 — Cursor (Environment)

**When:** After code is generated.

**What happens here:**
- Paste and run generated code
- Test functionality
- Handle git commits and version control
- Minor terminal and git fixes only — no AI-assisted coding here

**Key rule:** Cursor is the environment, not the brain. AI stays out of this layer except for small, isolated fixes.

---

## The Full Flow

```
Claude
  └── Architecture doc
        └── NotebookLM
              └── Structured prompt (TASK / STACK / CONSTRAINTS / CONTEXT / DONE WHEN)
                    └── MATHA before
                          └── Session brief (danger zones + decisions + contracts)
                                └── DeepSeek / MiMo (chat mode)
                                      └── Clean code output
                                            └── Cursor (run + test + git)
                                                  └── MATHA after
                                                        └── Brain updated for next session
```

---

## Why This Works

**Token efficiency** — Each LLM only sees what's relevant to its job. No wasted context, no hitting limits mid-project.

**No gap-filling** — The structured prompt format means the coding LLM receives unambiguous instructions. It doesn't need to make assumptions.

**Compounds over time** — MATHA's write-back means every session is warmer than the last. By session 20, the coding LLM is operating with weeks of accumulated project knowledge.

**Cost control** — Chat mode over reasoner mode. The reasoning happens upstream in Claude and NotebookLM. DeepSeek/MiMo only executes — no reasoning tokens wasted.

**Separation of concerns** — If something breaks, you know exactly which layer failed. Architecture wrong? Layer 1. Spec unclear? Layer 2. Context missing? Layer 3. Bad code? Layer 4.

---

## Budget Reference (ZAR)

*Based on $1 = R16.82*

| Model | Input /1M | Output /1M | Best for |
|-------|-----------|------------|----------|
| DeepSeek V3.2 chat | R4.71 | R7.07 | Primary — proven, reliable |
| MiMo V2 Flash | R1.68 | R5.04 | Trial — cheaper, strong coding benchmarks |


---

*Built through months of trial and error. The frustration was the curriculum.*
