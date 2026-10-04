# Rust NES Emulator

## Project Purpose

The Rust NES Emulator is a cycle-oriented software recreation of the Nintendo Entertainment System, implemented in Rust as part of the Intentional Computing computing-preservation effort.

Its purpose is not simply to run old games.

It is to understand, preserve, and reproduce an important piece of personal computing history using modern tools while retaining as much of the original machine's behavior and constraints as practical.

The project demonstrates a central idea of Intentional Computing:

> **Modern computing should make us more capable without requiring us to forget how the machines that came before us worked.**

An emulator allows a historical computer system to become understandable software.

---

# Why the NES Matters

The NES represents an important period in the development of personal and consumer computing.

It was:

* Hardware constrained
* Local
* Self-contained
* Deterministic
* Understandable at the machine level
* Designed around clear hardware responsibilities
* Capable of producing sophisticated results from very limited resources

The system's limitations were not merely obstacles.

They shaped the software, graphics, sound, programming techniques, and games created for it.

Preserving the system therefore means preserving more than the ability to launch its software.

It means preserving an understanding of how the machine worked.

---

# Why Build an Emulator?

An emulator is a particularly valuable preservation tool because it represents the machine as a model.

Instead of merely documenting the NES, the emulator attempts to reproduce its behavior.

Conceptually:

```text id="xq2v8n"
ORIGINAL HARDWARE
       ↓
UNDERSTAND HARDWARE
       ↓
MODEL HARDWARE
       ↓
IMPLEMENT MODEL
       ↓
TEST BEHAVIOR
       ↓
PRESERVE SYSTEM
```

The result is both a working machine and an executable technical explanation.

---

# Project Philosophy

The Rust NES Emulator applies several Intentional Computing principles.

### Preservation Is Progress

Old computing systems contain useful knowledge.

Preserving them expands our understanding rather than merely preserving nostalgia.

### Understandability Matters

The emulator should make the architecture understandable.

### Local Ownership

The emulator should run locally.

### Offline Capability

Once the software and legally obtained ROMs are available, the emulator should not require an internet connection to operate.

### Open and Inspectable Architecture

The implementation should be readable and modular.

### Minimal External Dependency

The emulator should avoid unnecessary external services.

### Deterministic Computing

The emulator should strive toward predictable, reproducible behavior.

### Capability Without Complexity

The implementation may be sophisticated internally while remaining understandable as a collection of hardware components.

---

# What the Project Is

The Rust NES Emulator is:

* An NES hardware emulator
* A preservation project
* A Rust systems-programming project
* A CPU emulation project
* A PPU emulation project
* An APU emulation project
* A cartridge and mapper project
* A memory-system project
* A debugging and testing environment
* A foundation for studying older hardware

It is also a practical example of implementing a complete computing system from documented behavior.

---

# What the Project Is Not

The project is not intended to become:

* A commercial game distribution service
* A ROM distribution platform
* A cloud gaming service
* An online social platform
* An account-based ecosystem
* A streaming service
* A platform that requires internet connectivity
* A black-box game compatibility layer with no understandable architecture

The emulator should remain a software representation of the machine.

---

# The NES as a Computer

The emulator should treat the NES as a collection of interacting hardware systems rather than as a single abstraction called "the game."

A simplified architecture is:

```text id="q5n7ab"
                    NES
                     │
       ┌─────────────┼─────────────┐
       ↓             ↓             ↓
      CPU            PPU           APU
       │             │             │
       └──────┬──────┴──────┬──────┘
              ↓             ↓
          Memory / Bus    Audio Output
              │
              ↓
          Cartridge
              │
              ↓
            Mapper
```

The emulator should preserve these conceptual boundaries.

---

# CPU Emulation

The CPU is one of the central components of the NES.

The emulator should model the relevant 6502-derived CPU behavior, including:

* Registers
* Status flags
* Program counter
* Stack
* Addressing modes
* Instruction execution
* Memory access
* Interrupt behavior
* Reset behavior
* Timing

The CPU implementation should prioritize correctness and understandability.

---

# CPU Architecture

The CPU should remain a distinct component rather than being tightly coupled to game-specific behavior.

Conceptually:

```text id="x8a6pk"
CPU
├── Registers
├── Flags
├── Program Counter
├── Stack Pointer
├── Decoder
├── Addressing Modes
├── Instruction Execution
└── Interrupt Handling
```

This separation makes the emulator easier to test and reason about.

---

# Memory Bus

The memory bus is the communication layer between the CPU and the rest of the machine.

It should model the NES memory map and route accesses appropriately.

Conceptually:

```text id="8i1w7c"
CPU
 │
 ↓
BUS
 ├── RAM
 ├── PPU Registers
 ├── APU / I/O
 ├── Cartridge
 └── Mapper
```

Keeping this relationship explicit is important.

The bus is not merely a convenience abstraction.

It represents a real architectural relationship in the original hardware.

---

# PPU Emulation

The Picture Processing Unit is one of the defining characteristics of the NES.

The emulator should model the PPU rather than simply rendering the final image through a high-level game abstraction.

Important areas include:

* Pattern tables
* Name tables
* Attribute tables
* Palettes
* Background rendering
* Sprite rendering
* Sprite evaluation
* Scrolling
* VBlank
* PPU registers
* Timing

The goal is to reproduce the behavior that NES software expects from the hardware.

---

# PPU Timing

Timing is particularly important.

The PPU does not simply produce a completed frame whenever the CPU asks for one.

Its behavior is tied to the machine's timing.

The emulator should therefore work toward an accurate relationship between:

```text id="2d6c6a"
CPU CYCLES
     ↓
PPU CYCLES
     ↓
SCANLINES
     ↓
PIXELS
     ↓
FRAME
```

Timing accuracy should be improved incrementally through tests and known behavior rather than by prematurely attempting to reproduce every undocumented hardware detail.

---

# APU Emulation

Audio is another important component of the NES.

The emulator should eventually provide a structured model of the Audio Processing Unit.

Relevant components include:

* Pulse channels
* Triangle channel
* Noise channel
* DMC
* Frame counter
* Envelope behavior
* Sweep behavior
* Length counters

Audio output should remain separated from the CPU and PPU architecture.

---

# Cartridge System

Cartridges are an important part of the NES architecture.

The emulator should treat the cartridge as a hardware component rather than simply as a file containing program data.

Conceptually:

```text id="4e1r0n"
ROM FILE
   ↓
CARTRIDGE
   ↓
MAPPER
   ↓
CPU / PPU MEMORY
```

This allows the emulator architecture to reflect the actual system.

---

# Mapper Architecture

The emulator should support cartridge mappers through a modular architecture.

The first and simplest target is:

> **Mapper 0 / NROM**

This provides a useful baseline because it represents a relatively straightforward cartridge configuration.

The architecture should allow additional mappers to be added later without redesigning the entire emulator.

Potential future mapper support may include:

* Mapper 0
* Mapper 1
* Mapper 2
* Mapper 3
* Other commonly encountered mappers

Mapper support should be implemented as hardware behavior rather than as game-specific exceptions.

---

# ROM Loading

The emulator should validate ROM files before execution.

The loader should inspect information such as:

* File format
* Mapper number
* PRG size
* CHR size
* Mirroring
* Trainer presence where relevant
* Battery-backed data where relevant

The emulator should fail clearly when a ROM cannot be supported.

It should not silently produce undefined behavior.

---

# Timing Model

Timing should be treated as a first-class architectural concern.

The emulator should avoid relying entirely on:

```text
one instruction = one arbitrary application update
```

Instead, it should work toward a relationship between the emulated components that reflects the original hardware.

The eventual conceptual model is:

```text id="t6j4sp"
MASTER CLOCK
     │
     ├── CPU
     │
     ├── PPU
     │
     └── APU
```

The exact implementation can evolve.

The important principle is that timing belongs to the machine model.

---

# Rendering

Rendering should preserve the characteristics of the original hardware.

The emulator should not treat NES graphics as arbitrary modern 2D graphics.

Instead, it should model:

* Tiles
* Nametables
* Attribute tables
* Palettes
* Sprites
* Scanlines
* PPU behavior

The final display is the result of the emulated hardware.

---

# Input

Controller input should be modeled as hardware interaction.

The emulator should provide a clear boundary between:

```text id="k0k4p8"
HOST INPUT
     ↓
CONTROLLER
     ↓
NES I/O
     ↓
GAME
```

This allows the emulator core to remain independent of the host platform.

---

# Host Platform

The host platform should provide only what is necessary to operate the emulator.

Conceptually:

```text id="n7q2cv"
        EMULATOR CORE
              │
       ┌──────┼──────┐
       ↓      ↓      ↓
   Display  Audio  Input
       │      │      │
       └──────┼──────┘
              ↓
        HOST PLATFORM
```

This separation makes the emulator easier to port and test.

---

# Rust

Rust is an appropriate language for this project because it provides:

* Strong type safety
* Memory safety
* Explicit ownership
* High performance
* Good systems-programming capabilities
* Cross-platform potential
* A useful balance between low-level control and modern tooling

The language itself also reinforces an important project goal:

> Modern tools can be used to preserve older computing systems without reproducing their historical development limitations.

---

# Understandable Architecture

The emulator should favor explicit hardware components over excessive abstraction.

A developer should be able to look at the project and understand:

```text
CPU
 ↓
BUS
 ↓
PPU / APU / CARTRIDGE
 ↓
MAPPER
 ↓
OUTPUT
```

Abstraction is valuable when it clarifies a real concept.

It is harmful when it hides the machine.

---

# Testing

Testing is one of the most important parts of emulator development.

The emulator should use multiple forms of testing.

## Unit Tests

Individual components should be tested independently.

Examples:

* CPU instructions
* Addressing modes
* Flags
* Memory behavior
* Mapper behavior
* PPU registers

## Integration Tests

Components should be tested together.

Examples:

* CPU ↔ Bus
* CPU ↔ Cartridge
* CPU ↔ PPU
* PPU ↔ Cartridge
* Controller ↔ CPU

## ROM Tests

Known diagnostic ROMs should be used where available and legally distributable.

## Regression Tests

Once a bug is fixed, the behavior should be captured in a regression test where practical.

---

# Debugging

The emulator should provide useful debugging facilities.

Potential tools include:

* CPU trace logging
* Memory inspection
* PPU state inspection
* Mapper state inspection
* Register inspection
* Breakpoints
* Frame stepping
* Instruction stepping
* Debug overlays

Debugging should help explain why the emulated machine behaves incorrectly.

It should not simply say that a game failed.

---

# Determinism

Given the same:

* Emulator version
* ROM
* Configuration
* Input sequence

the emulator should strive to produce the same behavior.

Determinism is valuable for:

* Debugging
* Testing
* Regression analysis
* Preservation
* Reproducibility

This is particularly important when diagnosing subtle emulator bugs.

---

# Compatibility

Compatibility should be approached incrementally.

The project should not define success as:

> "Every NES game works."

Instead, compatibility should improve through layers.

```text id="x2r5qa"
CPU Correctness
      ↓
Memory Correctness
      ↓
Mapper Correctness
      ↓
PPU Correctness
      ↓
APU Correctness
      ↓
Timing Accuracy
      ↓
Game Compatibility
```

A game failing is useful information.

It can identify which part of the machine model requires improvement.

---

# Legal and Preservation Boundaries

The emulator itself should remain separate from copyrighted game distribution.

The project can provide:

* Emulator source code
* Documentation
* Tests
* Hardware information
* Development tools
* Homebrew software where appropriate
* Public-domain or freely distributable test material

Users are responsible for obtaining ROMs they are legally entitled to use.

The preservation goal does not require redistributing copyrighted game data.

---

# Offline Operation

The emulator should be fully usable offline.

Once the emulator and legally obtained ROMs are available:

```text id="m2y8f4"
NO INTERNET
     ↓
LAUNCH EMULATOR
     ↓
LOAD LOCAL ROM
     ↓
PLAY
```

No online account should be required.

No remote service should be necessary for ordinary operation.

This is an important part of preserving the original relationship between person, machine, and software.

---

# Local Ownership

The emulator should treat local files as the primary source of truth.

The user should control:

* Emulator configuration
* Save data
* ROM files
* Screenshots
* Debug information
* Emulator state
* Build artifacts

The project should not require a cloud account to preserve this information.

---

# Save Data

Where supported, save data should remain local.

The user should be able to:

* Back it up
* Copy it
* Restore it
* Archive it
* Move it to another installation

Save data should not become dependent on a remote account.

---

# Configuration

Configuration should be explicit and understandable.

Potential settings include:

* Video scaling
* Audio settings
* Controller configuration
* Input mappings
* Region-related behavior where relevant
* Debugging options
* Emulator speed
* Save paths

Configuration files should be readable where practical.

---

# Interface

The user interface should remain secondary to the emulation.

The important actions should be obvious:

```text id="e4d7q1"
LOAD ROM
   ↓
PLAY
   ↓
PAUSE / RESET / EXIT
```

Advanced debugging functionality can exist without overwhelming ordinary use.

The emulator should not turn gameplay into a complicated desktop environment.

---

# Preservation Interface

The emulator should ideally provide an easy way to inspect the machine.

This creates an opportunity beyond simply playing games.

A future developer could launch a ROM and inspect:

* CPU state
* PPU state
* Memory
* Cartridge mapping
* Frame timing
* Input
* Audio state

This turns the emulator into an educational tool as well as a compatibility tool.

---

# Homebrew Development

The emulator should also provide a useful environment for NES homebrew development.

A developer should eventually be able to use:

```text id="2w8j6k"
ca65 / cc65
     ↓
NES ROM
     ↓
Rust NES Emulator
     ↓
Development / Debugging
```

This creates a modern development environment for an old computing platform.

The emulator therefore becomes part of a broader preservation ecosystem rather than merely a game player.

---

# Relationship to Mirage

The NES emulator and Mirage complement each other.

Mirage provides creative asset creation.

The emulator provides execution and preservation.

Together:

```text id="r7m2qz"
Mirage
  ↓
NES Artwork
  ↓
Asset / ROM Tooling
  ↓
NES ROM
  ↓
Rust NES Emulator
  ↓
Playable Result
```

This allows modern development tools to participate in an old hardware environment.

---

# Relationship to Sprite and Tile Tooling

Dedicated sprite and tile tooling provides another bridge between modern editing and historical hardware.

The broader workflow can become:

```text id="a5x3vc"
NES ROM
   ↓
Extract
   ↓
Sprite / Tile Mapper
   ↓
Mirage
   ↓
Edit Artwork
   ↓
Bake / Rebuild
   ↓
NES ROM
   ↓
Emulator
```

Each project remains focused on a specific task.

---

# Relationship to the SNES Emulator

The NES emulator is also an architectural reference for the future Rust SNES Emulator.

The two systems are different, but they share important concepts:

* CPU emulation
* Memory buses
* Graphics processors
* Audio processors
* Input
* Cartridges
* Timing
* Debugging
* ROM loading
* Host abstraction

The NES project therefore establishes engineering patterns that can inform later preservation projects.

---

# Relationship to the Atari 2600 Emulator

The NES project also participates in the broader computing-preservation effort alongside the Atari 2600 emulator.

The systems demonstrate different approaches to early game hardware.

Studying them together helps reveal:

* Different CPU architectures
* Different graphics models
* Different memory constraints
* Different cartridge designs
* Different approaches to timing
* Different approaches to sound
* Different programming techniques

The goal is not simply to emulate individual consoles.

It is to understand the evolution of computing hardware.

---

# Intentional Computing Principles Demonstrated

| Principle                 | Rust NES Emulator Implementation                    |
| ------------------------- | --------------------------------------------------- |
| Preservation is progress  | Recreates historical hardware                       |
| Local-first               | Runs entirely on local hardware                     |
| Offline capability        | No network required for operation                   |
| Ownership                 | Local ROMs and save data                            |
| Understandability         | Hardware-oriented architecture                      |
| Open architecture         | Emulator components are inspectable                 |
| Modularity                | CPU, PPU, APU, bus, mapper separation               |
| Replaceability            | Host interfaces can be separated from core          |
| Determinism               | Reproducible emulation behavior                     |
| Documentation             | Hardware behavior becomes executable knowledge      |
| Longevity                 | Modern implementation preserves historical behavior |
| Creation                  | Supports homebrew development                       |
| Interoperability          | Works with external development tools               |
| No unnecessary accounts   | Local operation                                     |
| No attention optimization | No engagement mechanics                             |

---

# Project Success Criteria

The emulator should not primarily be evaluated by the number of games it can launch.

More meaningful measures include:

* CPU correctness
* PPU correctness
* APU correctness
* Mapper correctness
* Timing accuracy
* Diagnostic test results
* Compatibility
* Stability
* Debuggability
* Architectural clarity
* Reproducibility
* Cross-platform operation
* Documentation quality

Compatibility is important, but it is the consequence of correctly modeling the hardware.

---

# Intentional Computing Test

The Rust NES Emulator should continually be evaluated against the following questions.

### Preservation

Does the project preserve meaningful knowledge about the original system?

### Understandability

Can another developer understand how the machine is represented?

### Ownership

Can the user operate the emulator using local files without unnecessary external dependencies?

### Offline Capability

Can the emulator function without internet access?

### Reproducibility

Can behavior be reproduced and debugged?

### Longevity

Could the project remain useful years from now?

### Interoperability

Can it work with other tools rather than requiring a closed ecosystem?

### Education

Does the implementation help people understand the original hardware?

### Simplicity

Is complexity introduced because the hardware requires it, rather than because the software architecture is unnecessarily complicated?

### Purpose

Does the project preserve and reproduce the machine rather than merely imitate its visible output?

---

# Anti-Patterns

The following should generally be avoided.

## Black-Box Emulation

Do not hide the machine behind an opaque compatibility layer.

## Game-Specific Hacks

Avoid implementing behavior solely because one particular game needs it when the correct solution is to model the underlying hardware.

Game-specific compatibility work may occasionally be necessary, but it should be clearly identified.

## Unnecessary Online Dependencies

The emulator should not require remote services for ordinary operation.

## ROM Distribution

The emulator should not become a mechanism for distributing copyrighted ROM collections.

## Excessive Abstraction

Do not abstract away hardware concepts that developers need to understand.

## Premature Accuracy

Do not attempt to model every obscure hardware edge case before establishing a correct, testable foundation.

## Feature Accumulation

Do not add features unrelated to emulation simply because they are technically possible.

## Platform Lock-In

Do not make the emulator dependent on a single host operating system when the architecture can reasonably remain portable.

---

# Development Priorities

Development should generally proceed in layers:

1. ROM loading
2. Cartridge representation
3. Mapper architecture
4. Memory bus
5. CPU core
6. CPU testing
7. PPU foundation
8. PPU rendering
9. PPU timing
10. Controller input
11. APU foundation
12. Audio output
13. Timing refinement
14. Diagnostic testing
15. Compatibility testing
16. Debugging tools
17. Performance optimization
18. Additional mapper support
19. Advanced hardware behavior

Correctness should generally take priority over premature optimization.

---

# Current Architectural Direction

The emulator should maintain a clear separation between the emulated machine and the host application.

A conceptual architecture is:

```text id="u8r2fd"
                    Emulator
                       │
        ┌──────────────┼──────────────┐
        ↓              ↓              ↓
       CPU            PPU            APU
        │              │              │
        └──────────────┼──────────────┘
                       ↓
                      BUS
                       │
                 ┌─────┴─────┐
                 ↓           ↓
            Cartridge      I/O
                 │
                 ↓
               Mapper
                       │
                       ↓
                Emulator Core
                       │
              ┌────────┼────────┐
              ↓        ↓        ↓
           Display    Audio    Input
```

The exact implementation may evolve.

The boundaries should remain conceptually clear.

---

# Long-Term Preservation

The ultimate value of an emulator is not limited to whether it runs games today.

A well-designed emulator can become a historical artifact itself.

Future developers may use it to understand:

* How the NES worked
* How early game software interacted with hardware
* How memory constraints shaped software
* How graphics were produced
* How sound was generated
* How cartridges extended hardware
* How programmers worked within severe limitations

The emulator should therefore preserve knowledge as well as behavior.

---

# The 10-Year Test

A useful question for the project is:

> If this repository were opened ten years from now, could someone understand what the emulator is doing?

That means:

* Clear source code
* Clear architecture
* Useful documentation
* Stable file formats
* Tests
* Build instructions
* Hardware explanations
* Minimal unnecessary dependencies
* Reproducible behavior

Longevity is part of correctness.

---

# The 90s Principle

The NES itself comes from an era when computing systems were comparatively bounded.

A game cartridge contained a finite program.

A console had a finite set of capabilities.

A person could turn the system on, play a game, turn it off, and be finished.

There was no requirement to:

* Maintain an online identity
* Check notifications
* Watch recommendations
* Accept behavioral tracking
* Remain connected
* Maintain a subscription

The emulator does not attempt to recreate every limitation of that era.

Instead, it preserves the useful characteristic of **bounded computing**.

---

# The Modern Principle

The emulator should use modern technology where it provides genuine benefit.

Rust provides:

* Memory safety
* Modern tooling
* Strong testing infrastructure
* Cross-platform capabilities
* Maintainability

Modern displays, audio devices, controllers, and computers provide capabilities that the original hardware could not.

That is acceptable.

The goal is not historical reenactment.

The goal is:

> **Preserve the machine while using modern tools to make preservation more reliable.**

---

# Why Rust Matters to Intentional Computing

The language choice also reflects a broader principle.

Modern software does not have to choose between:

```text
OLD COMPUTING
```

and:

```text
MODERN COMPLEXITY
```

It is possible to use modern engineering techniques while preserving the clarity and boundaries of older systems.

Rust provides a useful example of this.

The result can be:

```text id="k7f5wn"
OLD HARDWARE
     +
MODERN LANGUAGE
     +
MODERN TESTING
     +
MODERN TOOLING
     ↓
UNDERSTANDABLE PRESERVATION
```

---

# Future Direction

Potential future capabilities include:

* More accurate CPU behavior
* More accurate PPU behavior
* More accurate APU behavior
* Additional mapper support
* Better timing accuracy
* Save-state support
* Debugger
* Memory viewer
* CPU trace viewer
* PPU inspection tools
* Tile viewer
* Palette viewer
* Nametable viewer
* Controller configuration
* Improved audio
* Cross-platform packaging
* Automated compatibility testing
* Homebrew development support
* Hardware diagnostics
* Documentation of emulation decisions

These features should support the central purpose of the project.

---

# The Emulator as a Learning Tool

The project should ideally be useful even to someone who is not primarily interested in playing NES games.

A developer should be able to study it and learn:

* How a CPU executes instructions
* How memory buses work
* How graphics processors operate
* How timing affects hardware
* How interrupts work
* How cartridges map memory
* How constrained hardware can produce complex results

This makes the emulator a form of executable technical documentation.

---

# The Emulator as a Personal Computer

The NES is a specialized computer.

The emulator allows that computer to exist inside a modern personal computer as a local software environment.

The relationship becomes:

```text id="b1y5tp"
MODERN COMPUTER
       ↓
RUST
       ↓
NES EMULATOR
       ↓
NES HARDWARE MODEL
       ↓
NES SOFTWARE
```

The modern machine becomes a preservation environment rather than merely a consumption platform.

---

# Final Principle

The Rust NES Emulator exists to preserve a machine by understanding it.

It should not merely make games appear on a modern screen.

It should model the relationships that made the original system work.

The ideal project therefore looks like:

```text id="e2w8sr"
UNDERSTAND THE HARDWARE
        ↓
MODEL THE HARDWARE
        ↓
IMPLEMENT THE MODEL
        ↓
TEST THE BEHAVIOR
        ↓
RUN THE SOFTWARE
        ↓
PRESERVE THE KNOWLEDGE
```

The emulator should remain:

**Local.**

**Understandable.**

**Testable.**

**Reproducible.**

**Portable.**

**Owned by the user.**

And most importantly:

> **Preservation should make the past understandable rather than merely making it playable.**
