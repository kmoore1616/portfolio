# Portfolio Website Plan

## Scope
- Exclude `rc/` entirely.
- Exclude incomplete/not-yours projects previously identified.
- Build a portfolio using your original work plus a separate mini section for school (`cs-*`) projects.

## Primary Sections
1. Hero
2. About
3. Featured Projects
4. Mini School Projects
5. Contact

## Featured Projects
1. 6502 Project (Featured)
- Sources: `6502/iv/wozmon.s`, `6502/wozmon_inject/wozinject.py`, `6502/wozmon_inject/woztype.py`, `6502/sim.sh`
- Framing: low-level monitor ROM workflow, assembly + tooling, emulator/simulation workflow.

2. Gunnison GPS Tour
- Sources: `Gunnison-GPS-Tour/app.py`, `Gunnison-GPS-Tour/README.md`
- Framing: Flask + SQLite tour platform with route/polyline integration and admin/user views.

3. STM8 Clock Firmware
- Sources: `clock/main.c`, `clock/Makefile`
- Framing: interrupt-driven embedded clock/alarm logic, GPIO/LCD integration, resource-constrained firmware design.

## Mini School Projects (Academic)
Use compact cards with an `Academic` badge.

1. VanBus AC Heartbeat (Academic Embedded Mini)
- Source: `VanBus/ac_detect/ac_detect.ino`
- Copy: ESP32 firmware that publishes AC power heartbeat telemetry over MQTT with reconnect and diagnostics.

2. RISC-V Single-Cycle CPU Simulator (CS-330 HW4)
- Source: `cs-330/hw4/single_cycle_simulator.c`
- Copy: C simulator for simplified RISC-V execution with fetch/decode/execute and register-state tracking.

3. RISC-V Pipeline Simulator (CS-330 HW5)
- Source: `cs-330/hw5/pipeline_simulator.c`
- Copy: 5-stage pipeline model with explicit stage-state structs and cycle-by-cycle behavior.

4. Set-Associative Cache Simulator (CS-330 HW8)
- Source: `cs-330/hw8/cache_sim.c`
- Copy: Configurable cache sim with LRU replacement, hit/miss stats, and latency estimation.

5. Custom Archive Utility `myTar` (CS-370 HW4)
- Source: `cs-370/hw4/turnin/myTar.c`
- Copy: POSIX C archiver/extractor implementing a custom `.mtar` format with metadata + payload handling.

6. Multi-Client TCP Server/Client (CS-370 HW15)
- Sources: `cs-370/hw15/server.c`, `cs-370/hw15/client.c`
- Copy: Threaded TCP server and client with signal-driven shutdown and request/response flow.

7. Flask Stock Portfolio Tracker (CS-250 Final)
- Source: `cs-250/final/app.py`
- Copy: Account-based Flask app using SQLAlchemy and login/session handling with market-data integration.

8. Image Upload + Gallery Service (CS-497 HW5)
- Source: `cs-497/HW5/app.py`
- Copy: Flask endpoint to ingest raw JPEG bytes, persist timestamped images, and render a gallery.

## Card Format
- Title
- 1-line summary
- Stack tags (e.g., `C`, `Python`, `Flask`, `SQLite`, `Embedded`)
- `View Source` link
- Badge when relevant (`Featured` or `Academic`)

## Build Plan
1. Content prep
- Finalize project descriptions.
- Gather 1 visual per featured project.
- Redact any secrets/credentials before publishing.

2. Site implementation
- Single-page responsive layout first.
- Sticky nav and section anchors.
- Featured cards (large), mini cards (compact grid).

3. QA and deploy
- Test desktop + mobile.
- Accessibility pass (contrast, semantic headings, keyboard nav).
- Deploy to GitHub Pages, Netlify, or Vercel.

## Notes
- `rc/` is intentionally excluded.
- School items are intentionally grouped under `Mini School Projects` for context.
