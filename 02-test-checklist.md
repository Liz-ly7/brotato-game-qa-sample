# Test Checklist

## Test Result Summary

- **Total Checks:** 18
- **Passed:** 18
- **Failed:** 0
- **Blocked:** 0
- **Defects Identified:** 0

## Smoke Testing

| ID | Test Area | Test Check | Expected Result | Result |
|---|---|---|---|---|
| SM-01 | Launch | Launch the game through Steam | Game launches successfully and reaches the main menu | Pass |
| SM-02 | Run Start | Start a new run | Gameplay starts normally without blocking issues | Pass |
| SM-03 | Gameplay Flow | Progress through multiple waves | Waves progress normally and transition to the shop as expected | Pass |
| SM-04 | Full Run Flow | Progress through Wave 20 and reach the boss encounter | Final boss encounter triggers normally and the core gameplay loop remains functional | Pass |

## Shop Testing

| ID | Test Area | Test Check | Expected Result | Result |
|---|---|---|---|---|
| SH-01 | Purchase | Purchase an item with sufficient currency | Item is purchased successfully and currency is deducted correctly | Pass |
| SH-02 | Insufficient Currency | Attempt to purchase an item without enough currency | Purchase does not complete and currency remains unchanged | Pass |
| SH-03 | Reroll | Reroll available shop items | Shop inventory refreshes and the reroll cost is applied correctly | Pass |
| SH-04 | Lock / Unlock | Lock and unlock an item | Item lock state changes correctly | Pass |
| SH-05 | Lock + Reroll | Lock an item and reroll the shop | Locked item remains while unlocked items are refreshed | Pass |
| SH-06 | Multiple Rerolls | Keep an item locked across multiple rerolls | Locked item remains available across repeated rerolls | Pass |
| SH-07 | Multiple Locked Items | Lock multiple shop items | Each locked item retains its lock state correctly | Pass |
| SH-08 | Lock Across Wave | Leave an item locked, start the next wave, and return to the shop | Locked item remains available in the next shop phase | Pass |
| SH-09 | Unlock + Reroll | Unlock a previously locked item and reroll | Unlocked item is no longer protected from reroll | Pass |
| SH-10 | Rapid Interaction | Perform shop actions rapidly, including rerolling, locking, unlocking, and purchasing | Shop state remains consistent with no unexpected currency loss or UI desynchronization | Pass |

## Pause / Resume Testing

| ID | Test Area | Test Check | Expected Result | Result |
|---|---|---|---|---|
| PR-01 | Pause | Pause during active gameplay | Gameplay, enemies, and wave progression stop while paused | Pass |
| PR-02 | Resume | Resume from the pause menu | Gameplay continues normally from the paused state | Pass |
| PR-03 | Rapid Pause Input | Rapidly pause and resume multiple times | Pause state remains stable and gameplay continues normally | Pass |
| PR-04 | Settings During Pause | Open Settings while paused, return, and resume gameplay | Game remains in the correct state and resumes normally | Pass |
| PR-05 | Wave Transition | Pause and resume near the end of a wave | Wave completes and transitions to the shop normally | Pass |

## Settings Testing

| ID | Test Area | Test Check | Expected Result | Result |
|---|---|---|---|---|
| ST-01 | Audio | Change an audio setting and return to gameplay | Audio output reflects the selected setting | Pass |
| ST-02 | Persistence | Change a setting and verify it after leaving or restarting the relevant game state | Selected setting remains applied as expected | Pass |
| ST-03 | Display | Change available display settings and return to the previous configuration | Display behavior remains stable with no visible UI or gameplay issues | Pass |
| ST-04 | Settings During Gameplay | Access and modify settings from the pause menu | Settings apply correctly and gameplay resumes normally | Pass |

## Notes

- No blocking issues were encountered during the tested gameplay flow.
- No unexpected behavior was observed within the defined test scope.
- No defects were identified during this testing session.
- Testing was limited to the areas defined in `01-test-plan.md`.
