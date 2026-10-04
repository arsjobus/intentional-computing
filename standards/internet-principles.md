# Internet Principles

## Introduction

The internet is one of the most powerful tools ever created.

It provides access to:

* information
* knowledge
* communication
* software
* communities
* culture
* archives
* education
* commerce
* collaboration
* creative work

Intentional Computing does not reject the internet.

It rejects the idea that a person must permanently live inside the internet in order to use it.

The internet should be a resource that the individual can access deliberately.

> **The internet should serve the person, not become the environment that controls the person.**

---

# 1. The Internet Is a Tool

The internet should be treated as infrastructure and a resource.

It is not inherently:

* a destination
* a lifestyle
* a social obligation
* an entertainment loop
* a permanent environment

The user should be able to:

```text id="r4a7c2"
Need Information
      ↓
Use Internet
      ↓
Get Information
      ↓
Leave
```

Connection should have a purpose.

---

# 2. The Personal Computer Comes First

The computer should remain useful without an internet connection whenever practical.

The fundamental relationship should be:

```text id="g7m2p9"
PERSON
  ↓
PERSONAL COMPUTER
  ↓
LOCAL CAPABILITY
  ↓
OPTIONAL INTERNET
```

not:

```text id="q8x3v1"
PERSON
  ↓
INTERNET
  ↓
REMOTE SERVICE
  ↓
COMPUTER
```

The network should extend the computer.

It should not replace it.

---

# 3. Local First Where Practical

Applications should perform locally what can reasonably be performed locally.

This includes:

* storing files
* editing documents
* searching local data
* managing configuration
* processing information
* running software
* working with projects

Network services should provide additional value rather than being required unnecessarily.

---

# 4. The Internet Should Be Pull-Based Where Possible

Users should be able to ask for information when they want it.

Prefer:

```text id="d9k4s1"
User
 ↓
Intent
 ↓
Search
 ↓
Information
```

over:

```text id="w2j8n6"
System
 ↓
Recommendation
 ↓
Notification
 ↓
User attention
 ↓
Another recommendation
```

Push mechanisms have legitimate uses.

But they should not become the default relationship with the internet.

---

# 5. Search Before Feeds

Search is one of the most important intentional interfaces to the internet.

A user should be able to say:

> I want this.

and receive:

> Here are the relevant results.

rather than being placed into an endless stream of whatever an algorithm predicts might maintain attention.

Prefer:

```text id="n6r1b8"
Intent
 ↓
Search
 ↓
Filter
 ↓
Results
 ↓
Completion
```

---

# 6. Feeds Should Not Be Infinite by Default

Infinite feeds remove natural stopping points.

Where a finite collection is possible, prefer:

* pages
* result counts
* explicit "load more"
* categories
* archives
* saved lists
* bounded recommendations

The user should know when they have reached the end of the available information.

---

# 7. Recommendations Should Be User-Directed

Recommendations can be valuable.

They should generally answer an identifiable user interest.

For example:

> Show me ten technical articles about game development.

is different from:

> Here is an endless collection of things chosen to keep you here.

Recommendation should help discovery.

It should not become the primary mechanism for consuming the internet.

---

# 8. Curation Is Better Than Volume

The internet contains more information than any individual can consume.

The goal should therefore not be maximum exposure.

It should be useful selection.

Prefer:

```text id="k7p2m5"
Internet
 ↓
Search
 ↓
Filtering
 ↓
Deduplication
 ↓
Ranking
 ↓
Useful Information
```

The computer should handle volume.

The person should receive clarity.

---

# 9. The Personal Internet Layer

Intentional Computing envisions a personal layer between the individual and the public internet.

```text id="s5n8q2"
PERSON
  ↓
PERSONAL INTERNET LAYER
  ├── Search
  ├── Filters
  ├── Bookmarks
  ├── Archives
  ├── Local Data
  ├── AI
  ├── Preferences
  └── Personal Index
  ↓
PUBLIC INTERNET
  ↓
SELECTED INFORMATION
```

The public internet remains enormous.

The personal layer makes it manageable.

---

# 10. The Personal Layer Belongs to the User

The personal information layer should be:

* user-controlled
* portable
* configurable
* understandable
* replaceable
* locally accessible

It should not become another platform that demands dependency.

---

# 11. The Internet Should Be Source-Agnostic

The personal layer should not depend unnecessarily on one provider.

Information should be able to come from:

* websites
* APIs
* public archives
* local files
* RSS
* databases
* search engines
* personal collections
* other networks

The interface should be able to change sources without requiring the user to rebuild their entire environment.

---

# 12. Do Not Confuse Platforms With the Internet

A website or platform is not the internet itself.

Users should be able to distinguish between:

```text id="c4h7m1"
Internet
   ↓
Websites
   ↓
Platforms
```

and:

```text id="v8k2q6"
Internet
   ↓
Personal Access Layer
   ↓
Selected Information
```

A platform may be useful.

It should not become synonymous with the internet.

---

# 13. Do Not Build Another Platform Unless Necessary

Intentional Computing tools should avoid recreating the same centralized dynamics they are intended to escape.

Do not create:

* unnecessary social graphs
* engagement metrics
* follower systems
* infinite feeds
* artificial popularity rankings
* attention-driven recommendations

simply because those features are familiar.

Build tools.

Do not automatically build platforms.

---

# 14. Information Should Have an Exit Path

Information retrieved from the internet should be usable beyond the application that retrieved it.

Support where practical:

* saving
* exporting
* downloading
* bookmarking
* archiving
* copying
* local storage
* citation

The user should be able to take useful information with them.

---

# 15. Local Archives Are Valuable

Important information should not exist only at the moment it is viewed online.

Where legally and technically appropriate, users should be able to preserve:

* documents
* articles
* reference material
* images
* software
* metadata
* bookmarks

Archives turn temporary access into durable knowledge.

---

# 16. Preservation Is Part of Internet Computing

The internet changes constantly.

Websites disappear.

Domains expire.

Services shut down.

APIs change.

Content moves.

Intentional Computing therefore values preservation.

A useful personal internet should make it possible to distinguish:

```text id="z6b3n9"
Live Information
Archived Information
Personal Information
Historical Information
```

---

# 17. Prefer Stable References

Where practical, use references that remain understandable over time.

Examples include:

* URLs
* filenames
* document titles
* publication dates
* source names
* archive identifiers

Avoid relying entirely on temporary interface state.

---

# 18. Separate Retrieval From Storage

Finding information and owning a copy of information are different operations.

A useful architecture is:

```text id="m3q8v7"
Internet
 ↓
Retrieval
 ↓
Evaluation
 ↓
Optional Local Storage
 ↓
Personal Archive
```

The user decides what becomes part of their personal information environment.

---

# 19. Search Should Be Explainable

When possible, users should understand why information appeared.

Useful explanations include:

* matched search terms
* source
* date
* active filters
* sorting method
* ranking criteria

Search should not feel like an unexplained oracle.

---

# 20. Search Should Respect User Filters

Search results should honor explicit preferences.

Examples:

```text id="j8s4p2"
Exclude:
- Short-form videos
- Promotional content
- Certain categories

Prefer:
- Technical content
- Long-form material
- Specific sources
```

The user's information policy should be part of the search system.

---

# 21. Ranking Should Be Configurable Where Practical

Different people value different things.

Possible ranking factors include:

* relevance
* date
* quality
* source
* popularity
* length
* technical depth
* personal preference

Where practical, users should be able to choose how results are ordered.

---

# 22. Popularity Is Not the Same as Value

Views, likes, shares, and followers can provide useful signals.

They should not automatically determine relevance.

A highly viewed piece of content may be less useful than an obscure technical document.

The system should distinguish:

> popular

from:

> useful to this person.

---

# 23. Do Not Optimize for Virality

Intentional Computing systems should not optimize around:

* shares
* outrage
* controversy
* emotional reaction
* rapid consumption
* viral growth

unless virality is explicitly the user's objective.

The objective should remain usefulness.

---

# 24. Avoid Algorithmic Manipulation

Algorithms should not deliberately exploit:

* fear
* outrage
* loneliness
* boredom
* FOMO
* social pressure
* compulsive behavior

Ranking should help the user find information.

It should not manipulate the user into producing more engagement.

---

# 25. Notifications Should Be Rare

Internet-connected software should not constantly interrupt the user.

Notifications should be:

* meaningful
* relevant
* controllable
* actionable

Users should be able to disable unnecessary notifications.

---

# 26. Email Should Remain a Tool

Email is fundamentally useful because it is asynchronous.

It should not become another real-time attention stream.

Useful principles include:

* batch checking
* local archives
* search
* filtering
* rules
* explicit notifications
* user-controlled retention

The user should be able to process email and finish.

---

# 27. Social Communication Should Be Intentional

Intentional Computing does not reject social interaction.

People need:

* friends
* communities
* communication
* collaboration
* shared interests

The principle is not:

> Do not socialize online.

It is:

> **Social interaction should be something the person chooses rather than something an algorithm continuously demands.**

---

# 28. Communities Should Have Boundaries

Online communities should have understandable boundaries.

Users should be able to know:

* what the community is
* why they are there
* what information they will encounter
* how to leave

A community should not need to become an entire lifestyle.

---

# 29. Social Participation Should Have an Exit

Users should be able to:

* leave communities
* mute conversations
* disable notifications
* unsubscribe
* export their contributions where possible
* delete their accounts where applicable

Leaving should not be intentionally difficult.

---

# 30. Avoid Social Metrics as Primary Identity

Numbers such as:

* follower count
* karma
* likes
* streaks
* views
* subscriber counts

can distort the meaning of participation.

They should not become the primary measure of personal value.

---

# 31. Identity Should Be Proportional to the Task

Not every online activity requires:

* a permanent identity
* a profile
* a social graph
* personal tracking

Use identity where it provides genuine value.

Avoid unnecessary identity requirements.

---

# 32. Privacy Should Be Architectural

Privacy should not depend entirely on users finding the correct settings.

Prefer architecture that naturally limits exposure.

For example:

```text id="p2m7x4"
Local Data
   ↓
Local Processing
   ↓
Optional Network Request
```

is generally preferable to:

```text id="v9c3k8"
Everything
   ↓
Central Server
```

when both architectures can provide the required capability.

---

# 33. Minimize Tracking

Do not track users merely because tracking is technically possible.

If analytics are necessary, collect the minimum information needed.

Avoid building detailed behavioral profiles unless explicitly required for a legitimate user-directed function.

---

# 34. The Personal Internet Should Be Private by Default

A personal information layer may contain:

* bookmarks
* notes
* searches
* files
* preferences
* archives
* AI memory
* personal metadata

This information should remain private unless the user deliberately shares it.

---

# 35. The User Owns Their Personal Information Layer

The personal layer should not become a cloud account that the user merely rents.

Where practical, users should control:

* storage
* configuration
* archives
* indexes
* rules
* AI memory
* credentials
* exports

---

# 36. Open Formats Matter

Personal internet tools should favor portable formats.

Examples include:

* Markdown
* plain text
* HTML
* JSON
* CSV
* standard image formats
* standard document formats

The user should be able to move information between tools.

---

# 37. The Personal Internet Should Be Modular

A user should be able to replace:

```text id="a8k4p6"
Search Engine
AI Model
Archive
Browser
Indexer
Storage
Interface
```

without rebuilding their entire personal computing environment.

Modularity creates independence.

---

# 38. Services Should Be Replaceable

If one service disappears, the user's personal environment should survive where practical.

For example:

```text id="n3q7v5"
Search Provider A
       ↓
Personal Search Interface
       ↓
Search Provider B
```

The personal layer should absorb changes in external services.

---

# 39. Internet Access Should Degrade Gracefully

If the network disappears:

```text id="k5s2j8"
Local Files       ✓
Local Search      ✓
Local Archives    ✓
Local Tools       ✓
Remote Search     ✗
Online Services   ✗
```

The computer should remain useful.

---

# 40. Cache What Is Useful

Caching can reduce:

* network dependency
* latency
* repeated requests
* service outages

Cache information when doing so provides meaningful value and respects applicable rights and policies.

The cache should remain understandable and manageable.

---

# 41. Do Not Hide Network Activity

Users should be able to understand when applications communicate externally.

Important network activity should be:

* documented
* observable where practical
* purposeful
* configurable where appropriate

Background communication should not become invisible infrastructure by default.

---

# 42. Remote Services Should Provide Real Value

A network request should have a reason.

Examples of legitimate value include:

* accessing current information
* synchronization
* collaboration
* remote computation
* large-scale search
* communication
* retrieving public resources

Avoid network dependency for tasks that can easily happen locally.

---

# 43. Avoid Forced Cloud Dependence

Cloud services can be useful.

But applications should not automatically require them for:

* opening local files
* editing local projects
* basic configuration
* offline viewing
* ordinary local computation

Cloud should be an option where practical, not an unquestioned foundation.

---

# 44. Personal Search Should Compound

A useful personal search system should become more valuable over time.

It may eventually index:

* local documents
* bookmarks
* notes
* saved web pages
* source archives
* project files
* personal knowledge

The result is a personal information environment that belongs to the user.

---

# 45. Knowledge Should Compound, Not Disappear

When a person spends time learning something online, useful results should be able to become part of their long-term knowledge.

For example:

```text id="f6m8r3"
Discover
 ↓
Read
 ↓
Understand
 ↓
Save
 ↓
Organize
 ↓
Recall Later
```

This is fundamentally different from:

```text id="t1q5w9"
Consume
 ↓
Scroll
 ↓
Forget
 ↓
Consume Again
```

---

# 46. Prefer Libraries Over Streams

The internet can be thought of as a massive library and workshop.

Users should be able to:

* find information
* borrow information
* reference information
* save useful information
* create things
* contribute things

The goal is not to live inside the library.

The goal is to use it.

---

# 47. The Web Should Support Creation

The internet is not only for consumption.

Intentional Computing should encourage:

* publishing
* programming
* art
* documentation
* collaboration
* experimentation
* education
* open-source development

Creation should be treated as a first-class use of the network.

---

# 48. Do Not Confuse Consumption With Participation

Viewing content is not the only meaningful online activity.

A healthier information environment supports:

```text id="v4n7c2"
Learn
Create
Build
Share
Collaborate
Archive
Communicate
```

rather than optimizing primarily for:

```text id="b8m3q6"
Scroll
React
Scroll
React
Scroll
React
```

---

# 49. Serendipity Is Valuable

Intentional Computing should not become an information prison.

Unexpected discovery is valuable.

The goal is not to eliminate serendipity.

It is to make serendipity:

* bounded
* optional
* diverse
* user-directed

A user might choose:

> Show me five things outside my normal interests.

That is intentional discovery.

---

# 50. The Personal Bubble Should Be Permeable

A personal information environment should provide a boundary without becoming a wall.

The user should be able to deliberately explore beyond their normal information diet.

The distinction is:

```text id="r2k8m5"
Intentional Discovery
```

rather than:

```text id="x7p3n1"
Algorithmic Exposure
```

---

# 51. Diversity Should Not Require Infinite Consumption

A useful system can deliberately introduce:

* different sources
* different perspectives
* different authors
* different time periods
* different approaches

without requiring an endless feed.

Curated diversity is preferable to unlimited exposure.

---

# 52. Source Independence Matters

A personal information system should avoid depending on a single source of truth where practical.

Use multiple sources when appropriate.

This improves:

* resilience
* comparison
* accuracy
* availability
* independence

---

# 53. Verification Should Be Possible

Important information should be traceable back to sources.

Where practical, provide:

* source links
* citations
* publication dates
* original documents
* archive references

The personal layer should help users investigate rather than merely trust.

---

# 54. AI Should Help Navigate the Internet

AI can be particularly useful as a personal filter.

It can:

* classify results
* remove duplicates
* summarize sources
* compare documents
* identify relevant information
* enforce user rules
* translate
* organize archives

AI should make the internet smaller and more useful.

---

# 55. AI Should Not Become the Internet

The AI should remain a layer over information.

It should not become the only place information exists.

Prefer:

```text id="h3j6m9"
Internet
 ↓
Sources
 ↓
AI
 ↓
Understanding
```

over:

```text id="q8s4v2"
Internet
 ↓
AI
 ↓
Everything else disappears
```

Users should retain access to underlying sources.

---

# 56. The Internet Should Remain Open to Inspection

Where practical, users should be able to discover:

* where information came from
* what filters were applied
* how it was ranked
* whether AI modified it
* whether it was cached
* whether it was locally stored

Transparency creates trust.

---

# 57. Do Not Build an Information Prison

A personal internet environment should not become another closed ecosystem.

Avoid:

* proprietary-only archives
* inaccessible exports
* mandatory subscriptions
* permanent account requirements
* hidden ranking systems
* impossible migrations

The personal internet should remain open.

---

# 58. The Browser Is Not the Entire Personal Internet

A browser is an important tool.

But a personal internet can also include:

* local search
* file systems
* personal indexes
* archives
* command-line tools
* AI assistants
* local databases
* dedicated applications

The personal internet is an information architecture, not merely a browser tab.

---

# 59. Personal Information Should Be Searchable

Users should eventually be able to search across their own information environment.

For example:

```text id="c9v5m2"
Search

├── Local Files
├── Notes
├── Bookmarks
├── Saved Pages
├── Projects
├── Archives
└── Public Internet
```

The distinction between local and public information should remain visible.

---

# 60. Search Should Be the Universal Entry Point

A strong personal computing environment can increasingly revolve around:

> **What are you looking for?**

rather than:

> **Which application should you open?**

The system can then route the request to the appropriate source.

---

# 61. But Search Should Not Replace Direct Access

Search is powerful.

But users should still be able to browse:

* folders
* archives
* websites
* collections
* applications
* libraries

Direct access is valuable for understanding structure.

---

# 62. Preserve the Structure of Information

Do not reduce everything to a flat stream.

Information often has meaningful structure:

```text id="m7p4s8"
Library
 ├── Books
 ├── Articles
 ├── Projects
 ├── Notes
 └── Archives
```

Structure supports understanding and ownership.

---

# 63. The Internet Should Not Require Constant Presence

A person should be able to disconnect.

They should be able to:

* work offline
* read locally
* create locally
* play locally
* write locally
* organize locally

and reconnect later.

Disconnection should be a normal operating mode.

---

# 64. Offline Is Not Failure

An offline computer is not broken.

It is simply operating without one particular capability.

Applications should distinguish:

> Offline

from:

> Error.

---

# 65. Synchronization Should Be Explicit

If data synchronizes between devices, the user should understand:

* what is synchronized
* where it is stored
* when synchronization occurs
* what happens during conflicts
* how to disable it

Synchronization should not imply surrendering ownership.

---

# 66. Conflict Resolution Should Respect the User

When synchronized information conflicts, do not silently overwrite important work.

Provide:

* conflict information
* version history
* comparison
* recovery

The user should be able to understand what happened.

---

# 67. Do Not Assume Everything Needs Synchronization

Some information is valuable precisely because it remains local.

Allow users to decide what belongs on:

* one computer
* multiple computers
* a private server
* a removable drive
* a cloud service

---

# 68. The Internet Should Support Long-Term Ownership

Users should be able to accumulate:

* knowledge
* projects
* archives
* software
* references
* creative work

without that accumulation becoming dependent on a single platform.

The longer someone uses technology, the more valuable ownership becomes.

---

# 69. Design for Migration

Internet services change.

Therefore personal systems should support migration.

Examples:

```text id="j4n8p2"
Service A
   ↓
Export
   ↓
Personal Data
   ↓
Service B
```

not:

```text id="s6k3m9"
Service A
   ↓
Permanent dependency
```

---

# 70. The Internet Should Be Composable

Personal computing should be able to combine:

```text id="v2r7c5"
Local Software
+
Public Internet
+
Personal Archives
+
AI
+
Open Formats
+
Local Search
+
Optional Cloud Services
```

without requiring one company to control the entire environment.

---

# 71. Prefer Protocols Over Platforms

Platforms concentrate control.

Protocols allow independent systems to communicate.

Where practical, prefer:

* open standards
* documented protocols
* interoperable formats
* decentralized architectures

Platforms can still be useful.

Protocols provide greater long-term independence.

---

# 72. Build for a Multi-Service Internet

The future personal internet should not depend on a single provider.

A healthy environment can combine many services while maintaining one personal interface.

The personal layer becomes the stable part.

The external services become replaceable components.

---

# 73. The User Should Own the Interface to Their Information

A person's information environment should not require them to use whatever interface a service provider happens to provide.

Where practical, users should be able to choose:

* interface
* search method
* filtering
* sorting
* archive method
* AI layer
* storage

This restores personal computing control.

---

# 74. Internet Services Should Respect User Exit

A healthy service should make it possible to:

* export information
* unsubscribe
* disable notifications
* delete an account where applicable
* retrieve personal content
* stop using the service

Leaving should be a normal operation.

---

# 75. No Artificial Lock-In

Avoid designs where leaving becomes intentionally painful.

Do not use:

* inaccessible exports
* proprietary formats without justification
* unnecessary dependencies
* deliberately confusing migrations
* hidden subscriptions
* forced social graphs

A service should retain users through value.

Not captivity.

---

# 76. The Internet Should Help Real Life

The ultimate purpose of online information is usually something outside the internet itself.

It may help someone:

* learn
* build
* communicate
* work
* create
* solve a problem
* make a decision
* understand something

The internet should point back toward life.

---

# 77. Real Life Remains the Destination

The intended loop is:

```text id="p5x9r3"
INTENTION
   ↓
INFORMATION
   ↓
UNDERSTANDING
   ↓
ACTION
   ↓
COMPLETION
   ↓
LIFE
```

Not:

```text id="z2m6q8"
INTENTION
   ↓
INTERNET
   ↓
MORE INTERNET
   ↓
MORE INTERNET
   ↓
MORE INTERNET
```

---

# Internet Design Test

Before building an internet-connected feature, ask:

### Purpose

* Why does this need the internet?
* What useful capability does the network provide?

### Local Capability

* What works without the network?
* Could more functionality reasonably remain local?

### Attention

* Does this feature require attention?
* Does it generate unnecessary notifications?
* Does it create an endless interaction loop?

### Search

* Can the user explicitly search?
* Are results finite and understandable?

### Curation

* Can the user define what they want?
* Can unwanted information be filtered?

### Ownership

* Can useful information be saved?
* Can it be exported?
* Can the user leave?

### Privacy

* What information leaves the machine?
* Is tracking necessary?

### Independence

* Can the external service be replaced?
* Does the application depend on one provider?

### Preservation

* Can important information be archived?
* Will it remain useful if the service disappears?

### AI

* Is AI reducing information overload?
* Can the user inspect important sources?
* Is AI optional where practical?

### Real Life

* Does this feature help the user do something meaningful?
* Does it provide a natural stopping point?

---

# The Core Internet Principles

The entire standard can be reduced to ten rules:

1. **The internet is a tool, not a place to live.**
2. **The personal computer should remain useful without the network.**
3. **Search should generally come before recommendation.**
4. **Information should be curated rather than maximized.**
5. **The user's personal information layer should belong to the user.**
6. **Internet services should be replaceable and interoperable where practical.**
7. **Privacy, portability, and exit should be built into the architecture.**
8. **AI should make the internet smaller and more useful, not larger and more addictive.**
9. **Online activity should have natural stopping points.**
10. **The internet should ultimately point back toward real life.**

---

# Final Principle

The internet is an extraordinary achievement.

It connects people to more information, knowledge, software, culture, and opportunity than any previous generation could access.

The answer is not to abandon it.

The answer is to change the relationship.

A person should be able to enter the internet deliberately.

Search for something.

Learn something.

Find something.

Build something.

Communicate with someone.

Save something useful.

Then leave.

The internet should be enormous.

The user's personal experience of it does not need to be.

AI can help make the enormous manageable.

Local computing can provide independence.

Search can replace endless discovery.

Curation can replace information overload.

Archives can turn temporary access into lasting knowledge.

Open formats can preserve ownership.

Interoperability can preserve choice.

And a personal information layer can give the individual a stable environment even while the public internet changes around them.

The goal is not a smaller internet.

It is a **more intentional relationship with the internet**.

> **Use the network.**
>
> **Take what is useful.**
>
> **Build something with it.**
>
> **Preserve what matters.**
>
> **Then disconnect when you are done.**
