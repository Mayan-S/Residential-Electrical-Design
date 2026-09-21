# CEC Load Calculation

**Standard:** CSA C22.1:24 (CEC), Rule 8-200, single dwelling
**Supply:** 120/240 V, single-phase

## Inputs

- Floor area (incl. walls): 59.66 m² (measured in AutoCAD, 59,660,000 mm²)
- Interior area (excl. walls): 47.09 m² (reference)
- One electric range, rated 12 kW or less
- Base case: gas heat and gas water heater
- Both areas are under 90 m², so the basic load is 5,000 W

## Case A: gas heat

| Load | Basis | Value |
|------|-------|------:|
| Basic load, first 90 m² | 8-200(1)(a)(i) | 5,000 W |
| Electric range | 8-200(1)(a)(iv) | 6,000 W |
| **Total** | | **11,000 W** |

Current = 11,000 / 240 = **45.8 A**

## Case B: electric heat (10 kW, 3+ zones)

Electric space heating added per Rule 8-200(1)(a)(iii) (Section 62): first 10 kW at 100%, balance at 75% with 3+ zones.

| Load | Basis | Value |
|------|-------|------:|
| Basic load, first 90 m² | 8-200(1)(a)(i) | 5,000 W |
| Electric space heating | 8-200(1)(a)(iii), Section 62 | 10,000 W |
| Electric range | 8-200(1)(a)(iv) | 6,000 W |
| **Total** | | **21,000 W** |

Current = 21,000 / 240 = **87.5 A**

## Result

| Case | Load | Current | Service |
|------|-----:|--------:|:-------:|
| A, gas heat | 11,000 W | 45.8 A | 100 A |
| B, electric heat | 21,000 W | 87.5 A | 100 A |

**Recommended service: 100 A, 120/240 V.**
Case A uses under half of it. Case B uses most of it. Adding an electric water heater or EV charger would push toward 125 A or 200 A.

## Notes
- Assumed appliance ratings, not nameplate data.
- Per 8-200(1)(b): 100 A minimum where living area (excl. basement) is 80 m² or more, 60 A minimum where under 80 m². This house is 59.66 m², so 60 A is the code minimum; 100 A is chosen for headroom and standard practice.
