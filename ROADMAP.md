# Intentional Computing — Roadmap

> **Build powerful technology. Keep the human in control.**

This roadmap defines the long-term direction of the Intentional Computing project.

It is not a roadmap for a single application.

It is the roadmap for an ecosystem of software, tools, practices, and ideas built around the principles defined in:

* [`MANIFESTO.md`](MANIFESTO.md)
* [`PRINCIPLES.md`](PRINCIPLES.md)

The goal is to develop a practical alternative to the attention-driven computing model without rejecting modern technology.

---

# 1. Vision

Intentional Computing aims to demonstrate that modern technology can be:

* powerful without being addictive
* intelligent without being manipulative
* connected without being dependent
* personalized without exploiting the user
* modern without abandoning useful ideas from earlier computing
* automated without removing human agency
* capable without demanding constant attention

The long-term goal is a computing environment where:

> **The user decides what technology does, when it does it, and when it stops.**

---

# 2. The Core Direction

The project can be summarized as:

```text
                    INTENTIONAL COMPUTING
                            │
             ┌──────────────┼──────────────┐
             │              │              │
        PERSONAL        INTENTIONAL       AI
        COMPUTING       INTERNET        ASSISTANCE
             │              │              │
             └──────────────┼──────────────┘
                            │
                     HUMAN AGENCY
                            │
             ┌──────────────┼──────────────┐
             │              │              │
          OWNERSHIP       PRIVACY       ATTENTION
             │              │              │
             └──────────────┼──────────────┘
                            │
                    USEFUL SOFTWARE
```

---

# 3. Guiding Objective

Every project should ultimately help answer one question:

> **Can modern technology make an individual more capable without demanding more of their attention than necessary?**

A project does not need to satisfy every principle perfectly.

But intentional trade-offs should be documented.

---

# 4. Phase 0 — Foundation

**Status: IN PROGRESS**

Establish the philosophy and common language for the project.

### Documentation

* [x] Create `MANIFESTO.md`
* [x] Create `PRINCIPLES.md`
* [x] Create `README.md`
* [x] Create `DESIGN.md`
* [x] Create `PROJECTS.md`
* [x] Create `ROADMAP.md`
* [ ] Create contribution guidelines
* [ ] Define project terminology
* [ ] Define licensing strategy
* [ ] Define repository conventions

### Philosophy

* [x] Define human agency as a core principle
* [x] Define attention protection
* [x] Define completion over engagement
* [x] Define ownership and portability
* [x] Define local-first principles
* [x] Define intentional AI usage
* [x] Define the relationship with older computing
* [ ] Define an explicit "Intentional Computing Test"
* [ ] Define anti-patterns
* [ ] Define acceptable compromises

### Outcome

A new project should be able to read this repository and understand:

> **Why are we building this?**

---

# 5. Phase 1 — Demonstration Projects

**Status: IN PROGRESS**

The philosophy needs practical demonstrations.

The existing projects become early examples of Intentional Computing.

---

## 5.1 NoBSTube

### Objective

Create a personal video discovery environment that separates useful video information from the attention economy.

### Principles demonstrated

* search over feeds
* user-defined filtering
* AI-assisted curation
* finite results
* no engagement optimization
* local control
* user-defined exclusions

### Roadmap

* [x] Local self-hosted architecture
* [x] Multi-source search
* [x] AI classification
* [x] User-defined filtering
* [x] Multiple video sources
* [x] Sorting
* [x] Pagination
* [ ] Improve classification speed
* [ ] Stream useful results before full classification
* [ ] Improve caching
* [ ] Improve playback support
* [ ] Improve offline/local behavior
* [ ] Create explicit intentional-discovery mode
* [ ] Add configurable information diet
* [ ] Document architecture as an Intentional Computing example

### Desired outcome

A person should be able to say:

> "I want to find something interesting."

and receive a small, useful selection rather than entering an infinite feed.

---

# 6. Phase 2 — Intentional Creative Software

**Status: IN PROGRESS**

Build software that helps people create without surrounding the creative process with unnecessary distraction.

---

## 6.1 Mirage

### Objective

Create a lightweight pixel-art editor inspired by the strengths of established tools while maintaining an intentionally simple architecture.

### Principles demonstrated

* tool-first software
* local files
* ownership
* open formats
* no account requirement
* no social layer
* no advertising
* no attention economy

### Roadmap

* [x] Define Java/JavaFX architecture
* [x] Move toward Maven build system
* [x] Canvas
* [x] Pixel editing
* [x] Palette
* [ ] Layers
* [ ] Animation
* [ ] Selection
* [ ] Import/export
* [ ] Sprite-sheet tools
* [ ] NES-specific workflows
* [ ] SNES-specific workflows
* [x] Open project format
* [ ] Documentation
* [x] Offline-first operation

### Desired outcome

A creative tool that opens, lets the user make something, saves it, and gets out of the way.

---

# 7. Phase 3 — Computing Preservation

**Status: IN PROGRESS**

Preservation is a central component of Intentional Computing.

Old systems should remain understandable and usable.

---

## 7.1 NES Emulation

### Objective

Build accurate, understandable, maintainable emulation software.

### Roadmap

* [x] Mapper 0 foundation
* [x] CPU implementation
* [x] PPU implementation
* [x] Input
* [x] ROM loading
* [x] Basic game compatibility
* [x] Expand mapper support
* [x] Improve accuracy
* [x] Improve debugging
* [x] Improve tooling
* [x] Automated test ROM suite
* [ ] Documentation
* [ ] Preservation tooling

---

## 7.2 SNES Emulation

### Objective

Apply lessons from the NES project to a larger, more complex system.

### Roadmap

* [ ] Project initialization
* [ ] Documentation
* [ ] Roadmap
* [ ] CPU architecture
* [ ] Memory system
* [ ] PPU architecture
* [ ] DMA
* [ ] Input
* [ ] Audio architecture
* [ ] Cartridge system
* [ ] Initial ROM support
* [ ] Testing framework
* [ ] Debugger
* [ ] Accuracy work

### Desired outcome

A technically understandable emulator rather than a black box.

---

## 7.3 Atari 2600

### Objective

Continue preservation work across early console architectures.

### Roadmap

* [x] Basic emulator foundation
* [x] Improve CPU compatibility
* [x] Improve TIA accuracy
* [x] Improve timing
* [x] Improve cartridge compatibility
* [ ] Game compatibility testing
* [ ] Debugging tools
* [ ] Automated regression testing

---

# 8. Phase 4 — Personal Internet

**Status: PLANNED**

The long-term vision extends beyond individual applications.

We should explore what a **personal internet environment** could look like.

The objective is not to replace the internet.

It is to create a layer between the individual and the internet.

```text
                    INTERNET
                       │
            ┌──────────┴──────────┐
            │                     │
        AI / SEARCH          LOCAL SOURCES
            │                     │
            └──────────┬──────────┘
                       │
                  USER RULES
                       │
                PERSONAL FILTER
                       │
                       ▼
              PERSONAL INTERNET
                       │
                       ▼
                    HUMAN
```

---

## 8.1 Personal Information Layer

Explore software that lets a person define:

* subjects of interest
* sources they trust
* sources they reject
* content categories they avoid
* preferred formats
* desired information frequency
* acceptable notifications
* preferred AI behavior

### Goals

* [ ] Define personal information model
* [ ] Define source trust model
* [ ] Define filtering rules
* [ ] Define content classification
* [ ] Define AI summarization
* [ ] Define finite information delivery
* [ ] Define personal knowledge storage

---

# 9. Phase 5 — Intentional AI

**Status: PLANNED**

AI should become a general-purpose layer for intentional computing.

Rather than having dozens of services each competing for attention, a personal AI layer could act as a controlled interface to them.

---

## 9.1 Personal AI Assistant

### Objective

Create an AI system whose primary objective is:

> **Help the user accomplish things.**

Not:

> Maximize engagement.

### Capabilities

* search
* research
* summarization
* programming
* file organization
* media discovery
* local automation
* knowledge management
* software assistance
* personal workflows

### Principles

* user-configurable
* transparent
* local where practical
* privacy-conscious
* interruptible
* non-manipulative
* task-oriented

---

# 10. Phase 6 — Intentional Desktop

**Status: FUTURE**

Eventually explore whether these ideas can be expressed at the desktop level.

The objective would not necessarily be to create another operating system.

It could instead be a software environment layered over existing operating systems.

---

## Desired characteristics

### The desktop should:

* show what the user needs
* hide unnecessary noise
* minimize notifications
* make files accessible
* make applications easy to understand
* provide clear control over background activity
* support local workflows
* provide strong search
* provide AI assistance
* preserve user ownership

### The desktop should not:

* contain infinite feeds
* aggressively recommend content
* constantly notify the user
* require an account for basic functionality
* make cloud dependence unavoidable
* optimize itself around engagement

---

# 11. Phase 7 — Intentional Device

**Status: FUTURE**

Explore dedicated hardware for people who want an intentionally constrained computing environment.

Possible examples:

* offline gaming systems
* creative workstations
* personal media devices
* educational computers
* local AI machines
* focused writing machines

The philosophy:

> **The device exists to do a job.**

Not:

> **The device exists to keep you using it.**

---

# 12. Phase 8 — Personal Information Architecture

**Status: FUTURE**

Explore a personal information system that combines:

* files
* bookmarks
* notes
* saved webpages
* documents
* media
* software
* personal knowledge
* AI indexing

The system should make a person's own information easier to navigate without requiring a cloud platform to own it.

### Goals

* [ ] Local index
* [ ] Full-text search
* [ ] Metadata
* [ ] AI-assisted organization
* [ ] Semantic search
* [ ] Portable database
* [ ] Export
* [ ] Backup
* [ ] Offline operation

---

# 13. Phase 9 — The Personal Internet Bubble

**Status: LONG TERM**

The ultimate concept is a personal computing environment in which the individual defines the boundaries of their digital world.

The outside internet remains available.

But it is not automatically allowed inside.

```text
                 THE OPEN INTERNET
                         │
              ┌──────────┴──────────┐
              │                     │
           SEARCH                 SOURCES
              │                     │
              └──────────┬──────────┘
                         │
                  PERSONAL RULES
                         │
              ┌──────────┴──────────┐
              │                     │
           AI FILTER             USER FILTER
              │                     │
              └──────────┬──────────┘
                         │
                  PERSONAL BUBBLE
                         │
                  ┌──────┴──────┐
                  │             │
               KNOWLEDGE      MEDIA
                  │             │
                  └──────┬──────┘
                         │
                       USER
```

The bubble is not a prison.

The user can always leave it.

The purpose is simply to establish:

> **A boundary between the entire internet and the portion of it that a person actually wants in their life.**

---

# 14. Phase 10 — Intentional Computing Standard

**Status: LONG TERM**

If the ecosystem becomes mature enough, develop a formal standard for evaluating software.

Potential criteria:

### Agency

Does the user control the system?

### Attention

Does the system unnecessarily consume attention?

### Ownership

Can users retain their data and work?

### Privacy

Does the system collect only what is necessary?

### Transparency

Can users understand important system behavior?

### Portability

Can users leave without losing their work?

### Longevity

Can the system remain useful if dependencies or services disappear?

### AI Responsibility

Does AI serve the user's objectives?

### Exit

Can the user stop using the system easily?

---

# 15. Repository Ecosystem

As the project grows, individual repositories should remain independent.

The Intentional Computing repository acts as the **philosophical and architectural umbrella**.

```text
intentional-computing/
│
├── philosophy
│
├── standards
│
└── projects
        │
        ├── nobstube
        ├── pixelforge
        ├── rust-nes-emu
        ├── rust-snes-emu
        ├── rust-atari2600-emu
        ├── nes-sprite-tools
        └── intentional-devices
```

Individual projects should link back to this repository.

The umbrella repository should not absorb every project into one giant codebase.

**Separate implementation. Shared philosophy.**

---

# 16. Development Rules

Every new project should begin with:

* [ ] Problem definition
* [ ] User goal
* [ ] Intentional Computing principles involved
* [ ] Architecture
* [ ] Data ownership model
* [ ] Offline/local strategy
* [ ] AI usage policy, if applicable
* [ ] Privacy considerations
* [ ] Exit/export strategy
* [ ] Initial roadmap

Before adding major features:

* [ ] Does it improve capability?
* [ ] Does it increase unnecessary attention?
* [ ] Does it create lock-in?
* [ ] Does it introduce unnecessary complexity?
* [ ] Does AI genuinely improve the experience?
* [ ] Does the user retain control?

---

# 17. What We Explicitly Do Not Optimize For

Intentional Computing projects should generally not optimize primarily for:

* daily active users
* session length
* screen time
* notification response
* infinite consumption
* advertising impressions
* viral growth
* dependency
* lock-in
* behavioral manipulation

Growth may be useful.

Popularity may be useful.

Revenue may be necessary.

But they are not the fundamental definition of success.

---

# 18. What We Optimize For

We optimize for:

* usefulness
* capability
* clarity
* autonomy
* ownership
* reliability
* longevity
* privacy
* simplicity
* creativity
* learning
* preservation
* intentionality

The ultimate metric is:

> **Did this make the person's life better or their work more capable?**

---

# 19. Long-Term Vision

The project ultimately aims to demonstrate a different relationship between people and technology.

Not:

```text
PERSON
  ↓
PLATFORM
  ↓
ALGORITHM
  ↓
ATTENTION
  ↓
REVENUE
```

But:

```text
PERSON
  ↓
INTENTION
  ↓
TOOLS
  ↓
AI / COMPUTING
  ↓
CAPABILITY
  ↓
REAL LIFE
```

The computer should be the instrument.

The person should remain the musician.

---

# 20. Final Destination

There may never be a point where Intentional Computing is "finished."

Technology will continue changing.

New platforms will appear.

New forms of AI will emerge.

New problems will arise.

The roadmap therefore has no fixed final product.

The enduring objective is:

> **Keep building better ways for people to use increasingly powerful technology without surrendering control of their attention, data, environment, or lives.**

---

# Master Checklist

## Foundation

* [x] Manifesto
* [x] Principles
* [x] Roadmap
* [ ] README
* [ ] Design philosophy
* [ ] Project index
* [ ] Contribution guidelines

## Intentional Media

* [x] NoBSTube foundation
* [ ] Faster AI filtering
* [ ] Better discovery
* [ ] Personal information diet
* [ ] Intentional media environment

## Creative Tools

* [x] PixelForge foundation
* [ ] Pixel editor
* [ ] Animation
* [ ] Sprite tooling
* [ ] Open project format
* [ ] Offline-first workflow

## Preservation

* [x] NES emulator
* [x] Atari 2600 emulator
* [ ] SNES emulator
* [ ] Automated compatibility testing
* [ ] Preservation tooling
* [ ] Historical documentation

## Personal Internet

* [ ] Personal information layer
* [ ] Source filtering
* [ ] AI-assisted research
* [ ] Finite information delivery
* [ ] Personal knowledge system

## Intentional AI

* [ ] Personal AI architecture
* [ ] Local AI integration
* [ ] User-controlled AI rules
* [ ] AI transparency
* [ ] Task-oriented workflows

## Intentional Desktop

* [ ] Research
* [ ] Prototype
* [ ] Information architecture
* [ ] Notification system
* [ ] Personal AI integration
* [ ] Local-first architecture

## Intentional Devices

* [ ] Offline computing prototype
* [ ] Dedicated gaming device
* [ ] Focused creative device
* [ ] Local AI device

## Standards

* [ ] Intentional Computing Test
* [ ] Software design standard
* [ ] AI design standard
* [ ] Privacy standard
* [ ] Ownership standard
* [ ] Longevity standard

---

# The Direction

We are not trying to return to the past.

We are taking what was good about personal computing and combining it with what is good about modern technology.

**Old principle:**

> The computer belongs to you.

**Modern capability:**

> The computer can understand and assist you.

**Old principle:**

> You choose what software you use.

**Modern capability:**

> AI can help you navigate enormous software and information ecosystems.

**Old principle:**

> The internet is something you visit.

**Modern capability:**

> AI can make the entire internet searchable and manageable without requiring constant exposure to it.

The destination is neither the 1990s nor the current internet.

It is something new:

> **A future in which technology becomes dramatically more capable while becoming dramatically less demanding of the human being using it.**

That is the direction of Intentional Computing.
