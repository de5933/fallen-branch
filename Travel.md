# Travel

*Each file numbers its own sections independently starting at §1. Cross-references elsewhere in the bible take the form `[File §X.Y](File.md#X.Y)`, naming the target file before the section number.*

## Contents

- [1. Propulsion & Interplanetary Transit](#1)
  - [1.1 Interplanetary transit times](#1.1)
  - [1.2 The Danu Vehicle Fleet](#1.2)
  - [1.3 War-Era Vehicle Architecture (Nova Reach–Danu conflict)](#1.3)
  - [1.4 The Enlil System Vehicle Fleet](#1.4)

<a name="1"></a>
# 1. Propulsion & Interplanetary Transit
 
Farfield's standard in-system drive is a Trelium-fueled fusion torch, doped beyond a conservative baseline to a defensible "mid-range" spec: exhaust velocity of roughly 1,000–1,500 km/s. Ships fly an accelerate–coast–decelerate profile — high-thrust burns at departure and arrival bracketing a long ballistic coast — rather than a continuous-thrust torchship burn. This is deliberately a middle ground: far faster than a fuel-optimal Hohmann transfer, and far cheaper in propellant than sustained constant acceleration.
 
Standard mission budget: roughly 350–400 km/s total delta-v (split between departure and arrival burns), giving a propellant mass ratio around 1.3–1.4x at the stated exhaust velocities — i.e., only 25–30% of a ship's mass is propellant, comfortably realistic.
 
<a name="1.1"></a>
## 1.1 Interplanetary transit times
 
| Route | Distance | Transit time (at std. drive spec) |
| --- | --- | --- |
| Yemoja ↔ Olokun (Obatala) | ~9.05–9.95 AU ([Cosmology §5](Cosmology.md#5)) | recompute pending — see Open Questions |
| Lugh ↔ Boann/Mannannán (Danu) | ~5.85 AU | under 2 months |
| Safford (Mannannán moon) → Lugh (Danu) | ~5.85 AU | ~1.7–1.9 months |
| Safford (Olokun moon) → Yemoja (Obatala) | ~9.05–9.95 AU (Safford co-orbits Olokun, [Cosmology §5.3](Cosmology.md#5.3)) | recompute pending — see Open Questions |
| Safford (rubble pile, ~0.05 AU) → Ereshkigal (Enlil) | ~0.035 AU | under 2 days |
 
*For reference, a fuel-optimal (Hohmann) transfer between Yemoja and Olokun trades a much lower delta-v cost for a multi-year transit time at their current ~9–10 AU separation — see Open Questions for the precise recomputation still pending. A continuous-thrust torchship covers the same distance in weeks but at a delta-v cost of hundreds to thousands of km/s. The accelerate-coast-decelerate profile above was chosen specifically to avoid both extremes.*

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

Real-world electric regional aircraft already achieve 200–400 km ranges on current battery technology; at 30%+ better energy economy, Lugh's terminator-line hops between settlements sit comfortably within that same envelope. No exotic future battery tech required.

### Lugh Spaceplane (AOTS / Farfield Skyreach) — hybrid electric/H2-LOX, single-stage reusable, TAV

Surface-to-orbit-and-back transport, handing off cargo to the Interplanetary Transfer Vessel (below) at Lugh parking orbit. A gliding lander ([Cosmology §4.1](Cosmology.md#4.1)) — the underlying physics checks out favorably:

- **Reentry.** Scale height (H = RT/(Mg) ≈ 8.25 km at a representative 300 K terminator temperature) comes out almost identical to Earth's ~8.4 km, but column mass (P/g ≈ 26,200 kg/m²) runs **2.5× Earth's** — meaning more atmosphere to shed velocity into per unit of descent. Orbital velocity to dissipate is 6.53 km/s, versus Earth's 7.9 km/s. Net result: a *gentler* reentry environment than Earth's own Space Shuttle faced, confirming the lifting-body glide entry as the right approach for this vehicle.
- **Ascent — hybrid propulsion.** Ambient CO2 (fully-oxidized carbon) rules out an Earth-style air-breathing jet, but supports no such limitation on an electric ducted-fan/propeller stage: thrust from a propeller comes from momentum imparted to ambient gas, chemistry-agnostic. The spaceplane's low-speed, low-altitude climb — the segment where gravity losses are worst and a rocket is least efficient — runs on the same electric propulsion family as the Surface Aircraft, drawing thrust from the thick lower atmosphere for free. Once airspeed and altitude exceed what the fan can efficiently push against, the vehicle stages (functionally, not physically — same airframe, switched propulsion mode) to H2/LOX rocket for the high-speed climb and vacuum insertion.
- **Rocket-only ΔV budget:** orbital velocity (6.53 km/s) plus the remaining gravity/drag losses the rocket phase alone incurs, estimated at **~6.8 km/s** total after the electric-assist offload. At H2/LOX Isp ≈ 450s (ve ≈ 4,413 m/s): mass ratio e^(6800/4413) ≈ 4.67, or **~79% propellant fraction**.
- **Verdict:** single-stage, but a genuine engineering achievement rather than a comfortable margin — meaningfully below Earth SSTO concepts' ~90%+ propellant-fraction wall (which sank real designs like X-33 and Skylon), thanks to Lugh's lower g, lower total ΔV, and gentler reentry all pulling the same direction. A ~20% dry-mass fraction (tanks, structure, TPS, electric and rocket propulsion) is demanding but achievable — worth treating in-universe as a source of real engineering pride, a fully reusable spaceplane architecture Earth aerospace never quite closed the numbers on.

### Interplanetary Transfer Vessel (ITV) — Trelium fusion torch

Unchanged in kind from the network-standard drive ([§1](#1) above): makes the full Safford↔Lugh haul (5.85 AU, ~54–57 days one-way) at 350–400 km/s total ΔV, 25–30% propellant mass fraction — comfortable margin, no staging benefit. Reference sizing: ~5,000 t class vessel (~2,500 t cargo capacity), 5–6 vessel fleet covering Danu's ~22,500 t/yr export demand with margin for maintenance and wartime repurposing ([§1.3](#1.3)). Never enters atmosphere; operates exclusively between Safford and Lugh parking orbit, exchanging cargo with Lugh Spaceplanes via orbital rendezvous.

### ITV Artificial Gravity: Axial Spin-Gravity Architecture

At 54–57 days one-way, the Lugh-route ITV's coast phase is long enough for real zero-g deconditioning (bone/muscle loss) to matter — this crossing, and the longer Obatala-route Yemoja crossing once its transit time is recomputed ([§1.1](#1.1), Open Questions), are the network's only hauls that clear that bar. Short hops — Boann Shuttle (~35 hr), Safford OTO/Enlil variant (~32.6 hr, [§1.4](#1.4)) — stay well under a week, where zero-g exposure is real-world well-tolerated even by untrained civilians; no spin-gravity architecture is fitted to those hulls.

**Geometry: axial spin, spin axis = thrust axis.** The ITV is a rigid spine with the hab/cargo module on one arm and the reactor/drive/radiator module on the other, counterbalanced about a single gimbaled engine mounted at the hub — the center of rotation. This differs from a classic "tumbling pigeon" (spin axis perpendicular to the ship's length, engine off-axis) in one deliberate way: because the engine sits exactly on the spin axis, its thrust vector is unaffected by rotation. A burn along the ship's own axis — which is nearly the entire 350–400 km/s ΔV budget, since the accelerate-coast-decelerate profile ([§1](#1)) is two axial burns bracketing an unpowered coast — imparts no gyroscopic precession and needs no rotation-synced firing. Only fine, off-axis trajectory corrections require phased firing timed to the spin, a much smaller version of the problem a fully off-axis engine would have for every burn.

**Spin-up and spin-down: paired tangential RCS, no flywheel.** The ship spins up once after undocking and spins down once before docking, using tangential RCS thrusters mounted at both the hab end and the reactor end, fired as a torque couple (equal and opposite, same rotational sense) so the maneuver imparts no net translation. A compact flywheel was considered and rejected on the same physical grounds [Infrastructure §2.1](Infrastructure.md#2.1) already used to reject one for the Nova Reach habitat ring: canceling a rotating structure's angular momentum with a small on-axis wheel demands a rim speed that scales explosively as the structure's own radius shrinks (radius ∝ 1/ω² to hold gravity fixed, so the ship's angular momentum scales as roughly 1/ω³) — workable only in the 7.5–10 rpm range this design deliberately avoids for comfort reasons (below), and requiring an implausibly massive or fast wheel at any gentler spin rate. RCS avoids this because its lever arm is the ship's own long spine, not a compact hub wheel — the mechanism the flywheel needed to make small, RCS gets to keep large.

**Spin rate: 6 rpm — locked.** Selected as the fastest rate the source research still class as passenger-tolerable-with-adaptation rather than crew-only: multi-day adaptation required, some susceptible individuals will have real difficulty, but it is not disqualifying for ordinary colonists and administrators making the crossing, unlike the 7.5–10 rpm band above it.

Reference geometry and cost, using the ITV's established ~5,000 t class sizing (hab/cargo arm 2,700 t, reactor/drive/radiators/propellant arm 2,300 t — this split is a working assumption, not yet locked; see Open Questions):

| Figure | Value |
|---|---|
| Hab arm radius | 12.4 m |
| Reactor arm radius | 14.6 m |
| Total spine length | 27.0 m |
| Angular momentum at 6 rpm | 5.69×10⁸ kg·m²/s |
| Propellant per spin event (storable, ~3,000 m/s ve) | ~14.1 t |
| Propellant per spin event (H2/LOX, ~4,400 m/s ve) | ~9.6 t |
| Propellant per one-way crossing (spin-up + spin-down) | ~28.1 t (storable) / ~19.2 t (H2/LOX) |
| As fraction of total ship mass | ~0.56% — trivial against the 25–30% transit propellant budget |

**The mid-coast turnover.** The accelerate-coast-decelerate profile needs thrust flipped from prograde (departure) to retrograde (arrival) once per crossing. Rather than a mechanical turret swinging the hub engine through 180° — a new class of heavy moving hardware — this is executed as a slow RCS-driven precession of the spin axis itself, walking the ship's whole orientation around during the idle coast, with no time pressure and no despin required. This keeps the added complexity in guidance software rather than machinery, consistent with the same instinct already governing this design's spin-up/down choice.

**Structural note, flagged rather than solved.** The spine arms are under continuous centrifugal tension from the hab and reactor masses at their tips — a real whirl/resonance safety margin against the ship's natural bending frequency needs checking once arm material and cross-section are chosen (Open Questions), though centrifugal tension itself measurably stiffens a rotating beam against transverse flexing (the same effect analyzed in helicopter rotor design), which works in this design's favor rather than against it. Separately, this geometry sits at the ship's own major moment-of-inertia axis by construction — the dissipation-stable configuration for a real rotating body with any internal damping (energy loss from flex, slosh, etc. drives rotation toward the largest-moment axis over time) — the opposite of Explorer 1's 1958 tumble, which resulted from spinning about its smallest-moment axis. This is a genuine point in the design's favor, not just a neutral fact.

### Boann Shuttle (Farfield PDV-1) — single-stage H2/LOX, full surface-to-Safford route

Boann's situation is qualitatively different from Lugh's, and the vehicle architecture follows suit rather than mirroring it. Safford Danu sits co-orbital with Boann around Mannannán (<7 sec comm delay, [Infrastructure §5](Infrastructure.md#5)) — a short moon-to-moon hop, not an interplanetary transfer. Using Io/Europa-analog orbital radii (Boann ~421,700 km, Safford's moon ~671,100 km from Mannannán) and standard Hohmann-transfer math: **~3.2 km/s total ΔV, ~35 hour transit.**

Boann's own gravity well barely matters against that transfer cost: escape velocity is only 464 m/s (from 0.02g, [Cosmology §4.3](Cosmology.md#4.3)), versus the interorbital transfer's ~3.16 km/s — local escape is only ~15% of the mission total, the inverse of Lugh's situation, where local escape dominates. This makes splitting Boann's route into a lander-plus-tug pair pure overhead: there's no altitude regime around Boann deep enough for staging to buy anything (a 50 km parking orbit's circular velocity, ~314 m/s, is barely below surface orbital velocity itself, ~328 m/s). **A single Boann Shuttle flies the entire route, surface to Safford dock — no separate orbit-to-orbit vessel** ([§1.3](#1.3)).

Combining Boann's escape burn with transfer injection via the Oberth effect (most efficient deep in the well): launch ΔV ≈ √(464² + 1,676²) ≈ 1,740 m/s; arrival/circularization burn ≈ 1,488 m/s; **total ≈ 3,230 m/s.** At H2/LOX Isp ≈ 450s: mass ratio e^(3230/4413) ≈ 1.98, or **~49% propellant fraction** — an entirely ordinary single-stage budget.

**Launch and landing character.** No atmosphere means pure propulsive flight door to door — closer to a small-body landing (Philae, Hayabusa-style) than a planetary descent. With escape velocity this low, there's essentially no passive stability to lean on; the vehicle flies itself down under continuous active control the entire way, at approach speeds plausibly in the cm/s-to-low-m/s range near touchdown, since overshoot is trivial to induce and expensive in control authority (not fuel) to correct. The real hazard is plume-kicked debris: with escape velocity so low, exhaust interaction with loose ice or regolith near the pad can fling material at a meaningful fraction of escape velocity — the physical justification for the pad already being blast-diverted ([§1.2](#1.2), [§1.3](#1.3)) rather than open. Post-landing, the vehicle is grapple-anchored immediately on touchdown; 0.02g provides essentially no restraint against thermal creep or accidental bumps, so an unattached vehicle on the pad is closer to a docked spacecraft than a parked aircraft.

### Summary

| Vehicle | Designator | Route | Propulsion | Single-stage? | Key figures |
|---|---|---|---|---|---|
| Lugh Surface Aircraft | Farfield A-6 | Terminator city ↔ satellite settlements | Electric only | N/A (no staging) | ~30% lower energy/km than Earth-equivalent; ~3.7× payload/wing-area at matched speed |
| Lugh Spaceplane | AOTS / Farfield Skyreach (TAV) | Lugh surface ↔ Lugh parking orbit | Electric (low-speed climb) + H2/LOX (high-speed climb, vacuum insertion, reentry reserve) | Yes — ~79% propellant fraction, ~20% dry-mass target | Reentry: 2.5× Earth column mass, same scale height, 6.53 km/s to shed |
| Interplanetary Transfer Vessel | ITV | Lugh parking orbit ↔ Safford | Trelium fusion torch | Yes — 25–30% propellant fraction, comfortable margin | 350–400 km/s ΔV; ~5,000 t class; 5–6 vessel fleet; axial spin-gravity at 6 rpm, ~27 m spine (long-haul routes only, see below) |
| Boann Shuttle | Farfield PDV-1 | Boann surface ↔ Safford (direct, no parking-orbit handoff) | H2/LOX | Yes — ~49% propellant fraction | ~3.23 km/s total ΔV; ~35 hr transit; escape velocity only 464 m/s |

<a name="1.3"></a>
## 1.3 War-Era Vehicle Architecture (Nova Reach–Danu conflict, [History §3](History.md#3))

Consistent with [Infrastructure §1](Infrastructure.md#1)'s hard ceiling — no hull ever transits a gate, and nothing built in one system can fly to another — Farfield's interplanetary cargo (and, during the war, troop) logistics draw directly on the vehicle fleet above ([§1.2](#1.2)), not a separate wartime design:

- **Lugh front — split architecture.** The Interplanetary Transfer Vessel makes the long accelerate-coast-decelerate haul between Safford and Lugh parking orbit and never enters atmosphere; the Lugh Spaceplane ([§1.2](#1.2)) shuttles cargo and, during the war, troops between Lugh's surface and that parking orbit, handing off via orbital rendezvous. This split gives every Lugh incursion an unavoidable, highly visible orbital loiter phase — the transfer vessel sits exposed in parking orbit while its spaceplane is down on the surface — a predictable rhythm Danu's defenders can plan incursion response around.
- **Boann front — single-vessel architecture, no loiter phase.** The Boann Shuttle flies the complete route, surface to Safford dock, with no intermediate parking-orbit vessel at all ([§1.2](#1.2)) — Boann's shallow gravity well and short co-orbital hop to Safford make a lander/tug split pure overhead rather than an efficiency gain. Tactically, this means Nova Reach incursions against Boann lack the exposed loiter window that defines the Lugh front: no transfer vessel sits waiting in orbit for defenders to target or time a response around. Whether this makes a Boann incursion harder to detect coming, or simply removes one specific vulnerability while leaving others (the shuttle's own slow, unavoidable final approach, [§1.2](#1.2)) intact, is worth developing further if Boann ever gets its own dedicated incursion scene.

### Lugh: landing infrastructure

Built for high cargo throughput rather than defense: open ground, likely multiple pads/runway capacity, positioned near processing and storage facilities so harvested crops can move quickly from field to orbit. Tactically exposed — clean, unobstructed sightlines for defenders on slightly elevated ground or nearby structures, with nowhere for a landing party to take cover once down. A gliding shuttle-style landing (if confirmed) implies an actual runway with real approach/rollout margin, a larger and harder-to-seal target than a compact pad, but one that also exposes an inbound vehicle during a fast, low, hard-to-evade rollout.

### Boann: landing infrastructure

Boann has no coastlines and no open ocean — its surface is ice sheet throughout, and its "dry land" is the network of paved surface facilities built atop that ice near the borehole settlement ([Cosmology §4.3](Cosmology.md#4.3)). A propulsive hydrogen-oxygen landing here requires an engineered, heat-resistant, blast-diverted pad built directly into the reinforced ice/paved surface, since an unprepared site risks uncontrolled melt-through or cracking under landing-plume thermal and pressure loading. This gives Boann a small number of fixed, known, heavily fortified landing points rather than Lugh's more open, distributed exposure — defenders don't need to cover a whole region, just deny the handful of points that are the only physical way in.

### War mechanics: no ship-to-ship combat

Neither side possesses anything resembling a warship. Nova Reach's forces are a company security apparatus ([People §1](People.md#1), Castellane) improvising combat capability onto vehicles and personnel built for policing, not war; Danu has no space-based force at all. Orbital closing speeds are far too high for conventional projectile weapons to be effective at any range beyond point-blank/boarding distance, so there is no meaningful space combat in this conflict — a mounted gun is, at best, an improvised close-range boarding or intimidation weapon, not a warship's armament. **Safford itself is never attacked by anyone**: as the sole gate infrastructure connecting all four systems, an attack on it would unite every faction, Danu included, against the attacker, since Danu needs the gates as much as Nova Reach does.

The war is therefore fought entirely as a **ground/landing-zone conflict**, structurally similar to an opposed amphibious landing with no landing-craft doctrine on the attacker's side: Castellane's forces arrive via slow, unarmed transports with an unavoidable, visible final descent, and Danu's defenders don't need ships or orbital assets at all — they only need to make the small number of physical landing points (above) lethal with prepared fields of fire and repurposed equipment.

<a name="1.4"></a>
## 1.4 The Enlil System Vehicle Fleet

Ereshkigal has no atmosphere — locked canon, and a real physical consequence rather than a convenient assumption: the same red-giant expansion and subsequent intense post-formation UV/X-ray flux from Enlil A's exposed core ([Cosmology §6.1](Cosmology.md#6.1)) that shredded and polluted the original planets would already have stripped or photoionized away anything Ereshkigal might once have held. This shapes every part of the system below: no gliding entry anywhere in this system, unlike Lugh — everything is fully propulsive.

**Naming convention**, following [§1.2](#1.2)'s precedent: dry Farfield designators, kept as bare acronyms in most cases rather than given colloquial names — the exception being the cargo pod, where real mass-driver engineering terminology (dating to Gerard O'Neill's original 1970s concept) already supplies an authentic, unpretentious term:

| Vehicle | Official designator | Common usage |
|---|---|---|
| Crew launcher | Farfield PDV-2 | "PDV-2" (same lineage as Boann's Farfield PDV-1, [§1.2](#1.2) — both fully propulsive, airless-world shuttles) |
| Cargo vehicle (mass driver) | Farfield MD-C (Mass Driver – Cargo) | "a bucket" |
| Tank vehicle (mass driver → depot) | Farfield MD-T (Mass Driver – Tank) | "MD-T" |
| Orbital transfer vessel (Enlil variant) | ITV | "Safford OTO" |

### The Safford–Ereshkigal hop is deceptively expensive

Physical separation between Safford Enlil and Ereshkigal is the shortest branch-station pairing in the network (~0.035 AU) — naively this looks like Boann's cheap short hop. It isn't, because both bodies orbit deep in a white dwarf's gravity well. Enlil A packs 0.62 M☉ into an Earth-sized sphere; circular orbital velocity (√(GM/r)) at Ereshkigal's 0.015 AU works out to **191.5 km/s**, and at Safford's 0.05 AU to **104.9 km/s** — the same physics that gives real Mercury (0.39 AU from the Sun) its 47.9 km/s orbital speed, taken further. A Hohmann transfer between the two costs **~79.7 km/s total ΔV**, with a transit time of **~32.6 hours (1.4 days)** — consistent with, and a good validation of, the bible's existing "under 2 days" figure ([§1.1](#1.1)).

That ΔV is an order of magnitude beyond any chemical shuttle, so **this route runs on a leaner ITV variant** (trelium fusion torch, same class as Danu's, scaled down), not a small local craft. Because 79.7 km/s is well under the network-standard 350–400 km/s budget, the propellant fraction is trivial (~6% at mid-range exhaust velocity) — a fast, lean hull built for a short, violent hop deep in a well, rather than the long-haul Lugh-route configuration.

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
 
