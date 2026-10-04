# Intentional Computing

> **Modern technology without surrendering control of your attention, environment, or tools.**

Intentional Computing is an approach to building and using technology around **human agency rather than engagement**.

It does not reject modern technology.

It asks a different question about how that technology should be used:

> **What if computers became dramatically more capable without becoming dramatically more demanding of the person using them?**

This repository is the philosophical and architectural foundation for a collection of independent software and hardware projects exploring that idea.

---

## The Problem

Modern computing is extraordinarily powerful.

But much of the modern digital environment is designed around:

* attention
* engagement
* recommendation
* notifications
* infinite feeds
* platform dependency
* behavioral optimization
* centralized services
* constant connectivity

The result is a strange contradiction:

> Computers have become more capable while many digital experiences have become less intentional.

The problem is not technology itself.

The problem is what technology is being optimized for.

Intentional Computing starts from a different assumption:

> **Technology should increase human capability without demanding human attention in exchange.**

---

# The Idea

The computer should be a tool.

You decide what you want to do.

The computer helps you do it.

You finish.

Then you return to your life.

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

This sounds simple.

It is also increasingly unusual.

---

# What We Are Building

Intentional Computing is not one application.

It is an ecosystem of independent projects exploring different parts of the idea.

### Discovery

**NoBSTube**

A local video search and filtering system designed around search, curation, and user-defined information diets rather than engagement feeds.

### Creation

**Mirage**

A lightweight pixel-art and sprite editor designed around local ownership, direct manipulation, and long-term usability.

### Preservation

**Rust NES Emulator**

A serious NES emulation project focused on understanding and preserving historical computing.

**Rust SNES Emulator**

A future continuation of that preservation work for the considerably more complex SNES architecture.

**Rust Atari 2600 Emulator**

A preservation project exploring one of the earliest generations of home console computing.

### Tooling

**NES Sprite and Tile Tools**

Tools for extracting, editing, mapping, and rebuilding old game graphics while preserving their relationship to the original data.

### Hardware

**Offline Gaming Device**

A personal gaming machine designed to work locally without requiring accounts, cloud services, advertising, or persistent internet connectivity.

### Future

The longer-term direction includes exploration of:

* Personal Internet
* Personal Information Architecture
* Personal AI
* Intentional Desktop
* Intentional Devices

These are directions, not promises that every idea will become a product.

---

# The Core Principles

Intentional Computing is built around a few fundamental ideas.

1. **Human agency first.**
2. **Attention is not the product.**
3. **Completion is better than engagement.**
4. **Search is better than endless feeds.**
5. **Curation is better than volume.**
6. **AI should reduce complexity, not manufacture dependency.**
7. **Users should own their data and work.**
8. **Local and offline capability is valuable.**
9. **Software should be understandable and maintainable.**
10. **The user should always be able to walk away.**

These principles are expanded in [`PRINCIPLES.md`](PRINCIPLES.md).

---

# AI Has a Place Here

Intentional Computing is not anti-AI.

Quite the opposite.

AI may be one of the most powerful tools available for making computing more intentional.

The important distinction is **what the AI is optimizing for**.

An attention-driven system might use AI to produce:

```text
More recommendations
       ↓
More content
       ↓
More engagement
       ↓
More attention
```

An intentional system can use AI to produce:

```text
Complex information
       ↓
AI filtering
       ↓
Useful information
       ↓
Human decision
       ↓
Completed task
```

AI should increasingly absorb complexity on the user's behalf.

It should not become another thing demanding the user's attention.

---

# The 90s Principle

The 1990s are an important reference point for this project.

Not because everything from that era was better.

It wasn't.

Modern technology has enormous advantages:

* powerful processors
* high-resolution displays
* global connectivity
* sophisticated graphics
* modern programming languages
* machine learning
* AI
* inexpensive storage
* powerful development tools

We should keep those advantages.

What is worth recovering from earlier personal computing is the sense that:

* the computer belonged to you
* software was something you installed and used
* files were yours
* interfaces had natural boundaries
* applications generally had a beginning and an end
* the internet was something you accessed rather than somewhere you lived
* computers were tools for making things

The goal is therefore not:

> **Go back to the 1990s.**

It is:

> **Build the future without throwing away the things that made personal computing feel personal.**

---

# Personal Computing, Reconsidered

The traditional model looked roughly like:

```text
PERSON
  │
  ▼
COMPUTER
  │
  ▼
SOFTWARE
  │
  ▼
RESULT
```

Much of modern computing increasingly looks like:

```text
PERSON
  │
  ▼
PLATFORM
  │
  ▼
ALGORITHM
  │
  ▼
CONTENT
  │
  ▼
ENGAGEMENT
  │
  ▼
MORE ENGAGEMENT
```

Intentional Computing attempts to restore the first relationship while taking advantage of modern capabilities.

The desired model is:

```text
PERSON
  │
  │ intent
  ▼
COMPUTER
  │
  ├── Software
  ├── AI
  ├── Internet
  ├── Local Data
  └── Automation
  │
  ▼
CAPABILITY
  │
  ▼
RESULT
```

The technology can be extremely sophisticated.

The relationship does not need to be.

---

# A Personal Internet

One of the long-term ideas behind this project is a **Personal Internet**.

The internet itself is not the problem.

The problem is allowing enormous amounts of information to enter a person's environment without meaningful control.

A personal information layer could instead provide:

* deliberate search
* source selection
* filtering
* local archives
* personal indexes
* AI summarization
* configurable information rules
* offline access
* user-controlled discovery

The internet remains available.

But it becomes a resource rather than an environment that constantly competes for attention.

---

# Separate Projects, Shared Philosophy

This repository is intentionally **not a monorepo**.

Each major project should remain independently useful.

```text
intentional-computing
        │
        ├── Philosophy
        ├── Principles
        ├── Design
        └── Project Direction
                 │
                 ├── nobstube
                 ├── mirage
                 ├── rust-nes-emu
                 ├── rust-snes-emu
                 ├── rust-atari2600-emu
                 └── future projects
```

The projects share ideas, not necessarily code.

This allows each project to use the simplest technology appropriate for its purpose.

---

# Using This Repository With AI

This repository is also intended to act as a **context layer for AI-assisted development**.

When an AI coding agent works on one of the projects, it should understand not only the technical requirements but the philosophy behind them.

A useful context hierarchy is:

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

This helps prevent a common problem with AI-assisted development:

> Building something technically correct that is philosophically wrong.

A feature should not exist merely because it can be implemented.

It should exist because it improves the user's capability.

---

# Repository Structure

```text
intentional-computing/
│
├── README.md
├── MANIFESTO.md
├── PRINCIPLES.md
├── DESIGN.md
├── PROJECTS.md
├── ROADMAP.md
│
├── philosophy/
│   ├── intentional-computing.md
│   ├── personal-internet.md
│   ├── attention-and-algorithms.md
│   ├── local-first.md
│   ├── ownership.md
│   └── ai-as-a-tool.md
│
├── standards/
│   ├── software-principles.md
│   ├── interface-principles.md
│   ├── ai-principles.md
│   └── internet-principles.md
│
└── projects/
    ├── nobstube.md
    ├── mirage.md
    ├── rust-nes-emu.md
    ├── rust-snes-emu.md
    └── offline-gaming-device.md
```

The repository will grow as the philosophy develops.

---

# What This Project Is Not

Intentional Computing is not:

* anti-technology
* anti-internet
* anti-AI
* anti-modernity
* nostalgia for its own sake
* a rejection of smartphones or computers
* an attempt to tell everyone how they should live
* a movement against people who enjoy social media

People should be free to use technology however they want.

The goal is to provide another option.

---

# What This Project Is

It is an exploration of:

**technology with boundaries**

**AI without dependency**

**software without unnecessary complexity**

**internet access without information overload**

**power without manipulation**

**local computing without isolation**

**modern capabilities without surrendering control**

**personal computing that remains personal**

---

# The Intentional Computing Test

Whenever a new feature, application, service, or technology is considered, ask:

### Does it increase capability?

If not, why does it exist?

### Does it respect attention?

Could the same result be achieved without demanding continued engagement?

### Does the user remain in control?

Can important decisions be understood and overridden?

### Does the user own the result?

Can the work, data, and files remain useful outside the application?

### Is the complexity justified?

Could the same result be achieved with a simpler system?

### Can the user stop?

Does the system have a natural stopping point?

### Can the user leave?

Can the user walk away without losing everything?

If the answer to these questions is consistently yes, the system is probably moving in the right direction.

---

# Long-Term Vision

The long-term goal is not to build one giant application.

It is to explore an alternative relationship with computing.

A future where:

* computers are more powerful
* AI is more capable
* software is easier to create
* information is easier to find
* personal data remains personal
* local computing remains viable
* old software remains usable
* creative tools remain accessible
* the internet remains available
* technology becomes less intrusive

In other words:

> **More capability. Less noise.**

---

# The Direction

The fundamental direction of Intentional Computing can be summarized simply:

```text
MORE COMPUTING
      │
      ▼
MORE CAPABILITY
      │
      ▼
LESS HUMAN EFFORT
      │
      ▼
LESS UNNECESSARY ATTENTION
      │
      ▼
MORE TIME FOR LIFE
```

The purpose of better technology should ultimately be to give people **more ability to live their lives**, not more reasons to remain inside the technology.

---

# Final Principle

> **Technology should serve the person, not the other way around.**

Build powerful machines.

Build intelligent software.

Use AI.

Use the internet.

Preserve the past.

Build the future.

But keep the human in control.

**Make the computer powerful.**

**Make the interface calm.**

**Make the system understandable.**

**Protect attention.**

**Preserve ownership.**

**And let the user get back to life.**
