# NoBSTube

## Project Purpose

NoBSTube is a local, self-hosted video discovery application built around the principles of Intentional Computing.

Its purpose is simple:

> Help a person find useful video content without requiring them to enter an attention-optimized video platform.

NoBSTube treats video platforms as **sources of information**, not as environments that the user needs to inhabit.

The user should be able to:

1. Decide what they want.
2. Search for it.
3. Filter out unwanted material.
4. Review a finite set of useful results.
5. Watch what they found.
6. Stop.

The application should not need to keep the user engaged after the task is complete.

---

# Why NoBSTube Exists

Modern video platforms provide an enormous amount of useful information.

They also commonly surround that information with:

* Infinite recommendation feeds
* Autoplay
* Engagement optimization
* Notifications
* Trending content
* Click-driven thumbnails
* Behavioral profiling
* Algorithmic recommendations
* Social metrics
* Constant novelty
* Increasingly aggressive attempts to retain attention

The problem is not video.

The problem is the environment surrounding video.

NoBSTube explores a different model:

> **Use the internet's video resources without surrendering control of the user's attention to the platform providing them.**

The project therefore intentionally separates **video retrieval** from **platform participation**.

---

# Project Philosophy

NoBSTube is an implementation of several core Intentional Computing principles.

### Search Over Feeds

The primary interaction is search.

The user asks for something rather than being continuously presented with things chosen for them.

### Curation Over Volume

The internet contains far more information than a person can reasonably evaluate.

NoBSTube therefore attempts to reduce the amount of information presented to the user rather than maximizing the number of results.

### User-Defined Filtering

The user should be able to explicitly define what they do and do not want to encounter.

Filtering is a first-class feature rather than an afterthought.

### AI as a Tool

AI is used to classify, filter, organize, and reduce complexity.

It is not used to manufacture engagement.

### Finite Discovery

A search should produce a manageable set of results.

The user should reach a natural stopping point.

### Local Ownership

The application should run on the user's own computer.

Configuration, filtering rules, and application state should remain under the user's control.

### Source Independence

NoBSTube should not depend on a single video platform as the user's entire information environment.

The internet should remain a collection of sources that can be searched through a personal layer.

---

# What NoBSTube Is

NoBSTube is:

* A local video search application
* A personal video discovery layer
* A multi-source search tool
* A user-controlled filtering system
* An AI-assisted classification system
* A finite alternative to recommendation feeds
* A self-hosted application
* A demonstration of intentional information consumption

It is designed primarily for personal use.

---

# What NoBSTube Is Not

NoBSTube is not intended to become:

* A social network
* A video-sharing platform
* A creator economy
* An advertising platform
* An engagement-maximization system
* An infinite recommendation feed
* A behavioral profiling system
* A replacement social environment
* A platform that requires the user to maintain an account
* A system that tries to keep the user inside the application

NoBSTube should never need to ask:

> "How do we make the user stay longer?"

The more appropriate question is:

> "How do we help the user find what they wanted more effectively?"

---

# Core User Experience

The fundamental NoBSTube loop is:

```text
USER INTENT
     ↓
   SEARCH
     ↓
MULTIPLE SOURCES
     ↓
   FILTER
     ├── Hard Rules
     ├── User Rules
     └── AI Classification
     ↓
 RANK / SORT
     ↓
FINITE RESULTS
     ↓
 WATCH / SAVE / LEAVE
```

The application should make this loop easy to complete.

It should not introduce additional loops whose purpose is to extend the session.

---

# The Information Diet

One of NoBSTube's most important concepts is the idea of a **personal information diet**.

The user should be able to define categories of content that should generally be excluded from their discovery environment.

Examples might include:

* Influencer content
* Shock content
* Rage bait
* Clickbait
* Sensationalized material
* Certain entertainment categories
* Repetitive content
* Low-information content
* User-defined categories

These rules should persist.

The user should not have to repeatedly encounter the same unwanted category and manually dismiss it.

The principle is:

> **If the user knows they do not want something, the computer should help keep it out of their way.**

This is not intended to impose a universal definition of good or bad content.

Different users should be able to construct different information environments.

---

# AI's Role

AI is useful in NoBSTube because video metadata alone is often insufficient to determine whether a result is useful.

AI can help classify content according to the user's rules.

Possible AI tasks include:

* Categorization
* Content classification
* Relevance estimation
* User-defined exclusion detection
* Duplicate detection
* Metadata interpretation
* Ranking assistance
* Summarization where useful

The AI should remain subordinate to the user's intent.

## AI Should Not

The AI should not:

* Decide what the user should value
* Optimize for watch time
* Manufacture recommendations to increase engagement
* Create artificial urgency
* Hide why something was filtered where explanation is practical
* Become the only way to operate the application
* Prevent the user from overriding a classification

The system should be able to distinguish between:

```text
USER RULE
    ↓
AUTHORITATIVE FILTER
```

and:

```text
AI CLASSIFICATION
    ↓
BEST-EFFORT INTERPRETATION
```

AI classification should therefore be treated as a tool rather than unquestionable authority.

---

# Filtering Pipeline

The conceptual filtering pipeline is:

```text
SOURCE RESULTS
      ↓
NORMALIZE METADATA
      ↓
HARD REJECTION RULES
      ↓
USER FILTERS
      ↓
AI CLASSIFICATION
      ↓
RELEVANCE / QUALITY FILTERING
      ↓
SORTING
      ↓
FINITE RESULT SET
```

Where practical, inexpensive deterministic filtering should happen before expensive AI processing.

This reduces:

* AI computation
* Processing time
* Resource usage
* Unnecessary network activity

It also makes system behavior easier to understand.

---

# Multiple Video Sources

NoBSTube should treat video services as sources rather than as environments.

Initial sources include:

* YouTube
* PeerTube
* Internet Archive

Additional sources may be added later.

The architecture should make sources replaceable.

Conceptually:

```text
                NoBSTube
                    │
       ┌────────────┼────────────┐
       ↓            ↓            ↓
   YouTube       PeerTube   Internet Archive
       │            │            │
       └────────────┼────────────┘
                    ↓
              Unified Results
                    ↓
                Filtering
                    ↓
              User Interface
```

The user should not need to understand the implementation differences between sources in order to search them.

---

# Search

Search is the primary entry point.

The application should favor explicit search over passive discovery.

A search should have:

* A clear query
* Clearly visible filters
* Predictable sorting
* A finite result set
* Understandable result metadata
* A clear stopping point

Supported sorting should include useful criteria such as:

* Relevance
* Newest
* Oldest
* Views ascending
* Views descending
* Duration ascending
* Duration descending

Sorting should organize information rather than manipulate behavior.

---

# Finite Discovery

NoBSTube should deliberately avoid the concept of endless browsing.

The result set should be finite.

For example:

```text
Search
  ↓
100 candidates per source
  ↓
Classification / filtering
  ↓
Useful results
  ↓
10 results per page
  ↓
Page 1 ... Page N
```

Pagination should operate on a previously retrieved and classified candidate set where practical rather than triggering an entirely new search every time the user changes page.

This preserves predictability and reduces unnecessary network and AI work.

---

# Natural Stopping Points

A successful NoBSTube session should have an obvious end.

For example:

```text
Search
   ↓
Review results
   ↓
Find useful video
   ↓
Watch
   ↓
Done
```

There should be no requirement to continue.

The interface should not respond to completion with:

* "Keep watching"
* "You might also like..."
* Endless recommendations
* Artificial urgency
* Notifications
* Gamification

A person finishing their search is a successful outcome.

---

# Playback

When technically possible, video should play within NoBSTube.

The application should nevertheless recognize that the underlying video may belong to an external service.

If embedded or local playback is unavailable, NoBSTube should clearly explain the situation and provide an external link to the source.

The user should not be trapped.

The external platform is the **source of the video**, not the owner of the user's NoBSTube experience.

---

# Local-First Architecture

NoBSTube should remain useful as a local application even when network functionality is unavailable.

The network exists primarily to retrieve external information.

The application itself should remain local.

The conceptual architecture is:

```text
LOCAL COMPUTER
│
├── NoBSTube Application
├── Configuration
├── Filtering Rules
├── Local Database
├── Cached Metadata
├── AI Configuration
└── User Preferences
          │
          ↓
       INTERNET
          │
    ┌─────┼─────┐
    ↓     ↓     ↓
 YouTube PeerTube Archive
```

The network should extend the application rather than define it.

---

# No Unnecessary Accounts

NoBSTube should not require an account simply to perform basic video discovery.

Accounts introduce:

* Dependency
* Identity requirements
* Data collection
* Platform coupling
* Additional failure modes

For a local personal search application, they are generally unnecessary.

The preferred model is:

> Install the software. Configure it. Use it.

---

# Privacy and Ownership

NoBSTube should minimize unnecessary collection of information.

The application should avoid:

* Behavioral tracking
* Advertising profiles
* Engagement analytics
* Unnecessary telemetry
* Selling or sharing user activity

Where possible, information should remain on the user's machine.

The user should be able to understand where their:

* Search history
* Filtering rules
* Preferences
* Cached data
* AI configuration

are stored.

The user should be able to delete or export their local information.

---

# Thumbnails and Metadata

NoBSTube should prefer metadata and thumbnails supplied by the source where available.

The application should not needlessly generate replacement thumbnails.

Generated visual material can introduce:

* Additional processing
* Additional network requests
* Additional infrastructure
* Bot-detection problems
* Unnecessary complexity

The principle is:

> Use the information that already exists before creating more information.

---

# Interface Principles

The interface should remain deliberately simple.

The primary structure should make the following obvious:

```text
SEARCH
   ↓
FILTER
   ↓
SORT
   ↓
RESULTS
```

Important information should remain visible.

The interface should avoid:

* Infinite scrolling
* Engagement counters as primary UI
* Unnecessary animations
* Notification systems
* Social metrics
* Gamification
* Dark patterns
* Hidden filtering behavior
* Excessive interface chrome

The result grid should be useful rather than visually overwhelming.

---

# Performance

AI filtering can become the most expensive portion of the search process.

The system should therefore prioritize:

1. Fast initial source retrieval
2. Cheap deterministic filtering
3. Batched AI classification
4. Concurrency where appropriate
5. Classification caching
6. Streaming acceptable results where practical
7. Avoiding repeated work

A particularly important future goal is:

> Return the first useful results before the entire candidate set has finished processing.

This can make the system feel responsive even when the total classification workload is substantial.

---

# AI Classification Performance

The system should avoid treating every video as an isolated AI request when batching can provide better performance.

Potential architecture:

```text
SOURCE CANDIDATES
       ↓
HARD FILTER
       ↓
BATCH
 ┌───────────────┐
 │ Video 1       │
 │ Video 2       │
 │ Video 3       │
 │ ...           │
 │ Video N       │
 └───────────────┘
       ↓
     OLLAMA
       ↓
CLASSIFICATIONS
       ↓
FILTER / RANK
```

Classification results should be cacheable.

The same video should not necessarily need to be classified repeatedly when the relevant inputs have not changed.

---

# User-Defined Rules

User rules should be more important than hidden application assumptions.

A rule system should eventually allow users to express preferences such as:

```text
EXCLUDE:
    influencer content

EXCLUDE:
    shock content

PREFER:
    educational content

PREFER:
    technical demonstrations

PREFER:
    long-form explanations
```

The exact rule language can evolve.

The important architectural principle is that the user's information environment should be configurable.

---

# Source Independence

NoBSTube should not assume that one platform will always exist.

Source adapters should therefore be separated from:

* Search
* Filtering
* Classification
* Ranking
* Playback
* User interface

This makes it possible to add, remove, or replace sources without redesigning the entire application.

The user should own the layer that sits between themselves and the sources.

---

# Caching

Caching is valuable for both performance and intentional computing.

Potential cache targets include:

* Search results
* Video metadata
* Classification results
* Thumbnails
* Source responses

Caching can reduce:

* Network requests
* AI computation
* Search latency
* Dependence on external services

Caching should remain understandable and controllable.

The user should not have to wonder why stale information is appearing.

---

# Future Offline Capabilities

NoBSTube is primarily a discovery tool, but the broader Intentional Computing direction suggests potential future offline capabilities.

These could include:

* Local video archives
* Saved searches
* Cached metadata
* Saved classifications
* Local indexing
* Personal video collections

The long-term goal is not to download the entire internet.

It is to allow useful information to become part of the user's own computing environment when the user deliberately chooses to preserve it.

---

# Intentional Discovery Mode

A future feature could provide a bounded form of discovery.

Instead of:

> "Keep recommending things."

The system could offer:

> "Here are 10 things related to what you asked for."

The user could then:

* Review them
* Choose one
* Reject them
* Refine the search
* Stop

Discovery should remain bounded and user-directed.

---

# Relationship to the Personal Internet

NoBSTube is an early implementation of the broader **Personal Internet** concept.

The long-term model is:

```text
PERSON
   ↓
PERSONAL INFORMATION LAYER
   ↓
SEARCH / FILTER / AI / STORAGE
   ↓
PUBLIC INTERNET
   ↓
SELECTED INFORMATION
```

NoBSTube demonstrates this concept specifically for video.

Future personal-internet software could apply the same architecture to:

* Articles
* Documentation
* News
* Images
* Research
* Forums
* Public databases
* Other media

NoBSTube is therefore both a useful application and an architectural experiment.

---

# Intentional Computing Principles Demonstrated

| Principle                    | NoBSTube Implementation                |
| ---------------------------- | -------------------------------------- |
| Human agency                 | User chooses the search and filters    |
| Attention is not the product | No engagement optimization             |
| Completion over engagement   | Finite searches and natural stopping   |
| Search over feeds            | Search-first interface                 |
| Curation over volume         | Filtering and classification           |
| User-defined rules           | Persistent personal filters            |
| AI serves the user           | AI performs classification             |
| AI compresses complexity     | Large candidate sets become manageable |
| Local-first                  | Self-hosted application                |
| Ownership                    | Local configuration and data           |
| Source independence          | Multiple video providers               |
| No unnecessary accounts      | Basic use does not require an account  |
| Open information             | Multiple external sources              |
| Replaceability               | Source adapters remain modular         |
| Privacy by architecture      | Local data and minimal telemetry       |
| Right to stop                | No infinite result stream              |
| Right to leave               | No platform lock-in                    |

---

# Project Success Criteria

NoBSTube should not measure success using conventional platform metrics.

Poor measures include:

* Time spent in application
* Session length
* Number of videos watched
* Number of clicks
* Daily active users
* Return frequency
* Infinite scrolling depth

These metrics can encourage exactly the behavior the project is designed to avoid.

Better measures include:

* Time to useful result
* Search success rate
* Filtering accuracy
* Number of unwanted results avoided
* AI classification accuracy
* Search latency
* Classification latency
* Resource efficiency
* User control
* Ability to complete a task
* Ability to stop

The fundamental success question is:

> **Did NoBSTube help the user find what they wanted?**

---

# Intentional Computing Test

NoBSTube should continuously be evaluated against the following questions.

### Human Agency

Can the user control what they search for and what they see?

### Attention

Does the application require unnecessary attention?

### Completion

Can the user complete a search and naturally leave?

### Curation

Does the system reduce irrelevant information rather than increase it?

### AI

Does AI make the system more useful without taking control away from the user?

### Ownership

Can the user understand and control their local configuration and data?

### Privacy

Does the application collect information that it does not genuinely need?

### Independence

Can video sources be replaced without replacing the entire application?

### Exit

Can the user leave the application without losing access to their information?

### Purpose

Does every major feature help the user accomplish an explicit purpose?

---

# Anti-Patterns

The following should generally be rejected during development.

## Infinite Scroll

Do not replace pagination with an endless stream simply because it increases consumption.

## Autoplay Chains

Do not automatically start another video because the current one ended.

## Engagement Recommendations

Do not rank results according to what is likely to keep the user watching.

## Artificial Urgency

Do not manufacture urgency around ordinary video discovery.

## Notification Expansion

Do not introduce notifications merely to bring the user back.

## Hidden Personalization

Do not silently modify the user's information environment based on behavioral profiling.

## Platform Cloning

Do not reproduce unnecessary social-platform features merely because conventional video sites contain them.

## AI for Its Own Sake

Do not introduce AI when a simple deterministic solution is better.

## Infinite AI Processing

AI tasks must have bounded scope and a clear stopping condition.

## Unnecessary Accounts

Do not add account infrastructure without a real requirement.

---

# Development Priorities

Development should generally prioritize:

1. Correctness
2. User control
3. Search quality
4. Filtering quality
5. Performance
6. Local ownership
7. Reliability
8. Understandability
9. Source independence
10. Feature expansion

New features should be evaluated against the Intentional Computing principles before being added.

A feature that increases complexity or attention demand without providing proportional user value should be rejected.

---

# Future Development

Potential future improvements include:

* Faster AI classification
* Streaming first acceptable results
* Classification caching
* Better source adapters
* More precise filtering
* Better relevance ranking
* Improved playback support
* Local video archives
* Search history
* Saved searches
* Personal collections
* Configurable information diets
* Intentional discovery
* Local semantic search
* Personal indexing
* Better explanations for filtering decisions
* Offline-first capabilities
* Integration with the broader Personal Internet architecture

These should be implemented only when they provide meaningful user value.

---

# Relationship to the Intentional Computing Repository

NoBSTube is one of the primary demonstration projects for Intentional Computing.

It demonstrates that the philosophy can be implemented in practical software rather than remaining purely theoretical.

The relationship is:

```text
Intentional Computing
        ↓
     Principles
        ↓
      Design
        ↓
      NoBSTube
        ↓
     Real Software
```

NoBSTube therefore serves as a test of whether the principles actually produce useful software.

If the principles make the application worse without providing meaningful benefits, the principles should be reconsidered.

If the principles produce a system that is more useful, more understandable, less demanding, and more controlled, the project provides evidence that the approach is viable.

---

# Long-Term Vision

The long-term vision for NoBSTube is not to become the next YouTube.

It is almost the opposite.

The goal is to demonstrate that a person can use the enormous video resources of the modern internet without having to adopt the behavioral environment of the platforms that host them.

The internet provides the information.

NoBSTube provides a personal layer for accessing it.

The user provides the intent.

AI provides additional computational capability.

The computer performs the complexity.

The person makes the decisions.

And when the useful work is finished:

> **The application should let the user leave.**

---

# Final Principle

NoBSTube should always remember what it is for.

It is not here to maximize viewing.

It is not here to maximize engagement.

It is not here to become indispensable.

It is not here to compete for attention.

It is here to help a person find useful video information.

The ideal NoBSTube session is therefore:

```text
I know what I want.
        ↓
I search for it.
        ↓
NoBSTube removes what I don't want.
        ↓
I find something useful.
        ↓
I watch it.
        ↓
I'm finished.
        ↓
I close NoBSTube.
        ↓
I return to my life.
```

That is not a failed session.

**That is a successful one.**
