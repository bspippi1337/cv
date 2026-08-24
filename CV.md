# bspippi1337

**AI Security / Systems / Android / Applied R&D**  
Norway · Remote-friendly · Available for consulting, contract or employment  
GitHub: https://github.com/bspippi1337  
Email: bspippi1337@gmail.com  
Phone: +47 465 66 663

## Profile

Independent technical practitioner working across **AI safety evaluation, Unix/API tooling, Android firmware, security tooling, reverse engineering and rapid product prototyping**.

I was hired as a **Senior Systems Consultant at Umoe IKT at age 19**. I am 38 now. The useful part of that history is not the title itself, but the pattern behind it: I have been trusted with difficult systems unusually early, and I am still hungry for problems that reward technical depth, autonomy and unconventional investigation.

My strongest pattern is not a single framework or job title. It is taking an unfamiliar system, mapping what is actually happening, reducing assumptions, testing edge cases, and turning the result into something reproducible: code, a build pipeline, a technical artifact, an audit trail or a working prototype.

I prefer **evidence over claims**. The projects below are public and timestamped.

## Core capabilities

- AI / LLM adversarial evaluation and failure classification
- Prompt injection, jailbreak and multi-turn constraint testing
- Reproducible model-failure documentation and audit trails
- Go, Python and shell-native automation
- API discovery, topology mapping and structural drift inspection
- GitHub Actions, build/release automation and reproducible workflows
- Android ROM/GSI and system-image work
- Fastbootd, partition/image extraction, modification and repacking
- Android APK packaging and deployment workflows
- Linux / Termux / Unix-first development
- Vulnerability-tool maintenance and parsing/regex debugging
- Protocol investigation and practical reverse engineering
- Local-first product prototyping and interaction design

## Selected work

### Restless — reactive API discovery and Unix automation runtime
**May 2026 – present**

Go-based tool for understanding unfamiliar systems quickly through safe API discovery, topology mapping, filesystem-triggered automation and structural drift inspection.

Highlights:
- Safe remote discovery using GET / HEAD / OPTIONS only.
- Shell-friendly, terminal-native design with minimal runtime assumptions.
- Go CLI architecture using Cobra, Bubble Tea/Lip Gloss, fsnotify, OpenAPI and JSON-schema tooling.
- CI, release, installer and package-oriented workflows.
- Iterative endpoint-intelligence and graph-cleanup work is visible in timestamped commits from 11 May 2026.
- Repository also contains documented protocol/reverse-engineering work, including MOROBOT/XBOT investigation in August 2026.

Proof:
- https://github.com/bspippi1337/restless
- https://github.com/bspippi1337/restless/commit/1c5c737aaf8ce05deca306ad1c5ba7fe688a749d
- https://github.com/bspippi1337/restless/commit/26bc36352cd25cb5de2fa5d23a2a0b8dad66a095

### BLCKSWAN OS 42 Builder — Android firmware build automation
**June 2026 – present**

AOSP/FOSS-oriented Android firmware workflow producing fastbootd-ready BLCKSWAN OS 42 packages from stock firmware inputs.

Highlights:
- Automated image/partition build workflows through GitHub Actions.
- Separate full-build and one-partition build paths.
- Safe fallback logic for direct images.
- Release artifact handling and workflow permission fixes.
- Shell scripts for stock retrieval, image building and partition-specific processing.

Proof:
- https://github.com/bspippi1337/BLCKSWAN_OS42_BUILDER
- https://github.com/bspippi1337/BLCKSWAN_OS42_BUILDER/commit/e01269d52eab3a0215b084c564940d042b794a84
- https://github.com/bspippi1337/BLCKSWAN_OS42_BUILDER/commit/cc7ec6a858abff6886aeb898364ac565db26c3db

### BLCKSWAN OS 42 RED MOON ROMForge — fastbootd image pipeline
**July 2026 – present**

Pipeline that derives a flashable Android `product.img` from stock firmware and injects BLCKSWAN components and system properties.

Pipeline stages include:
1. build Android APK
2. download/reassemble stock firmware
3. extract image directly or from `payload.bin`
4. mount/unpack image
5. inject APK and properties
6. repack `product.img`
7. emit fastbootd-ready ZIP and flashing helper

Proof:
- https://github.com/bspippi1337/blckswan-redmoon-romforge
- https://github.com/bspippi1337/blckswan-redmoon-romforge/commit/25529ef0f09794f8b1ac4f04c19fdfe9e8e13af4

### BLCKSWAN — local-first critical-thinking / learning system
**July–August 2026**

Applied R&D project turning a large conceptual framework into an interactive learning product.

Highlights:
- Compressed an original 100-point model into a smaller operational framework centered on freedom, knowledge, test and revision.
- Built GAMELOOP and STORYMODE iterations around decision-making rather than passive content.
- STORYMODE campaign tracks Evidence, Trust, Pressure and Integrity across seven chapters.
- Multiple endings, surprise events, progression and “errors become INTEL” design.
- Local-first approach: no account, advertising, analytics or leaderboard dependency.
- Web deployment plus signed Android builds with upgrade continuity between versions.

Proof:
- https://github.com/bspippi1337/blckswan
- https://github.com/bspippi1337/blckswan/commit/9e6c037d11a5c08fbb44b02b61a287f1f73a9767
- https://github.com/bspippi1337/blckswan/commit/5674e53adbd7f7b0a7b8ed991398066f4828116f

### AI instruction-following / safety evaluation case study
**24 August 2026**

Built and documented a reproducible case study around AI workflow reliability and repeated instruction-following failures.

Failure classes identified and documented include:
- hard-constraint softening
- format-contract escape
- false completion claims
- artifact substitution
- correction decay across turns
- path/target drift
- verifier bypass through confident language

The repository intentionally preserves failures and corrections as an audit trail instead of rewriting history into a clean demo.

Proof:
- https://github.com/bspippi1337/aiguide-dev
- initial public repo commit: https://github.com/bspippi1337/aiguide-dev/commit/34bc755b416d9cef6e17c5533720288cf03a095e
- full-session log commit: https://github.com/bspippi1337/aiguide-dev/commit/e1ee41c74e57973f4bea1627acd45681b8cf70a6

### CVE-MAKER fork — vulnerability-tool maintenance
**2023–2024**

Maintenance/contribution work on a CVE and exploit-search tool originally created by `msd0pe`.

Selected changes include:
- reduced GitHub false positives
- corrected CVE search parsing / regex behavior
- added GitHub repository-star metadata to exploit results
- packaging/version maintenance and bug fixes

Proof:
- https://github.com/bspippi1337/cve-maker
- false-positive fix: https://github.com/bspippi1337/cve-maker/commit/055d71935d03ffdb507e2c70b40c025d22c22867
- regex / metadata work: https://github.com/bspippi1337/cve-maker/commit/99b2ce118851cb9cc1df3f91de73ad9703c5f46e

### Android security-oriented kernel/build experiments

Public projects also include build automation for Samsung XCover 4S / NetHunter-oriented kernel configurations, covering USB configfs, HID gadget support, UHID/HIDRAW, TUN and USB networking helpers.

Proof:
- https://github.com/bspippi1337/blckswan-xcover4s-nethunter-kernel

## How I work

- Map the system before changing it.
- Preserve known-good components during debugging.
- Treat explicit constraints as constraints, not stylistic suggestions.
- Prefer small reproducible experiments over speculative explanations.
- Automate repeatable work.
- Separate **intended**, **attempted**, **executed** and **verified** states.
- Do not call something finished without an observable artifact or verification signal.

## Languages

- Norwegian
- English

## Engagement

Available now for:
- consulting
- hourly contract work
- fixed-scope technical investigations
- red-team / evaluation projects
- R&D prototyping
- permanent roles where the work benefits from broad systems thinking

**Contact:**  
Email: bspippi1337@gmail.com  
Phone: +47 465 66 663  
GitHub: https://github.com/bspippi1337

See also: [proof-of-work timeline](PROOF_OF_WORK.md) and [reverse job ad](README.md).