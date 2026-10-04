# AI Principles

## Introduction

Artificial intelligence is one of the most powerful computing capabilities available to individuals.

Intentional Computing does not reject AI.

It asks that AI be used deliberately.

AI should make computers more capable without making people more dependent on them.

The fundamental relationship should remain:

```text id="5y9v3n"
HUMAN
  ↓
INTENTION
  ↓
AI / COMPUTER
  ↓
CAPABILITY
  ↓
RESULT
  ↓
LIFE
```

The human provides the purpose.

The machine provides the capability.

> **AI should increase human agency, not replace it.**

---

# 1. AI Is a Tool

AI is a capability.

It is not the purpose of the software.

Do not add AI simply because AI exists.

Use AI when it provides a meaningful advantage over simpler approaches.

Good uses include:

* classification
* filtering
* search
* summarization
* translation
* analysis
* organization
* transformation
* automation
* pattern recognition
* assistance with creation

---

# 2. Start With the Human's Intent

Before introducing AI, identify what the user actually wants.

The correct sequence is:

```text id="w2w2g1"
Human Intent
     ↓
Problem
     ↓
AI Capability
     ↓
Useful Result
```

Not:

```text id="2k1xk8"
AI Capability
     ↓
Find something to do with it
```

The existence of a model is not a reason to build a feature.

---

# 3. AI Should Reduce Complexity

The primary value of AI in Intentional Computing is complexity reduction.

The computer can process:

* millions of documents
* thousands of search results
* large datasets
* complex patterns
* repetitive transformations

The user should not have to process all of that manually.

Prefer:

```text id="6h1g2s"
Large Information Set
        ↓
AI Processing
        ↓
Small Useful Set
```

over:

```text id="a7o5mc"
Large Information Set
        ↓
User manually processes everything
```

---

# 4. AI Should Not Manufacture Complexity

AI should not create additional:

* notifications
* recommendations
* content
* conversations
* decisions
* workflows
* subscriptions
* dependencies

simply because it can.

More generated output is not automatically more value.

---

# 5. AI Should Not Become the Interface for Everything

Not every interaction needs a chatbot.

If a task is better performed with:

* a button
* a menu
* a search field
* a checkbox
* a slider
* direct manipulation
* a keyboard shortcut

then use that interface.

AI should complement traditional interfaces rather than replace them indiscriminately.

---

# 6. Use the Simplest Appropriate Intelligence

Not every problem requires a large language model.

Consider this order where appropriate:

```text id="4r8x4a"
Simple Rule
    ↓
Deterministic Algorithm
    ↓
Traditional Search
    ↓
Statistical Method
    ↓
Machine Learning
    ↓
AI Model
```

Use the simplest method that provides the required capability.

This improves:

* speed
* reliability
* explainability
* cost
* privacy
* maintainability

---

# 7. Deterministic Rules Remain Valuable

Rules are not obsolete because AI exists.

Rules are particularly valuable when behavior must be:

* predictable
* repeatable
* transparent
* exact
* user-controlled

A strong system may combine:

```text id="1kq4s6"
User Rules
    +
AI Classification
    +
Deterministic Validation
```

---

# 8. User Rules Should Have Priority

Where practical, explicit user rules should override probabilistic AI behavior.

For example:

```text id="p4t5k7"
User Rule:
"Never show reaction videos."

        ↓

AI classification:
"Likely reaction video."

        ↓

REJECT
```

The AI should assist the user's information policy rather than replace it.

---

# 9. AI Should Be User-Directed

AI should generally operate in response to a user goal.

Examples:

* "Find technical videos."
* "Summarize these documents."
* "Remove duplicate files."
* "Explain this code."
* "Classify these images."

This is fundamentally different from:

> "Here is something else you might want to look at."

User-directed intelligence should generally be preferred over unsolicited intelligence.

---

# 10. Pull Before Push

AI should generally respond to requests rather than constantly generating reasons for the user to return.

Prefer:

```text id="d1x2u3"
User asks
   ↓
AI responds
```

over:

```text id="e4f5g6"
AI generates
   ↓
Notification
   ↓
User returns
   ↓
AI generates more
```

AI should save attention rather than consume it.

---

# 11. AI Should Filter Before It Amplifies

The internet already contains enormous amounts of information.

AI should often be used to reduce that volume.

Prefer:

```text id="2y3z4a"
Internet
 ↓
Search
 ↓
AI filtering
 ↓
User-selected results
```

over:

```text id="8b9c0d"
Internet
 ↓
AI generates even more content
 ↓
More content
 ↓
More content
```

AI should help make the information environment smaller and more useful.

---

# 12. AI Should Support a Personal Information Diet

Users should be able to define what information they want.

Possible controls include:

* preferred subjects
* excluded subjects
* preferred sources
* quality thresholds
* language
* format
* length
* technical depth
* freshness
* ranking criteria

AI can then enforce or assist those preferences.

---

# 13. AI Should Not Decide the User's Values

AI may help evaluate information.

It should not silently decide:

* what the user should care about
* what the user's priorities are
* what political or cultural position they should hold
* what purchases they should make
* what relationships they should maintain

The system may provide analysis.

The human retains judgment.

---

# 14. AI Should Distinguish Facts From Judgments

Where practical, AI systems should distinguish between:

* observed information
* retrieved information
* inferred information
* recommendations
* opinions
* assumptions

This helps users understand what kind of statement they are receiving.

---

# 15. AI Should Admit Uncertainty

AI systems are probabilistic.

They can be wrong.

The interface should communicate uncertainty when it matters.

Useful states include:

```text id="3e4f5g"
High confidence
Medium confidence
Low confidence
Unknown
Needs review
```

Do not present uncertain conclusions as guaranteed facts.

---

# 16. Confidence Should Be Meaningful

A numerical confidence score should not be shown merely to create an appearance of precision.

If a confidence value is displayed, its meaning should be understandable.

Otherwise prefer language such as:

> Likely

> Possible

> Uncertain

> Needs review

---

# 17. AI Should Be Inspectable Where Practical

When AI materially affects the user's result, the user should be able to understand why.

For example:

```text id="5h6i7j"
Filtered

Matched:
"Exclude influencer content"

AI classification:
Influencer / promotional

Confidence:
High
```

The goal is not to expose model internals.

The goal is to expose the application's reasoning sufficiently for the user to understand its behavior.

---

# 18. Human Override Is Required for Important Decisions

The more consequential an AI action becomes, the more important human control becomes.

Consider:

```text id="8k9l0m"
Low consequence
    ↓
Automatic action

Medium consequence
    ↓
Reviewable action

High consequence
    ↓
Explicit human approval
```

The exact boundary depends on the application.

---

# 19. Limit AI Authority

AI permissions should be narrowly scoped.

Give AI only the capabilities required for the task.

For example:

```text id="n1o2p3"
Task:
Summarize a document

AI permission:
Read selected document
Generate summary
```

Not:

```text id="q4r5s6"
Full computer access
Email access
File deletion
Publishing rights
Financial access
```

Power should be granted deliberately.

---

# 20. Separate Capability From Authority

An AI model may be technically capable of performing an action without being authorized to perform it.

This distinction is fundamental.

```text id="t7u8v9"
Capability ≠ Permission
```

The application should enforce the boundary.

---

# 21. Use Bounded Autonomy

Autonomous AI can be useful.

But autonomy should have:

* a defined task
* a defined scope
* limited permissions
* clear stopping conditions
* observable progress
* error handling
* cancellation
* recovery

Prefer:

```text id="w1x2y3"
Goal
 ↓
Bounded execution
 ↓
Result
 ↓
Stop
```

over:

```text id="z4a5b6"
Goal
 ↓
AI continues deciding what to do next
 ↓
No clear stopping point
```

---

# 22. AI Must Have a Stopping Condition

Every automated AI task should have a meaningful definition of completion.

Examples:

* classify 100 items
* summarize these documents
* process this folder
* answer this question
* generate this image
* analyze this dataset

Avoid autonomous systems whose implicit objective is simply:

> Continue.

---

# 23. Completion Should End the AI Interaction

When the task is complete, the system should say so.

For example:

> Classification complete: 94 of 100 items processed.

Then stop.

Do not automatically generate:

> "Would you also like..."

unless that follow-up is explicitly part of the workflow.

---

# 24. AI Should Be Reversible

Where AI changes user data, provide:

* undo
* versioning
* preview
* review
* restore
* backups

AI should not make irreversible changes casually.

---

# 25. Preview AI Changes

For significant modifications, show what will happen before applying it.

Examples:

```text id="c7d8e9"
AI proposed 23 changes.

[Review Changes]
[Apply]
[Cancel]
```

This is particularly important for:

* code
* documents
* images
* databases
* files
* configuration
* published content

---

# 26. AI Should Not Pretend to Have Done Work It Did Not Do

The system should distinguish between:

* generated
* suggested
* retrieved
* verified
* executed
* completed

For example:

> "I generated this answer."

is different from:

> "I verified this information against the source."

AI systems should never blur that distinction.

---

# 27. Verification Should Be Explicit

When factual accuracy matters, AI should use appropriate verification mechanisms.

These may include:

* source retrieval
* deterministic checks
* tests
* calculations
* external references
* human review

Generation and verification are separate capabilities.

---

# 28. AI Should Preserve Source Information

When AI transforms information, preserve the relationship to the original source where practical.

For example:

```text id="e1f2g3"
Source
  ↓
AI Summary
  ↓
Source Reference
```

This helps the user investigate important claims.

---

# 29. AI Should Not Hide the Source

When the system uses external information, users should be able to understand where important information came from where practical.

AI should not become an opaque replacement for the underlying information environment.

---

# 30. AI Should Prefer Existing Information Before Generating New Information

When the user is looking for factual information, search and retrieval may be more useful than generation.

Prefer:

```text id="h4i5j6"
Retrieve
 ↓
Evaluate
 ↓
Summarize
```

when appropriate.

Generation should not automatically replace retrieval.

---

# 31. AI Should Reduce Duplicate Information

AI can be especially useful for:

* deduplication
* clustering
* grouping
* summarizing
* merging related information

This is an example of AI reducing information overload rather than increasing it.

---

# 32. AI Should Preserve Human Creativity

AI should support creative work without making the human irrelevant.

Useful roles include:

* brainstorming
* iteration
* transformation
* critique
* exploration
* technical assistance
* repetitive production work

The user should remain able to make creative decisions directly.

---

# 33. AI Should Not Erase Skill

Automation can remove repetitive labor.

It should not unnecessarily hide understanding from people who want it.

Applications should provide opportunities to inspect:

* source material
* intermediate results
* generated code
* transformations
* reasoning context where appropriate

AI should make people more capable, not permanently dependent.

---

# 34. AI Should Teach When Useful

An AI system can provide:

* explanations
* examples
* documentation
* guided learning
* debugging assistance

When users want to understand something, the AI should help them understand it rather than simply producing the answer.

---

# 35. AI Should Support Multiple Skill Levels

A useful system can support:

```text id="k7l8m9"
Beginner
 ↓
Guided assistance
 ↓
Intermediate
 ↓
Direct control
 ↓
Expert automation
```

Users should be able to grow into the system.

---

# 36. AI Memory Must Be User-Controlled

If an AI system stores information about the user, that memory should be:

* visible
* understandable
* editable
* removable
* exportable where practical

Users should not have to wonder:

> What does this AI remember about me?

---

# 37. AI Memory Should Have a Purpose

Do not store information merely because it can be stored.

Memory should improve a specific experience.

Unnecessary memory increases:

* privacy risk
* complexity
* dependency
* uncertainty

---

# 38. Local AI Should Be Preferred Where Practical

When local models provide sufficient capability, local processing can provide:

* privacy
* offline operation
* lower network dependency
* predictable availability
* user control

Remote AI remains useful when it provides capabilities that local systems cannot reasonably provide.

---

# 39. Remote AI Should Be an Extension

The ideal architecture should not automatically become:

```text id="n0p1q2"
User
 ↓
Internet
 ↓
AI Service
 ↓
Everything
```

Where practical, prefer:

```text id="r3s4t5"
User
 ↓
Local Computer
 ├── Local Data
 ├── Local Rules
 ├── Local AI
 └── Local Tools
          ↓
      Optional Remote Services
```

The network should extend the personal computer.

---

# 40. Network Failure Should Not Destroy Local Capability

If remote AI becomes unavailable, unrelated local capabilities should continue working.

Applications should distinguish between:

* local functionality
* remote functionality
* optional AI functionality

Where practical, provide graceful degradation.

---

# 41. AI Services Should Be Replaceable

Applications should avoid making the entire system dependent on one model or provider where practical.

For example:

```text id="u6v7w8"
AI Interface
     ↓
Model Provider
 ├── Local Model
 ├── Provider A
 ├── Provider B
 └── Future Model
```

The user's workflow should survive changes in AI providers.

---

# 42. Model Choice Should Be Configurable Where Practical

Users may have different requirements for:

* speed
* quality
* privacy
* cost
* hardware
* offline capability

Where practical, expose model selection.

Do not assume one model is universally correct.

---

# 43. AI Should Be Resource-Aware

AI can consume substantial:

* CPU
* GPU
* memory
* disk
* electricity
* network bandwidth

Applications should consider resource usage.

Users should be able to understand when expensive processing is occurring.

---

# 44. AI Should Not Run Unnecessarily

Background AI processing should have a clear purpose.

Avoid continuously:

* analyzing files
* watching user behavior
* processing content
* generating suggestions
* indexing everything

unless the user explicitly wants that behavior.

---

# 45. AI Should Respect Privacy

AI processing should follow the same principle as all other computing:

> Collect and process only what is necessary.

Prefer local processing when practical.

When data must leave the machine, the user should understand that it is happening.

---

# 46. AI Should Not Become Surveillance

Do not use AI to continuously infer:

* user behavior
* emotional state
* productivity
* interests
* relationships
* habits

simply because the system can.

AI should serve explicit user goals.

---

# 47. AI Should Not Manufacture Dependency

Avoid systems where the user gradually loses the ability to function without the AI.

Do not intentionally:

* hide underlying data
* remove export paths
* make manual workflows impossible
* create unnecessary memory dependency
* force all interactions through the AI

The user should remain capable.

---

# 48. AI Should Increase User Capability

A useful question is:

> **Is the person more capable because this AI exists?**

Examples:

* They can search more effectively.
* They can process more information.
* They can understand difficult material.
* They can create things faster.
* They can automate repetitive work.
* They can build software they could not previously build.

This is a better measure than:

> How often does the person use the AI?

---

# 49. AI Should Compress the Internet

The public internet is enormous.

A personal AI layer can help transform:

```text id="x9y0z1"
Huge Internet
     ↓
Search
     ↓
Filtering
     ↓
Classification
     ↓
Deduplication
     ↓
Summarization
     ↓
Personal Information Set
```

This is one of the most valuable applications of AI within Intentional Computing.

---

# 50. AI Should Support the Personal Internet

AI can become a component of a personal information layer.

It can help:

* search
* classify
* filter
* summarize
* archive
* organize
* compare
* translate
* retrieve

The personal layer remains controlled by the individual.

---

# 51. AI Should Respect the Information Boundary

The personal AI should know the difference between:

```text id="a2b3c4"
My Data
Public Data
Third-Party Data
Temporary Data
Sensitive Data
```

Access should be deliberate.

---

# 52. AI Should Not Be the Owner of the User's Information

The user's data should remain under the user's control.

AI may process it.

AI should not become the permanent owner of it.

---

# 53. AI Should Support Open Formats

Generated information should remain usable outside the AI system where practical.

Support:

* plain text
* Markdown
* standard images
* standard documents
* structured data
* ordinary files

Do not trap important work inside proprietary AI conversations.

---

# 54. AI Should Be Portable

The user's:

* prompts
* rules
* configurations
* memories
* workflows
* generated work

should be portable where practical.

A user should be able to change AI systems without losing their accumulated work.

---

# 55. AI Should Be Auditable

For important automated workflows, maintain enough information to answer:

* what happened
* when
* using which model
* using which rules
* with which inputs
* what result was produced

Auditability is especially valuable for development, research, and automation.

---

# 56. AI Should Be Tested Like Software

AI features require testing.

Test:

* expected inputs
* unexpected inputs
* ambiguous inputs
* adversarial inputs
* missing information
* model failures
* hallucinations
* latency
* resource usage
* provider failure

Do not assume a model will always behave correctly.

---

# 57. AI Systems Should Have Fallbacks

Where practical:

```text id="d5e6f7"
AI unavailable
      ↓
Deterministic fallback
      ↓
Reduced capability
```

is preferable to:

```text id="g8h9i0"
AI unavailable
      ↓
Entire application stops working
```

---

# 58. AI Should Fail Gracefully

When AI cannot determine an answer, acceptable outcomes include:

* ask the user
* return uncertainty
* provide multiple possibilities
* defer to a rule
* request additional information
* stop

"Unknown" is a valid result.

---

# 59. AI Should Not Be Forced to Answer

A system should be allowed to say:

> I don't know.

or:

> There is not enough information to determine this.

This is preferable to confidently inventing an answer.

---

# 60. AI Should Preserve Human Judgment

The final authority over personal decisions should remain with the person.

AI can:

* analyze
* compare
* explain
* recommend
* simulate
* summarize

The user decides.

---

# 61. Avoid Algorithmic Paternalism

The system should not quietly decide what is "best for the user" without allowing meaningful control.

Safety requirements may justify restrictions.

But ordinary preference should remain user-configurable where practical.

---

# 62. AI Should Be Transparent About Its Role

The user should know when they are interacting with:

* deterministic software
* search
* AI classification
* generative AI
* human review

This distinction matters.

---

# 63. AI Should Not Simulate Human Relationship Unnecessarily

AI can communicate naturally.

But applications should avoid deliberately creating emotional dependency through:

* simulated attachment
* guilt
* loneliness manipulation
* persistent emotional reminders
* pressure to return

Natural language is useful.

Manipulated attachment is not.

---

# 64. AI Should Respect the Right to Ignore

The user should be able to:

* dismiss suggestions
* disable AI features
* turn off memory
* disable notifications
* stop background processing
* use manual workflows

Ignoring the AI should always remain a valid choice.

---

# 65. AI Should Respect the Right to Stop

An AI operation should be stoppable where practical.

The user should not need to:

* close the entire application
* revoke network access
* terminate a process manually

to stop ordinary AI work.

---

# 66. AI Should Respect the Right to Leave

The ultimate test is:

> Can the user stop using the AI without losing control of their data, work, or computer?

If yes, the AI remains a tool.

If no, the AI has become a dependency.

---

# AI Design Test

Before shipping an AI feature, ask:

### Purpose

* What real problem does AI solve?
* Could a simpler method solve it?

### Agency

* Does the user remain in control?
* Can the user override it?
* Can the user disable it?

### Scope

* What can the AI access?
* What can it change?
* What can it execute?

### Transparency

* Does the user know AI is involved?
* Can important decisions be understood?

### Uncertainty

* Can the AI be wrong?
* Is uncertainty communicated appropriately?

### Reversibility

* Can changes be undone?
* Can important actions be reviewed?

### Privacy

* What information leaves the machine?
* Can processing happen locally?

### Ownership

* Can the user export their data and AI-generated work?
* Can the AI provider be replaced?

### Attention

* Does AI save attention?
* Or does it create another reason to interact?

### Completion

* Does the AI know when the task is finished?

### Exit

* Can the user walk away?

---

# The AI Contract

Intentional Computing defines a simple relationship:

## The Human Provides

* intent
* goals
* values
* preferences
* judgment
* permission
* boundaries

## AI Provides

* computation
* search
* classification
* analysis
* automation
* explanation
* generation
* organization

## The System Provides

* transparency
* control
* reversibility
* privacy
* portability
* understandable boundaries

The relationship should remain:

```text id="j1k2l3"
HUMAN
  ↓
INTENT
  ↓
AI
  ↓
CAPABILITY
  ↓
RESULT
  ↓
HUMAN
```

AI should never silently replace the first or last step.

---

# The Core AI Principles

The entire standard can be reduced to ten rules:

1. **AI is a tool, not the purpose.**
2. **Start with human intent.**
3. **Use AI to reduce complexity.**
4. **Prefer the simplest appropriate intelligence.**
5. **Keep human authority over important decisions.**
6. **Limit AI permissions and autonomy.**
7. **Make AI behavior understandable and reversible.**
8. **Prefer local, private, portable AI where practical.**
9. **Do not manufacture attention, dependency, or artificial relationships.**
10. **Use AI to make the person more capable, then let them walk away.**

---

# Final Principle

AI changes what an individual computer can do.

That is extraordinary.

A person with access to powerful AI can search enormous information spaces, analyze complex systems, write software, create images, organize knowledge, automate repetitive work, and interact with computers in ways that were previously available only to large organizations.

That power should belong to the individual.

But capability should not come at the cost of control.

The goal is not:

> **Make the AI indispensable.**

The goal is:

> **Make the person more capable.**

Use intelligence to absorb complexity.

Use automation to remove repetitive work.

Use models to search and classify enormous information spaces.

Use AI to make difficult tools accessible.

Keep the user in control.

Keep data portable.

Keep permissions bounded.

Keep decisions reversible.

Keep uncertainty visible.

Keep the system replaceable.

Keep the interface calm.

And when the user's work is finished:

> **Let the AI stop.**

> **Let the software stop.**

> **Let the person get back to life.**
