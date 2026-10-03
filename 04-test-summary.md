# Test Summary

## Overview

This QA portfolio sample focused on functional and exploratory testing of selected systems in *Brotato*.

Testing covered the core gameplay flow, shop interactions, pause/resume behavior, and selected settings. The scope was intentionally limited to keep the project focused and reproducible.

## Test Environment

- **Game:** Brotato
- **Version:** 1.1.15.4
- **Platform:** PC / Steam
- **Operating System:** Windows 10
- **Input Method:** Keyboard + Mouse
- **Display Mode:** Windowed
- **Resolution:** Not displayed in game settings
- **Test Dates:** October 2–3, 2026

## Test Execution Summary

| Category | Checks Executed | Passed | Failed |
|---|---:|---:|---:|
| Smoke Testing | 4 | 4 | 0 |
| Shop Testing | 10 | 10 | 0 |
| Pause / Resume Testing | 5 | 5 | 0 |
| Settings Testing | 4 | 4 | 0 |
| **Total** | **23** | **23** | **0** |

Exploratory testing was also performed across selected shop interactions, pause/resume behavior, wave transitions, and settings access.

## Key Observations

- The game launched successfully and the core gameplay loop remained functional through Wave 20.
- Shop purchasing, rerolling, locking, unlocking, and related state transitions behaved as expected during testing.
- Locked items remained stable across rerolls and wave transitions.
- Rapid shop interactions did not produce visible UI desynchronization or unexpected currency behavior.
- Pause and resume behavior remained stable during normal use, rapid input, and near wave transitions.
- Settings changes behaved as expected during the tested scenarios.
- No blocking issues were encountered within the defined scope.

## Defects

No defects were identified during this testing session.

This result only reflects the selected features and scenarios included in the defined test scope and should not be interpreted as confirmation that the game is defect-free.

## Conclusion

All 23 planned checks passed within the selected test scope.

The project demonstrated the use of smoke testing, focused functional testing, and exploratory testing on a released PC game while maintaining a clearly defined and limited scope.
