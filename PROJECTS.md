# Intentional Computing — Projects

> Separate implementation. Shared philosophy.

This document describes the projects that make up the Intentional Computing ecosystem.

The projects are intentionally maintained as separate repositories. The purpose of this repository is to provide the **shared philosophy, principles, design language, and direction** that connects them.

A project does not need to implement every principle of Intentional Computing.

Instead, each project should demonstrate one or more principles particularly well.

---

# 1. Why These Projects Exist

Intentional Computing is not primarily a software product.

It is a way of building software.

The projects in this ecosystem explore what happens when modern technology is designed around:

* human agency
* local ownership
* finite interfaces
* deliberate discovery
* completion rather than engagement
* understandable systems
* AI as a tool
* offline capability
* preservation
* user-defined environments
* long-term maintainability

Each project answers a practical question.

For example:

> Can AI make the internet smaller and more useful instead of larger and more addictive?

That question becomes **NoBSTube**.

> Can modern software provide powerful creative tools without becoming dependent on a large ecosystem?

That becomes **Mirage**.

> Can old computers and games remain usable through software that respects the original hardware?

That becomes the emulator projects.

The projects are therefore experiments in intentional computing.

---

# 2. Project Ecosystem

```text
                         INTENTIONAL COMPUTING
                                  │
                    ┌─────────────┴─────────────┐
                    │                           │
              PHILOSOPHY                    PRACTICE
                    │                           │
                    │             ┌─────────────┼─────────────┐
                    │             │             │             │
                    │          DISCOVERY     CREATION    PRESERVATION
                    │             │             │             │
                    │          NoBSTube       Mirage       Emulators
                    │                                          │
                    │                               ┌──────────┼──────────┐
                    │                               │          │          │
                    │                              NES        SNES      Atari
                    │
                    └────────────────────────────────────────────────────┐
                                                                         │
                                                                    FUTURE
                                                                         │
                                      ┌──────────────────────────────────┼──────────────┐
                                      │                                  │              │
                                Personal Internet                   Intentional    Personal
                                                                    AI            Computing
                                                                                  Device
```

The ecosystem is expected to grow.

New projects should be added when they explore an important part of the philosophy—not simply because another application can be built.

---

# 3. NoBSTube

**Repository:** `nobstube`

## Purpose

NoBSTube is a local, self-hosted video discovery system designed as an alternative to conventional video platforms.

It exists to explore a simple question:

> What would video discovery look like if the goal were finding something useful rather than keeping the user watching?

Traditional video platforms optimize heavily around:

* engagement
* recommendations
* watch time
* subscriptions
* notifications
* trending content
* infinite feeds

NoBSTube instead emphasizes:

* search
* finite results
* user-defined filtering
* AI-assisted classification
* multiple independent sources
* local control
* deliberate discovery

## Intentional Computing Principles

NoBSTube demonstrates:

* Search over feeds
* Curation over volume
* User-defined filtering
* AI as a tool
* Attention is not the product
* Completion over engagement
* No infinite by default
* Personal information diets
* Local-first software
* No unnecessary accounts

## Architecture

The project is intentionally local.

The basic architecture is:

```text
User
  │
  ▼
Local Web Interface
  │
  ▼
Local Application
  │
  ├── Search Sources
  │     ├── YouTube
  │     ├── PeerTube
  │     └── Internet Archive
  │
  ├── Filtering
  │     ├── Hard Rules
  │     ├── User Rules
  │     └── AI Classification
  │
  ├── Local Database
  │
  └── Results
```

AI is used to reduce the amount of information the user has to process.

It should not become another recommendation engine.

## Long-Term Direction

Potential future capabilities include:

* faster AI filtering
* streaming first acceptable results
* classification caching
* better local search
* configurable information diets
* playback improvements
* offline metadata
* intentional discovery modes
* source-independent search
* user-controlled ranking

The central constraint remains:

> NoBSTube should help the user find something and then get out of the way.

---

# 4. Mirage

**Repository:** `mirage`

## Purpose

Mirage is a lightweight pixel-art and sprite editor.

It explores the idea that creative software can be:

* powerful
* local
* understandable
* fast
* long-lived
* independent of subscription ecosystems

The goal is not to reproduce every feature of a modern commercial graphics suite.

The goal is to provide a focused tool for deliberate creation.

## Intentional Computing Principles

Mirage demonstrates:

* Creation over consumption
* Local ownership
* Direct manipulation
* Understandable interfaces
* Open formats
* Offline capability
* Minimal dependencies
* Progressive complexity
* User-owned files
* Preservation

## Technology

The project uses:

* Java
* JavaFX
* Maven

The architecture should remain deliberately understandable.

Heavy frameworks and unnecessary infrastructure should not be introduced merely because they are available.

## Long-Term Direction

Potential capabilities include:

* pixel canvas
* palette editing
* layers
* animation
* selections
* image import/export
* sprite-sheet workflows
* tile editing
* NES workflows
* SNES workflows
* reusable project formats
* scripting or automation where useful

The important constraint is:

> The tool should remain a creative instrument rather than becoming a platform.

---

# 5. NES Emulator

**Repository:** `rust-nes-emu`

## Purpose

The NES emulator project explores computing preservation.

The goal is not merely to run old games.

It is to understand, document, reproduce, and preserve a historical computing environment.

The project is being developed as a serious emulator rather than as a minimal demonstration.

## Intentional Computing Principles

The emulator demonstrates:

* Preservation
* Local ownership
* Offline capability
* Open technology
* Understandable systems
* Long-term compatibility
* Computing history
* Software independence

## Direction

The emulator should eventually provide a strong foundation for:

* accurate NES emulation
* debugging
* development
* ROM experimentation
* tooling
* preservation
* future hardware projects

The project also acts as an architectural reference for future emulator work.

---

# 6. SNES Emulator

**Repository:** `rust-snes-emu`

## Purpose

The SNES emulator extends the preservation work into a significantly more complex system.

It builds upon lessons learned from the NES emulator while dealing with:

* a more complex CPU
* multiple processors
* more advanced graphics
* audio hardware
* multiple cartridge configurations
* additional memory systems

## Intentional Computing Principles

The project demonstrates:

* Preservation
* Technical understanding
* Local software
* Offline capability
* Long-term compatibility
* Complexity made understandable

## Relationship With NES

The NES emulator is an important architectural reference.

The goal is not to blindly copy its implementation.

Instead:

```text
NES Understanding
       │
       ▼
Architectural Lessons
       │
       ▼
SNES Design
       │
       ▼
Improved Emulator Architecture
```

Each preservation project should make the next one better.

---

# 7. Atari 2600 Emulator

**Repository:** `rust-atari2600-emu`

## Purpose

The Atari 2600 emulator explores preservation at an even lower level.

The system is historically important because it demonstrates how extremely constrained hardware could produce complete interactive experiences.

Emulating it requires understanding the relationship between:

* CPU execution
* memory
* television timing
* graphics generation
* cartridge behavior
* input
* software timing

## Intentional Computing Principles

The project demonstrates:

* Preservation
* Hardware understanding
* Minimal computing
* Offline software
* Historical computing
* Long-term compatibility

The purpose is educational as well as functional.

---

# 8. NES Sprite and Tile Tooling

**Purpose**

The sprite tooling exists to make old game assets understandable and editable without requiring the user to manually reconstruct everything.

A typical workflow is:

```text
NES ROM
  │
  ▼
Extract Sprite Data
  │
  ▼
Visual Tile Sheet
  │
  ▼
Human Editing
  │
  ▼
Tile Mapping
  │
  ▼
Rebuild Original Structure
  │
  ▼
ROM
```

The important distinction is that the editor does not simply create a new image.

It preserves the relationship between the edited artwork and the original tile data.

## Intentional Computing Principles

This project demonstrates:

* Preservation
* Direct manipulation
* Human-readable tooling
* Reversible workflows
* User ownership
* Historical software modification
* Specialized tools over general complexity

---

# 9. Offline Gaming Device

**Purpose**

The offline gaming device explores what happens when modern hardware is designed around **deliberate ownership rather than connectivity**.

The intended system is approximately:

```text
                    ┌─────────────────┐
                    │   HDMI Display  │
                    └────────┬────────┘
                             │
                             │
                  ┌──────────▼──────────┐
                  │   Personal Device   │
                  │                     │
                  │   Linux             │
                  │   Rust Emulator     │
                  │   Local ROMs        │
                  └──────────┬──────────┘
                             │
                      ┌──────┴──────┐
                      │             │
                 Controller 1  Controller 2
```

The system does not need:

* social accounts
* cloud services
* advertisements
* telemetry
* persistent internet access
* recommendation engines

It simply needs to play games.

## Intentional Computing Principles

This project demonstrates:

* Offline-first computing
* Ownership
* Hardware independence
* Local software
* Simplicity
* No unnecessary connectivity
* Technology that disappears when the task begins

---

# 10. Personal Internet

## Status

Future project.

## Purpose

The Personal Internet project explores what the internet could look like when the individual—not the platform—is the primary organizing principle.

The modern internet is largely organized around:

```text
Platform
    ↓
Content
    ↓
Recommendation
    ↓
User
```

The Personal Internet reverses this:

```text
Person
   ↓
Intent
   ↓
Personal Information Layer
   ↓
Selected Sources
   ↓
Useful Information
```

The user decides what enters their environment.

## Possible Capabilities

* personal search
* local bookmarks
* personal indexes
* saved knowledge
* local metadata
* source filtering
* AI summarization
* information classification
* personal archives
* offline caches
* user-defined information rules

The goal is not to disconnect from the internet.

The goal is to make the internet **enter the user's environment on the user's terms**.

---

# 11. Personal AI Assistant

## Status

Future project.

## Purpose

The Personal AI Assistant explores AI as a local or user-controlled computing layer.

Instead of asking:

> How can AI keep the user engaged?

the system asks:

> How can AI remove unnecessary work from the user's life?

Potential responsibilities include:

* searching
* organizing
* summarizing
* filtering
* transforming
* automating
* writing
* coding
* managing local information
* interfacing with personal software

The AI should increasingly disappear into the system.

The desired result is not:

```text
User → AI → Everything
```

but:

```text
User
  │
  ▼
Intent
  │
  ▼
Software + AI
  │
  ▼
Completed Task
```

---

# 12. Intentional Desktop

## Status

Future project.

## Purpose

The Intentional Desktop explores an operating environment designed around calm computing.

It would prioritize:

* local files
* clear application boundaries
* finite information
* simple navigation
* predictable behavior
* minimal notifications
* offline operation
* user configuration

The desktop should not constantly compete for attention.

It should be a place where work happens.

---

# 13. Intentional Device

## Status

Future project.

## Purpose

The Intentional Device explores dedicated personal hardware.

The device should provide modern computational capability while avoiding the assumption that every device must be:

* connected
* synchronized
* social
* notification-driven
* account-dependent

The device could combine:

```text
Modern Hardware
      +
Local Software
      +
Personal AI
      +
Offline Capability
      +
User Ownership
```

This represents one possible physical realization of the Intentional Computing philosophy.

---

# 14. Personal Information Architecture

## Status

Future project.

This project explores the underlying structure connecting personal:

* files
* notes
* documents
* media
* bookmarks
* projects
* archives
* AI-generated information
* software configuration

The goal is to prevent personal information from becoming fragmented across unrelated services.

The fundamental principle is:

> Your information should remain understandable and usable even if a particular application disappears.

---

# 15. Project Relationships

The projects should reinforce one another without becoming tightly coupled.

For example:

```text
                    Intentional Computing
                            │
             ┌──────────────┼──────────────┐
             │              │              │
          Discovery       Creation     Preservation
             │              │              │
          NoBSTube        Mirage        Emulators
             │              │              │
             └──────────────┼──────────────┘
                            │
                     Shared Principles
                            │
             ┌──────────────┼──────────────┐
             │              │              │
        Personal AI   Personal Internet  Devices
```

A project may borrow:

* design principles
* architectural ideas
* file formats
* tooling
* AI techniques
* interface patterns
* documentation practices

But each repository should remain independently understandable.

---

# 16. What Makes a Project an Intentional Computing Project?

A project does not qualify simply because it is:

* local
* open source
* old-fashioned
* offline
* written in Rust
* written in Python
* written in Java
* AI-powered

Those are implementation details.

The deeper question is:

> Does the software increase the user's capability without unnecessarily demanding the user's attention, autonomy, or dependence?

A project should be evaluated against the principles in `PRINCIPLES.md` and the design guidance in `DESIGN.md`.

---

# 17. Project Evaluation

Before beginning a major new project, ask:

### Human Agency

* Does the user remain in control?
* Can the user understand what the software is doing?
* Can the user override important decisions?

### Attention

* Does the software have natural stopping points?
* Are notifications necessary?
* Does it encourage unnecessary continued use?

### Ownership

* Does the user own their files?
* Can the user export their data?
* Can the software continue working without an external account?

### Architecture

* Is the architecture simpler than it needs to be?
* Are dependencies justified?
* Could important functionality remain local?

### AI

* Is AI reducing complexity?
* Is AI making the user more capable?
* Is AI introducing unnecessary dependency?

### Longevity

* Could someone maintain this software in ten years?
* Are the formats documented?
* Are external services replaceable?

### Exit

* Can the user stop using the software without losing their work?

---

# 18. Project Maturity

Projects should progress through deliberate stages.

```text
IDEA
 │
 ▼
EXPERIMENT
 │
 ▼
USEFUL TOOL
 │
 ▼
RELIABLE SOFTWARE
 │
 ▼
MATURE PROJECT
 │
 ▼
PRESERVABLE SOFTWARE
```

Not every project needs to reach the final stage.

A small tool that solves one problem extremely well is preferable to a massive application that attempts to solve everything.

---

# 19. Separate Repositories, Shared Direction

The Intentional Computing repository is **not intended to become a monorepo**.

Instead:

```text
intentional-computing/
        │
        ├── Philosophy
        ├── Principles
        ├── Design
        └── Project Direction
                 │
       ┌─────────┼─────────┐
       │         │         │
       ▼         ▼         ▼
   nobstube   mirage   rust-nes-emu
                         │
                         ├── rust-snes-emu
                         └── rust-atari2600-emu
```

Each project has:

* its own repository
* its own README
* its own roadmap
* its own issues
* its own release cycle
* its own implementation

The umbrella repository provides the common direction.

---

# 20. Using This Repository With AI

This repository should also serve as a **context layer for AI-assisted development**.

When starting work on an Intentional Computing project, an AI coding agent should be able to understand the broader philosophy before making architectural or UX decisions.

Recommended context order:

```text
MANIFESTO.md
      ↓
PRINCIPLES.md
      ↓
DESIGN.md
      ↓
PROJECTS.md
      ↓
Project README
      ↓
Project ROADMAP
      ↓
Source Code
```

This creates an important distinction.

The AI should not simply ask:

> "How do I implement this feature?"

It should also understand:

> "Why is this feature being built, and what should it not become?"

This is particularly important when using AI coding agents because technically valid implementations can still violate the project's philosophy.

---

# 21. Adding New Projects

A new project should be added when it explores a meaningful problem within the philosophy.

Before adding one, document:

```text
Project Name
     │
     ├── Problem
     ├── Intended User
     ├── Why It Exists
     ├── Principles Demonstrated
     ├── Local/Offline Strategy
     ├── AI Role
     ├── Ownership Model
     └── Long-Term Direction
```

The project should have a clear reason for existing beyond:

> "It would be interesting to build."

Interest is welcome.

Purpose is required.

---

# 22. The Ecosystem Should Grow Slowly

Intentional Computing should not become another content machine.

There is no requirement to:

* release constantly
* build dozens of applications
* maintain unnecessary features
* chase trends
* maximize GitHub activity
* turn every idea into a product

The ecosystem should grow when useful.

A finished tool is a success.

A small tool is a success.

A tool that is used for ten years is a greater success.

---

# 23. The Common Thread

Although these projects appear unrelated, they share the same underlying goal.

NoBSTube asks:

> Can information be filtered to serve the person?

Mirage asks:

> Can powerful creative software remain a personal tool?

The emulators ask:

> Can computing history remain usable and understandable?

The offline device asks:

> Can modern hardware exist without unnecessary connectivity?

The Personal Internet asks:

> Can the individual regain control of their information environment?

The Personal AI asks:

> Can AI increase capability without demanding attention?

The Intentional Desktop asks:

> Can the computer become powerful without becoming intrusive?

These are all versions of the same question:

> **What would computing look like if it were designed around the person rather than the platform?**

---

# 24. Long-Term Direction

The projects may eventually converge into a larger personal computing environment:

```text
                         PERSON
                           │
                           ▼
                         INTENT
                           │
            ┌──────────────┼──────────────┐
            │              │              │
        INFORMATION     CREATION      COMPUTING
            │              │              │
       Personal Net      Mirage       Emulators
            │              │              │
            └──────────────┼──────────────┘
                           │
                           ▼
                      PERSONAL AI
                           │
                           ▼
                  INTENTIONAL DESKTOP
                           │
                           ▼
                   INTENTIONAL DEVICE
```

This is not a requirement that every project eventually merge.

It is a direction.

Each project explores one part of the larger system.

---

# 25. The Standard

Every project should ultimately answer yes to these questions:

> Does it give the user more capability?

> Does it preserve user control?

> Does it respect attention?

> Does it reduce unnecessary complexity?

> Does it preserve ownership?

> Does it remain useful without unnecessary dependency?

> Does it have a natural stopping point?

> Can the user walk away?

If the answer is yes, the project is moving in the right direction.

---

# Final Principle

The projects in this ecosystem are not attempts to recreate the past.

They are attempts to recover something valuable from it:

**computing that belongs to the person using it.**

The technology can be modern.

The processors can be faster.

The software can be more capable.

AI can be extraordinarily powerful.

The internet can remain available.

But the relationship should remain simple:

```text
PERSON
  │
  │ intent
  ▼
COMPUTER
  │
  │ capability
  ▼
RESULT
  │
  ▼
LIFE
```

The computer should help.

Then it should get out of the way.
