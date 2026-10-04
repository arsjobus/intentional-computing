# Software Principles

## Introduction

Intentional Computing is not only a philosophy.

It is also a way of building software.

These principles translate the broader Intentional Computing philosophy into practical engineering rules that can be applied to applications, tools, libraries, services, and operating environments.

They are not absolute laws.

Technical constraints, security requirements, accessibility needs, performance requirements, and project scope may require exceptions.

But exceptions should be deliberate.

> **Software should be built to increase human capability while minimizing unnecessary dependency, complexity, and attention consumption.**

---

# 1. Build for the User's Intent

Every application should have a clear answer to:

> **What is the user trying to accomplish?**

The software should make that task easier.

Avoid adding features simply because:

* competitors have them
* they increase engagement
* they create more data
* they generate more notifications
* they increase time spent in the application
* they make the product appear more sophisticated

A feature should have a reason to exist.

---

# 2. One Primary Purpose

Every application should have a clearly identifiable primary purpose.

The interface, architecture, and documentation should reinforce that purpose.

An application can grow over time.

But growth should not automatically result in:

```text
Simple Tool
    ↓
Feature
    ↓
Feature
    ↓
Feature
    ↓
Platform
    ↓
Everything App
```

More functionality does not automatically mean better software.

Prefer focused tools that work well.

---

# 3. Completion Is a Feature

Software should help users finish tasks.

The intended lifecycle is:

```text
INTENT
  ↓
ACTION
  ↓
RESULT
  ↓
COMPLETION
```

A successful interaction may therefore end quickly.

Do not interpret a user leaving the application as failure.

If the task is complete, the software has succeeded.

---

# 4. Do Not Optimize for Engagement

Avoid optimizing software around:

* session length
* daily active users
* repeated interactions
* endless scrolling
* notification frequency
* return frequency
* compulsive usage

These measurements can be useful in some contexts, but they should not become the primary definition of success for Intentional Computing software.

Prefer measuring:

* task completion
* accuracy
* usefulness
* reliability
* user satisfaction
* productivity
* time saved
* successful outcomes

---

# 5. Prefer Finite Interfaces

When a task has a natural endpoint, the interface should expose that endpoint.

Prefer:

```text
Page 1
Page 2
Page 3
...
Page 10
```

over:

```text
Keep scrolling forever.
```

Prefer:

```text
20 useful results
```

over:

```text
More results loading...
```

Finite interfaces make systems easier to understand.

They also create natural stopping points.

---

# 6. Search Before Feeds

When users know what they want, search should be available.

Prefer:

```text
User intent
    ↓
Search
    ↓
Results
```

over:

```text
Open application
    ↓
Algorithmic feed
    ↓
More feed
    ↓
More feed
    ↓
Maybe eventually find something useful
```

Recommendation can still be useful.

But it should complement search rather than replace intentional discovery.

---

# 7. Curation Over Volume

The goal is not to expose the user to the maximum amount of information.

The goal is to expose the user to useful information.

Prefer:

```text
1000 candidates
      ↓
Filtering
      ↓
Classification
      ↓
Deduplication
      ↓
20 useful results
```

over:

```text
1000 results
      ↓
User manually sorts everything
```

Machines should absorb information-processing complexity.

---

# 8. User-Defined Rules Are First-Class

Whenever software filters, ranks, recommends, or classifies information, users should have meaningful control over the criteria where practical.

Examples include:

* excluded categories
* preferred sources
* preferred formats
* blocked terms
* quality thresholds
* ranking preferences
* notification rules
* privacy settings

The system should not assume that its developer's preferences are the user's preferences.

---

# 9. Defaults Should Be Intentional

Most users do not change defaults.

Therefore:

> **Defaults are part of the product's philosophy.**

Default behavior should generally favor:

* privacy
* local storage
* finite results
* minimal notifications
* clear interfaces
* user control
* reversible actions
* explicit permissions

Do not make the user fight the software to obtain the intended behavior.

---

# 10. Prefer Direct Manipulation

When a task can be performed naturally through direct interaction, support it.

Examples:

* drag files
* click objects
* edit text
* move tiles
* resize panels
* select items
* manipulate graphics

AI and automation can complement direct manipulation.

They should not automatically replace it.

---

# 11. Make State Visible

The user should be able to understand the current state of the application.

Important state should not be hidden behind assumptions.

Examples include:

* selected object
* active tool
* current file
* current mode
* current filter
* synchronization status
* save status
* processing state
* network status

The interface should communicate what the machine believes is happening.

---

# 12. Prefer Reversible Actions

Where practical, actions should be reversible.

Support:

* undo
* redo
* cancel
* restore
* version history
* backups

Especially for destructive operations.

The more powerful automation becomes, the more important reversibility becomes.

---

# 13. Do Not Hide Destructive Actions

Destructive operations should be explicit.

Examples:

* delete
* overwrite
* replace
* publish
* remove
* permanently discard

The user should understand what will happen before it happens.

Do not use ambiguous labels such as:

> "Continue"

when the actual action is:

> "Delete permanently."

---

# 14. Use Progressive Complexity

Software should not expose every possible option immediately.

Prefer:

```text
Simple Default
      ↓
Common Options
      ↓
Advanced Options
```

This keeps the primary interface understandable while preserving power for advanced users.

Complexity should be available without becoming mandatory.

---

# 15. Configuration Over Hidden Behavior

If behavior matters, make it configurable when practical.

Prefer:

```text
Settings
  ├── Search Sources
  ├── Filters
  ├── Storage
  ├── Network
  └── AI
```

over undocumented behavior buried inside the application.

Configuration should be understandable.

---

# 16. Local-First Where Practical

Applications should perform work locally whenever reasonably possible.

Prefer local:

* files
* configuration
* caching
* search indexes
* databases
* processing
* AI inference where practical

Use remote services when they provide genuine value.

The network should extend the application rather than define it.

---

# 17. Do Not Require Accounts Without a Reason

A local application should not require an account merely to start using it.

Accounts should exist for genuine requirements such as:

* synchronization
* collaboration
* remote services
* purchases
* identity
* multiplayer

Avoid account requirements that exist primarily for:

* analytics
* marketing
* data collection
* engagement tracking

---

# 18. Make Data Portable

Users should be able to access and move their work.

Support:

* import
* export
* backup
* standard formats
* documented formats

Where practical, the application should not trap data inside itself.

---

# 19. Minimize Dependencies

Every dependency creates:

* maintenance cost
* security exposure
* compatibility risk
* upgrade pressure
* preservation risk

Use dependencies when they provide meaningful value.

Do not add dependencies simply because they are convenient.

A small, understandable system is often more resilient than a large dependency graph.

---

# 20. Prefer Boring Technology

Technology should be selected for suitability rather than novelty.

Prefer mature technologies when they adequately solve the problem.

Consider:

* stability
* maintainability
* documentation
* portability
* community support
* longevity
* complexity

The newest technology is not automatically the best technology.

---

# 21. Keep Architecture Understandable

A developer should be able to explain the application's architecture without requiring a diagram containing hundreds of components.

Prefer clear boundaries:

```text
UI
 ↓
Application Logic
 ↓
Domain Logic
 ↓
Storage / External Services
```

Complex systems may require more layers.

But each layer should have a reason to exist.

---

# 22. Separate Concerns

Keep responsibilities distinct.

For example:

```text
Interface
    ↓
Application
    ↓
Domain
    ↓
Infrastructure
```

This improves:

* testing
* maintenance
* replacement
* understanding
* debugging

Avoid systems where every component knows everything about every other component.

---

# 23. Make Components Replaceable

Important components should have clear boundaries.

If one component must eventually be replaced, the architecture should make replacement possible without rewriting the entire system.

Examples:

* storage provider
* AI model
* search engine
* network source
* rendering system
* export format

Replaceability reduces dependency.

---

# 24. Avoid Artificial Platform Lock-In

Do not design software around unnecessary proprietary infrastructure.

Where practical:

* use standard protocols
* use open formats
* document interfaces
* separate data from application logic
* provide exports
* avoid proprietary dependencies where alternatives are practical

The user should not be trapped by architecture.

---

# 25. Network Boundaries Should Be Clear

Applications should make external communication understandable.

Document:

* what communicates externally
* why it communicates
* what information is sent
* what services are contacted
* what happens without the network

Avoid unnecessary background communication.

---

# 26. Graceful Offline Behavior

If a network-dependent feature fails, unrelated local functionality should continue.

For example:

```text
Network unavailable

Local files       ✓
Local editing     ✓
Local search      ✓
Local settings    ✓

Remote sync       ✗
Online search     ✗
Remote AI        ✗
```

Failure of one capability should not unnecessarily destroy the whole application.

---

# 27. AI Must Have a Defined Role

Do not add AI simply because AI is fashionable.

Before adding AI, define:

* what problem it solves
* what data it needs
* what authority it has
* what happens when it is wrong
* whether local AI is practical
* whether the task could be solved more simply

AI should solve a real problem.

---

# 28. Limit AI Permissions

AI should receive only the permissions necessary for the task.

For example:

```text
Document summarization
    ↓
Read selected documents
    ↓
Generate summary
```

It should not automatically receive:

```text
Full filesystem
Email
Passwords
Financial accounts
Publishing permissions
```

Permissions should be proportional to the task.

---

# 29. Human Override

AI decisions should be overridable where practical.

Support:

* correction
* undo
* manual classification
* rejection
* rule changes
* confirmation

Automation should remain subordinate to user intent.

---

# 30. Make AI Decisions Explainable Where Practical

When AI affects important behavior, provide useful context.

For example:

```text
Filtered

Reason:
Matched user rule:
"Exclude reaction content"

Confidence:
92%
```

The explanation does not need to expose internal model mechanics.

It needs to explain the application's behavior.

---

# 31. Allow AI to Fail Safely

AI systems will make mistakes.

Design for that.

Prefer:

```text
Uncertain
    ↓
Review
```

over:

```text
Uncertain
    ↓
Automatic irreversible action
```

The greater the consequence, the stronger the human confirmation should be.

---

# 32. Use AI to Compress Complexity

A useful rule is:

> **The machine should absorb complexity so the human can see clarity.**

AI should handle:

* classification
* search
* summarization
* repetitive transformations
* pattern recognition
* large-scale analysis

The user should receive useful results rather than unnecessary implementation details.

---

# 33. Do Not Make AI Mandatory

If an application can reasonably perform a task without AI, users should generally have a non-AI path.

AI may improve the experience.

It should not automatically become the only interface.

---

# 34. Performance Is a Feature

Software should feel responsive.

Pay attention to:

* startup time
* input latency
* rendering
* memory usage
* disk usage
* network waits
* background processing

Do not assume modern hardware makes inefficiency irrelevant.

Performance affects the user's experience directly.

---

# 35. Long Operations Need Feedback

If an operation takes time, show useful progress.

Examples:

```text
Searching...
42 / 100 sources processed
```

or:

```text
Classifying
Batch 4 / 7
```

The user should know:

* that work is happening
* what is happening
* approximately how far it has progressed
* whether it can be cancelled

---

# 36. Never Pretend Work Is Finished

Software should distinguish between:

* queued
* running
* completed
* failed
* cancelled
* partially completed

Do not display success before the operation actually succeeds.

Trust depends on accurate state.

---

# 37. Errors Should Be Useful

An error message should answer:

1. What happened?
2. Why did it happen?
3. What can the user do?

Prefer:

> "Unable to open project because the file format is unsupported."

over:

> "Error 0x8004."

Technical details can be available for debugging.

The primary message should help the person.

---

# 38. Do Not Punish the User for Errors

Error recovery should be straightforward.

Prefer:

```text
Operation failed

[Retry]
[Choose Another File]
[Cancel]
```

over:

```text
Operation failed.

Restart application.
```

Errors should be recoverable where possible.

---

# 39. Logging Should Help Humans

Logs are valuable for development and troubleshooting.

They should contain useful information such as:

* timestamps
* operation
* relevant state
* errors
* warnings
* source
* duration

Avoid logging sensitive information unnecessarily.

Logs should help explain what happened.

---

# 40. Privacy by Default

Collect only what is necessary.

Prefer:

```text
Local processing
```

over:

```text
Upload everything
```

when both are technically viable.

Do not collect personal information simply because storage is inexpensive.

---

# 41. Telemetry Should Have a Purpose

If telemetry exists, there should be a legitimate reason.

Ask:

* What is being collected?
* Why?
* Is it necessary?
* Can it be disabled?
* Is it anonymous?
* How long is it retained?

Telemetry should improve the software.

It should not become surveillance.

---

# 42. Notifications Must Earn Their Place

Notifications should be:

* useful
* relevant
* timely
* controllable

Avoid notifications designed primarily to bring the user back into the application.

The default should favor calm computing.

---

# 43. No Artificial Urgency

Avoid unnecessary:

* countdowns
* streaks
* warnings
* badges
* red indicators
* "you might miss this" messages
* forced reminders

If something is genuinely urgent, communicate it clearly.

Do not manufacture urgency.

---

# 44. Respect the User's Attention

Applications should avoid unnecessary interruption.

Prefer:

```text
User requests information
        ↓
Information appears
```

over:

```text
Application interrupts user
        ↓
Notification
        ↓
Another notification
        ↓
Reminder
```

Pull-based interaction is generally preferable to push-based interaction.

---

# 45. Provide Natural Stopping Points

When work is complete, say so.

Examples:

```text
Export complete.
```

```text
Search complete.
20 results found.
```

```text
Build successful.
```

The user should not be encouraged to continue without a reason.

---

# 46. Preserve User Context

Software should avoid unnecessarily destroying the user's state.

Preserve where practical:

* current document
* selection
* workspace
* filters
* scroll position
* recent files
* settings

The computer should remember useful context without becoming invasive.

---

# 47. Make State Recoverable

Applications should protect against accidental loss.

Consider:

* autosave
* recovery files
* transactional updates
* backups
* version history

Recovery should be especially strong for long-running creative or technical work.

---

# 48. Design for Interruption

Real people get interrupted.

Applications should tolerate:

* closing unexpectedly
* losing power
* losing network
* switching tasks
* cancelling operations
* temporary failures

Software should recover gracefully.

---

# 49. Test the Failure Paths

Testing should include more than the successful case.

Test:

* missing files
* invalid input
* corrupted data
* network failure
* service failure
* AI failure
* insufficient storage
* interrupted operations
* permission errors
* unexpected shutdown

A resilient application expects things to go wrong.

---

# 50. Security Is Part of User Control

Security should protect the user's ownership and agency.

Consider:

* least privilege
* secure storage
* authentication where necessary
* safe updates
* dependency vulnerabilities
* input validation
* sandboxing where appropriate

Security should not become an excuse for unnecessary lock-in.

---

# 51. Updates Should Not Break Ownership

Software updates should preserve:

* user data
* configuration
* supported formats
* existing workflows

Where breaking changes are necessary:

* explain them
* provide migration
* provide backups
* document the change

The user should not fear updating software.

---

# 52. Compatibility Matters

Software should respect established formats and interfaces where practical.

Compatibility extends the useful life of:

* files
* hardware
* software
* projects
* archives

Do not break compatibility simply to force migration.

---

# 53. Documentation Is Part of the Product

A project is not complete when the code compiles.

Documentation should explain:

* installation
* usage
* configuration
* architecture
* dependencies
* file formats
* limitations
* troubleshooting
* development

Good documentation is a form of user control.

---

# 54. Document Important Decisions

Architectural decisions should be recorded.

Useful documentation includes:

* README
* architecture documentation
* design decisions
* roadmap
* changelog
* migration notes

Future developers should be able to understand why the system works the way it does.

---

# 55. Keep Development Reproducible

Projects should make it reasonably easy to reproduce a working development environment.

Document:

* language versions
* build tools
* dependencies
* environment variables
* build commands
* test commands

Where practical, pin important dependencies.

---

# 56. Prefer Small, Composable Systems

A collection of focused components can be easier to understand than a giant integrated system.

For example:

```text
Search
  ↓
Filtering
  ↓
Classification
  ↓
Ranking
  ↓
Presentation
```

Each component has a clear responsibility.

This makes the system easier to test and replace.

---

# 57. Do Not Over-Engineer

Intentional Computing does not mean building elaborate systems to satisfy philosophical purity.

Avoid:

* unnecessary abstractions
* excessive frameworks
* premature optimization
* unnecessary microservices
* needless infrastructure
* abstraction for its own sake

The simplest architecture that satisfies the requirements is often the best architecture.

---

# 58. Build for Longevity

Software should be designed with the possibility that:

* the original developer leaves
* a dependency disappears
* a company shuts down
* an API changes
* the internet becomes unavailable
* hardware changes
* operating systems evolve

Prefer technologies and architectures that can survive change.

---

# 59. Make the Project Understandable to Its Future Maintainer

A useful question is:

> **Could someone unfamiliar with this project understand it six months from now?**

They should be able to discover:

```text
What is this?
      ↓
How does it work?
      ↓
How do I run it?
      ↓
Where is the important code?
      ↓
How do I test it?
      ↓
What remains unfinished?
```

Maintainability is a form of longevity.

---

# 60. Build for Exit

Every project should have an exit path.

Users should be able to:

* export data
* remove the application
* stop network access
* replace dependencies
* migrate projects
* continue using their files

Developers should also be able to:

* replace components
* migrate formats
* remove services
* archive the project
* hand maintenance to others

Software should not depend on permanent existence.

---

# 61. Preserve Natural Boundaries

Software should have clear boundaries between:

* user
* application
* operating system
* network
* external services
* AI
* stored data

Clear boundaries make systems easier to reason about.

---

# 62. Prefer Explicitness

Important behavior should be visible in:

* configuration
* code
* documentation
* interface
* logs

Avoid magic where explicit behavior is reasonably possible.

Abstraction is useful.

Mystery is not.

---

# 63. Use Automation Carefully

Automation should remove repetitive work.

It should not remove user control unnecessarily.

A useful rule:

```text
Repetitive + Low Risk
        ↓
Automate

Irreversible + High Risk
        ↓
Confirm
```

The greater the consequence, the greater the need for human oversight.

---

# 64. Separate Automation From Authority

An automated system can perform an action without being given unlimited authority.

For example:

```text
AI
 ↓
Suggest change
 ↓
Human approves
 ↓
Application performs change
```

This is different from:

```text
AI
 ↓
Decides
 ↓
Acts
 ↓
Publishes
```

Authority should be explicitly granted.

---

# 65. Design for Interoperability

Software should communicate with other software where practical.

Useful mechanisms include:

* standard file formats
* documented APIs
* command-line interfaces
* import/export
* standard protocols

Interoperability increases user choice.

---

# 66. Command-Line Interfaces Are Valuable

A graphical interface is not always enough.

For appropriate software, provide a CLI when practical.

CLIs can provide:

* automation
* scripting
* reproducibility
* debugging
* batch processing
* integration

They also provide an interface that can survive changes to the graphical layer.

---

# 67. Human Interfaces Should Be Stable

Avoid changing interfaces merely for novelty.

Users develop knowledge of software.

A stable interface allows that knowledge to compound.

When changes are necessary:

* preserve familiar workflows where possible
* document changes
* avoid needless rearrangement
* provide migration guidance

---

# 68. Accessibility Is a Core Requirement

Intentional Computing is about human agency.

That includes people with different abilities.

Software should consider:

* keyboard access
* screen readers
* text scaling
* contrast
* captions
* alternative input
* reduced motion
* clear focus
* understandable language

Accessibility should be considered during design, not added only at the end.

---

# 69. Avoid Dark Patterns

Do not use interface techniques designed to manipulate users into actions they did not intend.

Avoid:

* deceptive buttons
* hidden cancellation
* confusing opt-outs
* forced subscriptions
* misleading warnings
* fake urgency
* intentionally difficult settings

The interface should communicate honestly.

---

# 70. The User Should Be Able to Leave

This is the final software principle.

A successful application should not need to convince the user to stay.

The user should be able to:

```text
Open
 ↓
Use
 ↓
Finish
 ↓
Close
```

without penalty.

No guilt.

No artificial loss.

No endless feed.

No unnecessary notification.

No attempt to pull the user back.

The software's job is complete.

---

# Engineering Priorities

When tradeoffs are necessary, Intentional Computing generally prioritizes:

```text
1. Human agency
2. Correctness
3. Security
4. Data integrity
5. Reliability
6. Usability
7. Maintainability
8. Performance
9. Portability
10. Convenience
```

The exact ordering may vary by project.

But convenience should not automatically defeat ownership, security, or agency.

---

# The Software Review

Before considering an Intentional Computing application complete, ask:

### Purpose

* Does the application have a clear purpose?
* Does every major feature support that purpose?

### Attention

* Does the application respect attention?
* Are there natural stopping points?
* Is engagement being optimized unnecessarily?

### Ownership

* Does the user control their data?
* Can they export it?
* Can they leave?

### Local-First

* What works offline?
* What requires the network?
* Are those boundaries intentional?

### AI

* Why is AI present?
* Does it reduce complexity?
* Can the user override it?
* Are its permissions limited?

### Architecture

* Is the system understandable?
* Are components replaceable?
* Are dependencies reasonable?

### Reliability

* What happens when things fail?
* Can the user recover?

### Longevity

* Could the software and its data remain usable years from now?

### Exit

* Can the user finish the task and walk away?

If the answers are good, the software is likely aligned with Intentional Computing.

---

# The Core Engineering Principles

The entire document can be reduced to ten rules:

1. **Build for human intent.**
2. **Optimize for useful outcomes, not engagement.**
3. **Make completion a first-class feature.**
4. **Prefer local capability and user ownership.**
5. **Keep data portable.**
6. **Use AI to reduce complexity, not create dependency.**
7. **Make important behavior understandable and reversible.**
8. **Minimize unnecessary dependencies and infrastructure.**
9. **Design for longevity and exit.**
10. **Let the user walk away.**

---

# Final Principle

Software is ultimately a relationship between a person and a machine.

The machine can be extraordinarily powerful.

The software can be extraordinarily sophisticated.

AI can absorb enormous amounts of complexity.

None of that changes the fundamental objective.

> **The software exists to help the person accomplish something they intended to accomplish.**

Build software that is:

**Powerful without being demanding.**

**Intelligent without being controlling.**

**Connected without being dependent.**

**Automated without removing agency.**

**Modern without abandoning ownership.**

**Complex internally, but clear externally.**

And when the user's work is finished:

**let the software get out of the way.**
