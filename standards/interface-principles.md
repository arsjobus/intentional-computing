# Interface Principles

## Introduction

An interface is the point where human intention meets machine capability.

Intentional Computing therefore treats interface design as more than visual presentation.

The interface should help the user:

* understand what the computer is doing
* express what they want
* perform actions directly
* recover from mistakes
* control complexity
* complete tasks
* leave when the task is finished

The interface should not compete with the user's attention.

> **A good interface makes the computer more capable while making the human's experience simpler.**

---

# 1. The Interface Serves the User

The interface exists to help the user accomplish something.

It should not exist primarily to:

* increase engagement
* promote content
* generate clicks
* collect attention
* encourage repeated interaction
* advertise unrelated features

Every significant interface element should have a reason to exist.

---

# 2. Make the Primary Task Obvious

When the user opens an application, they should be able to understand:

* what the application does
* what they can do
* where to begin

The primary action should not be buried underneath secondary features.

Prefer:

```text
Open Application
       ↓
Primary Task
       ↓
Result
```

over:

```text
Open Application
       ↓
Dashboard
       ↓
Promotions
       ↓
Recommendations
       ↓
Notifications
       ↓
Menus
       ↓
Maybe eventually find the task
```

---

# 3. One Primary Interface Goal

Each screen should have a primary purpose.

Ask:

> What should the user be able to accomplish here?

Secondary actions can exist.

But they should not compete equally with the primary task.

---

# 4. Reduce Cognitive Load

The computer can process enormous amounts of information.

The user should not have to.

Prefer:

```text
Complex system
      ↓
Processing
      ↓
Clear result
```

over:

```text
Complex system
      ↓
Expose every internal detail
      ↓
User interprets everything manually
```

Complexity should be absorbed by the machine whenever doing so preserves clarity and control.

---

# 5. Make Important Information Visible

Important state should not be hidden.

The user should be able to determine things such as:

* what is selected
* what mode is active
* what file is open
* what operation is running
* whether changes are saved
* whether the network is being used
* whether AI is active
* what filters are applied

If something materially affects the result, the user should be able to discover it.

---

# 6. Prefer Direct Manipulation

When practical, allow users to interact directly with the thing they are working on.

Examples:

* click an object
* drag an object
* resize an object
* edit text directly
* move a tile
* select a region
* rearrange items

Direct manipulation creates a strong relationship between:

```text
Action → Result
```

The user should not need to understand the internal architecture to perform ordinary work.

---

# 7. Make Controls Predictable

Controls should behave consistently.

For example:

* buttons should look like buttons
* menus should behave like menus
* selections should remain visible
* dragging should behave consistently
* keyboard shortcuts should follow conventions
* confirmation dialogs should use consistent language

Do not make every application interaction a puzzle.

---

# 8. Prefer Familiar Conventions

Existing conventions are valuable.

Use familiar patterns when they work:

* `Ctrl/Cmd + S` for save
* `Ctrl/Cmd + Z` for undo
* standard file dialogs
* standard menus
* standard keyboard navigation
* conventional scroll behavior

Innovation is useful when it solves a real problem.

Novelty by itself is not.

---

# 9. Make Actions Discoverable

Users should be able to discover important functionality without reading a manual.

Good interfaces provide:

* visible controls
* sensible menus
* contextual actions
* keyboard shortcuts
* tooltips where useful
* clear labels

Power should not require memorizing hidden commands.

---

# 10. Do Not Hide Everything Behind Icons

Icons can be useful.

But ambiguous icons increase cognitive load.

For important actions, prefer:

```text
[ Save ]
[ Export ]
[ Delete ]
```

over unexplained symbols.

Icons should supplement language rather than replace it everywhere.

---

# 11. Use Clear Language

Interface language should be:

* direct
* concise
* specific
* understandable

Prefer:

> Delete 3 selected files?

over:

> Are you sure?

Prefer:

> Connection unavailable.

over:

> Something went wrong.

Technical detail can be available when useful, but the primary interface should communicate clearly.

---

# 12. Make the Current State Obvious

The user should always be able to answer:

> Where am I?

> What am I editing?

> What mode am I in?

> What is selected?

> What will happen if I click this?

Visual state should communicate the answer.

---

# 13. Use Selection Clearly

Selected objects should be visually distinguishable.

This is especially important in:

* editors
* graphics applications
* file managers
* lists
* tables
* tile editors
* development tools

Selection should never be ambiguous.

---

# 14. Make Modes Explicit

If an application has modes, the current mode should be obvious.

For example:

```text
SELECT
DRAW
ERASE
PAN
ZOOM
```

The user should not have to remember an invisible mode.

---

# 15. Avoid Hidden Modes When Possible

Modes can make software powerful.

They can also make software confusing.

If direct manipulation can eliminate a mode without sacrificing capability, consider doing so.

Every additional mode increases the amount of state the user must remember.

---

# 16. Keep Navigation Shallow

Users should not need to travel through many layers of menus to perform common tasks.

Prefer:

```text
File → Export
```

over:

```text
Menu
  ↓
Tools
  ↓
Advanced
  ↓
Project
  ↓
Output
  ↓
Export
```

Deep hierarchies should be reserved for genuinely complex systems.

---

# 17. Provide Multiple Paths for Important Actions

Important actions may be accessible through:

* menu
* toolbar
* keyboard shortcut
* context menu
* command palette

This allows beginners and advanced users to work naturally.

The interface should not force everyone into the same interaction style.

---

# 18. Keyboard Access Matters

Common tasks should be possible without requiring constant mouse interaction where practical.

Support:

* keyboard navigation
* shortcuts
* focus indicators
* tab navigation
* escape/cancel
* standard editing commands

Keyboard interaction is not merely an accessibility feature.

It is also a productivity feature.

---

# 19. Mouse and Pointer Interaction Should Be Precise

Pointer-based interfaces should provide:

* reasonable target sizes
* predictable hit areas
* clear hover state
* clear selection
* sensible dragging behavior

Do not make important controls unnecessarily small.

---

# 20. Respect Screen Space

Interface elements should justify the space they occupy.

Avoid unnecessary:

* banners
* promotional areas
* oversized navigation
* decorative panels
* persistent recommendations
* empty dashboard widgets

The user's work should receive priority.

---

# 21. Content Comes Before Chrome

The application interface should support the user's work.

The work itself should remain the visual priority.

For example, in a graphics editor:

```text
Canvas
████████████████████

Tools
Layers
Palette
```

The canvas should not become a small window surrounded by interface machinery.

---

# 22. Use Progressive Disclosure

Advanced functionality should be available without overwhelming beginners.

Prefer:

```text
Basic Options
    ↓
Advanced Options
```

rather than displaying every setting simultaneously.

Progressive disclosure should hide complexity, not capability.

---

# 23. Configuration Should Be Discoverable

Users should be able to find important configuration.

Avoid settings that exist only in:

* hidden files
* undocumented environment variables
* obscure command-line flags

Technical configuration can exist.

But important user-facing behavior should have an understandable path to configuration.

---

# 24. Defaults Should Reflect the Philosophy

The first experience should already be reasonable.

Default settings should favor:

* privacy
* simplicity
* useful functionality
* local storage
* finite results
* low interruption
* safe behavior

Users should not need to configure the application into behaving responsibly.

---

# 25. Do Not Manipulate Through Defaults

Never use defaults to encourage behavior the user did not explicitly request.

Examples of questionable defaults include:

* unnecessary notifications
* automatic sharing
* automatic publication
* unnecessary telemetry
* infinite content loading
* aggressive recommendations
* automatic subscription
* persistent background activity

Defaults should serve the user.

---

# 26. Make Important Actions Reversible

Whenever possible:

```text
Action
 ↓
Undo
```

should be available.

For more complex operations:

```text
Action
 ↓
Preview
 ↓
Confirm
 ↓
Execute
```

may be appropriate.

The more destructive the action, the stronger the protection should be.

---

# 27. Confirmation Should Be Proportional

Do not ask for confirmation constantly.

Too many confirmations train users to click through them.

Use confirmation when:

* data may be permanently lost
* external communication will occur
* an important setting will change
* an irreversible operation will happen

Routine reversible actions should generally remain fast.

---

# 28. Preview Before Expensive or Destructive Actions

When an operation has significant consequences, provide a preview where practical.

Examples:

```text
Export Preview
Build Preview
Delete Preview
Batch Operation Preview
AI Change Preview
```

The user should understand the result before committing when the cost of being wrong is high.

---

# 29. Show Progress

Long operations should communicate progress.

Useful information includes:

* current operation
* progress
* number completed
* estimated remaining work
* ability to cancel

For example:

```text
Processing files

37 / 100 complete

[Cancel]
```

---

# 30. Cancellation Should Work

If an operation can reasonably be cancelled, provide cancellation.

The user should not have to:

> Force quit the application.

to stop an operation.

---

# 31. Do Not Block Unnecessarily

Long-running work should not freeze unrelated interface functionality.

Prefer:

```text
Application remains responsive
       ↓
Background work
       ↓
Progress
```

over:

```text
Application freezes
       ↓
User wonders whether it crashed
```

---

# 32. Errors Should Explain What Happened

Good error messages answer:

1. What happened?
2. Why?
3. What can I do?

Example:

> Unable to save `project.mirage` because the destination disk is full.

Then provide an appropriate recovery path.

---

# 33. Errors Should Preserve Context

Do not throw the user into an unrelated error screen when something fails.

Keep:

* current document
* current selection
* current task
* relevant settings

where possible.

The error should interrupt the task as little as possible.

---

# 34. Empty States Should Be Useful

An empty state should explain what the user can do next.

Instead of:

> No items.

Prefer:

> No projects yet. Create a project to begin.

An empty screen is an opportunity to establish the intended workflow.

---

# 35. Loading States Should Be Honest

Do not display fake progress.

If the system does not know how long something will take, say so.

Prefer:

> Searching...

over a progress bar that claims:

> 73%

when the number has no meaningful basis.

---

# 36. Distinguish Waiting From Failure

The interface should communicate whether the application is:

* working
* waiting
* blocked
* failed
* complete

These states should not look identical.

---

# 37. Use Animation Purposefully

Animation can communicate:

* transition
* cause and effect
* state change
* spatial relationship

It should not exist simply to make software feel more stimulating.

Avoid unnecessary:

* bouncing
* pulsing
* attention-grabbing movement
* automatic motion
* decorative transitions

---

# 38. Respect Reduced Motion

Where practical, support reduced-motion preferences.

Motion should never be required to understand the interface.

---

# 39. Visual Hierarchy Should Reflect Importance

The visual hierarchy should communicate:

```text
Primary
  ↓
Secondary
  ↓
Optional
```

Do not give every control equal visual weight.

If everything is emphasized, nothing is emphasized.

---

# 40. Avoid Visual Noise

Avoid unnecessary:

* badges
* gradients
* shadows
* animations
* decorative icons
* banners
* alerts
* competing colors

Visual simplicity is not the same as lack of capability.

A powerful interface can remain visually calm.

---

# 41. Use Color Intentionally

Color should communicate meaning.

For example:

* error
* warning
* success
* selection
* disabled state

Do not use color merely to attract attention.

Important information should not depend exclusively on color.

---

# 42. Accessibility Is Interface Quality

Interfaces should consider:

* readable text
* sufficient contrast
* keyboard navigation
* screen readers
* focus indicators
* text scaling
* alternative input
* reduced motion

Accessibility improves the interface for everyone.

---

# 43. Do Not Depend on Hover Alone

Important information or functionality should not be available only through hover.

Hover does not exist on every device.

Critical actions should have another access path.

---

# 44. Respect Platform Conventions

Applications should generally respect the conventions of the operating system they run on.

Examples include:

* window behavior
* menus
* keyboard shortcuts
* file dialogs
* clipboard
* copy/paste
* drag and drop
* accessibility APIs
* system appearance

A cross-platform application does not need to look identical everywhere.

It should feel appropriate to the platform.

---

# 45. Do Not Over-Abstract the Interface

Not every operation needs:

* a wizard
* a modal
* an AI assistant
* a dashboard
* a multi-step workflow

Sometimes the best interface is simply:

```text
[Button]
```

or:

```text
File → Open
```

Use the simplest interaction that provides the required capability.

---

# 46. Prefer Non-Modal Interaction

Modals interrupt context.

Use them when the user genuinely needs to make a decision before continuing.

Avoid using modals for:

* advertisements
* recommendations
* unnecessary announcements
* routine information
* unrelated promotions

The interface should not constantly interrupt the task.

---

# 47. Preserve Context

When moving between views, preserve useful context.

Examples:

* selected file
* current document
* search query
* filters
* scroll position
* current zoom
* current tool

The interface should feel like one continuous environment rather than a collection of disconnected screens.

---

# 48. Search Interfaces Should Be Intentional

Search should provide:

* clear input
* visible query
* understandable filters
* predictable sorting
* finite results where practical
* useful empty states

Search results should help answer:

> What did the system find?

not:

> How long can I continue browsing?

---

# 49. Filtering Should Be Visible

If results are being filtered, the user should be able to see the active filters.

For example:

```text
Search: game development

Filters:
[Educational]
[No Influencers]
[No Shorts]
[Technical]
```

Invisible filtering creates uncertainty.

---

# 50. Sorting Should Be Predictable

If the user chooses:

```text
Newest
```

the results should actually be ordered by newest.

The meaning of sorting options should be clear.

Avoid hidden ranking behavior that contradicts the visible controls.

---

# 51. Recommendations Must Remain User-Directed

Recommendations can be useful.

But they should not silently become an endless content environment.

Prefer:

```text
You asked for:
Game development tutorials

Here are 10 selected results.
```

over:

```text
Recommended for you
↓
More
↓
More
↓
More
```

---

# 52. AI Interfaces Should Be Bounded

AI should have a defined role.

For example:

```text
User
 ↓
Search
 ↓
AI filtering
 ↓
Results
```

is often preferable to:

```text
User
 ↓
Ask AI everything
 ↓
AI becomes the entire interface
```

AI should complement direct interaction.

---

# 53. Show When AI Is Acting

If AI is:

* filtering
* generating
* modifying
* ranking
* deleting
* classifying

the interface should make that clear where it materially affects the result.

The user should not have to guess whether a result came from a deterministic rule or an AI system.

---

# 54. Give AI Operations Clear Boundaries

An AI action should communicate:

* what it is allowed to change
* what it is changing
* what it did
* whether the action can be undone

The user should never need to wonder:

> What did the AI just do?

---

# 55. Keep AI Suggestions Separate From User Actions

Where practical, distinguish:

```text
AI suggestion
```

from:

```text
User decision
```

For example:

```text
Suggested changes: 14

[Review]
[Apply All]
[Cancel]
```

This preserves agency while still providing automation.

---

# 56. Do Not Manufacture Conversation

Not every application needs a chatbot.

Do not add conversational interfaces merely because they are fashionable.

If a button, menu, search field, or direct manipulation is faster and clearer, use it.

---

# 57. Interfaces Should Be Calm

A calm interface generally has:

* few unnecessary alerts
* limited animation
* clear hierarchy
* predictable controls
* finite information
* intentional defaults
* little promotional content
* no artificial urgency

Calm does not mean weak.

It means the interface does not constantly demand attention.

---

# 58. Interfaces Should Be Dense When Appropriate

Intentional Computing does not require minimalism at all costs.

Professional tools may legitimately contain:

* toolbars
* panels
* inspectors
* timelines
* status bars
* menus
* keyboard shortcuts

The goal is not to remove functionality.

The goal is to organize functionality so that complexity remains understandable.

---

# 59. Expert Interfaces Should Reward Learning

Advanced users should be able to become faster.

Support:

* shortcuts
* command palettes
* scripting
* automation
* batch operations
* customizable layouts
* power-user workflows

A simple interface should not become a permanently limited interface.

---

# 60. Interfaces Should Support Creation

Computers are tools for making things.

Interfaces should support:

* writing
* programming
* drawing
* editing
* organizing
* designing
* building
* experimenting

The goal is not merely to consume information.

---

# 61. The Interface Should Disappear During Deep Work

When the user is doing focused work, unnecessary interface elements should recede.

Examples:

* distraction-free writing
* canvas-focused editing
* full-screen development
* presentation mode
* focused terminal sessions

The interface should support concentration rather than interrupt it.

---

# 62. Do Not Confuse Simplicity With Restriction

A simple interface can still expose substantial power.

Good simplicity means:

> **The complexity exists where it belongs.**

It should exist inside the software rather than inside the user's mental workload.

---

# 63. Preserve User Knowledge

Users build mental models of software.

Avoid changing:

* terminology
* keyboard shortcuts
* control locations
* interaction behavior

without good reason.

Consistency allows knowledge to accumulate.

---

# 64. Interfaces Should Be Learnable

A new user should be able to begin without reading extensive documentation.

An experienced user should be able to become efficient.

A good interface supports both:

```text
Discoverability
      +
Efficiency
```

---

# 65. Interface Changes Should Have a Reason

Do not redesign an interface simply because:

* a trend changed
* a competitor changed
* the application needs to look new
* a framework changed
* visual novelty is desired

Change the interface when the change improves the user's experience or capability.

---

# 66. The Interface Should Not Lie

Visual presentation should accurately represent system state.

Do not:

* show saved when work is unsaved
* show connected when disconnected
* show completed when processing
* show deleted when data remains
* imply human review when AI made the decision

Trust depends on accurate representation.

---

# 67. The User Should Know What Happens Next

Actions should produce understandable consequences.

For example:

```text
[Export]

→ Choose location
→ Export
→ "Export complete"
```

Avoid interactions where the user cannot predict the result.

---

# 68. Keep Feedback Close to the Action

When an action occurs, feedback should appear near the relevant context where practical.

Examples:

```text
[Save] → Saved
```

```text
Delete → Item removed
```

```text
Export → Export complete
```

Immediate feedback builds confidence.

---

# 69. Do Not Overuse Notifications

Most application feedback does not need to become a system notification.

Use local interface feedback when the user is already inside the application.

Reserve system-level notifications for information that genuinely needs attention outside the application.

---

# 70. Respect the User's Time

Interfaces should minimize unnecessary steps.

Ask:

> Can this task be completed in fewer intentional actions?

But do not remove necessary steps merely to make interaction faster.

The goal is:

> **Efficient without being reckless.**

---

# 71. The Interface Should Support Stopping

When the task is finished, the interface should communicate completion.

For example:

```text
Export complete.
```

Then the user can close the application.

There should be no:

```text
Recommended next action
↓
Another task
↓
Another feature
↓
Another notification
```

unless the user explicitly wants it.

---

# Interface Quality Test

Before shipping an interface, ask:

### Intent

* Is the primary purpose obvious?
* Can the user begin immediately?

### Clarity

* Is important state visible?
* Are controls understandable?
* Are errors useful?

### Control

* Can users undo important actions?
* Can they configure important behavior?
* Can they cancel long operations?

### Attention

* Does the interface interrupt unnecessarily?
* Does it encourage endless interaction?
* Are there natural stopping points?

### Accessibility

* Can the interface be used with a keyboard?
* Is text readable?
* Is important information communicated without relying only on color?

### AI

* Is AI's role clear?
* Can AI actions be reviewed or reversed?
* Does AI reduce complexity?

### Ownership

* Can the user access their data?
* Can they export it?
* Can they leave?

### Longevity

* Does the interface use understandable conventions?
* Will existing user knowledge remain useful?

---

# The Core Interface Principles

The entire standard can be reduced to ten rules:

1. **Make the user's intention the center of the interface.**
2. **Make the primary task obvious.**
3. **Make important state visible.**
4. **Prefer direct manipulation and familiar conventions.**
5. **Make important actions reversible.**
6. **Use progressive disclosure instead of unnecessary complexity.**
7. **Keep interfaces calm, finite, and free of artificial urgency.**
8. **Use AI to simplify interaction rather than replace human agency.**
9. **Respect accessibility, platform conventions, and user knowledge.**
10. **When the task is finished, let the interface get out of the way.**

---

# Final Principle

The best interface is not the one that gets the user to interact with it the most.

It is the one that lets the user accomplish what they came to do.

The computer should be powerful.

The interface should be clear.

The controls should be predictable.

The state should be visible.

The actions should be reversible.

The complexity should be absorbed by the machine.

The user's attention should remain theirs.

And when the work is finished:

> **The interface should become quiet.**
