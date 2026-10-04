# Ownership in Computing

## Introduction

A personal computer should be personal in more than name.

The person using it should have meaningful control over:

* their data
* their files
* their software
* their configuration
* their hardware
* their creative work
* their computing environment

Intentional Computing treats ownership as a fundamental property of personal computing.

> **If something is part of a person's computing environment, that person should have as much practical ownership and control over it as reasonably possible.**

Ownership does not mean that every component must be open source.

It does not mean that every service must be free.

It does not mean that companies cannot make software.

It means the relationship between the person and the technology should not unnecessarily become one of dependency.

---

# The Personal Computer

The phrase "personal computer" originally implied something important.

It was a computer that belonged to an individual.

The person could:

* install software
* create files
* modify settings
* connect hardware
* write programs
* copy data
* back up files
* replace applications
* maintain the machine

The computer was a general-purpose tool.

Intentional Computing seeks to preserve that relationship.

Modern technology can make the machine dramatically more capable without making the user less capable of controlling it.

---

# Ownership Is More Than Possession

Buying a computer does not automatically mean owning the computing environment.

A person may physically possess a device while depending completely on external systems for its usefulness.

For example:

```text id="u8zq7j"
PHYSICAL POSSESSION

Computer
   │
   ├── Remote account
   ├── Remote storage
   ├── Remote authentication
   ├── Remote software
   └── Remote services
```

The person owns the hardware.

But much of the computing environment belongs elsewhere.

Intentional Computing considers practical control more important than physical possession alone.

---

# The Layers of Ownership

Computing ownership can be considered in several layers.

```text id="t4g0v5"
                    OWNERSHIP

                       USER
                         │
        ┌────────────────┼────────────────┐
        ↓                ↓                ↓
     HARDWARE           DATA           SOFTWARE
        │                │                │
     Device            Files          Applications
        │                │                │
        └────────────────┼────────────────┘
                         ↓
                    ENVIRONMENT
                         │
                         ↓
                       ACCESS
```

Each layer matters.

Owning the hardware while losing control over the data is incomplete ownership.

Owning the data while being unable to access it without a particular service is incomplete ownership.

Having software while being unable to export the work it produces is incomplete ownership.

Ownership should therefore be considered as a system.

---

# Data Ownership

Data is often the most important form of digital ownership.

Personal data may include:

* photographs
* documents
* source code
* artwork
* music
* videos
* notes
* bookmarks
* saved information
* configuration
* databases
* archives
* creative projects

The user should be able to identify where important data lives.

They should be able to:

* access it
* copy it
* back it up
* export it
* move it
* preserve it
* delete it

Data that exists only inside an inaccessible service is difficult to truly own.

---

# Your Files Should Remain Yours

A useful rule is:

> **The application should manage the user's files, not become the owner of them.**

An image editor should create images.

A writing application should create documents.

A music application should create music projects.

A development environment should create source code.

The application is a tool for working with the user's material.

The user's work should not become inseparable from the tool.

---

# Open and Portable Formats

Ownership requires portability.

If a file can only be opened by one application, the user may effectively be locked into that application.

Where practical, software should support:

* open formats
* documented formats
* standard formats
* export
* import
* conversion
* straightforward backup

This does not mean proprietary formats are forbidden.

They can provide legitimate advantages.

But proprietary formats should not be used unnecessarily to prevent users from leaving.

---

# The Export Test

A simple ownership test is:

> **Can the user export everything important?**

For a creative application, this might include:

```text id="p5i9h6"
PROJECT
   │
   ├── Source file
   ├── Images
   ├── Metadata
   ├── Configuration
   └── Exported assets
```

The user should ideally be able to take the project elsewhere.

If the answer is:

> "No, because the service owns the underlying representation."

then the user has limited ownership.

---

# The Backup Test

Another simple question:

> **Can the user make a complete backup without asking the service provider?**

A personal computer should make this possible whenever practical.

The user should be able to copy important data to:

* another drive
* another computer
* removable storage
* a home server
* an archive
* another application

Backups are not merely disaster recovery.

They are an expression of ownership.

If you can copy your data, you have leverage.

---

# The Migration Test

Ownership also means the ability to move.

Ask:

> **Can the user move their computing environment to another system?**

Perfect migration may not always be possible.

Different applications have different capabilities.

But software should avoid making migration unnecessarily difficult.

A healthy ecosystem allows:

```text id="q5o1kq"
APPLICATION A
     │
     ↓
  EXPORT
     │
     ↓
STANDARD / OPEN DATA
     │
     ↓
  IMPORT
     │
     ↓
APPLICATION B
```

This creates competition based on usefulness rather than captivity.

---

# Vendor Lock-In

Vendor lock-in occurs when leaving a product becomes unnecessarily expensive or difficult.

This can happen through:

* proprietary file formats
* inaccessible data
* mandatory subscriptions
* closed APIs
* account dependencies
* proprietary hardware
* undocumented systems
* artificial incompatibility
* loss of functionality after cancellation

Some forms of dependency are unavoidable.

Intentional Computing rejects unnecessary dependency.

The question is not:

> "Does this system have dependencies?"

Every system does.

The question is:

> **"Does the dependency unnecessarily remove the user's freedom?"**

---

# Ownership and Software

Software ownership is complicated.

Modern software is often licensed rather than sold.

Intentional Computing does not require every application to be open source.

However, users should ideally have meaningful rights to:

* use the software they obtained
* access their work
* retain their data
* export their data
* remove the software
* replace the software
* continue using locally created content

Open source is valuable because it can improve:

* transparency
* preservation
* auditability
* modification
* community maintenance

But open source is one tool for achieving ownership, not the complete definition of ownership.

---

# Understandability Matters

Ownership is difficult when the system is incomprehensible.

A user does not need to understand every line of code.

But they should be able to understand the important relationships.

For example:

```text id="5w3r2e"
Where are my files?
        ↓
Local directory

Where are my settings?
        ↓
Configuration

What goes online?
        ↓
Clearly defined services

How do I back everything up?
        ↓
Copy these files

How do I leave?
        ↓
Export and uninstall
```

The machine can be extremely sophisticated internally.

The user's relationship with it should remain understandable.

---

# Configuration Is Ownership

Configuration is another form of ownership.

Users should be able to control important aspects of their environment.

This can include:

* where data is stored
* what gets synchronized
* what gets indexed
* which sources are used
* what AI can access
* what notifications appear
* what happens automatically
* what services are enabled

A system that cannot be configured gradually becomes a system that controls the user.

Intentional Computing prefers:

> **Configuration over coercion.**

---

# Defaults Matter

Ownership can be undermined by defaults.

A system might technically allow a user to control something while making the control difficult to discover or use.

For example:

```text id="x5v5n8"
Default

Upload everything
      ↓
Automatic sync
      ↓
Remote processing
      ↓
Remote storage
```

versus:

```text id="u5xj52"
Default

Keep data local
      ↓
Optional sync
      ↓
Optional remote processing
      ↓
User chooses
```

The second model gives the user more meaningful ownership.

Defaults are therefore part of architecture.

---

# Ownership and AI

AI introduces new questions about ownership.

A personal AI system may have access to:

* documents
* photographs
* source code
* conversations
* notes
* projects
* browsing history
* preferences
* personal knowledge

That makes AI extremely powerful.

It also makes control extremely important.

The user should understand:

* what the AI can access
* where processing occurs
* what information is retained
* what is sent remotely
* what can be deleted
* what can be exported
* what can be forgotten

AI should become a tool inside the user's computing environment.

It should not quietly become the owner of that environment.

---

# Personal AI Memory

A future personal AI may maintain useful long-term memory.

This should be treated as personal data.

The user should ideally be able to:

* inspect it
* correct it
* delete it
* export it
* back it up
* control what is remembered

A useful architecture might look like:

```text id="v0h6mt"
                  PERSONAL AI
                       │
              ┌────────┴────────┐
              ↓                 ↓
        Local Knowledge      Optional
             Store          Remote AI
              │                 │
              ↓                 ↓
           USER DATA       External Service
```

The personal knowledge store should remain under user control.

---

# Hardware Ownership

Ownership extends beyond software and data.

Hardware can also become artificially restrictive.

Examples include:

* unnecessary hardware locks
* inaccessible storage
* repair restrictions
* proprietary connectors
* account activation requirements
* remote disabling
* mandatory cloud services

Not every hardware component can be user-replaceable.

Modern hardware can be extremely complex.

But when practical:

> **Hardware should remain understandable, maintainable, and useful without unnecessary external dependency.**

Repairability is one expression of ownership.

---

# Repair Is Ownership

A device that cannot be repaired is less meaningfully owned than one that can.

Repair can include:

* replacing storage
* replacing batteries
* replacing controllers
* replacing cables
* reinstalling software
* restoring backups
* replacing peripherals

The exact level of repairability will vary.

But the philosophy remains:

> **The user should have a reasonable path to restoring the machine they own.**

---

# Ownership and Preservation

Ownership creates a responsibility toward the future.

A file created today may need to remain accessible decades later.

This is why Intentional Computing values:

* local storage
* open formats
* documentation
* source availability
* export
* backups
* simple architectures
* minimal dependencies

A personal computer should not merely be useful today.

It should help preserve the user's work for tomorrow.

---

# Ownership and the Internet

The internet does not have to undermine ownership.

It can strengthen it.

The internet can provide:

* information
* collaboration
* software
* communication
* distribution
* synchronization
* discovery
* public archives

The key distinction is:

> **The internet should connect things the user owns, not replace the concept of ownership.**

A personal website can be hosted remotely.

A Git repository can be synchronized remotely.

A backup can exist in the cloud.

A document can be collaboratively edited online.

These can all be compatible with ownership when the user retains access, portability, and control.

---

# Ownership and Services

Services can be useful.

Intentional Computing does not require eliminating them.

Instead, services should occupy an appropriate place in the architecture.

For example:

```text id="5h0gqs"
USER
 │
 ↓
LOCAL COMPUTER
 │
 ├── Data
 ├── Applications
 ├── Configuration
 └── Projects
 │
 ↓
OPTIONAL SERVICES
 │
 ├── Backup
 ├── Sync
 ├── Collaboration
 ├── Search
 └── Remote AI
```

The services extend the personal environment.

They should not necessarily define it.

---

# Ownership Creates Leverage

The ability to leave creates negotiating power.

If the user can:

* export their data
* move to another application
* maintain local copies
* use open formats
* cancel a service
* replace hardware

then providers have an incentive to remain useful.

This is healthy.

The user stays because the software is good.

Not because leaving would destroy their digital life.

---

# Ownership and Competition

Portability encourages competition.

If applications can interoperate, developers must compete on:

* quality
* usability
* performance
* features
* reliability
* support

rather than merely preventing migration.

Intentional Computing therefore favors ecosystems where:

> **The best tool wins because it is the best tool.**

Not because the user is trapped.

---

# Ownership and Freedom

Ownership does not mean unlimited freedom.

Systems have constraints.

Hardware has physical limits.

Software has licenses.

Networks have rules.

Security requires boundaries.

Other people's rights matter.

Intentional Computing therefore uses a practical definition:

> **Ownership means meaningful control within the legitimate boundaries of the system.**

The objective is not absolute control.

It is avoiding unnecessary surrender of control.

---

# The Ownership Hierarchy

A useful way to think about ownership is:

```text id="9xk6df"
LEVEL 1
Can I use it?

        ↓

LEVEL 2
Can I access my data?

        ↓

LEVEL 3
Can I copy my data?

        ↓

LEVEL 4
Can I export my data?

        ↓

LEVEL 5
Can I move my data?

        ↓

LEVEL 6
Can I replace the software?

        ↓

LEVEL 7
Can I preserve the environment?

        ↓

LEVEL 8
Can I understand and control important behavior?
```

The higher the system goes, the stronger the user's practical ownership.

---

# The Ownership Test

Every Intentional Computing project should ask:

### Data

1. Where is the user's data stored?
2. Can the user access it directly?
3. Can the user copy it?
4. Can the user back it up?
5. Can the user export it?
6. Can the user delete it?

### Portability

7. Can data be moved to another application?
8. Are open or documented formats supported?
9. Is migration possible?

### Dependencies

10. Does the application require an account?
11. Does it require a remote service?
12. What happens if that service disappears?
13. What happens if the subscription ends?

### Control

14. Can the user configure important behavior?
15. Are important network connections understandable?
16. Can the user disable unnecessary external services?

### AI

17. What can AI access?
18. Where does AI processing occur?
19. What information is retained?
20. Can AI memory be inspected and deleted?

### Exit

21. Can the user leave without losing their work?

If the answer to the final question is yes, the system is much closer to genuine personal computing.

---

# Ownership Is a Relationship

Ownership should not be understood only as a legal concept.

It is also a relationship between:

```text id="t4q8b7"
PERSON
  │
  ├── understands
  ├── controls
  ├── maintains
  ├── backs up
  ├── modifies
  ├── moves
  └── preserves
       │
       ↓
    COMPUTER
```

The stronger this relationship is, the more personal the computer becomes.

The weaker it is, the more the computer becomes a gateway to somebody else's platform.

---

# The 90s Principle

The 1990s are useful here not because everything about that era was better.

They are useful because personal computing still strongly communicated:

> **This machine is yours.**

You could install software from a disc.

You could copy files.

You could write programs.

You could open directories.

You could configure the machine.

You could replace applications.

You could unplug the network.

The technology was dramatically less capable than today's technology.

But the relationship was often more direct.

Intentional Computing wants the modern equivalent:

> **The power of modern computing with the sense of ownership of personal computing.**

---

# The Modern Principle

Modern technology gives us capabilities that earlier generations could not imagine.

We can now:

* run powerful AI locally
* search enormous information collections
* process massive datasets
* communicate globally
* emulate historical hardware
* create sophisticated media
* automate complex workflows
* build personal information systems

The answer is not to reject these capabilities.

The answer is to put them inside an architecture that respects ownership.

The future should be:

```text id="t1q9h2"
MORE CAPABILITY
       +
MORE OWNERSHIP
       +
MORE CONTROL
       +
LESS DEPENDENCY
```

Not:

```text id="b0w6q1"
MORE CAPABILITY
       +
MORE DEPENDENCY
       +
MORE LOCK-IN
       +
LESS CONTROL
```

---

# Ownership and Intentional Computing

Ownership supports every major principle of Intentional Computing.

### Human Agency

The user controls the environment.

### Attention

The user is less dependent on systems designed to maximize engagement.

### Local-First

Important capabilities can remain available locally.

### Privacy

Personal information can remain under personal control.

### Longevity

Data can survive individual services.

### Simplicity

The relationship between user, machine, and data is clearer.

### Exit

The user can leave without abandoning their work.

---

# The Ideal Personal Computing Environment

The long-term goal can be represented as:

```text id="5d2n8v"
                         PERSON
                           │
                        INTENT
                           │
                           ↓
                ┌───────────────────┐
                │ PERSONAL COMPUTER │
                │                   │
                │ Applications      │
                │ Files             │
                │ AI                │
                │ Search            │
                │ Configuration    │
                │ Archives          │
                └─────────┬─────────┘
                          │
                ┌─────────┴─────────┐
                ↓                   ↓
             LOCAL              NETWORK
                │                   │
                │             Optional Services
                │                   │
                └─────────┬─────────┘
                          ↓
                       RESULT
                          ↓
                     COMPLETION
                          ↓
                         LIFE
```

The person remains at the center.

The computer provides capability.

The network provides optional reach.

The data remains portable.

The user retains the ability to leave.

---

# Final Principle

> **A personal computer should increase what a person can do without decreasing what they control.**

Modern computing should not require people to surrender their files, their privacy, their independence, or their ability to leave in exchange for convenience.

The machine should be powerful.

The software should be useful.

The network should be available.

AI should be capable.

But the person should remain the owner of the environment.

**Own the machine.**

**Own the data.**

**Own the work.**

**Understand the system.**

**Keep the ability to leave.**

That is personal computing.
