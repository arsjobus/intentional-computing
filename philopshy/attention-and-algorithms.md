# Attention and Algorithms

> **Human attention is a finite resource. Software should help people direct it, not compete to capture it.**

Modern computing has created an unusual situation.

Machines can now understand enormous amounts of information, predict behavior, personalize experiences, and generate content at extraordinary speed.

But human attention has not changed.

A person still has:

* limited time
* limited concentration
* limited working memory
* limited emotional energy
* limited ability to process information

The machines have become effectively unlimited.

The human has not.

Intentional Computing therefore treats **attention as a resource that technology should protect**.

---

# 1. The Attention Problem

The modern digital environment is often described as an information problem.

There is too much information.

But information volume is only part of the problem.

The deeper problem is that systems increasingly compete to determine **which information receives human attention**.

Consider the difference:

```text
INFORMATION PROBLEM

There is too much information.
        ↓
We need better filtering.
```

versus:

```text
ATTENTION PROBLEM

There are many systems
competing for attention.
        ↓
Each system attempts
to become more compelling.
        ↓
Human attention becomes
the scarce resource.
```

The second problem is much more important.

---

# 2. Attention Is Finite

A person cannot pay attention to everything.

Every:

* notification
* video
* headline
* message
* advertisement
* recommendation
* alert
* popup
* feed item

competes, directly or indirectly, for some portion of attention.

This creates an important asymmetry:

```text
MACHINE
────────
Can generate:
∞ information
∞ recommendations
∞ notifications
∞ content

HUMAN
─────
Has:
finite time
finite attention
finite energy
```

This asymmetry should influence how software is designed.

---

# 3. Algorithms Are Not the Enemy

Algorithms themselves are not inherently harmful.

An algorithm can:

* sort a list
* find a file
* compress an image
* detect spam
* translate text
* route traffic
* classify information
* recommend something useful
* help solve a problem

The issue is not:

> "Algorithms exist."

The issue is:

> **What objective is the algorithm optimizing?**

The same technical capability can serve radically different goals.

---

# 4. Optimization Determines Behavior

Suppose a system can predict which content a person is likely to interact with.

That prediction can be used to:

### Optimize for usefulness

```text
What information best answers the user's question?
```

Or:

### Optimize for engagement

```text
What information is most likely to keep the user interacting?
```

These are not equivalent objectives.

The first tries to solve a problem.

The second tries to extend a session.

Intentional Computing favors the first.

---

# 5. The Engagement Loop

A common digital pattern is:

```text id="f2b2s4"
USER
  ↓
CONTENT
  ↓
INTERACTION
  ↓
RECOMMENDATION
  ↓
MORE CONTENT
  ↓
MORE INTERACTION
  ↓
MORE RECOMMENDATION
  ↓
...
```

The system does not need a natural endpoint.

In fact, an endpoint can be undesirable if continued interaction is the objective.

This creates the **engagement loop**.

The loop becomes particularly powerful when the system continuously learns which stimuli produce responses.

---

# 6. Behavioral Optimization

Modern systems can measure enormous amounts of behavior.

For example:

* what was clicked
* what was ignored
* how long something was viewed
* what was searched
* what was shared
* what was replayed
* what was abandoned
* what was purchased
* when the user returned

This information can be used to improve the system.

The question is:

> Improve it for whom?

A system can become extremely good at predicting behavior without becoming better at serving the person's actual interests.

This distinction is central.

---

# 7. Engagement Is Not the Same as Value

A person spending an hour inside an application does not necessarily mean the application provided an hour of value.

Likewise:

> Less time spent does not necessarily mean less value.

Consider two systems.

### System A

A user searches for a technical answer.

The system finds the answer in three minutes.

The user leaves.

```text
Usage: 3 minutes
Value: high
```

### System B

A user searches for the same answer.

The system provides:

* related content
* recommendations
* trending topics
* notifications
* suggested videos

The user spends an hour exploring.

```text
Usage: 60 minutes
Value: uncertain
```

An engagement metric might prefer System B.

An intentional system may prefer System A.

---

# 8. Completion Is the Better Metric

Intentional Computing proposes a different success metric:

> **Did the user accomplish what they intended to accomplish?**

This is much harder to measure than screen time.

But it is much more meaningful.

A useful conceptual model is:

```text
SUCCESS
   │
   ├── Task completed
   ├── Information found
   ├── Problem solved
   ├── Creation finished
   └── User can leave
```

The last point is important.

A system should not regard the user's departure as failure.

---

# 9. The Feed

The feed is one of the most consequential interface patterns in modern computing.

A feed removes the question:

> What should I do next?

The system answers it automatically.

This is convenient.

It is also powerful.

Once the system controls what appears next, it controls a significant portion of the user's information environment.

---

# 10. Why Infinite Feeds Matter

A finite list has an endpoint.

An infinite feed does not.

Consider:

```text
1
2
3
4
5
...
```

There is no natural reason to stop at item 5.

The user must create the stopping point themselves.

An infinite feed therefore transfers the responsibility for stopping from the software to the human.

That may seem harmless.

At large scale, it matters.

---

# 11. The Infinite Scroll

Infinite scroll combines several properties:

* continuous content
* automatic loading
* minimal friction
* no clear endpoint
* algorithmic ranking

The resulting experience is:

```text id="r4h8i1"
CONTENT
   ↓
MORE CONTENT
   ↓
MORE CONTENT
   ↓
MORE CONTENT
   ↓
MORE CONTENT
   ↓
...
```

The interface does not ask:

> Are you finished?

It simply continues.

Intentional Computing therefore prefers **finite interfaces where practical**.

---

# 12. Natural Stopping Points

A healthy system can make stopping easy.

Examples include:

* a completed task
* a finite result set
* the end of an article
* the end of a document
* the end of a playlist
* the end of a game session
* a saved checkpoint

Stopping should not feel like leaving something unfinished.

A useful principle is:

> **Software should make completion visible.**

---

# 13. Recommendation

Recommendations are not inherently bad.

A recommendation can be extremely useful when the user wants one.

For example:

> "I need a good introductory book on this subject."

A recommendation can save considerable time.

The problem occurs when recommendation becomes the default relationship.

Instead of:

```text
USER → SEARCH → RESULT
```

the system becomes:

```text
SYSTEM → RECOMMEND → USER → RECOMMEND → USER
```

The second model shifts control toward the system.

---

# 14. Recommendation Should Be User-Directed

A more intentional model is:

```text
USER
  │
  │ "Find something like this."
  ▼
RECOMMENDATION ENGINE
  │
  ▼
SMALL SET OF OPTIONS
  │
  ▼
USER DECIDES
```

The user requested recommendation.

The system performs the work.

Then the user decides.

This keeps recommendation subordinate to intent.

---

# 15. Personalization

Personalization can make software dramatically better.

It can remember:

* preferences
* language
* interface settings
* favorite formats
* accessibility needs
* recurring workflows
* source preferences

But personalization can also become manipulation.

The key distinction is:

> **Personalization should make the software better for the user, not make the user easier for the software to influence.**

This distinction should guide every personalization feature.

---

# 16. Manipulation

A system becomes increasingly problematic when it deliberately uses knowledge of the user to produce behavior that primarily benefits the system.

Examples include:

* artificial urgency
* guilt-based prompts
* repeated notifications
* fear of missing out
* deliberately confusing controls
* hiding alternatives
* friction when leaving
* recommendations designed primarily for retention

These patterns are not necessary for useful software.

They are optimization strategies.

Intentional Computing rejects them.

---

# 17. Notifications

Notifications are one of the simplest ways software can interrupt attention.

Every notification effectively says:

> **Stop what you are doing and look at me.**

That is an extraordinary request.

Therefore notifications should earn their place.

A useful hierarchy might be:

```text
CRITICAL
Immediate attention may be justified.

IMPORTANT
Should be seen reasonably soon.

INFORMATIONAL
Can wait until the user checks.

OPTIONAL
Should generally remain inside the application.
```

Most software generates too many notifications because the cost of interruption is externalized onto the user.

---

# 18. Notifications Should Be Pull-Based Where Possible

Instead of:

```text
APPLICATION
    ↓
INTERRUPT
    ↓
USER
```

prefer:

```text
APPLICATION
    ↓
INFORMATION AVAILABLE
    ↓
USER CHECKS WHEN READY
```

The user remains in control of timing.

This is particularly valuable for:

* news
* recommendations
* social activity
* updates
* non-urgent information

---

# 19. Artificial Urgency

Many systems attempt to make ordinary information feel urgent.

Examples include:

* "Don't miss out."
* "Only available now."
* "Trending."
* "Everyone is talking about this."
* "You haven't checked in."
* "Come back."
* "Something is waiting for you."

Urgency can be legitimate.

But it should not be manufactured simply to increase engagement.

Intentional software should distinguish:

```text
REAL URGENCY
Something genuinely needs attention.
```

from:

```text
ARTIFICIAL URGENCY
The system wants attention.
```

---

# 20. The Difference Between Alerting and Interrupting

A notification can communicate information without demanding immediate action.

This suggests a useful design distinction:

```text
ALERT
"Something happened."

INTERRUPTION
"Stop what you're doing now."
```

Most events should be alerts.

Only a small subset should become interruptions.

---

# 21. Algorithmic Feeds and Agency

When an algorithm decides what appears next, it is making a series of choices on behalf of the user.

Those choices can be useful.

But the user should have meaningful alternatives.

An intentional system should ideally allow:

* chronological order
* relevance sorting
* source selection
* filtering
* finite result sets
* search
* explicit recommendation modes
* disabling recommendations

The algorithm should assist navigation.

It should not become the only navigation mechanism.

---

# 22. Transparency

Users do not need to understand every line of an algorithm.

But they should understand enough to make meaningful choices.

Useful transparency can include:

* why something was shown
* what filters were applied
* what sources were searched
* whether AI was involved
* what preferences affected ranking
* whether results are sponsored
* what information is being used

A simple explanation can restore significant agency.

---

# 23. User-Controlled Ranking

Ranking is unavoidable whenever there are more results than can be displayed.

The important question is:

> Who controls the ranking?

Possible inputs include:

```text
USER PREFERENCE
SOURCE QUALITY
DATE
RELEVANCE
POPULARITY
AI CLASSIFICATION
```

The user should be able to understand and, where practical, configure those inputs.

A ranking system should not become an invisible authority.

---

# 24. AI Changes the Equation

AI makes algorithmic systems considerably more powerful.

Traditional systems might rank content using relatively simple signals.

AI can now:

* understand language
* classify images
* analyze video
* summarize documents
* infer relationships
* predict relevance
* generate content
* adapt to user preferences

This creates enormous opportunities.

It also makes intentionality more important.

The more capable the system becomes at influencing information flow, the more important it is that the **objective remains aligned with the person**.

---

# 25. AI Should Filter Before It Amplifies

There is an enormous amount of content in the world.

AI could make it easier to generate even more.

That is not necessarily the most valuable use.

One of the most valuable uses may instead be:

> **AI should help humans deal with the information that already exists.**

For example:

```text
Internet
   │
   ▼
Millions of items
   │
   ▼
AI filtering
   │
   ├── Remove duplicates
   ├── Remove spam
   ├── Apply user rules
   ├── Identify relevance
   ├── Summarize
   └── Classify
   │
   ▼
Human-scale information
```

This is AI as a compression system rather than an attention-generation system.

---

# 26. The Attention Budget

A useful concept for future software is an **attention budget**.

Every system should implicitly ask:

> How much attention am I asking this person to spend?

That includes:

* reading
* clicking
* configuring
* responding
* monitoring
* remembering
* switching contexts
* dealing with notifications

A system that saves five minutes of mechanical work but creates ten minutes of cognitive overhead is not necessarily better.

The true objective should be:

> **Reduce total human effort.**

---

# 27. Cognitive Load Matters

Attention is not merely time.

A system can consume attention without being used for long.

For example:

* remembering where something is
* interpreting unclear controls
* deciding between too many options
* recovering from unexpected behavior
* monitoring background processes

Intentional Computing therefore also considers **cognitive load**.

The computer should handle complexity wherever practical.

---

# 28. Choice Overload

More options are not always better.

Suppose a user asks for a recommendation.

Giving:

```text
10,000 results
```

may technically provide more choice.

But giving:

```text
5 strong options
```

may provide more useful freedom.

This is the difference between:

> **More possibilities**

and:

> **More usable choices.**

Curation can therefore increase agency rather than reduce it.

---

# 29. Filtering Is Not Censorship

A personal filter is different from a universal information restriction.

A user saying:

> "I don't want this category in my personal environment."

is exercising control over their own attention.

Another person may make a different choice.

Intentional Computing therefore strongly supports **user-defined filtering**.

The personal environment should reflect the individual.

---

# 30. The Right to Ignore

A healthy digital environment should make it easy to ignore things.

The user should not have to:

* dismiss the same prompt repeatedly
* unsubscribe from dozens of lists
* fight recommendation systems
* constantly explain preferences
* close popups
* reject notifications

Good software remembers the user's choice.

> **No should mean no.**

---

# 31. The Right to Stop

Likewise, stopping should be easy.

The user should be able to:

* close the application
* stop a process
* disable notifications
* leave a service
* export data
* delete local data
* turn off recommendations

without being pressured to reconsider.

The software should not argue with the user.

---

# 32. The Right to Leave

The strongest expression of agency is the ability to leave.

A healthy system should not create artificial barriers such as:

* difficult exports
* obscure account deletion
* proprietary formats without justification
* unnecessary subscriptions
* dependency on one service
* loss of personal history

The user should retain an exit path.

---

# 33. The 90s Contrast

Earlier personal computing generally had much weaker behavioral optimization.

A computer could be distracting.

Games could certainly consume time.

But software was generally not connected to a continuously learning system whose business objective was to maximize ongoing engagement at enormous scale.

The distinction matters.

The goal is not to romanticize the past.

It is to recognize what has changed.

Modern technology can be much better at capturing attention.

Therefore modern technology needs much better **boundaries**.

---

# 34. A Better Optimization Function

Intentional Computing suggests a different conceptual objective.

Instead of:

```text
MAXIMIZE
────────
Engagement
Session length
Interactions
Notifications
Return frequency
```

prefer:

```text
MAXIMIZE
────────
Useful outcomes
Task completion
User satisfaction
Clarity
Capability
Ownership
Autonomy

MINIMIZE
────────
Unnecessary attention
Cognitive load
Dependency
Interruption
Friction
Manipulation
```

This is not merely a product decision.

It is a different definition of success.

---

# 35. Measuring the Right Things

A future Intentional Computing application might measure:

* tasks completed
* time saved
* errors avoided
* information successfully found
* user-defined goals achieved
* successful exports
* offline functionality
* recovery from failures

rather than primarily measuring:

* daily active users
* session duration
* clicks
* scrolling
* notification interactions
* return frequency

These metrics lead software development in different directions.

---

# 36. An Intentional Recommendation System

A recommendation system can be designed differently.

For example:

```text
USER:

"I want five interesting documentaries
about early computing."
```

The system:

```text
SEARCH
  ↓
FILTER
  ↓
CLASSIFY
  ↓
REMOVE UNWANTED CONTENT
  ↓
SELECT FIVE
  ↓
PRESENT RESULTS
```

Then:

```text
DONE
```

The system does not need to automatically generate:

```text
Related videos
More recommendations
Trending videos
Recommended channels
Daily suggestions
Notifications
```

unless the user asks for them.

---

# 37. Discovery Without Dependency

Discovery is valuable.

The goal is not to eliminate it.

The goal is to separate:

> **Discovering something useful**

from:

> **being continuously exposed to novelty.**

A deliberate discovery tool might provide:

> "Show me ten things I probably would not have found myself."

That is useful.

The user then chooses.

Discovery becomes a tool rather than a permanent environment.

---

# 38. The Algorithm Should Work for the User

Algorithms are most valuable when they perform work the user would otherwise have to perform manually.

For example:

```text
Human:
"Look through 5,000 documents and find the
ones relevant to this project."

AI:
"Here are the 12 that appear relevant."
```

The machine has saved the human enormous effort.

That is good automation.

The same capability becomes problematic when the algorithm instead says:

```text
"Here are 12 things designed to keep you here."
```

The technical sophistication may be identical.

The objective is different.

---

# 39. The Attention Contract

Every software system implicitly creates an attention contract with its user.

A healthy contract is:

> "You give me enough attention to accomplish the task, and I will help you complete it."

An unhealthy contract is:

> "You give me as much attention as I can obtain."

Intentional Computing adopts the first.

---

# 40. Technology Should Give Attention Back

The ultimate purpose of automation is not to create more digital activity.

It is to return time and attention to the human.

```text id="o9y0d6"
AUTOMATION
    ↓
LESS MANUAL WORK
    ↓
LESS COGNITIVE LOAD
    ↓
LESS SCREEN TIME
    ↓
MORE HUMAN TIME
```

This is a powerful measure of technological progress.

---

# 41. The Human Should Remain the Objective

An algorithm can optimize almost anything.

The critical question is what sits at the top of the objective function.

Intentional Computing places the human there.

Not:

* engagement
* advertising
* growth
* retention
* data collection
* platform dependency

but:

* capability
* autonomy
* usefulness
* understanding
* completion
* ownership
* time

---

# 42. Final Principle

The future will contain increasingly powerful algorithms.

That is inevitable.

The important decision is what those algorithms are built to do.

They can become:

```text
MACHINES THAT COMPETE FOR PEOPLE
```

or:

```text
MACHINES THAT WORK FOR PEOPLE
```

Intentional Computing chooses the second.

Algorithms should help people:

* find
* understand
* create
* decide
* organize
* automate
* communicate
* preserve

They should not make themselves the center of the person's life.

The ultimate goal is simple:

```text
HUMAN INTENTION
       ↓
ALGORITHM
       ↓
USEFUL RESULT
       ↓
COMPLETION
       ↓
LIFE
```

Not:

```text
HUMAN
  ↓
ALGORITHM
  ↓
ENGAGEMENT
  ↓
MORE ENGAGEMENT
  ↓
MORE ENGAGEMENT
  ↓
...
```

> **The best algorithm is not the one that keeps the user engaged the longest.**
>
> **It is the one that helps the user accomplish what they came to do—and then lets them leave.**
