# Mirage

## Project Purpose

Mirage is a lightweight, local-first pixel art and sprite editing application designed around the principles of Intentional Computing.

Its purpose is to provide a focused creative tool for making pixel art without turning the creative process into a subscription service, social platform, cloud environment, or unnecessarily complicated software ecosystem.

Mirage is intended to provide the capabilities a person needs to create pixel art while keeping the underlying system understandable, local, portable, and owned by the user.

The fundamental idea is:

> **A creative application should help a person make something, not become the place where the person is expected to live.**

---

# Why Mirage Exists

Modern creative software can be extremely capable.

It can also become increasingly complicated through:

* Cloud dependencies
* Subscription models
* Account requirements
* Online services
* Large dependency stacks
* Platform lock-in
* Proprietary project formats
* Social features
* AI features that are difficult to understand or control
* Interfaces designed around feature accumulation
* Constant updates
* Increasingly complex workflows

Pixel art is a particularly useful domain for exploring a different approach.

The fundamental operations are understandable:

* Draw a pixel
* Erase a pixel
* Choose a color
* Select an area
* Move something
* Copy something
* Create a frame
* Edit a sprite
* Save a file

The software can provide powerful capabilities without making the basic task complicated.

Mirage therefore explores:

> **How capable can a modern creative tool become while remaining understandable and calm?**

---

# Project Philosophy

Mirage applies the Intentional Computing principles to creative software.

### Creation Over Consumption

The application exists primarily to help the user create something.

It should not encourage endless browsing, social comparison, or passive consumption.

### Direct Manipulation

The user should be able to interact directly with the artwork.

If a person wants to change a pixel, they should be able to change the pixel.

### Visible State

The user should be able to understand:

* What tool is active
* What is selected
* What layer is active
* What color is selected
* What frame is active
* What changes have been made

### Local Ownership

The artwork should exist as a local file under the user's control.

The application should not require a remote service for ordinary creation.

### Open and Portable Data

Users should be able to preserve their work independently of Mirage where practical.

### Progressive Complexity

Basic pixel editing should remain simple.

More advanced capabilities can be available without forcing every user to understand them.

### Completion

When the artwork is finished, the application should get out of the way.

---

# What Mirage Is

Mirage is intended to be:

* A pixel art editor
* A sprite editor
* An animation editor
* A local creative application
* A palette-oriented graphics tool
* A sprite-sheet tool
* A tool for retro game development
* A tool for editing assets for NES, SNES, and similar systems
* A general-purpose pixel-art workspace

It should remain useful without an internet connection.

---

# What Mirage Is Not

Mirage is not intended to become:

* A social network
* An online art community
* A cloud storage service
* A subscription platform
* A marketplace
* A content feed
* An engagement platform
* A mandatory AI assistant
* A platform that requires an account for basic use

Mirage should not attempt to compete with every professional graphics application by accumulating every possible feature.

Its purpose is focused capability.

---

# Core User Experience

The primary creative loop should be:

```text id="v9i2nm"
INTENTION
    ↓
CREATE / EDIT
    ↓
SEE RESULT
    ↓
REFINE
    ↓
SAVE
    ↓
COMPLETION
```

The application should make this loop feel direct.

The interface should stay out of the way of the artwork.

---

# The Canvas Comes First

The canvas is the central object of Mirage.

The user should always be able to understand:

* Where the artwork is
* What area is being edited
* What scale is being used
* What pixels are affected
* What selection is active

Interface elements should support the canvas rather than compete with it.

The application should not surround a small editing area with unnecessary interface complexity.

---

# Pixel-First Editing

Pixel art has a fundamentally different relationship with the canvas than ordinary raster graphics.

Individual pixels can matter.

Mirage should therefore make pixel-level manipulation precise.

Core operations should include:

* Pencil
* Eraser
* Color selection
* Eyedropper
* Fill
* Line
* Rectangle
* Selection
* Move
* Copy
* Paste
* Transform where appropriate

The user should be able to zoom deeply into the artwork while retaining a clear understanding of the original pixel grid.

---

# Direct Manipulation

Whenever possible, the interface should allow the user to manipulate the artwork directly.

For example:

```text id="r6sy9x"
CLICK PIXEL
     ↓
CHANGE PIXEL
```

rather than requiring the user to navigate through several dialogs.

Similarly:

```text id="7zgl5n"
SELECT
   ↓
MOVE
   ↓
PLACE
```

should be straightforward.

Direct manipulation reduces the distance between intention and result.

---

# Canvas Zoom

Pixel art often requires significant magnification.

Mirage should support substantial zoom levels while preserving the relationship between the visible image and the actual pixel grid.

The user should be able to move between:

```text id="y0b1e9"
PIXEL LEVEL
    ↕
SPRITE LEVEL
    ↕
FULL IMAGE LEVEL
```

without losing context.

Zoom should change how the artwork is viewed, not change the artwork itself.

---

# Grid

A pixel grid should be available when useful.

The grid should make individual pixels obvious at high magnification without becoming visually distracting.

The user should be able to control:

* Grid visibility
* Grid behavior
* Zoom level
* Canvas presentation

The grid is a tool for precision, not decoration.

---

# Color and Palette

Pixel art often depends heavily on controlled palettes.

Mirage should therefore treat color selection as an important part of the workflow.

Potential capabilities include:

* Foreground/background colors
* Palette editing
* Palette creation
* Palette saving
* Color picking
* Color replacement
* Palette restriction
* Palette import/export

Palette operations should remain understandable.

The application should not obscure the actual colors being used behind unnecessarily abstract systems.

---

# Layers

Layers provide useful separation for more complex artwork.

Mirage should support layers while keeping their behavior obvious.

Users should be able to understand:

* Which layer is active
* Which layers are visible
* Which layers are locked
* Layer ordering
* Layer opacity where appropriate

Layer operations should be reversible.

The basic pixel-editing workflow should remain understandable even for users who do not need sophisticated layer workflows.

---

# Animation

Animation is a natural extension of pixel art.

Mirage should eventually support frame-based animation.

The fundamental model should remain understandable:

```text id="i8r3qv"
FRAME 1
FRAME 2
FRAME 3
FRAME 4
...
```

The user should be able to:

* Create frames
* Duplicate frames
* Delete frames
* Reorder frames
* Edit frames
* Preview animation
* Control frame timing

Animation controls should not obscure the artwork.

---

# Sprite Sheets

Sprite sheets are an important use case for Mirage.

The application should support working with collections of sprites in a single image.

Potential capabilities include:

* Grid-based sprite selection
* Sprite extraction
* Sprite arrangement
* Sprite duplication
* Sprite-sheet preview
* Sprite-sheet export
* Configurable tile dimensions

This is particularly relevant to retro game development.

---

# Retro Game Development

Mirage is intended to work particularly well alongside retro computing and emulator projects.

Potential workflows include:

```text id="3v4h2d"
GAME PROJECT
     ↓
SPRITE DATA
     ↓
MIRAGE
     ↓
EDIT ARTWORK
     ↓
EXPORT
     ↓
ROM / ASSET PIPELINE
```

The application should not need to understand every game engine.

Instead, it should provide reliable tools that can participate in external asset pipelines.

---

# NES and SNES Workflows

The Intentional Computing project includes preservation and development work around older hardware.

Mirage should therefore eventually support workflows relevant to:

* NES
* SNES
* Other tile-based systems

This may include:

* Tile-sized editing
* Palette limitations
* Sprite constraints
* Tile maps
* Sprite sheets
* Indexed color
* Export formats
* External tooling integration

The application should not hide hardware limitations from the user when those limitations are important.

Instead, constraints should become visible and useful.

---

# Sprite and Tile Tooling

Mirage should be able to work alongside dedicated sprite/tile tooling.

A broader workflow may eventually look like:

```text id="7b2f8s"
ORIGINAL ROM
     ↓
EXTRACTION TOOL
     ↓
SPRITE / TILE DATA
     ↓
MIRAGE
     ↓
ART EDITING
     ↓
MAPPING / ASSEMBLY TOOL
     ↓
REBUILD
     ↓
MODIFIED ROM
```

This separation is intentional.

Mirage does not need to become a ROM hacking tool merely because it is used within a ROM editing workflow.

Each tool can have a clear responsibility.

---

# Local-First Architecture

Mirage should be designed as a local application first.

The core editing workflow should not depend on:

* Internet access
* Cloud services
* Remote accounts
* Subscription validation
* Online storage

The basic relationship should be:

```text id="2a0s6c"
USER
  ↓
MIRAGE
  ↓
LOCAL FILE
```

The network should not be required for ordinary artwork creation.

---

# No Account Required

A pixel editor should not require an online identity simply to create a file.

Mirage should therefore avoid mandatory accounts.

The ideal initial experience is:

```text id="p0n9au"
Launch Mirage
     ↓
Create New Image
     ↓
Draw
     ↓
Save
```

No registration should be necessary.

---

# File Ownership

Artwork created with Mirage belongs to the user.

The application should make it straightforward to:

* Save files
* Copy files
* Back up files
* Move files
* Open files elsewhere
* Export artwork
* Archive projects

The user's work should not be trapped inside Mirage.

---

# Open Formats

Where practical, Mirage should support widely understood formats.

Potential formats include:

* PNG
* GIF where appropriate
* BMP where useful
* Other established image formats
* A documented native project format

The native project format should be documented sufficiently that users are not dependent on Mirage forever.

The principle is:

> **A creative application should preserve the user's work, not imprison it.**

---

# Native Project Format

Mirage may require a native format for information that ordinary image formats cannot represent.

For example:

* Layers
* Animation
* Palettes
* Selections
* Metadata
* Guides
* Project settings

A native format is acceptable when it provides meaningful value.

However, it should be:

* Documented
* Versioned
* Portable
* Backward-compatible where practical
* Recoverable
* Exportable

The native format should not become a lock-in mechanism.

---

# Undo and Reversibility

Creative work requires experimentation.

Mirage should therefore make actions reversible wherever practical.

Undo should be reliable.

The user should be able to experiment without fearing that a mistake will permanently destroy their work.

Important operations should have predictable undo behavior.

The principle is:

> **Make experimentation safe.**

---

# Selection

Selection is one of the most important tools in a graphics editor.

Mirage should provide clear selection behavior.

Potential selection operations include:

* Rectangular selection
* Free selection
* Color-based selection
* Invert selection
* Expand/contract where appropriate
* Copy
* Cut
* Paste
* Move

The active selection should always be visible.

Hidden selection state is dangerous because the user may not understand why an operation is affecting only part of the image.

---

# Interface Philosophy

Mirage should favor a calm, tool-oriented interface.

A conceptual layout might be:

```text id="u9d8h1"
┌──────────────────────────────────────────┐
│ Menu / Toolbar                           │
├───────┬──────────────────────┬───────────┤
│ Tools │                      │ Layers /  │
│       │       CANVAS         │ Palette   │
│       │                      │           │
│       │                      │           │
├───────┴──────────────────────┴───────────┤
│ Status / Zoom / Frame                    │
└──────────────────────────────────────────┘
```

The exact interface may change.

The principle should not:

> **The artwork is the primary content.**

---

# Progressive Complexity

Mirage should support beginners and experienced users without forcing either group into the other's workflow.

Basic operations should remain immediately accessible.

Advanced functionality can be progressively exposed.

For example:

```text
Basic
 ├── Pencil
 ├── Eraser
 ├── Color
 ├── Fill
 └── Selection

Advanced
 ├── Layers
 ├── Animation
 ├── Palette tools
 ├── Sprite tools
 └── Hardware constraints
```

Complexity should be available when needed rather than permanently visible.

---

# Keyboard and Mouse

Direct manipulation should work well with both keyboard and pointer input.

Common operations should have predictable shortcuts.

The user should be able to work quickly without navigating menus repeatedly.

Keyboard shortcuts should remain consistent.

The interface should not force mouse-only interaction where keyboard interaction would be more efficient.

---

# Tool State

The application should make current state visible.

At minimum, users should be able to determine:

* Current tool
* Primary color
* Secondary color
* Zoom
* Active layer
* Active frame
* Selection state
* Canvas dimensions

The user should not need to remember hidden application state.

---

# AI and Mirage

AI should not automatically become a central part of Mirage.

Pixel art is a domain where direct human creation is valuable.

AI may eventually provide useful capabilities, but those capabilities should be optional.

Potential useful AI features might include:

* Explaining a technical operation
* Helping organize assets
* Assisting with repetitive transformations
* Describing an image
* Helping convert formats
* Assisting with external tooling

AI should not replace the fundamental act of drawing when the user wants to draw.

The principle is:

> **Use AI where it removes tedious complexity, not where it removes meaningful creative control.**

---

# Automation

Automation can be valuable for repetitive work.

Potential automation includes:

* Batch export
* Palette conversion
* Sprite-sheet generation
* Image resizing
* Format conversion
* Asset validation

Automation should remain explicit.

The user should know what operation is about to happen and which files it will affect.

Automation should not silently modify unrelated artwork.

---

# Command-Line Integration

Mirage should work well alongside command-line tools.

This is especially useful for retro development pipelines.

A possible workflow:

```text id="6vckb9"
Mirage
  ↓
Export
  ↓
CLI Tool
  ↓
ROM / Asset Build
```

Command-line tooling should complement the graphical editor rather than duplicate it unnecessarily.

---

# External Tool Integration

Mirage should be designed to coexist with specialized tools.

Examples include:

* ROM extraction tools
* Tile mappers
* Asset converters
* Emulator projects
* Build systems
* Image processing tools

The goal is not to make Mirage responsible for everything.

A healthy ecosystem can contain several small tools that work together.

---

# Dependencies

Mirage should prefer a small and understandable dependency footprint.

The current direction is:

* Java
* JavaFX
* Maven

Gradle is deliberately not required.

The build environment should remain straightforward.

The application should avoid dependency complexity that does not provide meaningful value to the user.

---

# Platform Independence

Java and JavaFX provide a useful foundation for a cross-platform creative application.

The goal is for Mirage to eventually operate on common desktop platforms without requiring a different conceptual application for each platform.

The user experience should remain consistent while still respecting platform conventions.

---

# Offline Capability

Mirage should work fully offline for its core functionality.

A person should be able to:

```text id="f5m8op"
Disconnect Internet
       ↓
Launch Mirage
       ↓
Create Artwork
       ↓
Save Artwork
       ↓
Close Mirage
```

Nothing about this workflow should require a remote service.

Offline operation is not an emergency mode.

It is a legitimate operating mode.

---

# Privacy

Mirage should minimize unnecessary data collection.

The application should not require:

* Advertising identifiers
* Behavioral tracking
* Usage analytics
* Cloud accounts
* Remote project storage

If telemetry is ever considered, it should be:

* Optional
* Clearly explained
* Minimal
* User-controlled

Privacy should be architectural rather than merely contractual.

---

# Notifications

Mirage should generally have no reason to interrupt the user.

A creative application should not need to send:

* Promotional notifications
* Engagement reminders
* "Come back" messages
* Social notifications
* Artificial urgency

The application should wait for the user.

---

# Updates

Updates should improve the application without undermining ownership.

An update should not:

* Remove access to existing files
* Require a new account
* Force cloud storage
* Change the native format without migration
* Remove established workflows unnecessarily

Updates should respect existing work.

---

# Preservation

Mirage should be designed to remain useful over time.

The project should consider:

* File format longevity
* Exportability
* Documentation
* Build reproducibility
* Dependency stability
* Version compatibility
* Migration paths

A pixel editor should be able to open artwork years after it was created.

---

# Simplicity and Capability

Mirage should not confuse simplicity with lack of power.

The objective is:

> **Simple interface, powerful underlying capability.**

The internal implementation can be sophisticated where necessary.

The user-facing experience should remain understandable.

Complexity should be absorbed by the machine where doing so gives the user greater clarity.

---

# Creation as the Primary Metric

Mirage should not measure success by:

* Time spent in the application
* Number of sessions
* Number of clicks
* Number of features used
* Number of panels opened

A better measure is:

> **Did the user successfully create or modify the artwork they intended to create?**

The ideal session is often:

```text id="x4r3sk"
Open Mirage
    ↓
Create / Edit
    ↓
Save
    ↓
Close Mirage
```

A short successful session is better than a long session caused by unnecessary complexity.

---

# Intentional Computing Principles Demonstrated

| Principle                 | Mirage Implementation                                |
| ------------------------- | ---------------------------------------------------- |
| Human agency              | User directly controls artwork                       |
| Creation over consumption | Primary purpose is making things                     |
| Direct manipulation       | Pixel and canvas editing                             |
| Completion                | Save and close without engagement loops              |
| Local-first               | Core editing works locally                           |
| Ownership                 | User owns project files                              |
| Open formats              | Standard exports and documented project format       |
| No unnecessary accounts   | Local use without registration                       |
| Progressive complexity    | Advanced tools available without overwhelming basics |
| Reversibility             | Undo and recoverable editing                         |
| Understandability         | Visible tool and project state                       |
| Privacy                   | No unnecessary tracking                              |
| Offline capability        | Core editing does not require internet               |
| Replaceability            | External tools can participate in workflows          |
| Longevity                 | Documentation and portable files                     |
| Interoperability          | CLI and asset pipeline integration                   |

---

# Project Success Criteria

Mirage should be evaluated using outcomes rather than engagement.

Important measures include:

* Time from launch to productive editing
* Editing responsiveness
* Reliability
* File compatibility
* Export correctness
* Undo reliability
* Ease of learning
* Precision of pixel manipulation
* Animation workflow quality
* Sprite workflow quality
* Retro asset workflow compatibility
* Cross-platform stability
* Offline reliability

The central question is:

> **Can the user make the thing they intended to make?**

---

# Intentional Computing Test

Mirage should continually be evaluated against these questions.

### Human Agency

Does the user remain in direct control of the artwork?

### Attention

Does the application demand attention that is unrelated to creation?

### Completion

Can the user finish their work and leave?

### Ownership

Does the user control the files and project data?

### Understandability

Can the user understand what the application is doing?

### Reversibility

Can mistakes be undone?

### Portability

Can the user's artwork survive without Mirage?

### Offline Operation

Can the core creative workflow function without the internet?

### AI

If AI is present, does it provide useful capability without taking creative control away?

### Longevity

Will today's artwork remain accessible in the future?

### Purpose

Does each feature contribute meaningfully to creative work?

---

# Anti-Patterns

The following should generally be avoided.

## Subscription Lock-In

Do not make basic pixel editing dependent on an ongoing payment.

## Cloud-Only Projects

Do not require cloud storage for ordinary artwork.

## Mandatory Accounts

Do not require registration for basic local use.

## Social Features

Do not turn the editor into a social network merely because other creative applications have social components.

## Infinite Inspiration Feeds

Do not build an endless art-consumption feed into the editor.

## Engagement Metrics

Do not introduce follower counts, likes, streaks, or similar mechanisms as part of the core application.

## AI Everywhere

Do not add AI features simply because AI is fashionable.

## Hidden State

Do not make selections, layers, tools, or transformations behave invisibly.

## Feature Accumulation

Do not add functionality merely to make the feature list longer.

## Proprietary Lock-In

Do not make the user's artwork unnecessarily dependent on Mirage's native format.

---

# Development Priorities

Development should generally prioritize:

1. Correct pixel rendering
2. Reliable editing
3. Canvas interaction
4. File operations
5. Undo/redo
6. Selection
7. Layers
8. Palette management
9. Animation
10. Sprite workflows
11. Export
12. Retro development workflows
13. Performance
14. Platform compatibility
15. Advanced capabilities

The application should become more capable without becoming proportionally more complicated.

---

# Current Technical Direction

The current foundation is:

```text id="p4k3xq"
Java
  ↓
JavaFX
  ↓
Maven
  ↓
Mirage
```

The initial project architecture should remain understandable and modular.

Potential high-level components include:

```text id="qv7x2m"
mirage/
├── application
├── canvas
├── tools
├── model
├── project
├── palette
├── animation
├── selection
├── io
├── export
├── ui
└── platform
```

The exact implementation may evolve.

The architectural goal is clear separation between:

* Artwork data
* Editing operations
* Rendering
* User interface
* File formats
* Platform-specific behavior

---

# Relationship to the Intentional Computing Repository

Mirage is one of the primary demonstration projects for Intentional Computing.

NoBSTube demonstrates intentional information consumption.

Mirage demonstrates intentional creation.

Together they illustrate two sides of the philosophy:

```text id="e1g5vu"
INFORMATION
     ↓
  NoBSTube
     ↓
UNDERSTANDING


CREATION
     ↓
   Mirage
     ↓
   RESULT
```

The larger ecosystem is not simply about reducing consumption.

It is about creating a healthier relationship between people and computing.

Technology should help people:

* Find information
* Understand information
* Make things
* Preserve things
* Organize things
* Build things

Then it should get out of the way.

---

# Relationship to the Retro Computing Projects

Mirage has a particularly strong relationship with the preservation projects in the Intentional Computing ecosystem.

The broader workflow may eventually become:

```text id="v6n4e2"
             Intentional Computing
                     │
          ┌──────────┴──────────┐
          ↓                     ↓
       Mirage              Emulators
          ↓                     ↓
    Asset Creation        Hardware Preservation
          │                     │
          └──────────┬──────────┘
                     ↓
              Personal Computing
```

Mirage provides the creative side.

The emulator projects provide the preservation and execution side.

Sprite and tile tooling connects the two.

---

# Future Direction

Potential future Mirage capabilities include:

### Core Editing

* Pencil
* Eraser
* Fill
* Shapes
* Lines
* Selection
* Transform
* Copy/paste
* Undo/redo

### Pixel Art

* Pixel-perfect drawing
* Palette management
* Color replacement
* Dithering tools
* Symmetry tools
* Pixel-art-specific transformations

### Layers

* Multiple layers
* Layer groups
* Visibility
* Locking
* Opacity
* Ordering

### Animation

* Timeline
* Frames
* Frame duplication
* Frame reordering
* Playback
* Frame timing
* Onion skinning

### Sprite Work

* Sprite sheets
* Tile grids
* Sprite extraction
* Sprite arrangement
* Batch export

### Retro Systems

* NES palette workflows
* SNES palette workflows
* Tile-size constraints
* Sprite constraints
* Indexed formats
* External ROM tooling integration

### File Support

* PNG
* GIF
* BMP
* Documented native format
* Additional formats where justified

### Automation

* Batch conversion
* Batch export
* Asset validation
* CLI integration

These features should be introduced according to user value rather than feature count.

---

# The Long-Term Vision

The long-term goal for Mirage is not to become the largest graphics application.

It is to become a **small, capable, dependable creative instrument**.

Something a person can install, understand, use for years, and trust with their work.

A person should be able to return to Mirage after months away and immediately understand:

* Where their artwork is
* How to edit it
* How to save it
* How to export it
* What the application is doing

That familiarity is valuable.

Software does not need to constantly reinvent itself to remain useful.

---

# Final Principle

Mirage exists to help a person make something.

The ideal workflow is:

```text id="k8q2ws"
I have an idea.
       ↓
I open Mirage.
       ↓
I create it.
       ↓
I refine it.
       ↓
I save it.
       ↓
I'm finished.
       ↓
I close Mirage.
       ↓
The artwork remains mine.
```

The application does not need to keep the user inside it.

It does not need to monetize their attention.

It does not need to become their social environment.

It does not need to become their identity.

It simply needs to be a good tool.

> **Make the software capable.**
>
> **Make the interface calm.**
>
> **Make the artwork belong to the user.**
>
> **Make the system understandable.**
>
> **Make creation direct.**
>
> **And when the work is finished, let the user walk away.**
