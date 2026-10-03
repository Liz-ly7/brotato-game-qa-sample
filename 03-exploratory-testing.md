# Exploratory Testing

## Session Objective

Explore selected shop and gameplay state interactions in *Brotato* using unusual input sequences, repeated actions, and rapid interactions.

The goal was to identify unexpected behavior that may not be covered by straightforward functional checks.

## Areas Explored

- Shop item locking and unlocking
- Shop reroll behavior
- Multiple locked items
- Locked items across multiple rerolls
- Locked items across waves
- Rapid shop interactions
- Pause and resume behavior
- Pause behavior near wave transitions
- Settings access while gameplay is paused

## Exploratory Scenarios

| ID | Scenario | Observation | Result |
|---|---|---|---|
| EX-01 | Lock an item and perform multiple rerolls | Locked item remained available while other shop items refreshed normally | Pass |
| EX-02 | Lock multiple items at the same time | All selected items retained their lock state correctly | Pass |
| EX-03 | Keep an item locked, start the next wave, and return to the shop | Locked item remained available in the following shop phase | Pass |
| EX-04 | Lock an item, unlock it, then immediately reroll | Previously unlocked item was refreshed normally | Pass |
| EX-05 | Rapidly alternate between locking, unlocking, rerolling, and purchasing | Shop state remained consistent with no unexpected currency deduction or visible UI desynchronization | Pass |
| EX-06 | Rapidly pause and resume during active gameplay | Pause state remained stable and gameplay resumed normally | Pass |
| EX-07 | Pause and resume near the end of a wave | Wave completed normally and transitioned to the shop without unexpected behavior | Pass |
| EX-08 | Open Settings while paused, modify a setting, return, and resume gameplay | Settings applied correctly and gameplay resumed in the expected state | Pass |

## Observations

- No unexpected shop state behavior was observed.
- No visible UI desynchronization occurred during rapid shop interactions.
- Locked items behaved consistently across rerolls and wave transitions.
- Pause and resume behavior remained stable during repeated and transition-related testing.
- Settings accessed from the pause menu did not interfere with gameplay state.

## Session Result

No defects were identified during the exploratory testing session within the defined scope.

The session focused on combinations and interaction sequences that extended beyond basic normal-path testing while remaining within the project's limited test scope.
