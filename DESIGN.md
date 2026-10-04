# Intentional Computing — Design

> **Design technology around human intention, not technological compulsion.**

This document translates the philosophy of Intentional Computing into practical design guidance.

`MANIFESTO.md` defines **why**.

`PRINCIPLES.md` defines **what we believe**.

`ROADMAP.md` defines **where we are going**.

`DESIGN.md` defines **how things should be built**.

---

# 1. Design Philosophy

Intentional Computing is fundamentally a design discipline.

The central question is not:

> "What can the software do?"

It is:

> **"What is the person trying to accomplish, and how can the software help them accomplish it with the least unnecessary friction?"**

Technology should disappear into the task.

The user should think about:

> **what they want to do**

rather than:

> **how to operate the software.**

---

# 2. The Primary Design Loop

Every application should be designed around a simple loop:

```text
                    INTENTION
                        │
                        ▼
                     ACTION
                        │
                        ▼
                    RESULT
                        │
                        ▼
                    COMPLETION
                        │
                        ▼
                   REAL LIFE
```

Not:

```text
INTENTION
   ↓
ACTION
   ↓
RESULT
   ↓
RECOMMENDATION
   ↓
ANOTHER RECOMMENDATION
   ↓
ENGAGEMENT
   ↓
NOTIFICATION
   ↓
MORE CONTENT
   ↓
...
```

The first loop is the target.

The second is the anti-pattern.

---

# 3. Start With Intent

Every significant feature should begin by identifying the user's intention.

Examples:

```text
"I want to find a video about NES PPU programming."

"I want to edit this sprite."

"I want to understand this piece of code."

"I want to play this game."

"I want to research this subject."

"I want to organize these files."
```

The interface should then make the path from intention to result obvious.

---

# 4. One Primary Job

An application may eventually contain many capabilities.

But every screen should have a clear primary purpose.

Ask:

> **"What is the user here to do?"**

If the answer is unclear, the interface is probably doing too much.

A screen should not simultaneously compete for attention with:

* recommendations
* advertisements
* notifications
* unrelated statistics
* social activity
* trending content
* unrelated actions

The primary task gets priority.

---

# 5. The Three-Layer Interface

Where practical, applications should separate:

### 1. Intent

What the user wants.

### 2. Tools

What the software provides to accomplish it.

### 3. Information

What the system discovered or produced.

Conceptually:

```text
┌─────────────────────────────────────┐
│              INTENT                 │
│                                     │
│   Search / Create / Edit / Build    │
└──────────────────┬──────────────────┘
                   │
┌──────────────────▼──────────────────┐
│               TOOLS                 │
│                                     │
│   Actions required to accomplish    │
│   the task                          │
└──────────────────┬──────────────────┘
                   │
┌──────────────────▼──────────────────┐
│             INFORMATION             │
│                                     │
│   Results / files / output / data   │
└─────────────────────────────────────┘
```

Do not allow secondary information to overwhelm the primary intention.

---

# 6. Prefer Direct Manipulation

When a user can directly interact with something, prefer that over unnecessary abstraction.

Examples:

* drag a file
* click a tile
* paint a pixel
* move a sprite
* select a result
* edit a value
* rearrange a collection

Direct manipulation makes software understandable.

The interface becomes a representation of the task rather than a collection of unrelated controls.

---

# 7. Make State Visible

Users should understand the current state of the application.

Important state should be visible.

Examples:

```text
Unsaved changes
Search filters active
AI filtering enabled
Offline mode
Current tool
Current selection
Current file
Current project
Current playback state
```

Avoid hidden state whenever possible.

If something important affects the result, the user should be able to see it.

---

# 8. Make Actions Reversible

Prefer reversible operations.

Examples:

```text
Undo
Redo
Restore
Cancel
Revert
Reset
Export
Backup
```

When an operation cannot be reversed, make that fact clear before performing it.

A user should feel safe experimenting.

---

# 9. Progressive Complexity

Do not expose every capability simultaneously.

Start simple.

Reveal complexity when it becomes useful.

```text
Simple
  │
  ▼
Useful
  │
  ▼
Advanced
  │
  ▼
Expert
```

An expert should have access to powerful features.

A new user should not have to understand them.

---

# 10. Configuration Over Hidden Behavior

If behavior matters, expose configuration.

For example:

```text
Video filtering:
    Influencers        [blocked]
    Shock content      [blocked]
    Educational        [allowed]
    Gaming             [allowed]
```

is preferable to:

```text
Some invisible algorithm decides.
```

The user should understand the rules governing their environment.

---

# 11. Defaults Should Be Intentional

Defaults are design decisions.

They should favor:

* simplicity
* privacy
* low interruption
* local operation
* sensible security
* reversibility
* user control

Never choose a default primarily because it increases engagement.

---

# 12. Finite Interfaces

Where practical, interfaces should have natural boundaries.

Examples:

```text
10 search results
20 files
one project
one document
one task
one playlist
```

Finite interfaces create comprehension.

Infinite interfaces create continuation.

When more information is useful, provide an explicit action:

> **Load More**

rather than silently extending the world forever.

---

# 13. Stopping Points

Every major workflow should have an obvious stopping point.

Examples:

```text
Search complete.
File saved.
Export complete.
Download complete.
Queue empty.
Task complete.
```

Do not automatically replace completion with another engagement opportunity.

Completion should feel complete.

---

# 14. Navigation

Navigation should represent the user's mental model.

Prefer structures such as:

```text
Home
Projects
Files
Search
Settings
```

rather than:

```text
Trending
Recommended
For You
Popular
Live
Discover
Suggested
More
More
More
```

Navigation is not an opportunity to expose more content.

It is a map of the application.

---

# 15. Search Design

Search should be a first-class capability.

A good search interface should provide:

* clear input
* useful filtering
* meaningful sorting
* predictable results
* visible query state
* finite results
* useful metadata
* clear empty states

Search results should help the user decide.

They should not merely generate another browsing experience.

---

# 16. Curation

When an information space is enormous, curation becomes more valuable than volume.

A curation system should:

1. understand the user's request
2. search relevant sources
3. filter unwanted material
4. rank useful results
5. explain important filtering decisions
6. present a manageable result set

Conceptually:

```text
                    HUGE WORLD
                        │
                        ▼
                      SEARCH
                        │
                        ▼
                     FILTER
                        │
                        ▼
                     CURATE
                        │
                        ▼
                  SMALL SELECTION
                        │
                        ▼
                       USER
```

The goal is not to hide the world.

The goal is to make the world manageable.

---

# 17. AI Interface Design

AI should generally be presented as a tool rather than an authority.

Prefer:

> "Here are the results I found."

> "These were filtered because..."

> "I can perform this action."

over:

> "Trust me."

AI output should remain actionable and inspectable.

Where practical, provide:

* source information
* confidence
* relevant metadata
* filtering criteria
* user override
* retry
* correction
* manual control

---

# 18. AI Should Not Become the Interface for Everything

AI is powerful, but direct controls still matter.

Users should not have to ask an AI to perform something that could be more easily accomplished directly.

For example:

A paintbrush should still be a paintbrush.

A file should still be draggable.

A volume control should still be a volume control.

AI should enhance interfaces rather than eliminate understandable interfaces unnecessarily.

---

# 19. Human Override

AI decisions should be overridable where practical.

For example:

```text
AI says:
    Reject

User:
    Allow this result
```

Or:

```text
AI says:
    Category = "Entertainment"

User:
    Reclassify as "Education"
```

The system should learn from explicit corrections where appropriate.

The human remains the final authority.

---

# 20. Local-First Architecture

Applications should be designed with a local-first mindset.

Where practical:

```text
                 USER
                   │
                   ▼
             LOCAL APPLICATION
                   │
          ┌────────┴────────┐
          │                 │
       LOCAL DATA       LOCAL AI
          │                 │
          └────────┬────────┘
                   │
             OPTIONAL NETWORK
```

The network should extend functionality rather than automatically define the application's existence.

---

# 21. Network Boundaries

When network access is required, make it explicit.

The application should distinguish between:

* local data
* remote data
* cached data
* temporary data
* user-generated data

Users should be able to understand what requires the network.

---

# 22. Offline Graceful Degradation

If the network disappears, the application should fail gracefully.

Prefer:

```text
Network unavailable.

Local functionality remains available.
```

over:

```text
Application unusable.
```

Offline support should be considered during architecture, not retrofitted later.

---

# 23. Data Ownership

User data should be treated as belonging to the user.

Applications should provide, where appropriate:

* export
* backup
* import
* migration
* documented formats
* predictable storage locations

Avoid deliberately making user data difficult to extract.

---

# 24. Files Are Valuable

A file is often a better ownership model than a database controlled entirely by an application.

Prefer:

```text
project/
    project.json
    assets/
    exports/
```

when appropriate.

This makes projects:

* inspectable
* portable
* backup-friendly
* version-control-friendly
* long-lived

---

# 25. Open Formats

Where practical, use:

* PNG
* JPEG
* WAV
* FLAC
* JSON
* CSV
* XML
* plain text
* Markdown
* other well-documented formats

Proprietary formats may be justified when they provide genuine capabilities.

But users should not be trapped unnecessarily.

---

# 26. Project Formats

When an application requires a custom project format, document it.

A project file should ideally contain enough information to reconstruct the work.

Avoid formats that are intentionally opaque.

The application should not be the only place where the meaning of a project exists.

---

# 27. Privacy by Architecture

Privacy should not depend entirely on a checkbox.

The architecture should minimize unnecessary data collection.

Prefer:

```text
Data stays local.
```

over:

```text
Data is uploaded and we promise not to misuse it.
```

When remote processing is necessary, make that boundary clear.

---

# 28. No Unnecessary Accounts

An account should only exist when there is a genuine reason for one.

A local application should not require an account simply to:

* open a file
* create a project
* use basic tools
* configure preferences
* access offline features

Identity should be a feature, not a prerequisite.

---

# 29. Notifications

Notifications should be:

* rare
* meaningful
* configurable
* actionable

Every notification should answer:

> **"Why does this need the user's attention right now?"**

If there is no good answer, do not send it.

---

# 30. No Dark Patterns

Avoid:

* misleading buttons
* disguised advertisements
* forced subscriptions
* artificial scarcity
* hidden cancellation
* manipulative wording
* guilt-based prompts
* confusing opt-outs
* deceptive defaults

The interface should tell the truth.

---

# 31. No Engagement Loops

Avoid design patterns whose primary purpose is keeping users inside the application.

Examples:

```text
Infinite scrolling
Autoplay
Streak pressure
Constant recommendations
Unread-count inflation
Artificial notifications
"Don't leave" prompts
```

A useful application does not need to manufacture reasons for continued use.

---

# 32. Visual Design

Interfaces should be:

* clear
* calm
* readable
* functional
* consistent
* visually hierarchical

Visual complexity should communicate information rather than create stimulation.

Prefer:

```text
Purpose
  ↓
Hierarchy
  ↓
Clarity
```

over:

```text
More color
More movement
More badges
More notifications
More visual noise
```

---

# 33. Motion

Animation should communicate state or improve understanding.

Avoid animation whose only purpose is stimulation.

Good:

* transition between views
* show an operation completing
* indicate progress
* demonstrate spatial relationships

Bad:

* constant movement
* decorative looping
* attention-grabbing effects
* animations designed to prevent disengagement

---

# 34. Sound

Sound should be similarly intentional.

Provide:

* mute
* volume control
* sensible defaults
* meaningful feedback

Do not use sound simply to demand attention.

---

# 35. Accessibility

Intentional software should be usable by as many people as practical.

Consider:

* keyboard navigation
* readable text
* contrast
* scalable interfaces
* screen readers where applicable
* reduced motion
* alternative input
* clear focus state

Accessibility increases agency.

---

# 36. Error Design

Errors should explain:

1. what happened
2. why it happened, if known
3. what the user can do next

Prefer:

```text
Could not open the ROM.

The file appears to be truncated.

Try restoring the original file or selecting another ROM.
```

over:

```text
Error 0x8004.
```

Errors are part of the interface.

---

# 37. Empty States

Empty states should be useful.

Instead of:

> Nothing here.

Prefer:

> No projects exist yet.

> Create your first project to begin.

The system should distinguish between:

* nothing exists
* nothing was found
* something failed
* something is loading
* something is intentionally filtered

---

# 38. Performance

Performance is part of user agency.

Slow software consumes time.

Prioritize:

* fast startup
* responsive interaction
* background processing
* caching
* incremental work
* cancellation
* visible progress

Never make the user wait without explaining what is happening.

---

# 39. Long Operations

For expensive tasks:

```text
Start
  ↓
Progress
  ↓
Result
```

Provide:

* progress indication
* cancellation
* partial results where practical
* error reporting
* ability to continue other work where possible

AI classification is a particularly important example.

Do not make a user wait for 1,000 operations when the first useful result is already available.

---

# 40. Architecture

Prefer architectures that are:

* modular
* testable
* understandable
* replaceable
* local-first
* dependency-conscious

Separate major concerns where useful:

```text
UI
 │
Application Logic
 │
Domain Logic
 │
Data / Storage
 │
External Services
```

Avoid unnecessary layers.

Architecture should follow actual complexity.

---

# 41. External Services

External APIs and services should be treated as dependencies rather than foundations whenever possible.

Design for:

* unavailable services
* rate limits
* API changes
* authentication failure
* network failure
* service shutdown

A project should not collapse completely because one external service disappears unless that dependency is genuinely fundamental.

---

# 42. Replaceability

Major components should be replaceable where practical.

Examples:

```text
AI Provider
    ↓
Provider Interface
    ↓
Ollama
OpenAI
Local Model
Other Model
```

or:

```text
Video Source
    ↓
Source Interface
    ↓
YouTube
PeerTube
Internet Archive
Other Source
```

This prevents a single provider from becoming the architecture.

---

# 43. Testing

Testing should focus on behavior that matters to users.

Prioritize:

* correctness
* data integrity
* compatibility
* filtering
* search
* import/export
* persistence
* failure behavior

Regression tests should protect previously working behavior.

---

# 44. Documentation

Every project should document:

* what it does
* why it exists
* how it works
* how to build it
* how to configure it
* where data lives
* how to back up data
* how to troubleshoot it
* how to contribute

Documentation is part of the software.

---

# 45. Development Environment

Development tools should follow the same philosophy as the software.

Prefer:

* simple builds
* reproducible environments
* documented commands
* minimal tooling
* understandable configuration

Avoid adding tooling solely because it is fashionable.

---

# 46. Repository Structure

A typical Intentional Computing project should aim for a structure that communicates its architecture.

For example:

```text
project/
│
├── README.md
├── ROADMAP.md
├── LICENSE
├── docs/
├── src/
├── tests/
├── examples/
└── assets/
```

Not every project needs exactly this structure.

The principle is:

> **A repository should explain itself.**

---

# 47. Configuration

Configuration should be:

* explicit
* documented
* versionable where appropriate
* portable
* easy to reset

Avoid scattering configuration across:

* hidden files
* undocumented environment variables
* application databases
* platform-specific locations

unless there is a strong reason.

---

# 48. Logging

Logs should help humans understand the system.

Useful logs explain:

```text
what happened
why it happened
how long it took
what failed
what the system did next
```

Avoid noisy logs that obscure meaningful information.

---

# 49. AI Logging

AI-powered applications should record useful decision metadata where appropriate.

For example:

```text
Input:
video metadata

Model:
local classifier

Decision:
reject

Category:
clickbait

Confidence:
0.94
```

This supports debugging and user trust without requiring exposure of private model internals.

---

# 50. Security

Intentional Computing does not mean sacrificing security for simplicity.

Use:

* secure defaults
* least privilege
* dependency updates
* input validation
* safe storage
* explicit permissions

Security should protect user ownership and agency.

---

# 51. Compatibility

Prefer interoperability where practical.

Applications should work with existing:

* files
* formats
* controllers
* displays
* operating systems
* APIs
* standards

Do not create incompatibility merely to force users into a particular ecosystem.

---

# 52. Preservation and Longevity

When building software intended to last:

Ask:

> **Could another developer understand this ten years from now?**

That means favoring:

* clear code
* documentation
* stable formats
* tests
* simple dependencies
* reproducible builds
* archived specifications

Longevity is an architectural property.

---

# 53. Design for Exit

Every major system should have an exit strategy.

Users should be able to:

* export their data
* save their projects
* disable AI
* disable network services
* uninstall cleanly
* migrate elsewhere

A product that makes leaving difficult is not fully user-controlled.

---

# 54. Design Review

Before a major feature is accepted, evaluate it against:

### Intention

What user problem does this solve?

### Necessity

Does it need to exist?

### Attention

Does it consume attention unnecessarily?

### Agency

Does it increase or reduce user control?

### Ownership

Does it affect data ownership?

### Privacy

Does it introduce unnecessary data collection?

### Complexity

Does it add architectural complexity?

### AI

Would AI actually improve this?

### Exit

Can the user disable or remove it?

### Longevity

Will this still make sense years from now?

---

# 55. The Intentional Computing Scorecard

A feature can be informally evaluated:

| Dimension    | Question                                      |
| ------------ | --------------------------------------------- |
| Agency       | Does the user remain in control?              |
| Attention    | Does it avoid unnecessary interruption?       |
| Capability   | Does it make the user more capable?           |
| Ownership    | Does the user retain their work/data?         |
| Privacy      | Is unnecessary collection avoided?            |
| Simplicity   | Is the implementation justified?              |
| Transparency | Can the user understand it?                   |
| Portability  | Can the user leave with their work?           |
| Longevity    | Can the feature survive technological change? |
| Exit         | Can the user stop using it?                   |

A feature does not need a numerical score.

The purpose is to force deliberate design discussion.

---

# 56. Anti-Patterns

The following should trigger review:

### Infinite Feed

> "There is always more."

### Engagement Notification

> "Come back because we need you."

### Recommendation Loop

> "You finished this, so here is another thing."

### Account Wall

> "Create an account before you can use a local tool."

### Cloud Dependency

> "Your local data cannot function without our server."

### AI Authority

> "The AI decided, therefore the user must accept it."

### Hidden Automation

> "The software changed something without making it clear."

### Lock-In

> "You can use your data only inside our application."

### Complexity Creep

> "We added another framework because everyone uses it."

### Attention Decoration

> "The interface is moving because movement attracts attention."

These are not automatically forbidden.

They are **design-review triggers**.

---

# 57. The 90s Principle

Earlier personal computing provides useful design inspiration.

Not because old technology was inherently better.

But because many systems assumed:

> **The user owns the computer.**

Intentional Computing preserves that assumption while removing unnecessary historical limitations.

We want:

```text
1990s ownership
+
modern hardware
+
modern software
+
modern AI
+
modern networking
```

---

# 58. The Modern Principle

Modern technology should be used when it genuinely improves capability.

AI is welcome.

Cloud services are welcome.

High-speed networking is welcome.

Modern graphics are welcome.

Automation is welcome.

The question is never:

> "Is this modern?"

The question is:

> **"Does this improve the user's ability to accomplish something?"**

---

# 59. The Ultimate Interface

The ideal interface may eventually look surprisingly simple.

```text
                    WHAT DO YOU WANT TO DO?
                              │
          ┌───────────────────┼───────────────────┐
          │                   │                   │
        CREATE              FIND                DO
          │                   │                   │
          └───────────────────┼───────────────────┘
                              │
                              ▼
                           RESULT
                              │
                              ▼
                            DONE
```

Behind that simple interface may exist:

* sophisticated AI
* enormous databases
* powerful graphics
* complex networking
* advanced search
* emulation
* automation
* local processing

The complexity belongs in the system.

The human-facing experience should remain understandable.

---

# 60. Final Design Principle

The deepest design principle of Intentional Computing is:

> **Complexity should be absorbed by the machine wherever doing so gives the human more clarity, control, and capability.**

The computer can be extraordinarily sophisticated.

The user does not need to experience all of that complexity.

Technology should become:

**more powerful underneath**

while becoming:

**simpler and more intentional on the surface.**

The end result should not be a weaker computer.

It should be a **more capable computer that asks less of the person using it.**

---

# Design Test

Before shipping, ask:

> **What is the user's intention?**

> **What is the shortest honest path to fulfilling it?**

> **What unnecessary attention does this feature demand?**

> **What control does the user retain?**

> **What data does the system own versus the user?**

> **What happens when the network disappears?**

> **What happens when the AI is wrong?**

> **What happens when the user wants to leave?**

> **Will this still make sense ten years from now?**

If the answers are good, the design is probably moving in the right direction.

> **Make the machine powerful.**
>
> **Make the interface calm.**
>
> **Make the system understandable.**
>
> **Give the user control.**
>
> **And let the user get back to life.**
