# Local-First Computing

## Introduction

A computer should remain useful even when the network disappears.

Modern software increasingly assumes that an internet connection, remote service, account, subscription, or cloud platform is always available. This can make software convenient, but it also changes the relationship between the person and the computer.

The computer stops being a tool that belongs to the user and becomes a terminal for someone else's infrastructure.

Intentional Computing takes a different approach:

> **When practical, software should work locally first and use the network when the network provides genuine additional value.**

Local-first does not mean rejecting the internet.

It means refusing to make the internet a prerequisite for things that do not actually require it.

---

## The Original Personal Computer

The personal computer was originally personal in a very literal sense.

A person could:

* install software
* create files
* edit documents
* write programs
* play games
* organize information
* customize the environment
* save everything locally
* continue working without a network

The computer was a machine under the user's control.

The internet was an additional capability.

Intentional Computing seeks to preserve that relationship while taking advantage of modern technology.

The goal is not to recreate the 1980s or 1990s.

The goal is to combine:

**the ownership and independence of local computing**

with

**the capabilities of modern hardware, software, networks, and AI.**

---

# Local First Does Not Mean Offline Only

There is an important distinction.

Intentional Computing does not argue:

> "Never use the internet."

It argues:

> "Use the internet when it provides something the local machine actually needs."

There are many things that genuinely benefit from network access:

* searching the public internet
* downloading software
* communicating with other people
* accessing current information
* synchronizing devices
* retrieving remote data
* collaborating
* using distributed services

These are legitimate uses of networking.

The problem occurs when networking becomes an unnecessary dependency.

A text editor should not need a server to open a local document.

A drawing application should not need an account to create an image.

A media player should not require a subscription to play files the user owns.

A game should not require a remote server for a fundamentally single-player experience.

A personal database should not become unusable because a company changed its API.

Local-first computing draws a boundary between these two cases.

---

# The Local-First Principle

The fundamental principle is:

> **If a task can reasonably be performed locally, the local machine should be capable of performing it locally.**

This does not require every feature to be implemented locally.

It means the architecture should deliberately identify which capabilities actually require external infrastructure.

For example:

```text
LOCAL

Files
Configuration
Preferences
Projects
Caches
Search indexes
User-created content
Application state
History
AI models where practical


NETWORK

Public information
Remote collaboration
Optional synchronization
External services
Updates
Distributed resources
Current information
```

The boundary should be intentional.

It should not simply be whatever happens to be convenient for the developer or service provider.

---

# Local Is a Capability

Local computing should not be treated merely as an offline fallback.

It is a capability in its own right.

A local application can provide:

* lower latency
* greater privacy
* greater reliability
* predictable behavior
* offline operation
* user ownership
* easier preservation
* reduced dependency
* easier inspection
* easier backup
* greater control

These are not secondary benefits.

They are fundamental properties of personal computing.

---

# The Network Should Be an Extension

A useful model is:

```text
                    COMPUTER
                       │
                ┌──────┴──────┐
                │             │
             LOCAL          NETWORK
                │             │
             Core          Extension
             Work           Services
                │             │
                └──────┬──────┘
                       │
                     USER
```

The local computer should provide the foundation.

The network should extend its capabilities.

The reverse relationship is increasingly common:

```text
                  REMOTE SERVICE
                       │
                  INTERNET
                       │
                  APPLICATION
                       │
                    USER
```

In this model, the user's computer becomes little more than an interface to infrastructure they do not control.

Intentional Computing prefers the first model.

---

# Local Data

User-created data should be local and accessible whenever practical.

This includes:

* documents
* images
* projects
* configuration
* preferences
* bookmarks
* saved searches
* application data
* personal databases
* creative work
* source code
* archives

The user should know where important information lives.

Files should not disappear into an opaque application-specific system simply because the application developer decided that storage should happen remotely.

---

# Files Matter

Files are one of the most powerful abstractions in personal computing.

A file can be:

* copied
* backed up
* moved
* renamed
* inspected
* archived
* opened by another application
* transferred to another computer
* preserved for decades

This gives the user leverage.

Intentional Computing therefore treats files as valuable infrastructure rather than an outdated abstraction.

When appropriate:

> **The user should be able to find the data.**

Not merely:

> "The application knows where it is."

---

# Open Formats

Local ownership becomes less meaningful if the data is trapped inside proprietary formats.

Whenever practical, applications should prefer:

* open formats
* documented formats
* standard formats
* human-readable formats
* easily convertible formats

Proprietary formats are not automatically bad.

Sometimes they are technically justified.

But applications should avoid creating unnecessary barriers to migration.

A user should not have to remain subscribed to an application simply to retain access to their own work.

---

# No Unnecessary Accounts

Local software should not require an account merely because accounts are convenient for the service provider.

A local application that performs a local task should generally be usable without:

* creating an account
* providing an email address
* accepting a social profile
* connecting a third-party identity
* maintaining a subscription

Accounts make sense when there is a real reason for them.

Examples include:

* remote synchronization
* collaboration
* multiplayer services
* cloud storage
* purchases
* identity-dependent services

But account creation should solve a real problem.

It should not be the problem.

---

# Offline Capability

Offline operation is one of the clearest tests of local-first design.

A useful question is:

> **What happens when the network cable is unplugged?**

For a genuinely local application, the answer should often be:

> "The application continues working."

Perhaps some optional features disappear.

That is acceptable.

For example:

```text
Offline:

Open project       ✓
Edit project       ✓
Save project       ✓
Search local data  ✓
Export files       ✓
Use local AI       ✓

Unavailable:

Remote sync       ✗
Public search     ✗
Online updates    ✗
Remote services   ✗
```

This is graceful degradation.

The computer remains useful.

---

# Graceful Degradation

Network-dependent features should fail gracefully.

The user should not experience:

> "No internet connection. Application unusable."

when the task itself does not require the internet.

Instead:

```text
NETWORK AVAILABLE
        ↓
Full capability


NETWORK UNAVAILABLE
        ↓
Local capability remains
        ↓
Optional network features disabled
```

The absence of the network should reduce capability only where necessary.

It should not collapse the entire application.

---

# Local-First AI

AI makes local-first computing particularly interesting.

Modern AI systems can provide enormous capabilities, but many AI services are remote by default.

Intentional Computing should prefer local AI where it is practical.

A local model can provide:

* privacy
* offline operation
* predictable availability
* user control
* lower marginal cost
* independence from an external provider

This does not mean every AI model should run locally.

Large remote models can provide capabilities that may be impractical to reproduce locally.

The principle is:

> **Use the most appropriate intelligence source while preserving local capability where practical.**

A hybrid architecture can therefore be intentional:

```text
LOCAL AI
   ↓
Fast / Private / Offline
   ↓
Handle ordinary tasks


REMOTE AI
   ↓
More capable when necessary
   ↓
Handle optional advanced tasks
```

The user should know which is being used.

---

# Local AI as a Tool

AI should not automatically become another reason for the user to remain connected.

A local AI assistant could help with:

* searching personal files
* classifying information
* organizing documents
* filtering media
* writing code
* analyzing local data
* indexing archives
* finding relationships between files

This is particularly powerful because the AI can operate on information the user already owns.

The machine becomes capable of understanding the user's personal computing environment without requiring that environment to be uploaded somewhere else.

---

# The Personal Information Layer

Local-first computing becomes increasingly powerful when combined with the idea of a personal information layer.

For example:

```text
                    PUBLIC INTERNET
                           │
                           ↓
                    ┌──────────────┐
                    │ Personal     │
                    │ Information  │
                    │ Layer        │
                    └──────┬───────┘
                           │
             ┌─────────────┼─────────────┐
             ↓             ↓             ↓
          Search         AI          Archives
             │             │             │
             └─────────────┼─────────────┘
                           ↓
                       COMPUTER
                           ↓
                          USER
```

The personal layer can:

* remember
* organize
* filter
* index
* summarize
* search
* archive
* classify

without requiring the public internet to become the user's permanent environment.

---

# Local Search

Local-first computing should make personal information easy to search.

A computer may contain years of:

* documents
* photographs
* source code
* notes
* saved webpages
* books
* music
* videos
* projects
* archives

The user should be able to ask:

> "Where is that thing I worked on three years ago?"

and have the computer help find it.

This is an important role for AI.

Instead of forcing the user to remember where information was stored, the machine can absorb the complexity of indexing and retrieval.

The user gets the result.

The complexity remains inside the machine.

---

# Local Caches

Caching is another important local-first technique.

When remote information is legitimately needed, applications should consider whether useful information can be retained locally.

For example:

```text
NETWORK
   ↓
Retrieve information
   ↓
LOCAL CACHE
   ↓
User
```

This can improve:

* performance
* resilience
* offline access
* reliability
* network efficiency

Caches should be understandable and manageable where practical.

They should not silently become permanent hidden data stores.

---

# Synchronization Should Be Optional

Synchronization is useful when a person owns multiple devices.

For example:

```text
Laptop
   ↕
Phone
   ↕
Desktop
```

But synchronization should extend ownership rather than replace it.

A healthy model is:

```text
DEVICE A
  │
  ├── local copy
  │
  └──── sync ────┐
                 │
              SERVICE
                 │
  ┌──── sync ────┘
  │
  └── local copy
DEVICE B
```

Each device can remain useful.

An unhealthy model is:

```text
DEVICE A ──┐
DEVICE B ──┼──> CLOUD
DEVICE C ──┘
               │
               ↓
        Everything depends on it
```

Synchronization should connect personal environments.

It should not become the environment itself.

---

# Replaceability

Local-first architecture should make components replaceable.

If a service disappears, the user's core data and workflows should remain recoverable.

For example:

```text
Application
    │
    ├── Local Files
    ├── Local Database
    ├── Export
    └── Optional Services
```

rather than:

```text
Application
    │
    └── Proprietary Remote Platform
              │
              └── Everything
```

Replaceability is a form of freedom.

It means the user can change software without losing their computing environment.

---

# Dependency Is a Design Decision

Every external dependency should answer a question:

> **Why does this need to be external?**

The answer may be completely reasonable.

For example:

* public web search requires the web
* multiplayer requires other players
* cloud collaboration requires shared infrastructure
* remote backups require remote storage

But sometimes the answer is merely:

> "Because that is how the service was designed."

That should not automatically be accepted.

Architecture determines power relationships.

A local architecture generally gives more power to the user.

A centralized architecture generally gives more power to the service provider.

Intentional Computing treats that as a design consideration.

---

# Local-First and Privacy

Privacy is often a natural consequence of local-first design.

If data never leaves the computer, there is less external infrastructure capable of collecting it.

This does not automatically make software private.

Local applications can still:

* collect telemetry
* communicate externally
* expose local data
* log sensitive information
* include unnecessary tracking

Therefore:

> **Local-first is an architectural advantage, not a substitute for privacy engineering.**

Good local-first software should make its network boundaries understandable.

---

# Network Transparency

A user should be able to understand when software communicates externally.

Important questions include:

* What data leaves the computer?
* Why does it leave?
* Where does it go?
* Can the feature work without it?
* Can the user disable it?
* Is the data retained?
* Is an account required?

The network should not be invisible simply because networking is technically easy.

---

# Local-First Does Not Mean Isolation

A local-first computer can still be highly connected.

It can:

* browse the web
* download files
* communicate
* use remote AI
* synchronize
* access public databases
* collaborate
* stream media
* update software

The difference is architectural.

The computer remains the user's computer.

The network becomes something the computer uses.

It does not become the thing the computer depends upon for its identity and basic usefulness.

---

# Preservation

Local-first architecture improves the chances that software and data can survive.

A system built around:

* local files
* documented formats
* minimal dependencies
* understandable software
* exportable data

is easier to preserve.

A system built around:

* proprietary APIs
* remote databases
* mandatory authentication
* constantly changing services
* undocumented formats

is much harder to preserve.

This matters because personal computing should outlive individual companies.

A photograph should not disappear because a startup shut down.

A document should not become inaccessible because a subscription ended.

A creative project should not require a particular SaaS provider forever.

---

# The Ten-Year Test

Intentional Computing should ask:

> **Could this user's work still be accessible ten years from now?**

The answer does not need to be perfect.

But architecture should make preservation possible.

A useful hierarchy is:

```text
Best

Local file
Open format
Documented format
Exportable database
Self-contained project

↓

Increasing dependency

Proprietary application format
Remote API
Mandatory account
Subscription service
Closed platform

Worst
```

The higher the dependency, the greater the preservation risk.

---

# The Exit Test

Another important question is:

> **Can the user leave?**

A healthy local-first application should make exit possible.

The user should be able to:

* export their files
* copy their data
* stop using the application
* uninstall the software
* switch to another tool
* continue using their existing work

The ability to leave is not an edge case.

It is part of ownership.

---

# Local-First as a Spectrum

Not every application can be completely local.

Local-first therefore exists on a spectrum.

```text
100% LOCAL
│
├── Text editor
├── Image editor
├── Emulator
├── Media player
│
├── Local AI application
│
├── Hybrid application
│
├── Cloud-assisted application
│
└── Network-dependent service
                                      100% REMOTE
```

The goal is not to force every application to the left.

The goal is to avoid moving applications to the right without a good reason.

---

# Local-First and Intentional Computing

Local-first architecture directly supports the broader Intentional Computing philosophy.

It provides:

### Human Agency

The user controls the environment.

### Attention Protection

The application does not need a constant connection to a platform designed around engagement.

### Ownership

Files and projects remain accessible.

### Privacy

Less information needs to leave the machine.

### Reliability

Core functionality can continue when services fail.

### Longevity

Software and data are easier to preserve.

### Understandability

The boundaries of the system are clearer.

### Exit

The user can leave without abandoning their work.

---

# The Local-First Test

Every Intentional Computing project should ask:

1. What can reasonably run locally?
2. What genuinely requires the network?
3. Can the application remain useful without the network?
4. Where is the user's data stored?
5. Can the user access the underlying files?
6. Are open or documented formats available?
7. Is an account actually necessary?
8. Can network-dependent features fail gracefully?
9. Can the user export their data?
10. Can the user replace the application or service?
11. Can the system use local AI where practical?
12. Are network boundaries understandable?
13. Could the user's work survive the disappearance of the service?
14. Can the user leave?

If the answers are good, the system is probably respecting the local-first principle.

---

# Local-First Architecture

A general Intentional Computing architecture can be represented as:

```text
                    USER
                      │
                      ↓
              ┌───────────────┐
              │ LOCAL SYSTEM  │
              │               │
              │ Data          │
              │ Preferences   │
              │ Projects      │
              │ Search        │
              │ AI            │
              │ Applications  │
              └───────┬───────┘
                      │
             Optional Network
                      │
                      ↓
              ┌───────────────┐
              │ PUBLIC /      │
              │ REMOTE WORLD  │
              │               │
              │ Web           │
              │ Services      │
              │ Collaboration │
              │ Remote AI     │
              │ Updates       │
              └───────────────┘
```

The local system is the foundation.

The network is the extension.

The person remains the center.

---

# The Bigger Goal

Local-first computing is not primarily about offline mode.

It is about restoring the idea that a computer belongs to the person using it.

Modern computers are extraordinarily powerful.

They can process enormous amounts of information.

They can run sophisticated AI models.

They can communicate with almost any system on Earth.

They can access an effectively unlimited library of information.

None of that requires surrendering ownership.

The future should therefore not be:

> **More powerful cloud terminals.**

It should be:

> **More capable personal computers that can use the cloud when useful.**

That distinction matters.

---

# The Ideal

The ideal Intentional Computing machine might look like this:

```text
                    PERSONAL COMPUTER
                           │
        ┌──────────────────┼──────────────────┐
        │                  │                  │
      FILES               AI               APPS
        │                  │                  │
        └──────────────────┼──────────────────┘
                           │
                      USER INTENT
                           │
                           ↓
                    USE THE NETWORK
                     WHEN NEEDED
                           │
                           ↓
                    RETURN TO LOCAL
                           │
                           ↓
                       COMPLETION
                           │
                           ↓
                         LIFE
```

The internet becomes something the computer can reach.

AI becomes something the computer can use.

Software becomes something the user owns.

Data becomes something the user controls.

And the computer remains useful even when everything outside it goes quiet.

---

# Final Principle

> **The network should expand the capabilities of the computer, not replace the computer.**

A powerful personal computer should be able to stand on its own.

It should work offline.

It should keep the user's data accessible.

It should use open formats where practical.

It should make external dependencies visible.

It should allow the user to leave.

And when the network is available, it should become a powerful extension of the machine rather than a prerequisite for its existence.

The future of computing does not have to choose between local and connected.

It can be both.

**Local by foundation.**

**Connected by choice.**

**Owned by the person.**

**Controlled by the person.**
