# CEC Branch Circuits & Panel Schedule

**Panel:** 100 A, 120/240 V, single-phase

**House:** as per load calc (59.66 m², 2 bed/living, kitchen, bath, WC)

## Circuit schedule

| Ckt | Serves | Breaker | Conductor | Protection | Leg | Load (W) | Load (A) |
|----:|--------|---------|-----------|-----------|:---:|--------:|--------:|
| 1 | Bedroom + Living lighting, ceiling fans & smoke/CO detectors | 15 A, 1-pole | 14/2 AWG | AFCI | A | 615 | 5.1 |
| 2 | Bedroom + Living receptacles | 15 A, 1-pole | 14/2 AWG | AFCI | B | 1,000 | 8.3 |
| 3 | Kitchen / Bath / WC lighting & exhaust | 15 A, 1-pole | 14/2 AWG | AFCI | A | 450 | 3.8 |
| 4 | Kitchen counter receptacles (split) | 15 A, 2-pole | 14/3 AWG | GFCI | A+B | 2,880 | 12.0 |
| 5 | Refrigerator (dedicated) | 15 A, 1-pole | 14/2 AWG | - | B | 700 | 5.8 |
| 6 | Bathroom receptacle (dedicated) | 15 A, 1-pole | 14/2 AWG | GFCI | A | 1,440 | 12.0 |
| 7 | Outdoor receptacles (front/rear entry) | 15 A, 1-pole | 14/2 AWG | GFCI, weatherproof | B | 600 | 5.0 |
| 8 | Electric range | 40 A, 2-pole | 8/3 AWG | - | A+B | 6,000 | 25.0 |
| 9-10 | Spare | - | - | - | - | - | - |

Load values are estimates for sizing (a real design uses appliance nameplate ratings). For the 2-pole circuits (4 and 8), Load (A) is the current in each hot leg. All circuits are within the 80% safe-loading limit (120 V circuits at or under 12 A; the range's 25 A under 32 A). Total connected load is about 57 A, within the 100 A service.

## Required vs design choice

**Required by code:**
- **Kitchen counter circuits** must be split 15 A, or two 20 A T-slot circuits, so counter appliances have enough power.
- **GFCI near water** (shock protection) is required by any sink and outdoors.
- **Dedicated range circuit:** the stove gets its own 240 V circuit.
- **AFCI (fire protection)** is required on living-area receptacle circuits.
- **Smoke/CO detectors** required in the bedroom and in the central area near the sleeping room and gas appliances; hardwired to a lighting circuit (circuit 1) so they are always powered.

**My design choices:**
- **Grouped bedroom + living** onto shared circuits because their loads are small.
- **Dedicated fridge circuit** so a trip elsewhere never spoils food.
- **Dedicated bathroom circuit** because a hair dryer alone nearly maxes a 15 A circuit.
- **Two spare breakers** left open for future loads.

## Legend

**Breaker (e.g. "15 A, 1-pole").** The safety switch in the panel that cuts power if the circuit draws too much current, protecting the wire from overheating. "15 A" is the current at which it trips. A **pole** is one connection to a live (hot) wire: "1-pole" connects to one 120 V hot wire (normal circuits); "2-pole" connects to both hot wires at once for a 240 V load like the range, and both sides cut off together.

**Conductor (e.g. "14/2 AWG").** The wire feeding the circuit. **AWG** (American Wire Gauge) is the wire thickness, where a lower number means a thicker wire that carries more current (14 AWG = 15 A, 8 AWG = 40 A). The number after the slash is how many insulated wires are in the cable: **14/2** = one hot + one neutral (plus a bare ground); **14/3** = two hots + one neutral (plus ground), used for split and 240 V circuits.

**GFCI (Ground-Fault Circuit Interrupter).** Cuts power instantly if electricity leaks to ground, protecting people from shock. Required near water: kitchens, bathrooms, and outdoors.

**AFCI (Arc-Fault Circuit Interrupter).** Cuts power if it detects dangerous arcing or sparking in the wiring, preventing fires. Required on most living-area circuits.

**Leg (A / B).** The service enters as two 120 V "legs" (A and B) that together make 240 V. Each 120 V circuit connects to one leg; a 240 V circuit like the range uses both, shown "A+B". Circuits are spread across A and B so the load is balanced roughly evenly on each side.

**Load (W / A).** The estimated power a circuit carries, in watts (W), and the current in amps (A = W divided by voltage). These are estimates for sizing, not measured values; a real design uses each appliance's nameplate rating. Each circuit is kept at or below 80% of its breaker rating (12 A on a 15 A breaker). For 2-pole circuits, the amps shown are the current in each hot leg. The sum of all circuit loads is higher than the single demand figure used to size the whole service, because the service calculation assumes not everything runs at once.
