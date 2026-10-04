# Intentional Computing — Quick Rules

This is the compact engineering contract for the Intentional Computing project.

Use these rules when designing, implementing, reviewing, or modifying software in this ecosystem.

The full philosophy and standards live elsewhere in this repository. This file exists so they do not need to be loaded for every task.

---

## 1. Human Agency First

Software exists to help the user accomplish something they intended to accomplish.

* The user chooses the goal.
* The user controls important decisions.
* The user can override automation.
* Do not manipulate the user into additional interaction.
* Do not optimize for engagement when usefulness is the actual goal.

**Optimize for capability, not captivity.**

---

## 2. Completion Over Engagement

Prefer:

```text
INTENTION → ACTION → RESULT → COMPLETION → LIFE
```

over:

```text
INTENTION → ACTION → MORE CONTENT → MORE ENGAGEMENT → MORE ENGAGEMENT
```

Software should have natural stopping points.

Avoid unnecessary:

* infinite scrolling
* engagement loops
* artificial urgency
* notifications
* gamification
* autoplay
* FOMO
* recommendation loops

When the user's work is finished, let the software stop.

---

## 3. Search Over Feeds

When information is needed, prefer intentional retrieval over continuously presented content.

Prefer:

* search
* explicit navigation
* bookmarks
* archives
* user-selected sources
* finite result sets
* user-controlled sorting and filtering

Recommendations may exist when they genuinely help the user's stated goal, but they should not become the default mechanism for consuming information.

---

## 4. Curation Over Volume

More information is not automatically better.

Prefer:

```text
FILTER → CURATE → PRESENT
```

over:

```text
COLLECT EVERYTHING → PRESENT EVERYTHING
```

User-defined filters and preferences are first-class functionality.

AI may help filter, classify, summarize, rank, organize, or deduplicate information, but the user's values and rules take priority.

---

## 5. AI Is a Tool

AI should reduce complexity rather than manufacture dependency.

Use AI where it provides meaningful leverage:

* search
* classification
* filtering
* analysis
* organization
* explanation
* tedious transformation
* automation
* generation

Do not use AI merely because it is available.

Prefer deterministic logic when deterministic logic is sufficient.

AI must not silently take control of important user decisions.

Keep AI:

* bounded
* inspectable where practical
* replaceable
* configurable where useful
* reversible
* honest about uncertainty

**The goal is not to make the AI indispensable. The goal is to make the person more capable.**

---

## 6. Local First

Work locally whenever practical.

Prefer:

* local data
* local files
* offline capability
* local processing
* explicit synchronization
* transparent network boundaries

Network services should be an extension of the application rather than an unnecessary foundation.

Do not require an account or cloud service when the application does not genuinely need one.

---

## 7. Ownership

Users should retain practical control over their work and data.

Prefer:

* open or documented formats
* export
* backup
* migration
* inspectable files
* replaceable services
* minimal vendor lock-in

Do not make user-created work dependent on an opaque service unnecessarily.

A user should have a reasonable path to leave the software without losing their work.

---

## 8. Keep Software Understandable

Prefer simple, explicit, maintainable systems.

* Avoid unnecessary dependencies.
* Avoid unnecessary abstraction.
* Avoid cleverness when straightforward code works.
* Keep architecture visible.
* Separate responsibilities clearly.
* Prefer boring technology when it is sufficient.
* Document important non-obvious behavior.
* Make failure modes understandable.

**Complexity should be absorbed by the machine where doing so gives the human more clarity and capability — not where it merely hides complexity from developers.**

---

## 9. Intentional Defaults

Defaults should serve the user's interests.

Before adding a default, ask:

> Does this help the user accomplish their intended task?

Avoid defaults that primarily:

* increase engagement
* collect unnecessary data
* create dependency
* interrupt
* encourage compulsive use
* hide important behavior

Important behavior should be configurable and discoverable.

---

## 10. Visible State and Reversible Actions

Users should be able to understand what the software is doing.

Prefer:

* visible state
* clear feedback
* previews
* progress indicators for long operations
* cancellation
* undo
* reversible operations
* explicit modes and selections

Do not silently perform consequential actions when the user could reasonably expect control.

---

## 11. Respect Attention

Attention is a finite human resource.

Minimize unnecessary:

* interruptions
* context switching
* notifications
* cognitive load
* waiting
* repetitive work
* interface noise

Do not make the user repeatedly interact with software merely to keep the software active.

**The interface should become quiet when the task is complete.**

---

## 12. Create More Than Consume

Software should help people make things, understand things, solve problems, and accomplish goals.

Prefer creation, exploration, learning, and useful work over mechanisms designed primarily to maximize passive consumption.

---

## 13. Preserve the Good Parts of Computing

Modern capability is welcome.

Do not discard valuable qualities of earlier personal computing:

* ownership
* local files
* direct manipulation
* understandable software
* general-purpose tools
* user configuration
* offline operation
* finite interfaces
* personal control

The goal is not nostalgia.

**Preserve the good constraints while adding modern capability.**

---

## 14. No Artificial Restrictions

Intentional Computing does not mean making software artificially primitive.

Do not remove useful capability merely to make an interface "simple."

Instead:

> Put complexity where it belongs.

Advanced functionality may exist. Progressive disclosure can keep it out of the way until needed.

The user should be able to grow with the software.

---

## 15. Prefer Replaceability

Important components should have reasonable replacement paths.

Avoid unnecessary dependence on:

* a single provider
* a single AI model
* a single cloud service
* proprietary storage
* proprietary APIs
* unnecessary accounts

When an external service is necessary, isolate the dependency behind a clear boundary where practical.

---

## 16. Fail Gracefully

When something fails:

* explain what happened
* preserve the user's work
* preserve context
* provide a useful next step
* avoid pretending success
* avoid destructive recovery

If an optional service fails, the core application should continue working where reasonably possible.

---

## 17. Test the Human Outcome

Do not judge a feature only by whether the code works.

Ask:

1. Does it accomplish the intended task?
2. Does it reduce unnecessary effort?
3. Does it preserve user control?
4. Does it avoid unnecessary attention demands?
5. Does it preserve ownership?
6. Does it remain understandable?
7. Does it provide a stopping point?
8. Can the user undo or recover?
9. Can the user leave?

---

## 18. The Intentional Computing Test

Before accepting a significant feature, ask:

> **Does this increase human capability without unnecessarily demanding human attention?**

If yes, continue.

If no, determine whether the capability is genuinely necessary.

If the feature primarily exists to increase engagement, dependency, surveillance, or platform control, reconsider it.

---

## Priority Order

When principles conflict, use this general order:

```text
USER INTENT
    ↓
USER CONTROL
    ↓
CORRECTNESS / SAFETY
    ↓
USEFULNESS
    ↓
OWNERSHIP / PORTABILITY
    ↓
CLARITY / UNDERSTANDABILITY
    ↓
EFFICIENCY
    ↓
CONVENIENCE
```

Do not sacrifice fundamental user control merely for convenience.

---

## Development Loop

For meaningful changes:

```text
UNDERSTAND INTENT
      ↓
DEFINE BEHAVIOR
      ↓
IMPLEMENT
      ↓
TEST
      ↓
CHECK USER CONTROL
      ↓
CHECK ATTENTION COST
      ↓
CHECK OWNERSHIP / EXIT
      ↓
DOCUMENT
```

---

## Final Rule

Build technology that is:

**Powerful without being demanding.**

**Intelligent without being controlling.**

**Connected without being dependent.**

**Automated without removing agency.**

**Modern without abandoning ownership.**

**Complex internally, but clear externally.**

And when the user's work is finished:

**Let the software get out of the way.**
