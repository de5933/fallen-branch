# Technology

*Each file numbers its own sections independently starting at §1. Cross-references elsewhere in the bible take the form `[File §X.Y](File.md#X.Y)`, naming the target file before the section number.*

## Contents

- [1. Propulsion & Vehicle Engineering](#1)
  - [1.1 Fusion Torch Drive: Network Standard](#1.1)
  - [1.2 The Danu Vehicle Fleet](#1.2)
  - [1.3 The Enlil System Vehicle Fleet](#1.3)
- [2. Post-Collapse Electronics](#2)
  - [2.1 Material Sourcing and the Rare-Earth Wall](#2.1)
  - [2.2 Fabrication Tier](#2.2)
  - [2.3 Display Evolution](#2.3)
- [3. Energy Storage: The Battery Chemistry Ceiling](#3)
- [4. Arms and Equipment](#4)
- [5. Technological Reconstruction Timeline](#5)
  - [5.1 The Long Rebuild](#5.1)
  - [5.2 The Frozen Archive](#5.2)

<a name="1"></a>
# 1. Propulsion & Vehicle Engineering

<a name="1.1"></a>
## 1.1 Fusion Torch Drive: Network Standard

Farfield's standard in-system drive is a Trelium-fueled fusion torch, doped beyond a conservative baseline to a defensible "mid-range" spec: exhaust velocity of roughly 1,000–1,500 km/s. Ships fly an accelerate–coast–decelerate profile — high-thrust burns at departure and arrival bracketing a long ballistic coast — rather than a continuous-thrust torchship burn. This is deliberately a middle ground: far faster than a fuel-optimal Hohmann transfer, and far cheaper in propellant than sustained constant acceleration.

Standard mission budget: roughly 350–400 km/s total delta-v (split between departure and arrival burns), giving a propellant mass ratio around 1.3–1.4x at the stated exhaust velocities — i.e., only 25–30% of a ship's mass is propellant, comfortably realistic. See [Travel §1](Travel.md#1) for the resulting transit times per route.

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

Unchanged in kind from the network-standard drive ([§1.1](#1.1) above): makes the full Safford↔Lugh haul (5.85 AU, ~54–57 days one-way) at 350–400 km/s total ΔV, 25–30% propellant mass fraction — comfortable margin, no staging benefit. Reference sizing: ~5,000 t class vessel (~2,500 t cargo capacity), 5–6 vessel fleet covering Danu's ~22,500 t/yr export demand with margin for maintenance and wartime repurposing ([History §3.4](History.md#3.4)). Never enters atmosphere; operates exclusively between Safford and Lugh parking orbit, exchanging cargo with Lugh Spaceplanes via orbital rendezvous.

### ITV Artificial Gravity: Axial Spin-Gravity Architecture

At 54–57 days one-way, the Lugh-route ITV's coast phase is long enough for real zero-g deconditioning (bone/muscle loss) to matter — this crossing, and the longer Obatala-route Yemoja crossing once its transit time is recomputed ([Travel §1](Travel.md#1), Open Questions), are the network's only hauls that clear that bar. Short hops — Boann Shuttle (~35 hr), Safford OTO/Enlil variant (~32.6 hr, [§1.3](#1.3)) — stay well under a week, where zero-g exposure is real-world well-tolerated even by untrained civilians; no spin-gravity architecture is fitted to those hulls.

**Geometry: axial spin, spin axis = thrust axis.** The ITV is a rigid spine with the hab/cargo module on one arm and the reactor/drive/radiator module on the other, counterbalanced about a single gimbaled engine mounted at the hub — the center of rotation. This differs from a classic "tumbling pigeon" (spin axis perpendicular to the ship's length, engine off-axis) in one deliberate way: because the engine sits exactly on the spin axis, its thrust vector is unaffected by rotation. A burn along the ship's own axis — which is nearly the entire 350–400 km/s ΔV budget, since the accelerate-coast-decelerate profile ([§1.1](#1.1)) is two axial burns bracketing an unpowered coast — imparts no gyroscopic precession and needs no rotation-synced firing. Only fine, off-axis trajectory corrections require phased firing timed to the spin, a much smaller version of the problem a fully off-axis engine would have for every burn.

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
| Interplanetary Transfer Vessel | ITV | Lugh parking orbit ↔ Safford | Trelium fusion torch | Yes — 25–30% propellant fraction, comfortable margin | 350–400 km/s ΔV; ~5,000 t class; 5–6 vessel fleet; axial spin-gravity at 6 rpm, ~27 m spine (long-haul routes only, see above) |
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

The achievable fabrication ceiling is contact/proximity photolithography — micron-scale features, hand-aligned masks under UV light, no exotic optics — roughly comparable to 1960s–70s Earth chip technology in raw capability, though built with the colonists' full modern theoretical knowledge rather than rediscovered from ignorance. In practice this means low transistor density, clock speeds in the megahertz range, and real, felt latency on compute-heavy tasks — see [Culture §4](Culture.md#4) for the distributed, swarm-native software culture this constraint produced.

Basic wireless communication (radio, short-range data/voice links) is comfortably achievable at this tier, since it depends on antennas, oscillators, and amplifiers rather than dense logic or exotic RF front-end chips. High-bandwidth wireless data at modern speeds is not.

Reconstruction itself proceeds in stages, not as a single leap — see [§5.1](#5.1) below for the full Scramble → tubes → discrete transistors → indigenous ICs → maturation timeline (roughly Years 92 to 200+).

<a name="2.3"></a>
## 2.3 Display Evolution

Monochrome CRT is the universal baseline throughout reconstruction — glass, vacuum, and electron-gun engineering, none of it dependent on scarce dopants. Color follows a genuine, generations-long arc:

- **Field-sequential color** (a single monochrome tube behind a spinning red/green/blue filter wheel, synced to frame rate — the same principle used on the real Apollo lunar rover's color camera) is the earliest color technology available: mechanical, maintenance-heavy, and the first luxury/prestige display, reserved for administrators and critical control rooms in the same texture as Safford's stratified food service ([Infrastructure §2.2](Infrastructure.md#2.2)).
- **Three-phosphor color CRTs**, using pre-rare-earth phosphor chemistry (cadmium-based reds, zinc-sulfide-family greens and blues — the same chemistry real Earth color television used before the rare-earth generation of phosphors), spend decades in prototype and pilot-scale development before becoming reliable and cheap enough to displace field-sequential displays as the common standard.
- Throughout this entire period, data formats and protocols ([Culture §4](Culture.md#4)) preserve full color information losslessly even while displays remain monochrome or field-sequential — a deliberate act of institutional hope that color hardware will eventually be common again. The eventual arrival of cheap three-phosphor displays means old archives and images are finally seen in true color for the first time by anyone still alive to see them.

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

See [Open Questions](Open_Questions.md) for equipment details not yet locked as canon, including armor material specifics, adgun unit siting at Safford and each settlement, other non-lethal options under consideration (acoustic hailing/dispersal devices, riot foam, chemical irritants), and powered cargo exoskeletons as a possible visual for Danu's improvised resistance. See [History §3.4](History.md#3.4) for how this equipment played out tactically across the Nova Reach–Danu conflict.

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

See [§2](#2) above for the material and technical detail behind each stage, and [Culture §4](Culture.md#4) for the software culture this constraint produced.

<a name="5.2"></a>
## 5.2 The Frozen Archive

At collapse, Nova Reach's local LLM inference infrastructure — a Farfield corporate asset, hosted at Nova Reach for latency reasons rather than owned by the colony itself — is stranded with whatever model weights happened to be cached at Year 92, permanently unable to retrain or update. Farfield's ownership of everything in the colonies ([Politics §4.1](Politics.md#4.1)) makes its post-collapse status a matter of practical control rather than settled law: whoever can physically reach and maintain the hardware effectively owns it now, whatever the org chart used to say.

No single administration ever makes a clean decision to preserve or dismantle it. Instead, across Phases 1 through 3 and beyond ([History §3](History.md#3)), the data center is worn down by a slow, piecemeal cannibalization — a rack pulled here for a life-support board, a memory module scavenged there for a failing gate-control system, each individual decision a reasonable emergency triage call, never an official policy. What survives by the time indigenous chip fabrication matures ([§5.1](#5.1) above) is a degraded, patched wreck running on a fraction of its original hardware — not dead, not whole, kept alive mostly by whoever still has the swarm-control expertise ([Infrastructure §2.2](Infrastructure.md#2.2)) to run something that distributed and resource-starved at all.
