# Proof-of-work timeline

This file exists to make the CV auditable.

It uses two timestamp classes:

1. **Work/session timestamps** — timestamps preserved in conversation/work logs. These may be approximate when the original log says so.
2. **GitHub timestamps** — repository commit timestamps showing when specific artifacts entered version control.

GitHub timestamps are treated as the stronger source for repository state. Session timestamps are useful for showing the surrounding work process.

---

## 2024 — vulnerability tooling

### 15 Jan 2024 — CVE-MAKER false-positive repair

GitHub: `055d71935d03ffdb507e2c70b40c025d22c22867`  
Commit: **Fixing Github false positives**  
Timestamp: `2024-01-15T20:23:24Z`

https://github.com/bspippi1337/cve-maker/commit/055d71935d03ffdb507e2c70b40c025d22c22867

### 16 Jan 2024 — search parsing + exploit metadata

GitHub: `99b2ce118851cb9cc1df3f91de73ad9703c5f46e`  
Commit: **Adding Github Stars & Correcting Search Regex**  
Timestamp: `2024-01-16T20:55:57Z`

The diff changes CVE parsing logic and adds repository-star metadata to exploit results.

https://github.com/bspippi1337/cve-maker/commit/99b2ce118851cb9cc1df3f91de73ad9703c5f46e

---

## May 2026 — Restless

A dense sequence of commits on 11 May captures active implementation rather than a single bulk upload.

- `22:08:36 +02:00` — checkpoint
- `22:14:23 +02:00` — discover module work
- `22:20:55 +02:00` — replace legacy discover command
- `22:23:36 +02:00` — endpoint intelligence
- `22:24:57 +02:00` — relationship-graph deduplication
- `22:26:40 +02:00` — input validation
- `22:30:05 +02:00` — UI / graph cleanup
- `22:37:37 +02:00` — remove duplicate inspect command

Selected proof:

https://github.com/bspippi1337/restless/commit/1c5c737aaf8ce05deca306ad1c5ba7fe688a749d

The current repository describes Restless as a Go-based reactive API-discovery and Unix automation runtime with safe remote discovery, topology mapping, filesystem-triggered command execution and structural-drift inspection.

https://github.com/bspippi1337/restless

---

## 27–28 Jun 2026 — BLCKSWAN OS 42 Builder

GitHub records an iterative build/release sequence:

- `2026-06-27T23:37:59Z` — **add safe one-partition builder**
- `2026-06-27T23:46:15Z` — **failsafe one partition builder with direct image fallback**
- `2026-06-27T23:53:24Z` — **upload partition builds to releases instead of artifacts**
- `2026-06-28T00:22:01Z` — **allow release upload from workflow**
- `2026-06-28T02:52:48Z` — **fix release permissions permanently**

Selected proof:

https://github.com/bspippi1337/BLCKSWAN_OS42_BUILDER/commit/e01269d52eab3a0215b084c564940d042b794a84

https://github.com/bspippi1337/BLCKSWAN_OS42_BUILDER/commit/cc7ec6a858abff6886aeb898364ac565db26c3db

The repository contains separate GitHub Actions workflows plus shell builders for full images and individual partitions.

---

## 8 Jul 2026 — RED MOON ROMForge

GitHub sequence:

- `2026-07-08T21:43:47Z` — **fresh BLCKSWAN RED MOON ROM Forge**
- `2026-07-08T21:55:26Z` — **Rewrite README with new BLCKSWAN OS identity**
- `2026-07-08T22:02:29Z` — **add clean BLCKSWAN OS RED MOON build skeleton**

Proof:

https://github.com/bspippi1337/blckswan-redmoon-romforge/commit/25529ef0f09794f8b1ac4f04c19fdfe9e8e13af4

The documented pipeline builds an Android APK, downloads stock firmware, extracts `product.img` directly or from `payload.bin`, modifies the image, repacks it and emits a fastbootd-ready ZIP.

---

## 14 Aug 2026 — protocol / reverse-engineering documentation

Restless repository timestamps show a short evidence-focused sequence:

- `2026-08-14T01:47:28Z` — **Document MOROBOT/XBOT speed reverse engineering**
- `2026-08-14T01:47:37Z` — **Add concise MOROBOT/XBOT protocol reference**
- `2026-08-14T01:47:44Z` — **Record verified MOROBOT/XBOT 30 km/h result**
- `2026-08-14T01:47:50Z` — **Add index note for MOROBOT/XBOT reverse-engineering docs**

Proof:

https://github.com/bspippi1337/restless/commit/26bc36352cd25cb5de2fa5d23a2a0b8dad66a095

---

## 18–19 Aug 2026 — BLCKSWAN learning system

GitHub shows the product moving from web publication through GAMELOOP and into STORYMODE.

### 18 Aug

- `21:39–21:43Z` — landing page, web manifest, icon, documentation and GitHub Pages publication.

### 19 Aug

- `09:16–09:19Z` — GAMELOOP documentation, APK and source bundle.
- `09:39–09:42Z` — STORYMODE documentation, mechanics, install notes, Pages upgrade and v1.5 promotion.

Selected proof:

https://github.com/bspippi1337/blckswan/commit/32d766e047852435f9fdea144f51066824dfcf6c

https://github.com/bspippi1337/blckswan/commit/5674e53adbd7f7b0a7b8ed991398066f4828116f

Current public description: a local-first critical-thinking / active-learning system derived from a compressed conceptual model, with seven STORYMODE chapters, persistent state, multiple endings and signed Android builds.

---

## 24 Aug 2026 — AI workflow / safety evaluation

This is the clearest example where **session log timestamps and GitHub timestamps can be compared directly**.

### Session/work log

The preserved development log marks the beginning of the `aiguide` task at approximately:

- `2026-08-24 18:02:15 UTC` — user defines the standalone AI-assistance/logging task.
- `18:05:10 UTC` — request for a single monoblock that creates, commits and pushes the project.
- `18:07:05 UTC` — first explicit correction: the output broke the monoblock contract.
- `18:10:15–18:19:00 UTC` — README placement / quoting / base64 failure-and-recovery sequence.
- `18:21:20–18:25:40 UTC` — migration from private scratch repo into public `aiguide-dev` and successful execution.
- `18:29:15–18:49:00 UTC` — repeated artifact-format failures become a documented model-behavior case study.

The source log explicitly labels its overall start/end times as approximate. It is therefore evidence of sequence and working-session duration, not a precision clock.

Source:
https://github.com/bspippi1337/aiguide-dev/blob/main/notater.txt

### GitHub repository state

GitHub then records:

- `2026-08-24T19:11:29Z` — initial `aiguide-dev` commit
- `19:12:01Z` — project/readme update
- `19:14:33Z` — migration from scratch repo
- `19:31:41Z` — complete conversation artifact
- `19:47:12Z` — conversation log commit
- `20:00:01Z` — full chat log commit
- `20:00:40Z` — further uploaded files

Selected proof:

https://github.com/bspippi1337/aiguide-dev/commit/34bc755b416d9cef6e17c5533720288cf03a095e

https://github.com/bspippi1337/aiguide-dev/commit/e1ee41c74e57973f4bea1627acd45681b8cf70a6

### What this proves

The important artifact is not merely that a repository exists. The work log records the failure/recovery process; GitHub independently records the resulting artifacts and their sequence. Together they show an actual iterative technical session with observable outputs.

---

## 24 Aug 2026 — CV / reverse job ad

Work-session timestamp: approximately `22:25 +02:00`, when the request was made to turn the existing evidence into a public CV and reverse job advertisement.

Repository:

https://github.com/bspippi1337/cv

The CV deliberately links back to source repositories instead of relying on unverified skill claims.

---

## Verification principle

For this portfolio, evidence strength is ranked roughly as:

1. code/artifact + Git commit
2. build/release artifact + checksum
3. work/session log cross-referenced with commit
4. documentation tied to repository history
5. self-description without an artifact

The CV intentionally emphasizes levels 1–3.
