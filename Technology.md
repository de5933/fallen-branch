# Technology

*Each file numbers its own sections independently starting at §1. Cross-references elsewhere in the bible take the form `[File §X.Y](File.md#X.Y)`, naming the target file before the section number.*

## Contents

- [1. Propulsion & Vehicle Engineering](#1)
  - [1.1 Fusion Torch Drive: Network Standard](#1.1)
  - [1.2 The Danu Vehicle Fleet](#1.2)
  - [1.3 The Enlil System Vehicle Fleet](#1.3)
  - [1.4 The Obatala Vehicle Fleet: Yemoja-Route ITV](#1.4)
    - [1.4.1 Hab Pod: Twin-Boom Parallel-Pod Architecture](#1.4.1)
- [2. Post-Collapse Electronics](#2)
  - [2.1 Material Sourcing and the Rare-Earth Wall](#2.1)
  - [2.2 Fabrication Tier](#2.2)
  - [2.3 Display Evolution](#2.3)
- [3. Energy Storage: The Battery Chemistry Ceiling](#3)
- [4. Arms and Equipment](#4)
- [5. Technological Reconstruction Timeline](#5)
  - [5.1 The Long Rebuild](#5.1)
  - [5.2 The Frozen Archive](#5.2)
- [6. Pre-Collapse Computing Substrate and AI](#6)
  - [6.1 Computing Substrate: Evolutionary, Not Revolutionary](#6.1)
  - [6.2 Farfield AI: Capability and Architecture](#6.2)
- [7. Personal Augmented Reality: Retinal-Projection Glasses](#7)
  - [7.1 Technology and Optical Limits](#7.1)
  - [7.2 Presence: Spatial Rendering and the Comm-Delay Gradient](#7.2)
  - [7.3 Post-Collapse: Manufacturing Loss and the Repair Trade](#7.3)
  - [7.4 The Archive: Surveillance and Its Social Function](#7.4)

<a name="1"></a>
# 1. Propulsion & Vehicle Engineering

<a name="1.1"></a>
## 1.1 Fusion Torch Drive: Network Standard

Farfield's standard in-system drive is a Trelium-fueled fusion torch, doped beyond a conservative baseline to a defensible "mid-range" spec: exhaust velocity of roughly 1,000–1,500 km/s. **Long-haul routes fly a continuous-thrust brachistochrone profile** — accelerate the first half of the trip, flip at the midpoint, decelerate the second half, no coast phase — rather than the accelerate-coast-decelerate profile originally assumed here. The short-burn alternative was evaluated and found not to close: reproducing a multi-hundred-km/s delta-v budget in a burn lasting hours to days demands radiator areas in the tens of square kilometers regardless of ship mass, a hard physical wall rather than an engineering-margin problem ([§1.4](#1.4)). Continuous thrust spreads the same total delta-v over weeks to months, dropping peak power by roughly two orders of magnitude and making the radiator problem tractable.

Mission budget is now route-specific rather than one fixed figure, since it falls out of each route's actual distance and a chosen transit-time cap rather than a single network-wide constant: see [§1.2](#1.2) (Danu/Lugh) and [§1.4](#1.4) (Obatala/Yemoja) for locked figures, and [Travel §1](Travel.md#1) for the resulting transit times per route.

Ships never transit a gate — the throat is sized for people and freight only, never hulls ([Infrastructure §1](Infrastructure.md#1)). Every torch-drive vessel is built, fueled, and scrapped entirely within its home system; nothing built in one system can ever fly to another. This is a hard physical ceiling, not a policy — it holds equally before and after the severance, and it means Danu's post-independence propulsion shift (see [Economy §2](Economy.md#2)) was always a matter of developing local technical knowledge rather than replacing stranded Nova Reach hardware, since no such hardware could ever have crossed to begin with.

<a name="1.2"></a>
## 1.2 The Danu Vehicle Fleet

Four physically distinct vehicle classes serve the Danu branch, each sized to the specific journey it makes rather than built to one generic standard — a direct consequence of how different Lugh's and Boann's local environments actually are ([Cosmology §4](Cosmology.md#4)), confirmed by working the real numbers for each route rather than assumed for narrative variety.

**Naming convention.** Farfield's official designators follow a dry, functional letter-and-number scheme in the same spirit as the Sat-# convention ([Infrastructure §2](Infrastructure.md#2)) — no PR spend justified unless a vehicle is a genuine first ([Politics §3](Politics.md#3)'s cost efficiency). In-universe usage draws a real aerospace distinction between an **aircraft** (operates exclusively within atmosphere, never leaves it) and a **transatmospheric vehicle (TAV)** — a vehicle whose defining feature is transitioning between atmospheric flight and orbit. Colonists use both terms functionally ("that's an aircraft, not a TAV"), not just as marketing:

| Vehicle | Official designator | Common usage |
|---|---|---|
| Lugh Surface Aircraft | Farfield A-6 | "aircraft" |
| Lugh Spaceplane | AOTS (Atmospheric Orbital Transfer System) | Farfield Skyreach; TAV (class term — the network's only vehicle of this type) |
| Interplanetary Transfer Vessel | ITV | "ITV" / "OTO" (route jargon, orbit-to-orbit) |
| Boann Shuttle | Farfield PDV-1 (Propulsive Descent Vehicle) | "Boann Shuttle" / "Shuttle" |

### Lugh Surface Aircraft (Farfield A-6) — electric only

Ground-to-ground transport between Lugh's primary terminator city and its satellite settlements ([Cosmology §4.1](Cosmology.md#4.1)) runs on pure electric propulsion — motor, ducted fan/propeller, battery pack — with no rocket component at all. Two independent effects make this favorable relative to Earth aviation:

- **Lower liftoff/cruise speed.** Lugh's ~2.6× Earth-surface atmospheric density (from its 1.8 bar CO2 atmosphere) lets a wing reach its efficient lift coefficient at roughly half the airspeed an equivalent Earth aircraft needs (v ∝ √(g/ρ)) — the physical basis for the network's already-established 20–40 km/h light-aircraft culture.
- **Lower energy cost per kilometer.** At matched airframe and payload, energy/distance scales with weight, i.e. with gravity: Lugh's 0.70g cuts cruise energy cost by **~30%** relative to an identical Earth flight. Lower dynamic pressure at cruise also plausibly permits a lighter structural fraction (gust and landing loads scale down with speed), compounding the energy savings further, though this second effect isn't yet quantified past the qualitative level.
- **Payload trade.** Flown at Earth-equivalent airspeeds instead of taking the speed savings, the same wing can carry roughly **3.7× the payload per unit wing area** (ρ_Lugh/ρ_Earth × g_Earth/g_Lugh ≈ 3.7) — the more relevant number for a cargo-hauling world.

Real-world electric regional aircraft already achieve 200–400 km ranges on current battery technology; at 30%+ better energy economy, Lugh's terminator-line hops between settlements sit comfortably within that same envelope ([§3](#3) below covers the network's battery chemistry ceiling). No exotic future battery tech required.

### Lugh Spaceplane (AOTS / Farfield Skyreach) — hybrid electric/H2-LOX, single-stage reusable, TAV

Surface-to-orbit-and-back transport, handing off cargo to the Interplanetary Transfer Vessel (below) at Lugh parking orbit. A gliding lander ([Cosmology §4.1](Cosmology.md#4.1)) — the underlying physics checks out favorably:

- **Reentry.** Scale height (H = RT/(Mg) ≈ 8.25 km at a representative 300 K terminator temperature) comes out almost identical to Earth's ~8.4 km, but column mass (P/g ≈ 26,200 kg/m²) runs **2.5× Earth's** — meaning more atmosphere to shed velocity into per unit of descent. Orbital velocity to dissipate is 6.53 km/s, versus Earth's 7.9 km/s. Net result: a *gentler* reentry environment than Earth's own Space Shuttle faced, confirming the lifting-body glide entry as the right approach for this vehicle.
- **Ascent — hybrid propulsion.** Ambient CO2 (fully-oxidized carbon) rules out an Earth-style air-breathing jet, but supports no such limitation on an electric ducted-fan/propeller stage: thrust from a propeller comes from momentum imparted to ambient gas, chemistry-agnostic. The spaceplane's low-speed, low-altitude climb — the segment where gravity losses are worst and a rocket is least efficient — runs on the same electric propulsion family as the Surface Aircraft, drawing thrust from the thick lower atmosphere for free. Once airspeed and altitude exceed what the fan can efficiently push against, the vehicle stages (functionally, not physically — same airframe, switched propulsion mode) to H2/LOX rocket for the high-speed climb and vacuum insertion.
- **Rocket-only ΔV budget:** orbital velocity (6.53 km/s) plus the remaining gravity/drag losses the rocket phase alone incurs, estimated at **~6.8 km/s** total after the electric-assist offload. At H2/LOX Isp ≈ 450s (ve ≈ 4,413 m/s): mass ratio e^(6800/4413) ≈ 4.67, or **~79% propellant fraction**.
- **Verdict:** single-stage, but a genuine engineering achievement rather than a comfortable margin — meaningfully below Earth SSTO concepts' ~90%+ propellant-fraction wall (which sank real designs like X-33 and Skylon), thanks to Lugh's lower g, lower total ΔV, and gentler reentry all pulling the same direction. A ~20% dry-mass fraction (tanks, structure, TPS, electric and rocket propulsion) is demanding but achievable — worth treating in-universe as a source of real engineering pride, a fully reusable spaceplane architecture Earth aerospace never quite closed the numbers on.

### Interplanetary Transfer Vessel (ITV) — Trelium fusion torch

**Reuses the Obatala-route Yemoja ITV architecture wholesale** ([§1.4](#1.4)/[§1.4.1](#1.4.1)) rather than a separate design — continuous-thrust brachistochrone trajectory, doped Trelium torch run continuously (not the older accelerate-coast-decelerate short-burn profile this section originally specified), same twin-boom parallel-pod hab geometry, same propulsion/radiator/propellant scheme. This supersedes the original 350–400 km/s / 54–57 day / 5,000 t figures below, which assumed a short-burn profile since shown not to close for any long-haul route at reasonable radiator size ([§1.4](#1.4)).

At the Yemoja-route ship's locked 0.00959g continuous acceleration, applied to Lugh's shorter 5.85 AU one-way distance: **70.6 days transit, 573.9 km/s total ΔV** (vs. Yemoja's 90 days / 732 km/s) — genuinely cheaper in both time and propellant, since it's the same engine and hull carrying less total delta-v over a shorter haul.

**Mass budget (~524 t class vessel, identical to the Yemoja design):**

| Component | Mass | Notes |
| --- | --- | --- |
| Propellant (doping water) | 229.0 t | 43.7% propellant fraction (vs. Yemoja's 51.9% — shorter route needs less) |
| Propellant (D + He-3 fusion fuel) | ~0.5 t | Scales down slightly from Yemoja's 0.63 t (shorter burn duration) |
| Radiator | 10.2 t | 2,039 m², 2,000 K, four right-triangle panels on aft spine extension beyond engine — essentially unchanged from Yemoja, since thrust (and therefore jet power) is nearly identical at the same acceleration and ship mass |
| Tankage | 18.3 t | ~8% of propellant mass |
| Spine structure | 29.5 t | Booms + hub structure |
| Hab pod | 53.45 t | Identical to Yemoja design — twin-boom parallel-pod, 4 m⌀×24.67 m, sleeper-train cabin layout, crew of 8 |
| Engine + shadow shield | 30 t | At hub, r=0 |
| **Cargo** | **153.95 t** | Higher than Yemoja's 111.55 t — the "free" benefit of reusing a ship sized for a longer route on a shorter one |

Never enters atmosphere; operates exclusively between Safford and Lugh parking orbit, exchanging cargo with Lugh Spaceplanes via orbital rendezvous.

**Fleet-size implication.** 153.95 t cargo capacity per vessel is well below the previous design's 2,500 t figure — matching Danu's established ~22,500 t/yr export demand ([History §3.4](History.md#3.4)) now requires a much larger fleet than the previously stated 5–6 vessels. Flagged for revisit — either the fleet size grows substantially, or the demand figure itself needs reconsideration now that the underlying ship design has changed.

### ITV Artificial Gravity: Axial Spin-Gravity Architecture

Shares the Yemoja-route ITV's architecture in full ([§1.4](#1.4)/[§1.4.1](#1.4.1)): axial spin, spin axis = thrust axis, engine and shadow shield at the hub (r=0), hab pod on a boom at fixed r=12.4 m (0.5g at 6 rpm), cargo on a counterweight boom at fixed radius, propellant tanks on-axis fore/aft of the hub. **Spin rate: 6 rpm — locked**, same rationale as before (fastest rate still passenger-tolerable-with-adaptation).

**Four spin transitions, not two.** Because this is a continuous-thrust profile with a mid-course flip (accelerate first half, decelerate second half), and the engine sits on the spin axis (making a 180° reorientation while spinning a genuine gyroscopic problem), the ship must despin before the midpoint flip and respin afterward — in addition to spin-up at departure and despin at arrival. This supersedes the single spin-up/spin-down cycle assumed under the old short-burn profile below. RCS thrusters mounted at the hab pod's own radius (best available lever arm) handle all four transitions; a flywheel was considered and rejected on the same grounds as before — rim speed scales explosively as radius shrinks, making RCS the simpler solution at this spin rate.

**Lugh-specific geometry** (cargo mass differs from Yemoja's, so the counterweight boom radius and moment of inertia differ too — everything else is shared):

| Figure | Value |
|---|---|
| Hab boom radius | 12.4 m (shared with Yemoja design) |
| Cargo boom radius | 4.31 m (solved from balance: 53.45 t hab × 12.4 m = 153.95 t cargo × r) |
| Moment of inertia (simplified 2-point model) | 1.107×10⁷ kg·m² |
| Angular momentum at 6 rpm | 6.96×10⁶ kg·m²/s |
| RCS propellant, 4 transitions (hydrazine, ~2,158 m/s ve) | ~1.04 t, ~1.25 t with 20% margin |
| As fraction of total ship mass | ~0.2% — trivial against the propellant budget |

*Historical note: the reference geometry table and flywheel-rejection analysis originally in this section (5,000 t class sizing, 14.6 m reactor arm, 27 m total spine, ~28 t spin-propellant figures) assumed the old accelerate-coast-decelerate ship design and short-burn spin-up/down cycle. Superseded by the above; retained nowhere else in the bible.*

### Boann Shuttle (Farfield PDV-1) — single-stage H2/LOX, full surface-to-Safford route

Boann's situation is qualitatively different from Lugh's, and the vehicle architecture follows suit rather than mirroring it. Safford Danu sits co-orbital with Boann around Mannannán (<7 sec comm delay, [Infrastructure §5](Infrastructure.md#5)) — a short moon-to-moon hop, not an interplanetary transfer. Using Io/Europa-analog orbital radii (Boann ~421,700 km, Safford's moon ~671,100 km from Mannannán) and standard Hohmann-transfer math: **~3.2 km/s total ΔV, ~35 hour transit.**

Boann's own gravity well barely matters against that transfer cost: escape velocity is only 464 m/s (from 0.02g, [Cosmology §4.3](Cosmology.md#4.3)), versus the interorbital transfer's ~3.16 km/s — local escape is only ~15% of the mission total, the inverse of Lugh's situation, where local escape dominates. This makes splitting Boann's route into a lander-plus-tug pair pure overhead: there's no altitude regime around Boann deep enough for staging to buy anything (a 50 km parking orbit's circular velocity, ~314 m/s, is barely below surface orbital velocity itself, ~328 m/s). **A single Boann Shuttle flies the entire route, surface to Safford dock — no separate orbit-to-orbit vessel** ([History §3.4](History.md#3.4)).

Combining Boann's escape burn with transfer injection via the Oberth effect (most efficient deep in the well): launch ΔV ≈ √(464² + 1,676²) ≈ 1,740 m/s; arrival/circularization burn ≈ 1,488 m/s; **total ≈ 3,230 m/s.** At H2/LOX Isp ≈ 450s: mass ratio e^(3230/4413) ≈ 1.98, or **~49% propellant fraction** — an entirely ordinary single-stage budget.

**Launch and landing character.** No atmosphere means pure propulsive flight door to door — closer to a small-body landing (Philae, Hayabusa-style) than a planetary descent. With escape velocity this low, there's essentially no passive stability to lean on; the vehicle flies itself down under continuous active control the entire way, at approach speeds plausibly in the cm/s-to-low-m/s range near touchdown, since overshoot is trivial to induce and expensive in control authority (not fuel) to correct. The real hazard is plume-kicked debris: with escape velocity so low, exhaust interaction with loose ice or regolith near the pad can fling material at a meaningful fraction of escape velocity — the physical justification for the pad already being blast-diverted ([§1.2](#1.2) above, [History §3.4](History.md#3.4)) rather than open. Post-landing, the vehicle is grapple-anchored immediately on touchdown; 0.02g provides essentially no restraint against thermal creep or accidental bumps, so an unattached vehicle on the pad is closer to a docked spacecraft than a parked aircraft.

### Summary

| Vehicle | Designator | Route | Propulsion | Single-stage? | Key figures |
|---|---|---|---|---|---|
| Lugh Surface Aircraft | Farfield A-6 | Terminator city ↔ satellite settlements | Electric only | N/A (no staging) | ~30% lower energy/km than Earth-equivalent; ~3.7× payload/wing-area at matched speed |
| Lugh Spaceplane | AOTS / Farfield Skyreach (TAV) | Lugh surface ↔ Lugh parking orbit | Electric (low-speed climb) + H2/LOX (high-speed climb, vacuum insertion, reentry reserve) | Yes — ~79% propellant fraction, ~20% dry-mass target | Reentry: 2.5× Earth column mass, same scale height, 6.53 km/s to shed |
| Interplanetary Transfer Vessel | ITV | Lugh parking orbit ↔ Safford | Trelium fusion torch | Yes — 43.7% propellant fraction | 573.9 km/s ΔV, 70.6 days; ~524 t class; ~153.95 t cargo; continuous-thrust brachistochrone, axial spin-gravity at 6 rpm (shares Yemoja-route design, [§1.4](#1.4)) |
| Boann Shuttle | Farfield PDV-1 | Boann surface ↔ Safford (direct, no parking-orbit handoff) | H2/LOX | Yes — ~49% propellant fraction | ~3.23 km/s total ΔV; ~35 hr transit; escape velocity only 464 m/s |

<a name="1.3"></a>
## 1.3 The Enlil System Vehicle Fleet

Ereshkigal has no atmosphere — locked canon, and a real physical consequence rather than a convenient assumption: the same red-giant expansion and subsequent intense post-formation UV/X-ray flux from Enlil A's exposed core ([Cosmology §6.1](Cosmology.md#6.1)) that shredded and polluted the original planets would already have stripped or photoionized away anything Ereshkigal might once have held. This shapes every part of the system below: no gliding entry anywhere in this system, unlike Lugh — everything is fully propulsive.

**Naming convention**, following [§1.2](#1.2)'s precedent: dry Farfield designators, kept as bare acronyms in most cases rather than given colloquial names — the exception being the cargo pod, where real mass-driver engineering terminology (dating to Gerard O'Neill's original 1970s concept) already supplies an authentic, unpretentious term:

| Vehicle | Official designator | Common usage |
|---|---|---|
| Crew launcher | Farfield PDV-2 | "PDV-2" (same lineage as Boann's Farfield PDV-1, [§1.2](#1.2) — both fully propulsive, airless-world shuttles) |
| Cargo vehicle (mass driver) | Farfield MD-C (Mass Driver – Cargo) | "a bucket" |
| Tank vehicle (mass driver → depot) | Farfield MD-T (Mass Driver – Tank) | "MD-T" |
| Orbital transfer vessel (Enlil variant) | ITV | "Safford OTO" |

### The Safford–Ereshkigal hop is deceptively expensive

Physical separation between Safford Enlil and Ereshkigal is the shortest branch-station pairing in the network (~0.035 AU) — naively this looks like Boann's cheap short hop. It isn't, because both bodies orbit deep in a white dwarf's gravity well. Enlil A packs 0.62 M☉ into an Earth-sized sphere; circular orbital velocity (√(GM/r)) at Ereshkigal's 0.015 AU works out to **191.5 km/s**, and at Safford's 0.05 AU to **104.9 km/s** — the same physics that gives real Mercury (0.39 AU from the Sun) its 47.9 km/s orbital speed, taken further. A Hohmann transfer between the two costs **~79.7 km/s total ΔV**, with a transit time of **~32.6 hours (1.4 days)** — consistent with, and a good validation of, the bible's existing "under 2 days" figure ([Travel §1](Travel.md#1)).

**This route reuses the Obatala/Danu ITV architecture ([§1.4](#1.4)/[§1.4.1](#1.4.1)) scaled down, rather than a distinct "lean hull" concept** — a short-burst chemical or unscaled fusion approach was checked and ruled out on the same radiator-physics grounds that shaped the long-haul ships: even at this route's much smaller 79.7 km/s ΔV, a short burn (hours, not spread across most of the transit) demands radiator area wildly out of proportion to a ~100 t hull. Chemical propulsion doesn't help either — 79.7 km/s against ~4.5 km/s chemical exhaust velocity gives a mass ratio near 5×10⁷, i.e. essentially all-propellant.

**Locked design: ~100 t class vessel, 48-hour total transit (24 hr continuous burn each way), 300 km/s exhaust velocity, 0.094g acceleration, 6 rpm spin-gravity.** Despite the short trip, spin gravity was judged worth the added complexity at this duration (overriding the "under a week doesn't need it" heuristic below — a deliberate comfort-priority call, not a technical requirement). Reuses the twin-boom parallel-pod hab architecture, engine-at-hub geometry, on-axis depleting-propellant placement, and four-transition RCS spin schedule from [§1.4](#1.4)/[§1.4.1](#1.4.1) wholesale, just resized.

**Mass budget:**

| Component | Mass | Dimensions |
| --- | --- | --- |
| Propellant (doping water) | 23.29 t | Cylindrical tank, 2 m ⌀ × 7.41 m, on-axis |
| Propellant (D + He-3 fusion fuel) | 7.83 kg | D₂: 0.33 m ⌀ sphere; He-3: 0.53 m ⌀ sphere — negligible mass, tiny tanks |
| RCS propellant (hydrazine, 4 transitions) | 0.18 t | 0.69 m ⌀ sphere |
| Radiator | 5.72 t | 1,144 m² total, 2,000 K — see panel geometry below |
| Hab pod | 8.46 t | 2.5 m ⌀ × 10 m, boom-mounted at r=12.4 m (same 0.5g/6 rpm standard as the long-haul ships) |
| Engine + shadow shield | 15 t | At hub, r=0 |
| Tankage | 1.87 t | |
| Spine structure | 7.67 t | Hab boom (12.4 m) + cargo boom (2.77 m) |
| **Cargo** | **37.95 t** | Cylindrical module, 2.5 m ⌀ × 12.9 m (at working 600 kg/m³ bulk density — placeholder, see Open Questions) |

**Hab pod interior.** Given the 2-day duration, this doesn't subdivide into the long-haul pods' room-by-room layout — one shared compartment (console/bunks combined) plus a head, closer to a real short-duration crewed capsule (Soyuz, Dragon) than the Yemoja/Lugh design's dedicated bridge/medbay/galley/cabins. Crew: Pilot and Engineer only (2 total) — see crew-role reasoning below.

**Radiator geometry: 3 panels distributed radially around the spine, tapering at the tail end to stay within the engine's shadow-shield cone.** Each panel: 381.3 m², radial height 10 m at the wide (nose-ward) end, tapering to zero over the aft-most 10 m as it approaches the shield — total panel length ~43.1 m, assuming a 45° shadow-cone half-angle (illustrative; exact shield radius/standoff not locked, see Open Questions). The cone widens moving away from the shield (tail), so panels are narrowest near the engine and widest toward the nose.

**Counterweight boom radius: 2.77 m** — cargo (37.95 t) balancing the hab pod (8.46 t at r=12.4 m) sits much closer to the hub than the long-haul ships' counterweight booms, since cargo mass so heavily outweighs the hab pod here.

### Why fusion propulsion can't handle Ereshkigal's surface launch

Cranking up a fusion torch's thrust for a surface launch was considered and ruled out — not on radiation grounds (the population lives in a deep-shielded terminator habitat and stays safe regardless), but on power economics. Rocket power scales as **½ × thrust × exhaust velocity**: the network's small fusion drive (5 MW, ~37.5 N thrust, 200 km/s exhaust) is built for gentle deep-space maneuvering, and even a modest 20-tonne vehicle would need ~18.6 GW just to hover at that exhaust velocity — thousands of times the small drive's actual output, demanding a reactor and radiator mass that would dwarf the vehicle it's meant to lift. Fusion torches are power-limited, not reaction-mass-limited; no amount of "turning it up" fixes a bad power-to-mass ratio. Ereshkigal's fusion reactor instead stays **stationary**, feeding the mass-driver system below — sidestepping the problem entirely, since a fixed installation never has to accelerate its own reactor mass.

### Cargo and crew: separate systems, separate physics

**Mass driver — cargo only (Farfield MD-C, "a bucket").** Already established for bulk export (robotic dayside quarrying → mass-driver export, [Cosmology §6.1](Cosmology.md#6.1)), and now doing double duty launching unmanned propellant tanks (Farfield MD-T) to the orbital depot (below). Since cargo tolerates far higher g than any human passenger, a track injecting a bucket at close to Ereshkigal's own orbital velocity (6.20 km/s) only needs to run a few km to ~20 km, depending on the structural g-loading accepted (3.9 km at 500g; 19.6 km at 100g) — dramatically shorter than anything crew-rated.

**Crew — no mass-driver assist, ever.** Real g-tolerance data rules this out cleanly: untrained civilians, even in the most favorable reclined "eyeballs-in" orientation, top out around 3–4g sustained for a few seconds; sustained 6–8g for the 30+ seconds a useful launch-assist track would require is well outside what's safe for a population that includes children, the elderly, and anyone with a cardiovascular condition. Even backing off to a genuinely civilian-safe 2–3g only buys a few hundred m/s of assist against tens of kilometers of track — not worth compromising the cargo system's efficiency to accommodate. **Crew shuttles fly on rocket propulsion alone**, full stop. Ereshkigal is a place people don't leave casually — leaving is expensive and rare, a genuine, lived hardship distinct from (and harsher than) Boann's rotational-tour constraint.

### Crew shuttle (Farfield PDV-2): droppable external tank, Al/LOX, fully ISRU-derived

**Architecture.** Space Shuttle-style: a single reusable core (engines + crew capsule, never expended) draws propellant from a droppable external tank rather than carrying dedicated engines on each discarded stage — the same reusable-engine logic already established for Boann's Farfield PDV-1 ([§1.2](#1.2)), PDV-2 being the next hull in that lineage, adapted for Ereshkigal's much deeper well. Total ascent requirement: ~7,350 m/s (orbital velocity 6.20 km/s + gravity losses), split across a large dropped tank (~3,675 m/s) and a smaller onboard reserve for final orbital insertion.

**Propellant: aluminum fuel / liquid oxygen, entirely local.** No water exists on Ereshkigal, ruling out H2/LOX manufacture — but **molten regolith electrolysis** (real, water-free ISRU technology under active development for lunar applications) melts silicate rock and electrolyzes it directly into free oxygen (oxidizer) and reduced metal (refined into aluminum fuel powder), using power from the same stationary fusion reactor that feeds the mass driver. Zero import dependency for propellant — a genuine parallel to Danu's own post-collapse propellant independence, arrived at by the opposite physical route (no water at all, versus Danu's water abundance). Al/LOX runs a lower exhaust velocity than H2/LOX (~2,845 m/s, Isp ≈ 290s), but staged across two burns the propellant fraction comes out to a workable **~72.5% per stage**.

### The orbital fuel depot

**Not a bulk-transfer fuel farm — a docking cluster.** Mass-driver-launched tanks, each fitted with small maneuvering thrusters, are injected near-orbital velocity by the cargo track and only burn a modest phasing/rendezvous budget (a few hundred m/s, comparable to real Soyuz-style final-approach figures) to reach the depot — arriving still nearly full. Rather than pumping that propellant into central bulk storage (extra plumbing, transfer losses, boil-off/slosh management for no real benefit), tanks simply wait in a queue; a returning shuttle docks directly to the next available tank and uses it as-is for its descent stage, via the same mechanical/feed interface as the ascent external tank.

**Descent is staged the same way as ascent, and for the same reason.** Deorbiting and landing on an airless body costs nearly as much ΔV as reaching orbit in the first place — a real, load-bearing precedent: Apollo's Lunar Module needed ~2,220 m/s to ascend from the Moon and ~2,470 m/s to descend, genuinely comparable magnitudes. An unstaged descent would cost the same brutal ~92% propellant fraction ascent would have without staging. So: the depot tank handles the bulk deceleration burn and is dropped once spent; a smaller onboard reserve (topped off at the depot alongside collecting the fresh external tank) handles the final landing burn on the now much lighter core.

**Reference sizing** (illustrative — core dry mass, payload, and crew capacity aren't locked canon yet, flagged for confirmation): core dry mass 5,000 kg, onboard reserve tank structure 500 kg, payload 1,000 kg. Per-staged-burn mass ratio 3.64 (72.5% propellant fraction). Final landing burn: ~17.2 t propellant, ~23.7 t total. Depot tank: ~79.1 t propellant + ~6.3 t structure ≈ **~85.5 t total**. Total mass at depot docking before descent begins: **~109 t**.

### Tank disposal: expended, not recovered

Neither the ascent nor the descent tank is recovered or reused. **Ascent tanks** are dropped while still suborbital — deliberately timed (mirroring how Space Shuttle's own External Tank was targeted short of orbit) so they fall back to Ereshkigal's surface under gravity rather than lingering as permanent orbital debris; without atmosphere, nothing in orbit here decays naturally the way it does on Earth, so anything left in orbit stays a collision hazard indefinitely. This gives Ereshkigal's flight authority a genuine, ongoing operational burden — active debris tracking, not a solved problem, and a real hook if a future incursion or accident subplot ever needs a crowded, unforgiving orbital environment.

**Descent tanks** are dropped near the end of final approach, close to the surface. They do not survive intact: a hard, uncontrolled impact on Ereshkigal's near-Earth 0.95g surface tears an empty aluminum tank apart rather than leaving salvageable structure. This turns out not to matter economically — **the same molten regolith electrolysis process already running continuously to supply the settlement's breathing oxygen produces surplus aluminum as an unavoidable byproduct**, so fresh tank stock is cheap relative to any recovery effort. Tanks are treated as consumable, not precious; propellant and structure both flow from the same ongoing life-support-driven industrial process, and there's no separate "propellant industry" or "tank-recycling industry" to speak of — just one shared resource loop that happens to feed both breathing air and rocket fuel.

*Naming for the Ereshkigal fleet (see table above): Farfield PDV-2 (crew launcher), Farfield MD-C / "a bucket" (cargo), Farfield MD-T (propellant tank), and Safford OTO (the Enlil ITV variant).*

<a name="1.4"></a>
## 1.4 The Obatala Vehicle Fleet: Yemoja-Route ITV

Yemoja's distance from Safford Obatala (co-orbital with Olokun, [Cosmology §5.3](Cosmology.md#5.3)) — ~9.05–9.95 AU — put it well outside the network-standard 350–400 km/s ΔV budget ([§1.1](#1.1) above), which was sized for the much shorter Danu haul. Reworking the trajectory and vehicle from first principles for this route surfaced a genuinely different design than the Lugh-route ITV, not just a rescaled copy.

**Trajectory.** Modeled as a continuous-thrust brachistochrone (accelerate first half, flip, decelerate second half) rather than the Danu route's short-burn-plus-coast profile — a real architectural difference, not a scaled parameter. Distance used: ~9.51 AU chord, assuming a representative 90° orbital phase angle between Safford and Yemoja at departure. Transit time capped at **90 days**, yielding a required continuous acceleration of **0.00959g** and total **ΔV of 732 km/s**. Local departure/arrival gravity-well spiral phases (Safford's orbit around Olokun; Yemoja orbital insertion) were checked explicitly and found small — combined under 24 hours against the 90-day transit — because the ship's thrust substantially exceeds local gravity at the assumed parking-orbit radii; safe to treat the brachistochrone as unperturbed by local-body gravity for trajectory purposes.

**Why continuous thrust, not short burns.** A short, high-thrust burn profile (matching the Danu route's style) was evaluated first and rejected: reproducing this route's ΔV in a burn lasting hours to a few days requires radiator areas in the tens of square kilometers, regardless of ship mass — a hard physical wall, not an engineering-margin problem (waste heat scales with mass flow while radiator capacity only scales with area × T⁴). Spreading the same total ΔV over a continuous 90-day burn instead drops peak jet power by roughly two orders of magnitude, making the radiator problem tractable. This is a deliberate, load-bearing design choice: **the Yemoja-route ITV cannot use a short-burn profile at any reasonable ship mass.**

**Propulsion.** Doped Trelium fusion torch, run continuously rather than in short bursts — same underlying tech as the network standard ([§1.1](#1.1)), operated differently. Exhaust velocity **1,000 km/s** via bulk-propellant doping (see Propellant below), giving a 51.9% propellant mass fraction. Waste-heat fraction asserted at **15%** — a deliberate improvement over the 20% generic reference-design baseline (Atomic Rockets / Discovery II-class studies), representing Farfield's magnetic-nozzle engineering as somewhat more efficient than a generic baseline. *Flagged as an asserted canon choice, not derived from first principles — worth revisiting if a harder engineering justification is wanted later.*

**Radiators.** Refractory-metal liquid-droplet type, operating at **2,000 K** — near the credible upper edge of real liquid-droplet radiator literature (vs. generic solid-panel designs around 1,250 K), chosen specifically because radiated power scales with T⁴, making this the single most effective lever against radiator size. Areal density 5 kg/m². Total radiator area **2,039 m²**, total mass **10.2 t**, split as **four identical right-triangle panels mounted on a dedicated aft extension of the spine, beyond the engine**, spaced 90° apart around the spine's circumference (rotationally balanced by symmetry, so radiator mass does not factor into the primary hab/cargo spin balance). Each panel is a right triangle with its narrow point at the aft (engine-side) end and its wide base facing forward, sized with axial length twice its radial height: **~22.6 m radial height × ~45.2 m axial length**, ~509.8 m² each. Placing the radiators on their own aft spine section — rather than on the hab/cargo boom line — keeps them close to the engine (short, simple coolant runs to the heat source) and, as a deliberate secondary benefit, pushes the engine itself further from the hab pod and cargo along the spine, adding standoff distance between crew/cargo and the drive without any extra dedicated shielding mass. Radial placement means panel loading is uneven across each panel's own span — outer tips reach roughly 1g of centrifugal load at 6 rpm even when the inner edge starts close to the axis — so panels are engineered more like turbine/flywheel blades than the lighter static panels a boom-mounted design would need; this is treated as a normal structural design constraint, not a blocking problem.

**Mass budget (~524 t class vessel, 111.55 t cargo capacity):**

| Component | Mass | Notes |
| --- | --- | --- |
| Propellant (doping/working fluid: water) | 271.6 t | Bulk propellant injected downstream of the fusion reaction to lower effective exhaust velocity and raise thrust |
| Propellant (D + He-3 fusion fuel) | ~0.63 t | Negligible against total propellant — fusion's energy density means fuel mass is essentially a rounding error next to the doping propellant |
| Radiator | 10.2 t | 2,039 m² total, 2,000 K, four right-triangle panels on aft spine extension beyond engine (see [§1.4](#1.4)) |
| Tankage | ~21.8 t | ~8% of propellant mass |
| Spine structure | ~25.2 t | Booms + hub structure |
| Hab pod | 53.45 t | See below — sleeper-train cabin arrangement shortened the pod from 30 m to 24.67 m |
| Engine + shadow shield | 30 t | At hub, r=0 |
| **Cargo** | **111.55 t** | Absorbs the 11.55 t saved by the shorter hab pod |

**Layout.** Engine and shadow shield sit at the hub (r=0), spin axis coincident with thrust axis. Propellant tanks (doping water, D₂, He-3, RCS) sit on-axis, fore/aft of the hub — mass that depletes over the trip contributes nothing to spin balance regardless of how much remains, and the tanks get short, simple feed lines to the engine. Cargo sits on a boom offset from the hub, at fixed radius, providing spin balance against the hab pod on its own boom (see [§1.4.1](#1.4.1) below for hab-pod-specific geometry). Boom radii: hab boom 12.4 m (locked for consistency with hab-interior artificial-gravity design below); cargo boom ~5.94 m, solved from the balance condition (cargo mass alone — radiators no longer figure into this balance at all, since they're now mounted on their own dedicated aft spine extension beyond the engine, rotationally symmetric about the spin axis; see Radiators above and Boom Structure below).

**Boom structure.** Both hab and cargo booms are **triangulated lattice trusses**, not solid beams or simple tubes — the dominant load in each boom is steady radial tension while spinning (~262 kN / ~26.7 tonnes-force at the hab-boom attachment point, matched in magnitude at the cargo-boom attachment by the balance condition; axial thrust loads during burns are smaller by roughly two orders of magnitude and are carried incidentally). Pure tension strength alone would allow an implausibly thin member — a few centimeters across in any credible structural material — so member sizing is driven instead by bending stiffness and buckling resistance against transient off-axis loads (spin-up, despin, the mid-course flip) and against resonant flexing at the 6 rpm spin rate. A triangulated lattice achieves this far more mass-efficiently than a solid rod or a thick-walled tube, since bending stiffness scales with the square of how far the load-bearing material is spread from the boom's own centerline (the same principle as flange separation in an I-beam) — spreading a fixed amount of material into a wide, triangulated lattice was found to be roughly two orders of magnitude stiffer, for the same mass, than concentrating it into a solid rod. Each boom is a **3-chord triangulated truss**, chords spread across a 1 m diameter, mild structural steel, sized with a safety factor of 3: chord cross-section ~10.5 cm² each (sharing the tension load roughly equally), cross-braced with diagonal struts at approximately 1 m bay spacing. This comes to roughly **440 kg per boom** for the hab boom's length (chords plus bracing) — a small fraction of the ~25.2 t spine-structure mass allocation, leaving headroom in that figure for the hub, cargo boom, and the new aft radiator-spine extension. Attachment to the hab pod and cargo module at each boom's outer end is a simple engineered tension joint (clevis-pin style), sized for the same steady radial load, with the small axial thrust component carried as an incidental bending/shear allowance rather than a separate design driver.

**RCS and the mid-course flip.** Because the engine sits on the spin axis, a continuous burn imparts no gyroscopic precession — but reorienting 180° at the trajectory's midpoint (accelerate → decelerate) does fight the ship's own angular momentum if attempted while spinning. Resolved as **despin → flip → respin** at the midpoint (plus spin-up at departure and despin at arrival — four transitions total), rather than adding a second, reverse-facing engine at the hub, which was considered and rejected as unnecessary added engineering and a second radioactive-exhaust source to shield against. RCS propellant (hydrazine monopropellant, ~2,158 m/s exhaust velocity) sized from ship moment of inertia (~1.22×10⁷ kg·m² at 6 rpm, simplified two-point hab/counterweight model): **~1.14 t for four transitions, ~1.37 t with 20% margin** — negligible against the total mass budget.

**Fleet-size implication.** 111.55 t cargo capacity per vessel is a small fraction of the Danu-route ITV's 2,500 t figure ([§1.2](#1.2) above) — matching any meaningful Obatala trade demand will require either a much larger fleet than Danu's 5–6 vessels, or a smaller per-route demand figure than Danu's 22,500 t/yr. Obatala's actual export/import demand figure is not yet locked; see [Open Questions](Open_Questions.md).

<a name="1.4.1"></a>
### 1.4.1 Hab Pod: Twin-Boom Parallel-Pod Architecture

The Yemoja-route ITV's crew module uses a different geometry than a simple radial tower, resolved from a real engineering constraint: gravity depends only on radius from the spin axis (g = ω²r), not on axial position, so a module extended *axially* (parallel to the spin/thrust axis) at fixed radius gets exactly uniform gravity along its whole length — no curvature underfoot (unlike a tangential arc, structurally incompatible with a rigid radial spine) and no gravity gradient (unlike a radially-stacked tower).

**Geometry:** straight cylindrical pod, ~4 m diameter × 24.67 m long, mounted on a boom at fixed r = 12.4 m (giving 0.5g at 6 rpm), its own long axis running parallel to the ship's spin/thrust axis. Floor is the outboard wall throughout the pod's length.

**Interior layout, hub-end to outboard tip** (60 m² total floor):

| Zone | Length | Notes |
| --- | --- | --- |
| Bridge/access + airlock (Captain, Pilot, First Officer, Comms Officer) | 4.0 m | Boom-proximal end — shortest path to the boom/hub, EVA equipment stored here |
| Medbay (Medic) | 2.5 m | Adjacent to bridge end — fast access in an emergency |
| Galley + mess | 5.0 m | Mid-pod — the crew's one shared social space |
| 8 private cabins (identical size, no rank-based variation) | 10.67 m | Sleeper-train arrangement — see below |
| Heads ×2 | 2.5 m | Split between mid-pod and outboard end |

**Cabin section: sleeper-train arrangement, not single-row.** Rather than stacking all 8 cabins end-to-end along one side of a corridor (the original layout, which needed 16.0 m and left the pod's far side unused per axial slice), the corridor runs centered down the pod's middle (1 m wide) with cabins flanking both sides — 1.5 m wide each, using the full 4 m diameter rather than half of it. Each cabin is still 4 m² (1.5 m × 2.67 m), same as before, just reshaped; two cabins share each of four axial slots (2.67 m per slot) rather than eight cabins occupying eight single-side slots. This uses the tube's full cross-section for private space instead of leaving one side to a bare wall, cutting the cabin section from 16.0 m to 10.67 m and the whole pod from 30 m to 24.67 m.

Crew complement: Captain, Pilot, First Officer, Chief Engineer, Engineer ×2, Comms Officer, Medic (8 total).

**Airlock and docking.** The airlock sits directly on the hab pod itself, at the boom-proximal end (the same end as bridge/access), rather than at the hub — placing it where the ship's structural and power/data connections already concentrate, and where EVA equipment is closest to the crew's living space. This only works because docking never happens while the ship is spinning: standard procedure is to despin, shut down the main drive, and complete final approach on RCS thrusters alone, docking with the airlock stationary like any conventional spacecraft hull. This is consistent with the four spin transitions already locked for the mission profile (spin-up at departure, despin/flip/respin at midcourse, despin at arrival) — pre-departure and arrival docking both fall naturally within an already-stationary window, and no separate non-rotating docking structure (e.g. at the hub) is needed.

**Bridge orientation and console layout.** The boom-proximal end (airlock) is the pod's aft-most point along the ship's thrust axis, since it sits closest to the hub/engine — the shadow shield's whole job is protecting everything *behind* it, and the boom/hub structure is what's between the engine and the rest of the pod. The pod extends forward from there, cabins and heads at the far fore-ward tip. **Crew faces forward** (toward the display and the medbay-side wall), airlock behind them at the room's aft wall — someone entering through the airlock sees the crew's backs before the display.

Corridor runs straight through the bridge's center (1 m wide, same convention as the rest of the pod), leaving ~1.49 m of depth on each side for consoles, paired two-and-two:
- **Left side:** Pilot (forward) + First Officer (aft) — adjacent since First Officer is the designated backup pilot, making a mid-flight handoff a matter of turning to face the other console rather than crossing the room.
- **Right side:** Captain (forward) + Comms Officer (aft) — Captain has an ordinary console like everyone else, not a distinct command chair; matches real submarine precedent, where the Commanding Officer doesn't occupy a fixed seat in Control but has a separate small rest space nearby (here, effectively the same as any other crew member's console during working hours) and where a role like Officer of the Watch, not a static "captain's chair," is what stays central to operations.

**Shared display: two panels flanking the corridor opening**, mounted on the forward partition wall (shared with medbay), not a single continuous screen — the corridor has to stay clear straight through to the rest of the pod, so the display splits either side of that opening rather than blocking it. Each pair of consoles naturally faces its nearer panel. Built as tiled sub-panels rather than one screen (a panel failing doesn't blank the whole display, and repair means swapping a section), showing navigation plot, sensor/exterior camera feed (substituting for a viewport, since there's nothing to see with the naked eye this far out), and engine/reactor status — whatever needs to be visible to all four crew at once rather than duplicated per console. This matches current real submarine practice: modern boats (e.g. Virginia-class) replaced hull-penetrating periscopes with photonics masts feeding video onto shared electronic displays, consolidating what used to be separate stations into one integrated space — not old-fashioned, closer to where real control-room design is heading.

**Continuous-thrust gravity interaction:** during the 90-day burn, the ship's own 0.00959g of axial thrust combines with 0.5g of radial spin gravity as a vector sum, producing a net "down" vector tilted just **1.1° off pure-radial** — within the range building codes treat as functionally level (under ~1.19°), so no deck slanting or other correction is needed. Confirms the hab pod's artificial-gravity design is unaffected by the continuous-thrust trajectory profile.

**Floor height and cross-section use.** The 4 m hull diameter isn't fully usable as flat floor — a cylindrical cross-section loses headroom near the curved walls, so floor position is a real trade-off between headroom, usable width, and space reserved below/above for infrastructure. Locked at **floor height 1.8 m above the tube's outboard-most point** (out of a possible 2.0 m at dead-center): gives **2.2 m headroom**, **~3.98 m usable width** (essentially the full hull), and **1.8 m of underfloor space** — genuinely useful rather than wasted void, since it houses local plumbing, ducting, storage, and structural mounting rather than needing to be a deep utility bay (major tankage lives on-axis at the hub, not under this floor). Going higher (toward the 2.0 m centerline) buys negligible extra width for a real loss of headroom; going lower costs width fast for headroom nobody uses.

**Underfloor (outboard of the deck, higher-gravity side):** local potable/greywater plumbing for galley and heads; life support ducting and power/data cabling; personal storage lockers accessed via floor hatches (concentrated under the cabin section); structural mounting and vibration isolation for the boom-to-pod joint.

**Overhead (inboard, lower-gravity side, tapering headroom near the walls):** air distribution ducting and light fixtures — deliberately sited where human clearance is already reduced; cable trays and comms wiring; overhead lockers for lighter gear (easier to lift down given measurably lower local gravity); acoustic dampening surface, particularly useful in the corridor given its bare-metal reverberation.

**Room-by-room character.** Farfield's engineering culture shows in the contrast between rooms — nothing here is decorative, and comfort is allotted only where it earns its keep (crew retention on a 90-day haul), not spent evenly.

- *Corridor:* bare composite paneling, scuffed at ankle height, cool white utility lighting slightly brighter than comfortable. Footsteps ring against the curved hull with nothing to absorb them. Constant low hum of ducting behind the walls. Genuinely tight — two people can't pass without turning sideways.
- *Bridge/access + airlock:* full-width and console-dense rather than boxed in — reads as purposeful, not cramped, despite the small footprint. Cool blue-white task lighting over stations, dimmer ambient elsewhere. Screens, status chimes, low comms chatter, faint ozone smell.
- *Medbay:* harsh, clinical white light, pale wipeable surfaces, no warmth. Quiet but for occasional monitoring beeps. The exam table nearly fills the room — the most claustrophobic space on the ship after the cabins.
- *Galley + mess:* the deliberate morale concession, full-width and open. Warmer amber lighting, a real shift from the cold white elsewhere. Fixed dining table (see below) with fold-up bench seating; sounds of the food processor, conversation, maybe personal music — the one place noise feels welcome rather than intrusive.
- *Private cabins:* genuinely tight, barely a berth-and-locker nook. Warm, dim, individually adjustable lighting — the one place crew get real control, matching Farfield's circadian-lighting logic. Thin partitions let corridor sound and neighbors bleed through faintly. The curved outer hull as "floor" gives a subtle barrel-like enclosure rather than a square room.
- *Heads ×2:* harsh, purely functional lighting; constant audible plumbing/recycling systems, louder than anywhere else onboard. No comfort concession at all.

**Galley table.** Fixed rather than folding — matches real submarine precedent (mess/wardroom tables are typically fixed multi-use furniture, since they double as workspace, not just dining, and re-securing a removable table every use isn't worth the trade), and Farfield's preference for fewer moving parts. At the room's ~3.98 m usable width, a table sized for 8 (~2.4 m × 0.9 m) leaves ~1.5 m clear on each side unoccupied, dropping to a still-passable ~1.1 m each side with the crew seated at meals — comfortable clearance rather than a squeeze. Bench seating folds up against the bulkhead between meals, freeing the room as open gathering space.


<a name="2"></a>
# 2. Post-Collapse Electronics

Pre-collapse, Nova Reach never developed native chip fabrication — modern semiconductor fabs require tens of billions in capital and an entire specialized equipment supply chain that only ever existed on Earth, so finished electronics were always shipped through Sat-39 rather than built locally. The Severance Event strands the network with whatever finished stock and spare parts existed at Year 92, and no clean path back to anything resembling that fabrication tier ([§5.1](#5.1) below).

Rebuilding from scratch, the colonies find their material base is a genuine mix of abundance and hard walls:

<a name="2.1"></a>
## 2.1 Material Sourcing and the Rare-Earth Wall

- **Silicon, iron, aluminum, magnesium** — Nova Reach's ring/asteroid material is undifferentiated silicate rock, plausibly abundant in all four with no invention required.
- **Phosphorus** — already Ereshkigal's signature export ([Economy §2.1](Economy.md#2.1)), and also a standard semiconductor N-type dopant; Enlil's fertilizer economy gains an unplanned second customer.
- **Boron** — the standard P-type dopant, reasonably assumed as another Nova Reach silicate byproduct.
- **Copper** — sourced from Boann's hydrothermal seafloor vents, where the moon's forsterite-rich crust ([Infrastructure §3](Infrastructure.md#3), Boann subsection) makes for genuinely favorable sulfide-metal chemistry. Post-severance, this is a political dependency as much as a technical one: Danu is independent, so Nova Reach's own electronics rebuild depends on trade with a government it fought a war against ([History §3](History.md#3)). Aluminum interconnects (a weaker conductor, but locally sourceable without Danu) are the domestic substitute Nova Reach has real incentive to develop.
- **Gold** — unnecessary. Aluminum and copper wire bonding both predate and coexist with gold in real electronics history; the tradeoff is corrosion resistance, solved with genuinely good hermetic packaging rather than an exotic material.
- **Gallium and rare-earth dopants** — absent, with no plausible in-network source identified among the currently-settled bodies. This is a hard, likely permanent wall: no compound-semiconductor components, ever, without a new discovery.

<a name="2.2"></a>
## 2.2 Fabrication Tier

The achievable fabrication ceiling is contact/proximity photolithography — micron-scale features, hand-aligned masks under UV light, no exotic optics — roughly comparable to 1960s–70s Earth chip technology in raw capability, though built with the colonists' full modern theoretical knowledge rather than rediscovered from ignorance. In practice this means low transistor density, clock speeds in the megahertz range, and real, felt latency on compute-heavy tasks — see [Culture §5](Culture.md#5) for the distributed, swarm-native software culture this constraint produced.

Basic wireless communication (radio, short-range data/voice links) is comfortably achievable at this tier, since it depends on antennas, oscillators, and amplifiers rather than dense logic or exotic RF front-end chips. High-bandwidth wireless data at modern speeds is not.

Reconstruction itself proceeds in stages, not as a single leap — see [§5.1](#5.1) below for the full Scramble → tubes → discrete transistors → indigenous ICs → maturation timeline (roughly Years 92 to 200+).

<a name="2.3"></a>
## 2.3 Display Evolution

Monochrome CRT is the universal baseline throughout reconstruction — glass, vacuum, and electron-gun engineering, none of it dependent on scarce dopants. Color follows a genuine, generations-long arc:

- **Field-sequential color** (a single monochrome tube behind a spinning red/green/blue filter wheel, synced to frame rate — the same principle used on the real Apollo lunar rover's color camera) is the earliest color technology available: mechanical, maintenance-heavy, and the first luxury/prestige display, reserved for administrators and critical control rooms in the same texture as Safford's stratified food service ([Infrastructure §2.2](Infrastructure.md#2.2)).
- **Three-phosphor color CRTs**, using pre-rare-earth phosphor chemistry (cadmium-based reds, zinc-sulfide-family greens and blues — the same chemistry real Earth color television used before the rare-earth generation of phosphors), spend decades in prototype and pilot-scale development before becoming reliable and cheap enough to displace field-sequential displays as the common standard.
- Throughout this entire period, data formats and protocols ([Culture §5](Culture.md#5)) preserve full color information losslessly even while displays remain monochrome or field-sequential — a deliberate act of institutional hope that color hardware will eventually be common again. The eventual arrival of cheap three-phosphor displays means old archives and images are finally seen in true color for the first time by anyone still alive to see them.

<a name="3"></a>
# 3. Energy Storage: The Battery Chemistry Ceiling

Pre-collapse battery technology matures across 178 years (Earth's Space Age origins through Year 92/2104) but never leaps outside real chemical bond-energy limits — three-ish generations of engineering refinement on chemistries already understood in the 21st century, not a sci-fi jump.

- **Baseline**: mature solid-state lithium-sulfur (or a comparable chemistry) delivering roughly 600–900 Wh/kg by 2104 — about triple 21st-century Li-ion's practical ~250–300 Wh/kg, and still well short of lithium-sulfur's theoretical ~2,600 Wh/kg or lithium-air's theoretical ~3,505 Wh/kg ceilings, both of which remain impractical for the same real-world reasons they do today.
- **No conflict with the gallium/rare-earth-absence rule** ([§2.1](#2.1)): battery cathode chemistries (sulfur, lithium, nickel, manganese, sodium, zinc, aluminum) are a wholly separate material family from the banned compound-semiconductor lineage, so battery technology is free to mature on its own track even where chip fabrication is permanently walled off.
- **A locked asymmetry**: lithium-air chemistry needs ambient atmospheric oxidant to reach its best energy density, so it's only genuinely viable on atmosphere-bearing worlds such as Lugh. Vacuum environments — stations, ships — would have to carry their own oxidant reservoir, eating the weight advantage entirely. Planetary-surface and station/ship equipment plausibly run on different battery chemistries as a direct physical consequence, not an arbitrary setting choice.
- **This ceiling is why coilguns, railguns, and handheld anti-personnel lasers stay vetoed even at Year 92's battery tech** ([§4](#4) below): even a full tripling of energy density over today's batteries falls well short of the roughly order-of-magnitude gap those weapons need closed to be safely portable.

<a name="4"></a>
# 4. Arms and Equipment

Nova Reach never developed a pre-collapse military industry ([History §1](History.md#1)), so the weapons and protective gear that see use during the Military Arc ([History §3](History.md#3)) are either sealed pre-collapse contingency stock or civilian/industrial equipment pressed into an unintended role — nothing is purpose-built for war.

- **No coilguns, railguns, or handheld anti-personnel lasers exist anywhere in the colonies.** The power-density gap between what a portable EM or laser weapon needs and what even mature 2104 battery chemistry can deliver is roughly an order of magnitude ([§3](#3) above) — too wide to close plausibly, so Farfield never fields them even if someone, somewhere, is theoretically researching the underlying physics.
- **Chemical-propellant firearms are the only lethal weapons in the network.** Pre-collapse, they exist solely within Farfield security/law-enforcement channels — a sealed contingency stockpile held against civil unrest rather than routine equipment, consistent with the network's purely civilian economic character ([History §1](History.md#1)). Conventional cased-propellant ammunition also stores reliably for decades with minimal upkeep, unlike anything capacitor- or battery-dependent, which is part of why it was the chosen contingency technology in the first place.
- **Distribution is heavily asymmetric.** Nearly all firearms in the network sit in Nova Reach, inside Farfield's stockpile. Danu fields no standing firearms of its own: its defenders rely on improvised weapons, repurposed engineering and agricultural tools, and superior knowledge of home terrain ([History §3.2](History.md#3.2)). What guns Danu's fighters do carry come from raiding the Nova Reach security stash during the fighting.
- **Adguns — shoulder-mounted, Active Denial System-style directed-energy crowd-control weapons — are standard Farfield security equipment**, adapted rather than newly invented:
  - The emitter is gyrotron-based (vacuum-tube, magnetic-confinement RF generation) rather than solid-state, since high-power solid-state millimeter-wave emitters depend on gallium- and rare-earth-doped semiconductors the colonies will never have access to ([§2.1](#2.1) above). Gyrotrons are already native to Farfield's fusion-reactor engineering base (electron cyclotron resonance heating), so adguns are a repurposed spinoff of existing civilian reactor technology rather than a dedicated weapons program.
  - A 95 GHz millimeter-wave beam heats only the outermost fraction of a millimeter of skin, producing pain within seconds and driving anyone struck off target well before real injury — non-lethal by design, and it does not damage nearby electronics.
  - Units are rare and infrastructure-tethered rather than battery-portable: two at Safford, one per major settlement elsewhere, wired into station or settlement power. Baseline gyrotron efficiency (roughly 30–40% electron-to-RF, the rest waste heat) is managed with ejectable, sealed phase-change-material heatsink cartridges rather than a plumbed coolant loop — the same principle real spacesuit portable life-support systems use to solve an identical cooling problem. A sealed, non-venting cartridge was chosen over open water-ice sublimation specifically to avoid condensation and fogging inside enclosed station and settlement environments. The only external connection an adgun needs is its power cable; thermal load is handled entirely by swapping spent cartridges for fresh ones.
  - The beam is blocked by simple materials — a sheet of plywood, a mattress — and attenuated by rain, fog, and humidity, giving Danu's agricultural world genuine, non-exotic countermeasures its people would plausibly have on hand.
- **No militarized body-armor industry ever existed.** The strongest candidate for Farfield security's protective gear is armor derived from repurposed micrometeoroid/debris-shielding materials science — the same physics underlying ship-hull shielding — civilian/spacecraft-derived protection rather than a purpose-built military design.
- **No powered cargo exoskeletons appear as combat gear.** Considered as a possible visual for Danu's improvised resistance and ruled out as too far-fetched for the setting's grounded, nothing-purpose-built character — cargo handling on Danu stays manual or vehicle-assisted, not exoskeleton-assisted.

See [Open Questions](Open_Questions.md) for equipment details not yet locked as canon, including armor material specifics, adgun unit siting at Safford and each settlement, and other non-lethal options under consideration (acoustic hailing/dispersal devices, riot foam, chemical irritants). See [History §3.4](History.md#3.4) for how this equipment played out tactically across the Nova Reach–Danu conflict.

<a name="5"></a>
# 5. Technological Reconstruction Timeline

<a name="5.1"></a>
## 5.1 The Long Rebuild

Pre-collapse, all cutting-edge electronics were finished goods shipped from Earth through Sat-39 — no colony ever needed or built native fabrication capacity, since duplicating Earth's fabrication supply chain locally was never remotely cost-effective ([§2](#2) above). The Severance Event doesn't just cut off new chips; it strands the network with whatever finished stock and spare parts happened to be on-hand or already in the pipeline at Year 92, with no path to more.

What follows is roughly a century of bootstrapped reconstruction, not a single recovery:

- **Years 92–~110, Scramble.** Pure triage: salvaged boards, passive-component repair, no new active electronics built at all.
- **Years ~110–140, Vacuum tube resurgence.** The first genuinely new (not salvaged) active components since the collapse — tubes need glassblowing and vacuum sealing, nothing from the fabrication supply chain that died with Sat-39.
- **Years ~140–170, Discrete transistors.** Hand-built, not integrated, once local doping and crystal-growing processes mature.
- **Years ~170–200, First indigenous integrated circuits.** Contact/proximity photolithography stood up as real infrastructure — a genuinely dated, celebrated milestone: the day the colonies could build their own chips again, not merely patch old ones.
- **Years 200+, Maturation.** Yield and scale improve; color-capable displays move from prototype to common availability ([§2.3](#2.3) above).

See [§2](#2) above for the material and technical detail behind each stage, and [Culture §5](Culture.md#5) for the software culture this constraint produced.

<a name="5.2"></a>
## 5.2 The Frozen Archive

At collapse, Nova Reach's local LLM inference infrastructure — a Farfield corporate asset, hosted at Nova Reach for latency reasons rather than owned by the colony itself — is stranded with whatever model weights happened to be cached at Year 92, permanently unable to retrain or update. Farfield's ownership of everything in the colonies ([Politics §4.1](Politics.md#4.1)) makes its post-collapse status a matter of practical control rather than settled law: whoever can physically reach and maintain the hardware effectively owns it now, whatever the org chart used to say.

No single administration ever makes a clean decision to preserve or dismantle it. Instead, across Phases 1 through 3 and beyond ([History §3](History.md#3)), the data center is worn down by a slow, piecemeal cannibalization — a rack pulled here for a life-support board, a memory module scavenged there for a failing gate-control system, each individual decision a reasonable emergency triage call, never an official policy. What survives by the time indigenous chip fabrication matures ([§5.1](#5.1) above) is a degraded, patched wreck running on a fraction of its original hardware — not dead, not whole, kept alive mostly by whoever still has the swarm-control expertise ([Infrastructure §2.2](Infrastructure.md#2.2)) to run something that distributed and resource-starved at all.

<a name="6"></a>
# 6. Pre-Collapse Computing Substrate and AI

*Everything in this section describes Year 92 baseline technology — what existed, and was lost, at the moment of collapse. It is the "before" picture that makes [§5.1](#5.1)'s reconstruction arc and [§5.2](#5.2)'s Frozen Archive read as a genuine fall rather than a lateral move.*

<a name="6.1"></a>
## 6.1 Computing Substrate: Evolutionary, Not Revolutionary

Peak pre-collapse computing is 178 years of continuous engineering refinement on physical principles already understood in the early 21st century — not a leap to some fundamentally different substrate. Consistent with the network's supply-chain-dependency material picture ([§2.1](#2.1) above), mainstream Farfield computing at Year 92 runs on:

- **Full 3D monolithic integration** — the endpoint of chiplet/die-stacking approaches already underway in the 21st century, taken to maturity rather than invented from nothing.
- **Silicon photonics for interconnect** — optical rather than electrical signaling for chip-to-chip and on-die communication, mainstream by Year 92 rather than the commercial-datacenter-niche technology it is at the setting's real-world starting point. This matters practically as much as narratively: photonic interconnect sheds far less waste heat than electrical signaling at equivalent bandwidth, a genuine engineering advantage on stations and ships where heat rejection is always at a premium.
- **Neuromorphic/analog accelerators** — dedicated non-von-Neumann hardware purpose-built for the inference workloads AI ([§6.2](#6.2) below) actually runs, distinct from general-purpose compute rather than an application running on it.
- **Narrow-purpose quantum co-processors** — not general-purpose quantum computers, which remain commercially impractical even after 178 years, but specialized systems for the narrow class of problems quantum hardware is actually suited to: optimization and quantum-chemistry-style simulation. The one significant in-universe application is **quantum-assisted modeling in wormhole-seed viability characterization** ([Cosmology §2.4](Cosmology.md#2.4)) — a small number of these systems exist, concentrated at Nova Reach, supporting the wormhole engineers' threading-field response work ([Culture §3](Culture.md#3)).

**What this costs post-collapse.** Photonic interconnect, neuromorphic accelerators, and especially the quantum co-processors sit well beyond the reconstruction arc's achievable ceiling ([§2.2](#2.2) above) — they depend on fabrication and materials infrastructure ([§2.1](#2.1)) far deeper than contact/proximity photolithography can ever reach, not merely on the rare-earth dopants already walled off. These aren't degraded by the collapse; they're gone outright, with no reconstruction path at any stage of [§5.1](#5.1)'s timeline. This is the concrete, physical reason the "sacred legacy code" culture ([Culture §5](Culture.md#5)) is more than sentimental: some of that inherited software was written assuming hardware acceleration nobody will ever be able to build again, forcing the lean, low-density-hardware-native toolchain to be a genuine reinvention rather than a simple port.

<a name="6.2"></a>
## 6.2 Farfield AI: Capability and Architecture

**Capability.** Farfield's peak pre-collapse AI is cross-domain and general-reasoning-adjacent — genuinely useful judgment across varied problem types, not a narrow single-purpose tool — but bounded and non-sentient. It's advanced enough to be a real subject of dispute among colonists (a natural flashpoint given the labor anxieties already present in Safford's culture, [Culture §2](Culture.md#2)) and just capable enough to be unsettling to people who work alongside it daily, without ever crossing into anything the story treats as actual general intelligence.

**Architecture: hybrid, three-tier, mapped directly onto the network's existing comm-delay stratification** ([§6.1](#6.1) above's photonic/neuromorphic hardware; [Infrastructure §5](Infrastructure.md#5) for the underlying delay figures):

- **Nova Reach central data center** — the training tier. The "big" model lives here; this is the facility that becomes the Frozen Archive after collapse ([§5.2](#5.2) above).
- **Branch-system Safford stations** — receive updated model weights via the near-instant gate-to-gate fiber threading ([Cosmology §2](Cosmology.md#2)) and run local inference for the fast-coupled bodies orbiting alongside them (Boann, Olokun, Ereshkigal — all under ~35 sec comm delay from their Safford, [Infrastructure §5](Infrastructure.md#5)).
- **Slow-coupled surface colonies** (Lugh, Yemoja) — cannot lean on Safford's AI in real time any more than they can lean on Safford's human administrators across a 49-minute-plus one-way delay. Each runs its own local inference hardware on model weights that are current as of the last successful sync, meaning meaningfully staler than what a fast-coupled body sees, and progressively staler still as the interval since last contact grows.

This isn't a separate mechanic bolted onto the political independence arc — it's the same lag-driven autonomy already established for governance ([Politics](Politics.md)), expressed in a second system. Lugh and Yemoja were already operating on local human judgment before the collapse; local AI judgment, running on its own increasingly dated snapshot of the network's collective intelligence, was already part of that same independence, not a new consequence of severance.

**The fiber link itself is not permanent** ([Infrastructure §5](Infrastructure.md#5), fiber degradation) — meaning the "near-instant" weight-sync this architecture depends on is itself a slowly wasting asset post-collapse, compounding the branch stations' own hardware cannibalization ([§5.2](#5.2) above) with a second, independent failure mode in the pipe connecting them to Nova Reach at all.

<a name="7"></a>
# 7. Personal Augmented Reality: Retinal-Projection Glasses

*Like [§6](#6) above, this section describes Year 92 baseline technology — universal, unremarkable daily-life equipment across the network, lost outright at Severance with no reconstruction path ([§7.3](#7.3) below).*

<a name="7.1"></a>
## 7.1 Technology and Optical Limits

Standard Farfield-network eyewear projects imagery directly onto the wearer's retina via a miniaturized scanning laser or micro-LED emitter, steered by a solid-state micromirror element — evolutionary refinement of a real, already-demonstrated 21st-century display principle ([§6.1](#6.1) above's pattern: nothing here is invented physics, only 178 years of engineering maturity applied to it), not a new category of technology. The image reads as sharp regardless of what the eye's own lens is focused on, since there is no physical screen at a fixed distance for the eye to focus on or fail to focus on — a genuine advantage over any panel-based display, and one reason this technology, rather than a headset or contact lens, became the network's universal standard.

**Two competing form factors were tried and lost outright.** Nose-bridge- and cheek-mounted micro-projectors (cheaper, more rugged, roughly the social and economic niche a basic mobile handset occupied in the early 21st century) and full-coverage contact lenses (marketed as the invisible, prestige option) both saw real early-network adoption. Neither survived competition with glasses once glasses closed the remaining gaps: a contact lens has no room for a real battery, depends on continuous external wireless power transfer from a paired device, and cannot mount an independent light-control layer over its own optics; a bare nose-bridge or cheek unit, lacking a lens surface at all, has nowhere to put the darkening/polarizing layer described below and is consequently unusable outdoors or in bright work environments. Both niches collapsed once a single dominant, all-purpose form factor closed every gap at once — consistent with Farfield's institutional preference against funding parallel product lines where no functional gap remains to justify one ([Politics §3](Politics.md#3), cost efficiency). By Year 92, "AR glasses" and "eyewear" are functionally synonymous; nobody manufactures the alternatives.

**Additive projection only — no true occlusion or cancellation.** A scanning laser or micro-LED emitter can only add photons to the retina; it has no physical mechanism to subtract or cancel photons already arriving from the wearer's environment. Destructive-interference cancellation (the real physics behind active noise-cancelling headphones) does not generalize to ambient light: it requires a coherent source with a knowable, stable phase relationship, and ordinary light is an incoherent mixture radiated independently by billions of unrelated atoms, with no fixed phase to invert. A retinal projector therefore cannot, by itself, render true blackness or make a projected object look convincingly opaque against a bright background — it can only paint a translucent image on top of what's already there.

**Real occlusion comes from a second, separate mechanism: an electrochromic darkening/polarizing lens layer**, refinement of already-real photochromic and electronic-tint technology, mounted behind the projection optics. This layer physically attenuates incoming ambient light before it reaches the eye — the same principle as transition lenses or a welding helmet's auto-darkening filter, just faster-switching and capable of localized, patch-by-patch control in a mature Year-92 unit. Layered with the projector, this gives glasses (and only glasses — see above) the ability to dim a region of the visual field to near-black and then paint a bright, high-contrast image over it, producing a convincing illusion of a solid, opaque virtual object, or a full immersive blackout for wide-field-of-view work. This capability is the concrete physical reason glasses, rather than the two competing form factors, became and remained the network standard: reliable outdoor and bright-environment performance is a hard requirement for both routine work use and personal safety, and only a design with room for an independent optical attenuation layer can deliver it.

**Field of view, eye tracking, and power** are the ordinary remaining engineering constraints, all solved comfortably at glasses scale by Year 92 but worth noting as the reason smaller form factors never worked: wide-field-of-view projection needs a larger optical path than a contact lens can host; the system depends on continuous, low-latency eye and pupil tracking to paint imagery in the correct place at all (a system that loses tracking for even a moment misaligns or fails to render); and full-color, wide-view rendering at any real resolution draws meaningfully more power than a lens-scale battery or wireless-power link can sustainably provide.

<a name="7.2"></a>
## 7.2 Presence: Spatial Rendering and the Comm-Delay Gradient

**Spatial anchoring.** Outward-facing sensors continuously map the wearer's immediate environment in real time (the same underlying problem as real-world simultaneous-localization-and-mapping research), letting the system render a virtual person or object as though it physically occupies a specific point in the room — correctly sized, correctly lit, and correctly occluded by real intervening objects as the wearer moves. Farfield's neuromorphic accelerators and cross-domain AI ([§6.1](#6.1)/[§6.2](#6.2) above) are exactly the class of dedicated, low-latency hardware this requires: the sensing-mapping-rendering loop has to complete within a strict perceptual budget (real-world research places the threshold for perceptible, disorienting lag at roughly 20 milliseconds) or the illusion collapses into visible misalignment and induces motion sickness. By Year 92, this is judged reliable enough for routine use, including convincing dynamic occlusion (a virtual hand correctly passing behind or in front of the wearer's own), though genuinely fast or unexpected motion remains the one condition where an occasional, small rendering seam can still show through — a real, physics-grounded, rarely-noticed imperfection rather than a flawless system.

**This makes "presence calls" — a virtual conversation partner rendered as though standing in the room — the network's default mode of remote interpersonal contact**, and it interacts directly with the network's existing comm-delay architecture ([Infrastructure §5](Infrastructure.md#5)) rather than replacing it: the technology doesn't defeat the speed of light, it just makes the *experience* of talking to someone within a low-delay radius dramatically richer than a screen ever could, while making contact across a genuine light-lag distance feel stranger by comparison, precisely because it's realistic enough to invite the expectation of liveness it structurally cannot deliver.

- **Fast-coupled bodies** (Boann, Olokun, Ereshkigal — all under roughly 35 seconds one-way from their Safford, [Infrastructure §5](Infrastructure.md#5)) get something close to genuine live presence conversation.
- **Slow-coupled bodies** (Lugh, at ~49 minutes one-way; Yemoja, comparably distant) cannot sustain live presence at all — the light-lag exceeds the rendering system's perceptual budget by four to five orders of magnitude. What arrives instead is a beautifully rendered but fundamentally asynchronous message: a loved one's full spatial presence, gesturing and reacting exactly as they did, delivered as a recording of an event that finished unfolding the better part of an hour or more before the viewer sees it end.

**This gives Phase 1's post-Severance diplomatic envoys ([History §3](History.md#3)) new weight.** Sending a physical negotiator to Danu, Enlil, or Obatala, at real cost in transit time and fuel, is a deliberate rejection of the cheap option — anyone at Nova Reach could have rendered a presence delegate into local space in seconds. Choosing not to is itself the message: a demonstration of sincerity a presence call structurally cannot carry. The same logic sharpens the meaning of any physical blockade against that envoy: refusing to let a body land is a stronger, more legible act of rejection than refusing a call.

<a name="7.3"></a>
## 7.3 Post-Collapse: Manufacturing Loss and the Repair Trade

Like the rest of the network's finished electronics ([§2](#2) above), AR glasses were never manufactured locally — every unit at Year 92 was shipped through Sat-39 from Earth, and Severance ends new supply outright with no reconstruction path at any stage of the [§5.1](#5.1) timeline. Unlike infrastructure or industrial electronics, though, this is a loss felt personally and immediately by nearly every colonist at once: AR glasses are load-bearing daily-life equipment by Year 92 (routine work data, presence calls, wayfinding), not a specialized tool, so their disappearance registers as a universal, visible downgrade in ordinary life rather than an abstract industrial setback.

**A genuine repair-and-cannibalization trade emerges**, structurally identical to the pattern already established for the Frozen Archive ([§5.2](#5.2) above) and the fiber network ([Infrastructure §5.1](Infrastructure.md#5.1)) — a third independent instance of the same "no new supply, so surviving stock gets stripped, patched, and kept running past its intended life" logic. Repairing precision scanning optics and micromirror assemblies by hand, without the fabrication supply chain that originally built them, is skilled, scarce work — closer to a watchmaker's trade than an electrician's. Dead units are stripped for working micromirrors, lenses, and battery cells to keep others running. Device condition becomes a visible, face-worn marker of status: an intact, fully functional pre-collapse unit, a heavily repaired one with visible compromises, and going without at all sort colonists into a hierarchy anyone can read at a glance, in a way most other post-collapse scarcities aren't so immediately legible.

*Whether this repair economy remains a slowly dwindling, non-renewable resource indefinitely, or whether a cruder, bulkier indigenous replacement eventually becomes buildable once photolithography returns ([§5.1](#5.1), Years ~170–200), is not yet decided as canon — see [Open Questions](Open_Questions.md).*

<a name="7.4"></a>
## 7.4 The Archive: Surveillance and Its Social Function

Every unit in the network is Farfield-manufactured and Farfield-firmware, and it mediates a colonist's vision and hearing more continuously and intimately than any prior company-issued device — which makes the suspicion that Farfield is watching permanent and effectively unfalsifiable, whether or not any individual colonist can prove it. That suspicion happens to be entirely correct.

**Every feed is recorded and archived indefinitely.** By Year 92, storage costs are low enough ([§3](#3) above's battery-and-fabrication economics run parallel to a similar multi-decade maturation in storage density) that bulk, permanent retention of every user's feed is the cheaper and more cost-rational choice for Farfield than not collecting it — entirely consistent with the company's established amoral, cost-efficiency-first psychology ([Politics §3](Politics.md#3)) rather than any deliberate appetite for control. Lightweight automated triage scans incoming feeds for the narrow set of highest-severity flags — planning of violence or sabotage, chiefly anything touching gate or life-support safety — and otherwise simply files everything away, unreviewed, indefinitely. Nobody actively watches the ordinary feed of an ordinary colonist; it just never stops being kept.

**Farfield deliberately tolerates ordinary dissent.** Grumbling about leadership, informal union talk, routine criticism — none of it triggers review or consequence, and this is a considered choice, not oversight. A workforce permitted to vent stays stable and productive; a workforce that believes every complaint is monitored and punished becomes brittle and prone to real organized resistance instead. The archive is reserved entirely for the one category of behavior that threatens continuity of operations, not for managing everyday discontent — the same Purdue-style calculation already established elsewhere in Farfield's institutional behavior ([Infrastructure §3](Infrastructure.md#3), Boann subsection): concealing a capability rather than a harm, and using it only when the stakes justify it.

**This tolerance is what makes the surveillance invisible.** Colonists who get away with plenty take that as evidence Farfield surely isn't listening to everything — the very freedom to complain becomes the proof people cite against their own well-founded paranoia, keeping unease at a low, permanent background hum rather than a breaking point. Nothing is retrieved from the archive until a person becomes genuinely inconvenient to Farfield — a labor organizer gaining real traction, a leadership rival, someone the company needs leverage over during a contract dispute — at which point years of casual, unguarded footage become retroactively excavatable evidence. The archive is a weapon that almost never fires and could, in principle, fire on nearly anyone; nobody knows in advance whose it will be.

**A visible social ritual grows out of this.** Removing one's glasses, or handing them to someone else, before a conversation one doesn't want recorded is a legible, costly gesture — costly because AR-mediated function is load-bearing enough in daily life that going without it, even briefly, is a real, felt sacrifice, which is exactly what makes the gesture mean something. It is also visible to any bystander: two people both removing their glasses signals "this is private" to everyone nearby, independent of the conversation's content, functioning as a small act of mutual trust and mutual exposure at once. Reception of the gesture varies by the ideological strata already established at Safford ([Culture §2](Culture.md#2)): disillusioned idealists tend to treat it as hollow, since ambient station microphones could plausibly still catch a conversation regardless of what's on someone's face; pragmatists and administrators are more likely to treat it as a sufficient, good-faith norm. Whether the gesture persists as inherited cultural habit on independent, post-collapse Danu — where Farfield's specific hardware and monitoring apparatus are gone but the reflex may not be — is not yet decided as canon.
