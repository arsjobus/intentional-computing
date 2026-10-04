# Intentional Computing — Principles

> **Principles for designing technology that increases capability without unnecessarily consuming attention, agency, or ownership.**

This document translates the Intentional Computing Manifesto into practical design principles.

The manifesto describes what we believe.

These principles describe how we build.

They are guidelines rather than commandments. There will be situations where a principle conflicts with another principle or where practical constraints require compromise. When that happens, the trade-off should be explicit rather than accidental.

---

# 1. Human Agency First

The user should remain the primary decision-maker.

Software should assist a person's decisions rather than quietly making decisions on their behalf.

### Prefer

* explicit choices
* understandable defaults
* user-configurable behavior
* reversible actions
* visible system state
* predictable behavior

### Avoid

* dark patterns
* hidden incentives
* manipulative defaults
* unnecessary automation
* irreversible actions without confirmation
* interfaces designed to pressure the user

### Test

Ask:

> **"Does this feature give the user more control or less?"**

If it gives less control, there should be a compelling reason.

---

# 2. Attention Is Not the Product

A user's attention should not be treated as a resource to maximize.

The goal of software is to accomplish useful work.

Not:

> maximize session length

Not:

> maximize daily active users

Not:

> maximize notifications

Not:

> maximize scrolling

Instead:

> **maximize useful outcomes.**

A user finishing a task quickly is a success.

A user closing the application because they have finished is a success.

---

# 3. Completion Over Engagement

Software should make it easy to finish.

A well-designed application should answer:

> What is the user trying to accomplish?

Then remove unnecessary steps between the user and that outcome.

Examples:

### Good

```text
Search
  ↓
Find useful information
  ↓
Save / use it
  ↓
Done
```

### Bad

```text
Search
  ↓
Recommendation
  ↓
Related recommendation
  ↓
Trending
  ↓
Short video
  ↓
Advertisement
  ↓
Another recommendation
  ↓
Another recommendation
  ↓
...
```

If the user's task is complete, the application should not invent another task.

---

# 4. No Infinite by Default

Infinite systems should be treated with suspicion.

Infinite feeds, endless recommendations, continuous autoplay, and dynamically expanding content streams remove natural stopping points.

Where practical, prefer:

* pages
* collections
* queues
* finite result sets
* explicit "load more"
* explicit search
* completion states

A person should be able to answer:

> **"How much is there?"**

---

# 5. Search Over Feeds

When a person knows what they want, help them find it.

When they do not know what they want, provide useful discovery without creating an endless stream.

Search should generally be preferred over passive consumption.

A good discovery system should produce:

> **a useful selection**

rather than:

> **an infinite supply.**

AI can be especially valuable here by filtering enormous information spaces into manageable collections.

---

# 6. Curation Over Volume

More information is not necessarily more useful.

A system should prioritize:

* relevance
* quality
* clarity
* provenance
* usefulness
* diversity where appropriate

over raw quantity.

Ten excellent results can be more useful than ten thousand mediocre ones.

The objective is not to expose the user to everything.

The objective is to help the user find what matters.

---

# 7. User-Defined Filters Are First-Class Features

People should be able to define what they do not want.

Filtering should not be treated as an obscure advanced option.

A user should be able to say:

```text
I don't want:
- celebrity content
- influencer content
- rage bait
- shock content
- gambling
- endless short-form content
```

And the system should respect those choices.

The user's definition of a useful environment is more important than a platform's generic definition of engagement.

---

# 8. Personalization Without Manipulation

Personalization can be useful.

Manipulation is not.

A system may learn:

> "This person prefers technical explanations."

That can improve search.

It should not become:

> "This person responds strongly to outrage, therefore show more outrage."

Personalization should improve **relevance**, not exploit **vulnerability**.

---

# 9. AI Serves the User

AI should function primarily as an amplifier of human capability.

Good uses include:

* searching
* filtering
* summarizing
* translating
* explaining
* programming
* organizing
* creating
* analyzing
* automating repetitive work

AI should not automatically become:

* an engagement engine
* a persuasion engine
* a notification engine
* a social replacement
* an attention-retention mechanism

The question should always be:

> **"What does the AI make easier for the person?"**

---

# 10. AI Should Compress Complexity

One of the most valuable applications of AI is reducing the amount of complexity a person must personally process.

The internet may contain millions of documents.

The user may need five.

AI should help bridge that gap.

```text
Huge information space
          ↓
        AI
          ↓
Relevant information
          ↓
Human decision
```

AI should reduce the cognitive cost of reaching useful information.

It should not merely increase the amount of information being presented.

---

# 11. Local First Where Practical

Applications should work locally whenever there is a reasonable benefit to doing so.

Prefer:

* local data
* local configuration
* local processing
* offline operation
* local caches
* exportable files

when practical.

Online services are appropriate when they provide genuine value.

But an internet connection should not automatically be a prerequisite for functionality that could reasonably exist locally.

---

# 12. Ownership Over Dependency

Users should be able to retain control of the things they create.

Prefer:

* open file formats
* export
* backups
* migration
* self-hosting
* local copies
* documented storage formats

Avoid unnecessary lock-in.

If a user leaves the software, their work should not disappear with it.

---

# 13. Open Formats

The preferred data format is one that another program can understand.

Where practical:

> **Use documented, portable formats rather than proprietary containers.**

This improves:

* preservation
* interoperability
* longevity
* migration
* user choice

A file should ideally outlive the application that created it.

---

# 14. Minimize Dependencies

Every dependency creates another point of failure.

Prefer:

* simple architectures
* small dependency sets
* mature libraries
* standard technologies
* understandable build systems

Do not add infrastructure simply because it is fashionable.

Complexity should solve a real problem.

---

# 15. Prefer Simple Technology

Use the simplest technology capable of solving the problem well.

A project does not become better because it contains:

* more services
* more frameworks
* more abstraction
* more cloud infrastructure
* more dependencies

Complexity should be justified by capability.

---

# 16. Understandability Matters

A developer should be able to open the project and understand its architecture.

Prefer:

```text
clear structure
+
clear naming
+
clear documentation
+
predictable behavior
```

over:

```text
magic
+
hidden behavior
+
unnecessary abstraction
+
configuration scattered everywhere
```

Software should be maintainable by humans.

---

# 17. Transparency Over Magic

Automation is useful.

Invisible behavior is not.

When software performs an important action, users should be able to understand:

* what happened
* why it happened
* what data was involved
* what can be changed
* how to undo it

This becomes particularly important when AI is involved.

---

# 18. AI Decisions Should Be Inspectable Where Practical

When AI makes a meaningful decision, the system should preserve enough information to understand the decision.

For example:

```text
Decision:
REJECT

Category:
Clickbait

Confidence:
0.91

Reason:
Title and metadata indicate engagement-oriented sensational content.
```

This does not require exposing internal model reasoning.

It means exposing the **decision context and useful explanation**.

---

# 19. User Configuration Is Part of the Product

Configuration should not be an afterthought.

If a user has meaningful preferences, those preferences should be:

* visible
* editable
* persistent
* portable
* documented

A configuration file can sometimes be better than a hidden database setting.

The user should be able to understand:

> **"These are the rules my computer is operating under."**

---

# 20. Defaults Matter

Most users will not configure everything.

Therefore defaults are important.

Defaults should favor:

* privacy
* simplicity
* low interruption
* reasonable security
* local operation
* reversibility
* user control

A default should never exist primarily because it benefits the software provider.

---

# 21. Notifications Must Earn Their Place

Notifications interrupt human activity.

Therefore every notification should have a reason to exist.

Before adding one, ask:

> **"Would the user reasonably want to be interrupted for this?"**

If not, do not notify.

Prefer:

```text
User checks information when ready.
```

over:

```text
Software interrupts user because information exists.
```

---

# 22. No Artificial Urgency

Avoid unnecessary:

* countdown timers
* "trending now"
* "everyone is watching"
* "don't miss out"
* artificial scarcity
* social pressure

Information should be presented because it is useful, not because urgency makes it more clickable.

---

# 23. Preserve Natural Stopping Points

Good interfaces have endings.

Examples:

```text
Search results: 10 items
Task: Complete
Article: Finished
Queue: Empty
Project: Saved
Game: Over
```

These stopping points are valuable.

Do not automatically replace every ending with another recommendation.

---

# 24. Offline Capability Is Valuable

An application that works without the internet can provide:

* reliability
* privacy
* resilience
* ownership
* independence

Offline operation should be considered during architecture rather than added at the end.

---

# 25. Build for Longevity

Software should ideally remain useful after:

* the original developer moves on
* a service shuts down
* a platform changes
* a dependency disappears
* an API changes
* a company changes direction

Favor technologies and formats that have a reasonable chance of surviving those events.

---

# 26. Preservation Is a Feature

Old software should not become inaccessible simply because the original platform disappeared.

Where appropriate, support:

* emulation
* archival formats
* conversion
* documentation
* source preservation
* ROM/tool preservation
* reproducible builds

Computing history is worth keeping.

---

# 27. Create More Than You Consume

Technology should encourage creation.

The ideal computer is not primarily a television.

It is a workshop.

It should help people:

* write
* draw
* program
* compose
* design
* research
* build
* learn
* experiment

Consumption has a place.

Creation should remain central.

---

# 28. The User May Leave

This is one of the strongest principles.

The software should never assume that keeping the user is the objective.

If the user:

* finishes the task
* closes the application
* turns off the computer
* goes outside
* talks to another person
* works on something else

the software has not failed.

**Human life exists outside the application.**

---

# 29. Technology Should Strengthen Real Life

Computing should support:

* relationships
* creativity
* learning
* work
* hobbies
* exploration
* independence
* physical activity
* rest

It should not attempt to become the entirety of a person's environment.

A computer should fit into life.

Life should not have to fit around the computer.

---

# 30. Do Not Confuse Convenience With Progress

A newer technology is not automatically better.

A more automated system is not automatically better.

A more connected system is not automatically better.

A more intelligent system is not automatically better.

Progress should be measured by outcomes such as:

* capability
* autonomy
* reliability
* understanding
* freedom
* quality
* longevity

not simply by technological novelty.

---

# 31. The 90s Are a Reference Point, Not a Requirement

Intentional Computing is inspired by useful properties of earlier personal computing and the early web.

It does not require reproducing their limitations.

We can keep:

* ownership
* simplicity
* personal computing
* deliberate discovery
* local files
* software collections
* finite experiences
* user control

while discarding:

* slow hardware
* limited storage
* insecure systems
* poor accessibility
* primitive networking
* unnecessary technical limitations

The goal is not nostalgia.

The goal is **selective preservation of good ideas**.

---

# 32. Build the Future, Deliberately

We should not reject new technology simply because it is new.

We should evaluate it.

For every new technology, ask:

### What does it enable?

### What does it replace?

### What does it cost?

### What does it make easier?

### What does it make harder?

### Who gains control?

### Who loses control?

### Does it increase human capability?

### Does it increase human dependence?

### Can the user opt out?

### Can the user leave?

These questions should precede adoption.

---

# 33. The Intentional Computing Test

Before shipping a significant feature, evaluate it against five questions:

### 1. Agency

**Does the user remain in control?**

### 2. Attention

**Does this consume attention unnecessarily?**

### 3. Ownership

**Does the user retain access to their data and work?**

### 4. Capability

**Does this genuinely make the user more capable?**

### 5. Exit

**Can the user stop using this without being punished or trapped?**

A feature that performs well across these five dimensions is likely aligned with Intentional Computing.

---

# 34. The Ultimate Design Goal

The objective is not to build software that people cannot live without.

The objective is to build software that makes people **more capable when they choose to use it**.

The best outcome is not:

> "The user spent all day in our application."

It is:

> **"The user accomplished something they could not have accomplished as easily before."**

And then they went and lived their life.

---

# Core Principles

If this entire document had to be reduced to ten rules:

1. **Human agency comes first.**
2. **Attention is not the product.**
3. **Completion is better than engagement.**
4. **Search is better than endless feeds.**
5. **Curation is better than volume.**
6. **AI should reduce complexity, not manufacture dependency.**
7. **Users should own their data and work.**
8. **Local and offline capability are valuable.**
9. **Software should be understandable and maintainable.**
10. **The user should always be able to walk away.**

> **Build powerful tools.**
>
> **Make them understandable.**
>
> **Give people control.**
>
> **Protect their attention.**
>
> **Preserve their ownership.**
>
> **And never make captivity a measure of success.**
