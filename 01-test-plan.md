# Test Plan

## 1. Objective

The objective of this project is to perform focused functional and exploratory testing on selected systems in *Brotato*.

The testing focuses on the core gameplay flow, shop interactions, pause/resume behavior, and selected settings. The goal is to verify that these features behave as expected under normal use and selected edge-case interactions.

## 2. Test Environment

- **Game:** Brotato
- **Version:** 1.1.15.4
- **Platform:** PC / Steam
- **Operating System:** Windows 10
- **Input Method:** Keyboard + Mouse
- **Display Mode:** Windowed
- **Resolution:** Not displayed in game settings
- **Test Dates:** October 2–3, 2026

## 3. In Scope

The following areas are included in this testing sample:

- Game launch and basic run initialization
- Core gameplay progression through waves
- Shop interactions
  - Purchasing items
  - Rerolling items
  - Locking and unlocking items
  - Multiple locked items
  - Locked items across rerolls and waves
  - Purchase attempts with insufficient currency
  - Rapid shop interactions
- Pause and resume behavior
- Pause-related gameplay state transitions
- Selected settings behavior
  - Audio changes
  - Setting persistence
  - Display mode behavior
  - Accessing and changing settings while paused

## 4. Out of Scope

The following areas are intentionally excluded to keep the testing focused:

- Testing all characters
- Testing all weapons and items
- Balance testing
- Damage calculation validation
- All difficulty levels
- Achievement testing
- Long-duration performance testing
- Full progression testing
- Comprehensive compatibility testing
- Controller input testing

## 5. Test Approach

The testing uses a combination of:

- **Smoke Testing** — to verify that the game launches successfully and the main gameplay loop is functional.
- **Functional Testing** — to verify expected behavior of selected shop, pause/resume, and settings features.
- **Exploratory Testing** — to investigate feature behavior using unusual input sequences, rapid interactions, and state transitions.

Testing was intentionally limited to a small, defined scope in order to produce a focused and reproducible QA portfolio sample.
