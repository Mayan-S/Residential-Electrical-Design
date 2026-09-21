# CEC Voltage-Drop Check

**Standard:** CSA C22.1:24 (CEC), Rule 8-102

**Supply:** 120 V branch circuit

## Worst-case run

Only the single longest branch run is checked: if it passes, every shorter run passes automatically.

The longest run is the outdoor receptacle near the entry (circuit 7). Distance measured in AutoCAD by following the wall route the cable would actually take (down the right wall, along the south wall, through the door, out to the receptacle): **10.45 m** (10,450 mm).

## Inputs

- Routed one-way length: 10.45 m (measured along walls, not straight-line)
- Conductor: 14 AWG copper, resistance about 8.3 ohms/km (at 20 C)
- Current: 12 A (80% of the 15 A breaker, worst case)
- Voltage: 120 V

## Calculation

Formula (single-phase): Vd = (2 x L x I x R) / 1000
(the x2 accounts for current flowing out and back through two conductors)

Vd = (2 x 10.45 x 12 x 8.3) / 1000 = 2.08 V

As a percentage: 2.08 / 120 = 1.7%

## Result

| Length | Voltage drop | % of 120 V | Limit | Pass? |
|--------|-------------:|-----------:|------:|:-----:|
| 10.45 m routed | 2.08 V | 1.7% | 3% | Yes |

**Passes.** Even at full 12 A load and using the real wall-following cable length, the drop is 1.7%, under the 3% branch limit. Voltage drop is not a concern for this house: the runs are short and 14 AWG is adequate.

## Notes

- Rule 8-102 limits voltage drop to 3% in a branch or feeder, and 5% total from the service to the point of use. This branch is checked against the 3% limit.
- Current is an estimate (worst-case 80% of breaker); a real design uses appliance nameplate data.
