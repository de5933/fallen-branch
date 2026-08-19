# Cosmology

*Each file numbers its own sections independently starting at §1. Cross-references elsewhere in the bible take the form `[File §X.Y](File.md#X.Y)`, naming the target file before the section number.*

<a name="1"></a>
# 1. Setting-Wide Principles

<a name="1.1"></a>
## 1.1 No Native Extraterrestrial Life — Locked Principle

None of the four systems' worlds — settled, uninhabited, or merely catalogued — harbor native extraterrestrial life of any kind, biological or otherwise. This holds across the entire setting, for every world discussed anywhere in the bible, past, present, and future. Any apparent hook toward alien biology (e.g. Boann's hydrothermal vent chemistry, [Infrastructure §3](Infrastructure.md#3)) should be read as purely abiotic geochemistry — real mineral/hydrothermal processes that happen to resemble the conditions life exploits on Earth, not evidence of, or groundwork for, actual organisms. This is a deliberate genre choice: the story's stakes stay grounded in physics, engineering, corporate politics, and human survival, not first-contact or astrobiology, and it should be treated as a standing constraint to check future worldbuilding against rather than a one-off note.

<a name="1.2"></a>
## 1.2 Host Galaxies

Each of the four systems sits in its own separate galaxy, not merely a distant star within one shared galaxy. This is a deliberate extension of [§2](#2)'s core premise — a harvested wormhole seed's far end can be anywhere, "possibly at effectively unreachable distance or even in a different universe" — taken to its logical conclusion. It also sharpens the severance stakes considerably: even before Sat-39 collapses, nothing about this network was ever reachable by conventional means. Danu, Obatala, and Enlil aren't just interstellar distances from Sol — they're tens of millions of light-years away, in different galaxies entirely, meaning even a light-speed radio signal between any two of these systems would take millions of years. The wormhole network was always the only connection of any kind between these places. Severance doesn't strand the branch systems further from Earth; it removes the one and only thread that ever tied any of this together.

| System | Host galaxy | Hubble type | Distance from Sol |
| --- | --- | --- | --- |
| Nova Reach | Nova Reach Galaxy | E3 (giant elliptical) | ~1.2 Mpc (~100 Mly) |
| Danu | Danu Galaxy | SBb (barred spiral) | ~1.3 Mpc (~103 Mly) |
| Obatala | Obatala Galaxy | Sc (spiral) | ~1.3 Mpc (~108 Mly) |
| Enlil | Enlil Galaxy | S0 (lenticular) | ~1.4 Mpc (~114 Mly) |

*Nova Reach Galaxy's type is load-bearing, not decorative: an ancient, low-metallicity giant elliptical is exactly the stellar population that produces a K-dwarf primary rather than a younger, metal-rich star ([§3](#3)), and gives Goibniu's helium enrichment ([§3.1](#3.1)) a genuine astrophysical basis rather than an arbitrary flourish. The other three galaxy types were chosen for visual/tonal variety across the branch systems rather than to satisfy a specific narrative requirement — Enlil Galaxy's lenticular (S0) classification was picked to echo that system's own "dead system" character (an aging, largely quiescent galaxy type), but this is a stylistic pairing, not a physical necessity, and any of the four types can be swapped freely if the story ever needs it.*

<a name="2"></a>
# 2. Wormhole Physics

Grounded in real theoretical physics: fermionic wormhole theory (Blazquez-Salcedo, Knoll, and Radu — B-SKR — as popularized by John G. Cramer, Analog AV-216).

- Primordial wormhole seeds are tiny, extremely massive, electrically charged particle-like objects left over from the Big Bang. Each seed is already a two-mouth object — the far end already exists somewhere, possibly at effectively unreachable distance or even in a different universe. It has simply never been opened.
- Seeds behave gravitationally and electromagnetically like charged dust, so over cosmic timescales they migrate into resonance bands within planetary ring systems — the same mechanism that concentrates ordinary ring particles.
- Engineers "inflate" a seed by pumping fermions and electric flux through it, growing the throat. Inflation is staged by cost and risk (see [§2.2](#2.2)).
- Gates are inherently unstable and need constant precise tuning: the structure is an artificially inflated quantum object fighting its natural tendency to collapse back to a sub-atomic particle.
- **Transit permanently shifts mass, it does not just perturb it.** Per standard wormhole conservation-law treatment (Visser), a wormhole's mass, charge, and momentum are conserved locally at each mouth: matter entering one mouth adds its mass to that mouth's reading, and matter exiting the far mouth subtracts it from that mouth's reading — permanently, not as a transient blip that resolves once the object clears. An uncorrected one-way flow between two mouths therefore causes the two ends of the same wormhole to drift apart in mass, without limit, for as long as the imbalance goes uncorrected. This is why passenger/cargo transit ([Infrastructure §1](Infrastructure.md#1)) is built around simultaneous, mass-matched crossings rather than one-way trips: a perfectly matched pair crossing in opposite directions cancels this drift exactly, at both mouths, regardless of how much mass either train carries.
- **A stray seed stops almost instantly on contact with matter — it does not sink.** A seed's throat radius (a few hundred Planck lengths) is so far below a nucleus's size that it has essentially no mechanical cross-section; classical drag/settling (Stokes-law sinking) does not apply. What stops it instead is its own charge (~330 elementary charges): electromagnetic stopping power scales with charge squared, so a seed loses momentum to any matter it passes near — solid, liquid, gas, ionized or not — within a sub-micron-to-micron distance, the same physics that stops an alpha particle in a short path through shielding. A seed that arrives before or during a body's molten/differentiating phase gets carried toward the core as that body settles; a seed that arrives after a body has already solidified (e.g. via a later meteorite impact) simply stops in place near the surface, under whatever gravity that body has — not buried, but not usable either if that gravity isn't negligible ([§2.4](#2.4)). A seed embedded in a ring particle or small asteroid, which never differentiates at all, stays exactly where it landed, permanently accessible.
- **Genuinely extreme plasma can destroy a raw seed outright.** Ordinary charge-stripping is glacially slow and never seriously threatens a seed's Qe/M margin, but stellar cores, supernova remnants, and magnetar magnetospheres are violent and dense enough to drive that same charge-exchange process fast enough to matter, or to perturb the threading field directly. Because a raw seed's mass is milligram-scale, its evaporation time on failure ([§2.6](#2.6)) is on the order of 10⁻³⁴ seconds — instantaneous and silent, with no observable signature. This is a real, ongoing loss channel thinning the surviving primordial seed population over cosmic time, invisibly, with no bearing on anything in the story's timeline.
- **B-SKR's result is also a real answer to Weak Cosmic Censorship.** The classical over-charged-black-hole case (Qe > M) is usually treated as producing a naked singularity — a violation of Penrose's censorship conjecture. B-SKR's solutions are continuous with extremal Reissner-Nordström black holes, so in this setting, censorship holds: nature's answer to over-charging a compact object isn't a naked singularity, it's a wormhole.
- Communication between gate ends is effectively near-instant via fiber-optic threading of the wormhole; only in-system distances incur light-speed delay (see [Infrastructure §5](Infrastructure.md#5) for in-system comm delay figures).
*Source: https://www.npl.washington.edu/AV/altvw216.html*

<a name="2.1"></a>
## 2.1 Manufactured Wormholes: A Theoretical Frontier

B-SKR's framework is treated as a confirmed, valid solution to the Einstein-Dirac-Maxwell equations in this setting — not merely an untested proposal. That has a direct consequence beyond primordial seeds: any process capable of pushing a compact charged object's charge past its own mass (Qe > M) should, in principle, produce the same stable throat as a primordial seed. A wormhole mouth could, someday, be *made* rather than found.

- Every wormhole Farfield has ever used is primordial — a relic seed harvested, never created. Staged inflation ([§2.2](#2.2)) only ever widens a throat that already exists; it does nothing to explain how one would push an ordinary charged mass past its own extremal limit from scratch. Manufacturing a mouth from nothing is a genuinely different, much harder problem.
- This capability remains firmly theoretical through Year 92 and for a long time after. It is multiple fundamental breakthroughs away from anything Sat-48-era engineering can reach — sequel/epilogue-horizon technology, not something available to any character in this story's timeline.
- The stakes are worth remembering even though the technology stays off-page: a working manufacturing process would sever the network's entire economic logic ([Economy §1](Economy.md#1)–10.5) from its fixed, cosmologically-determined seed supply. New gates on demand, anywhere, would be a civilization-scale rupture, not an incremental gain — which is exactly why it is held in reserve rather than casually solved.
### The day it finally works: Chronology Protection stops being a hypothesis

- Every gate in the existing network is fixed and non-rotating at both mouths by hard engineering necessity ([Infrastructure §2.1](Infrastructure.md#2.1)) — nobody has ever had independent control over one mouth's velocity or gravitational depth relative to its twin. That constraint was built for structural reasons, not to prevent time travel, but it quietly does that job for the entire span of this story.
- A manufactured *pair* — both mouths built locally, under a team's direct control — removes that accidental safeguard for the first time in the network's history. The first thing anyone tries, deliberately or by careless curiosity, is exactly the configuration that starts to open a closed timelike curve: give one mouth a different velocity or a different gravitational potential than the other, and let their proper-time histories diverge.
- Nature's answer arrives before the geometry ever gets there. As the mouths' histories approach the point where causality violation would become possible, vacuum fluctuations circulating through the throat run away and destroy it — the same terminal mouth-to-black-hole collapse already described in [§2.6](#2.6), this time triggered by the experiment itself rather than an external failure. Hawking's Chronology Protection Conjecture, confirmed the hard way, likely at serious cost: a destroyed lab, a dead research team, a career-ending catastrophe.
- From that moment on, it is not a conjecture anymore. "You cannot build a time machine, and here is the wreckage that proves it" becomes plain fact to anyone in the field — the first and last time anyone ever seriously tries.
*This section is forward-looking lore, well beyond the story's timeline. It is on record for setting consistency, not intended to be dramatized on-page in the current novel.*

<a name="2.2"></a>
## 2.2 Discovery Method: Staged Inflation, Not Surveying

Destination systems cannot be surveyed or targeted in advance — they may be at effectively unreachable distance, or in another universe entirely. "Discovery" is blind: a corporation inflates a harvested seed just enough to see what happens to be on the other side, then decides whether to invest further. This produces a three-stage funnel:

- **Stage 1 — Peek.** Minimal inflation, just enough throat area to pass gamma-ray wavelengths. Cheap, done at scale across many harvested seeds. Yields coarse imaging/spectroscopy of the far side (star type, presence of planets/rings, atmospheric hints).
- **Stage 2 — Characterize.** For promising peeks, further partial inflation for better resolution — enough data for an informed colonization go/no-go call, still short of cargo/personnel scale.
- **Stage 3 — Full expansion.** Reserved for confirmed winners. The expensive, committed step: inflating the throat to the network's 2.5 m passenger/cargo standard ([Infrastructure §1](Infrastructure.md#1)) — sized for the counterweighted twin-train transit system, never for a ship's hull. The true point of no return, where the corporation is on the hook for full colony logistics.
Most seeds are discarded after Stage 1 (empty space, dead systems, hazardous environments). Only a fraction reach Stage 2, and fewer still reach Stage 3.

<a name="2.3"></a>
## 2.3 How Inflation Actually Works

"Inflating" a seed is not stretching one fixed object — since the fermion pair *is* the wormhole ([§2](#2)), there's nothing to deform. It's coherently adding more entangled fermion pairs plus matched threading flux, climbing a family of successively larger, heavier B-SKR solutions rather than expanding a single one. This is closer to how nuclear fusion builds heavier nuclides one nucleon at a time than to inflating a balloon: each stage is a genuinely different bound state, all recognizably part of one continuous family.

Because the throat has essentially no mechanical cross-section ([§2](#2)), engineers can't aim matter into it the way you'd load a target. Instead, a precisely phase-matched fermion stream is fired at the seed, and the real question is whether it couples coherently into the existing entangled state (successful inflation) or simply scatters off as waste heat (failed coupling) — closer to stimulated emission in a laser than to marksmanship. This is exactly what the threading-field response wormhole engineers test for ([Culture §3](Culture.md#3)): whether a given seed's state is currently receptive to coherent addition.

Because throat area — and therefore the flux/fermion input required — scales explosively with radius (roughly the square, so getting from a seed's ~10⁻³² m throat to the network's 2.5 m standard is on the order of 60+ orders of magnitude in required charge), Stage 3 isn't a linear cost step up from Stage 2, it's a categorically different cost tier. This is the real reason Stage 3 functions as the funnel's one true point of no return rather than a gradual ramp.

<a name="2.4"></a>
## 2.4 The Usability Calculation: Near Mouth vs. Far Mouth

Whether a given seed is ever usable splits into two separate questions with very different answers — one Farfield controls by choice of harvesting site, one it doesn't control at all.

**Near mouth — the one Farfield chooses where to harvest: ~100% usable.** Real planetary-science thresholds put differentiation onset around 100–200 km body radius, while ring particles and rubble-pile moonlets top out in the tens-to-hundreds-of-meters range — three to four orders of magnitude too small, ever, to have melted and sorted a core. A seed harvested from ring or small-asteroid material ([Economy §1](Economy.md#1)) is essentially guaranteed to still be sitting exactly where it landed, fully accessible, never buried by differentiation. This is why ring/asteroid siting ([Infrastructure §2.1](Infrastructure.md#2.1)) is doubly justified: it's the only class of host that guarantees a usable near mouth *and* it happens to supply free ballast ([Infrastructure §1](Infrastructure.md#1)).

**Far mouth — wherever that end of the primordial pair happens to be, entirely uncontrolled.** This is the real bottleneck, and it's estimable as a chain of independent odds:

| Step | Estimated probability | Basis |
| --- | --- | --- |
| Far mouth is in a galaxy at all | ~10% | Baryon-census work consistently finds the large majority of the universe's ordinary matter sits in the diffuse intergalactic/circumgalactic medium, never collapsed into a galaxy |
| ...is in planetary solid material, not the star itself or interstellar gas | ~0.11% | Within a galaxy, ~85% of baryonic mass is locked in stars; of a star system's own mass, planetary solid material is only ~0.13% (Solar System calibration: ~447 Earth masses of planets against the Sun's ~333,000 Earth masses) |
| ...is in a small, undifferentiated body rather than a planet or moon | ~3–5% | Asteroid-belt/Kuiper-belt/comet-class material is a small fraction of a system's total solid mass against its planets and major moons |

Chained together: 0.10 × 0.0011 × 0.04 ≈ 5×10⁻⁶ — call it, very roughly, **1-in-100,000 to 1-in-a-million**. Every other outcome is a total loss: swallowed by a star, buried in a differentiated planetary interior, adrift in interstellar or intergalactic space with nothing to ever anchor a station to, or (per [§2](#2)'s "possibly a different universe") not in reachable spacetime at all.

**Combined odds a single seed is ever fully usable end to end:** since the near mouth is deliberately engineered to ~100% by choice of harvesting site, the far mouth's ~1-in-100,000-to-a-million figure sets the overall odds almost entirely on its own. This is the quantitative backbone under "most seeds are discarded after Stage 1" ([§2.2](#2.2)): Stage 1 exists specifically because this number is so brutal that a dedicated, cheap peek-and-discard step is the only economical way to find the rare hits, rather than gambling everything on Stage 3 directly.

<a name="2.5"></a>
## 2.5 The Severance Event

The triggering cause originates specifically on the Sol side (Sat-39 Sol). Cause unknown and unknowable in-universe (the failure occurs on the far side of the gate from Nova Reach's perspective, or the initiating event is otherwise never determined). Because both segments of Sat-39 share one mass ([§2.6](#2.6), [History §2](History.md#2)), both convert to black holes at once, each with a mass equal to the mass of the gate mouth it replaced, per local conservation of mass.

<a name="2.6"></a>
## 2.6 Failure Mode: Unified

A wormhole is stable only while its charge exceeds its mass (Qe/M > 1, [§2](#2)). Both known ways of losing that condition converge on the identical outcome: the throat snaps shut and both mouths convert to black holes, each carrying whatever mass that mouth held at the moment of failure. There is no difference in outcome between the two paths in, only in how a mouth got there:

- **The high edge — mass climbing toward charge.** Reached either by a single-transit overshoot (an unbalanced crossing's mass approaching the mouth's own, [Infrastructure §1](Infrastructure.md#1)) or by chronic net-import drift (a mouth on the receiving end of a long-term uncorrected trade imbalance, [§2](#2)).
- **The low edge — mass draining away from the stable configuration.** Reached by chronic net-export drift (a mouth steadily losing mass to uncorrected one-way outflow, [§2](#2)). The exact low-mass mechanism is not resolved by the underlying physics literature, which only establishes a two-fermion minimum for a valid B-SKR state — but whether the state fails by forced vacuum pair-production at the extreme field limit or by outright decoherence at the floor, the result is the same terminal collapse as the high-mass case.
**Mouth mass design constraint:** because both edges are dangerous, target mass is chosen between a floor and a ceiling, not simply maximized for safety margin. The floor is set by evacuation time, not by the theoretical instability point itself, which is poorly constrained — engineers deliberately hold well clear of it rather than operating close to an edge they can't fully see. The ceiling is set by installation and maintenance cost, which scales steeply with mass ([§2.1](#2.1)). This pushes every gate's target mass into the thousands-to-tens-of-thousands-of-tons range, rather than the milligram-scale minimal wormhole described in the underlying physics literature.

**Evaporation behavior:** Hawking evaporation time scales with the cube of mass. At the thousands-to-tens-of-thousands-of-tons range, the resulting black hole is far too small to be a gravitational threat to the system, but does not vanish instantly either — it persists for something between hours and several months, fading and finally ending in a brighter terminal burst of hard gamma radiation as the last of its mass converts to radiation.

<a name="3"></a>
# 3. Nova Reach System

**System name:** Nova Reach, formerly known only by its gate designation, Sat-39.

Nova Reach is Farfield's root colony — the oldest system in this branch of the network, and the one severed from Sol when Sat-39 collapses. It is not the first wormhole colony Farfield ever founded (that gate is Sat-39 of a sequential build history — 38 gates preceded it), but it is the first and oldest system in the branch that becomes cut off. "Nova Reach" was adopted as a friendlier public name once permanent colonization began (likely via a corporate-staged colonist naming contest / PR gesture), alongside the station's own drifted nickname (see [Infrastructure §3](Infrastructure.md#3)).

**Primary star:** K-dwarf, K3V–K5V. Locked to reflect Nova Reach's setting in an ancient, low-metallicity elliptical galaxy — a population where O/B/A and actively-forming stars are absent, and where a metal-poor star of a given mass runs slightly hotter/bluer than a metal-rich equivalent. A mid-range K-class keeps Nova Reach distinct from Danu A (K2V) and Obatala (G8V–K0V) while remaining consistent with the same old, metal-poor stellar population.

Nova Reach itself is mostly just Goibniu and its two orbiting stations; the system's small rocky inner planets are not narratively significant and can remain uncatalogued or use simple numeric designations if ever needed.

<a name="3.1"></a>
## 3.1 Goibniu

### Etymology

**Gas giant:** Goibniu (Irish smith-god, fitting the system's extraction/refining economy)

- Formal pronunciation: GOV-nyoo (Old Irish /ˈɡovʲnʲu/)
- Colloquial colonist pronunciation and spelling: "Govnu" — the settled, simplified form English-speaking colonists actually use, both spoken and written. "Goibniu" persists in formal/corporate documentation and star charts.

**Origin of the wormhole seed:** Sourced from Saturn's rings in Sol — hence the "Sat-#" convention, and the choice of Irish/Titan-adjacent mythology for this branch of the network (Saturn = Cronus; Irish myth chosen instead of Greco-Roman to avoid an overused convention).

### Physical Description

Atmosphere: notably helium-enriched relative to a typical young gas giant (~20% He vs. the ~10% seen in Sol's own Jupiter) — an old, low-metallicity system has had more time for preferential atmospheric hydrogen escape than a young giant, giving Goibniu an unusually rich helium/Trelium source and a real physical reason (beyond mere convenience) that Farfield's whole extraction economy centers here. Visually: a hazy, deep-blue-tinted giant, with trace hydrocarbons (methane and heavier) driving the color via the same chemistry responsible for Neptune's blue. **Rings:** a visible but modest ring system — thin and subtle compared to Mannannán's broad, Saturnian rings ([§4.2](#4.2)) — inner radius ~99,100 km, outer radius ~113,800 km (roughly 1.35–1.55 planetary radii). This is the same ring band the network's founding wormhole seeds were harvested from ([§4](#4)).

### View From Orbit

A hazy, deep blue-tinted giant with slowly shifting cloud bands, girdled by its thin ring (inner ~99,100 km / outer ~113,800 km) as a fine, sharp line rather than a broad sweep. Tiny artificial specks nearby mark Sat-39, Sat-48, and Structure 4's frozen, unfinished skeleton ([Infrastructure §2.1](Infrastructure.md#2.1)) — visibly artificial clutter against an otherwise untouched giant.

<a name="3.2"></a>
## 3.2 Sat-48 / Safford Nova Reach

### Siting

Sited on Goibniu's dwarf moon, in close orbit around the gas giant itself. Full architectural detail — spin gravity, deck geometry, growth history — lives in [Infrastructure §2.1](Infrastructure.md#2.1); this section covers only the view from the viewport.

### View From the Station

Goibniu owns the sky — a hazy, deep blue-tinted giant, trace hydrocarbons driving the same coloring chemistry responsible for Neptune's blue, filling a huge arc of the view at close moon-orbit range, its cloud bands shifting visibly over the course of a shift. A visible but modest ring system girds it — thin and subtle compared to Mannannán's broad, dramatic rings (below) — inner radius ~99,100 km, outer radius ~113,800 km ([§3.1](#3.1)). The star itself (K4V, Teff 4,460K) sits at 5.13 AU from Goibniu — far enough to read as a small, hard amber-orange point rather than a disc with real presence, more like how the Sun looks from Ganymede than from Earth. Behind it all: no Milky Way band. Nova Reach Galaxy is an ancient giant elliptical (E3) — the background sky is a diffuse, roughly even wash of dim orange-red points, no blue giants, no nebulae. Quiet and still. Structure 4's unfinished skeleton is visible nearby on the same spine — a frozen-mid-construction landmark for anyone looking out a habitat window ([Infrastructure §2.1](Infrastructure.md#2.1)).

<a name="4"></a>
# 4. Danu System — Irish mythology

All three branch systems are reached via Sat-48 in Nova Reach and were established before the eventual wormhole collapse, discovered and founded via the same staged-inflation method ([§2.2](#2.2)) using seeds harvested locally from Goibniu's own ring band. Each uses a distinct mythological naming convention, chosen deliberately to avoid the overused Greco-Roman well: Irish (Danu), Yoruba (Obatala), and Mesopotamian (Enlil). Each system's own Sat-48-designated wing — Safford — is sited on a distinct local body; see each system's own section below and [Travel §1](Travel.md#1)–14 for the resulting transit and communication figures, and [Infrastructure §2.1](Infrastructure.md#2.1) for each wing's habitat tier.

Founding years (see [timeline.md](./timeline.md)): Danu, Year 19; Enlil, Year 22; Obatala, Year 30.

**Star(s):** Wide binary. Danu A: K2V, ~0.8 M☉ (primary; all planets orbit this star). Danu B: M4V red dwarf companion, ~0.25 M☉, separated by roughly 500–800 AU — negligible gravitational effect on the planets; visible as a fixed, reddish second point of light in the sky. Barycentric orbital elements: Danu A at 148.78 AU from the barycenter, Danu B at 507.28 AU — total separation ~656 AU, consistent with the ~500–800 AU figure above. Both stars share a single, physically consistent eccentricity (e = 0.014) and inclination (i = 0.19°), since a real two-body system's pair of barycentric orbits are geometrically similar ellipses — same shape and tilt, opposite sides of the barycenter at all times — rather than independently-set values. Kepler's third law on this pair gives an orbital period of roughly 16,400 years, so on any story or gameplay timescale Danu B is effectively fixed in the sky — no orbital motion worth modeling.

**Stellar composition: high Mg/Si ratio.** Rocky-planet bulk composition inherits its host star's refractory-element ratios — magnesium, silicon, and iron condense from the same disk material the star itself formed from, so a star's photospheric abundances are a real, physically-grounded proxy for what its planets are made of. Danu A is set with an elevated magnesium-to-silicon ratio relative to solar, chosen specifically (working backward from Lugh's desired surface geology, below) rather than assumed by default. This is a deliberate divergence from the "roughly solar" assumption used elsewhere in the network unless and until another system's planetary geology calls for its own deviation.

<a name="4.1"></a>
## 4.1 Lugh (Danu c)

### Etymology

Named for the many-skilled Irish sun god Lugh; fits the world's light/dark divide.

### Orbital Data

0.1465 AU (e = 0.024, i = 0.19°) — tidally locked eyeball world, sitting at the inner habitable-zone edge.

### Geology and Deep Time

**Migrating substellar point.** Lugh locked to Danu A very early in its history — tidal locking is fast on geological timescales relative to a planet's overall lifespan — but the exact substellar point has not stayed fixed since. Over tens of millions of years, continental drift and internal mass redistribution can shift a locked world's precise sub-stellar center, letting it wander slowly across the surface over deep time. This is treated as a real, deep-time process for Lugh (not something noticeable within the story's timeframe — Farfield has only been present for a few decades) rather than a fixed, static configuration: regions currently deep in permanent daylight may show old geological or erosional signatures consistent with having once sat nearer the terminator, or even briefly within reach of the nightside ice, and vice versa. This gives Lugh's geology a layered, quasi-archaeological quality — worth mining for scene-setting detail (dry ancient lakebeds under today's scorched dayside, old erosion patterns in terrain that's now arid) without needing to be pinned to a specific rate or timeline; it is explicitly a deep-time backdrop, not an active process within the novel's timeframe.

**Tidal heating, volcanism, and magnetic field.** Lugh's position within Danu's system produces genuine ongoing tidal stress, and this is used as a real internal heat source beyond ordinary radiogenic decay — driving active volcanism and vigorous mantle convection. That same extra heat plausibly accelerates core heat loss, supporting a healthy, long-lived magnetic field (the research on this point is mixed — tidal locking can suppress dynamo action in some models — but the bible's locked choice, given Lugh's real tidal stress and the story value of the outcome, is a strong field). This gives Lugh geothermal power potential as a colony resource, meaningful radiation shielding beyond what its atmosphere alone provides (relevant given Danu A's more active K-dwarf flare behavior relative to Sol), and active, story-usable volcanic terrain.

**Cratering is essentially absent.** Lugh's ~1.8 bar CO2 atmosphere (2.5× Earth's column mass, per the reentry-physics analysis in [Travel §1.2](Travel.md#1.2)) burns up or dramatically decelerates all but the largest incoming impactors before they reach the surface, and Lugh's lower gravity (0.70g) further reduces terminal impact velocities for anything that does get through. Combined with active volcanic resurfacing (above), Lugh's surface reads as young and smooth by comparison to an airless or thin-atmosphere world — old impact scars are erased faster than they can accumulate, and only the rare, genuinely large impactor would ever leave a lasting mark.

**Composition: high-magnesium, forsterite-dominated silicates.** Danu A's elevated Mg/Si ratio (above) means Lugh's mantle and crust run forsterite-rich rather than the more balanced olivine/pyroxene mix a solar-composition star would produce. Practically, this means a stiffer, higher-viscosity mantle than Earth's (forsterite resists deformation more readily than a pyroxene-rich mix), and — the visually load-bearing consequence — volcanic and exposed mantle rock across Lugh runs pale, yellow-green, glassy in fresh exposures, closer to a peridot-toned landscape than Earth's typical dark basalt fields. This is a deliberate, distinctive visual signature for Lugh's terrain, chosen specifically over the alternative "iron-rich, rust-red" mineralogy (see also the parallel consequence for Boann's seafloor chemistry, [§4.3](#4.3)).

**Weather-driven erosion.** Consistent with eyeball-world climate modeling, atmospheric moisture converges and precipitates continuously near Lugh's substellar point, producing a band of persistent, heavy chemical weathering there (carbonic-acid-style rock weathering from CO2-charged precipitation, similar in kind to Earth's own carbonate weathering cycle) — likely Lugh's most Earth-like-looking terrain, ironically, despite sitting at the planet's hottest point. Lugh's inhabited terminator band, by contrast, sees steadier, drier, wind-dominated erosion (trade-wind-like circulation, per the terminator wind analysis below) rather than heavy rainfall — consistent with the terminator's already-established role as the planet's habitable, agriculturally-developed zone, and distinct in character from the wetter substellar terrain nobody actually lives in.

**Terminator wind regime and the katabatic hazard boundary.** Modeling of tidally-locked "eyeball" climates consistently shows the open terminator band itself carrying moderate, trade-wind-like circulation (working figure: ~4–5 m/s, comparable to real Antarctic interior katabatic flow) rather than constant storm conditions — survivable and unremarkable for both aviation and ground infrastructure. The genuine hazard sits specifically at the boundary where the nightside ice cap's edge meets the terminator: cold, dense air draining off the ice under gravity accelerates through any funneling terrain into real katabatic winds, by analogy with real Antarctic coastal katabatic flow reaching 15–20+ m/s sustained, with documented extreme gusts near 40–50 m/s in the worst funneling terrain. This sets a working operational threshold for Lugh's aviation and infrastructure: the open terminator band is safe for both fixed-wing and (hypothetically) lighter-than-air operations, but anywhere near the nightside ice edge crosses into fixed-wing-only territory, since sustained winds above roughly 15 m/s exceed typical airship crosswind limits. This boundary is the specific physical reasoning behind ruling out airships as a Lugh vehicle class for any settlement or route that might extend toward the ice margin.

*Note on eq-temperature: the data grid's 504.7 K figure for Lugh is a no-greenhouse blackbody average and predates this atmosphere; a real CO2 atmosphere at this thickness would trap meaningfully more heat than that number reflects. Treat 504.7 K as a floor value, not the actual expected surface temperature, until a proper radiative-transfer pass is done.*

### Sky and Landscape

CO2 Rayleigh-scatters more strongly than N2/O2 (larger, more polarizable molecule), so absent heavy dust loading (unlike Mars' thin, dust-choked atmosphere), Lugh's thick 1.8 bar CO2 sky reads as a rich, saturated blue — deeper than Earth's, not washed out. Because the primary city sits at the leading terminator by design ([Infrastructure §2.1](Infrastructure.md#2.1)), Danu A never rises far: the whole settled band lives in a permanent, warm amber near-sunset/near-sunrise light, blue at zenith shading to deep orange at the horizon where the star sits. Danu B is a small, unmoving red point elsewhere in the sky. Landscape: pale, yellow-green, peridot-toned volcanic rock (forsterite-rich, per the geology above) rather than Earth's dark basalt; young, smooth terrain almost free of cratering; agricultural domes topped with mirror arrays catching the low light; light aircraft and gliders riding terminator thermals; dust storms and thermal updrafts marking the day/night boundary; streaming dust visible near the katabatic winds off the ice-cap edge.

### View From Orbit

The classic eyeball-world silhouette. A bright, pale-hazed dayside hemisphere (thick CO2 reflecting hard) meets a sharp terminator; beyond it, a dark, frozen nightside dominated by a great antistellar ice cap. The habitable terminator ring shows as a thin band between the two extremes — scattered mirror-array glints and settlement lights tracing the line where people actually live. Sparse cratering and visible volcanic features mark the young, pale yellow-green (peridot-toned) terrain even from orbit; occasional pale dust-storm streaks cross the dayside.

<a name="4.2"></a>
## 4.2 Mannannán (Danu e)

### Physical Description

Gas giant, 6.04 AU (e = 0.012, i = 0.28°). Has a ring system, inner radius 84,636.3 km / outer radius 148,067.9 km — purely a visual/setting detail, not yet load-bearing for plot or engineering.

### View From Orbit

The dramatic one: strong banding, a bold Saturn-like ring system sweeping wide across the disc (inner 84,636.3 km / outer 148,067.9 km), with Boann and Safford Danu visible nearby as small moons threading the ring plane.

<a name="4.3"></a>
## 4.3 Boann (Mannannán I)

### Etymology

Named for the goddess of the River Boyne and a hidden, forbidden well.

### Orbital Data

Tidally-heated subsurface ocean moon. Orbital distance: 350,000 km from Mannannán, e = 0.008 (i = 1.26°) — sustained by a **3:2 mean-motion resonance with Mannannán III** (real analog: Neptune/Pluto), not eccentricity alone in isolation.

### Seafloor Chemistry

Because Boann shares Danu A's high-Mg/Si stellar composition with Lugh ([§4.1](#4.1)), its rocky core is likewise forsterite-rich rather than solar-typical — and forsterite is close to the purest possible ultramafic feedstock for **serpentinization**, the real hydrothermal process (well-documented at Earth's own deep-sea vent systems, and the leading theorized energy source for Europa's and Enceladus's own subsurface oceans) where ultramafic rock reacts with seawater to release free hydrogen. This makes Boann's seafloor a genuinely favorable site for vigorous serpentinization chemistry — plausibly richer hydrogen production and more vigorous hydrothermal vent activity than an Earth-composition seafloor would produce, a purely abiotic geochemical process throughout (no native or introduced life anywhere in the setting — [§1.1](#1.1)). This was a deliberate factor in setting the high-Mg/Si stellar composition: the choice pays off for Lugh's visible surface geology and for Boann's seafloor hydrogen-production chemistry simultaneously, rather than trading one off against the other.

### Sky and Landscape

No sky at all — the deliberate contrast against Lugh already established ([Infrastructure §2.1](Infrastructure.md#2.1)): people on Lugh can see their sky, people on Boann cannot. The "landscape" is ice tunnels lit by electric light, a submerged station over hydrothermal vents at the ocean floor (abiotic chemistry only, above), and the ever-present low-grade hazard of icequakes from tidal flexing. Total absence of daylight — only the constant artificial day of station lighting.

### View From Orbit

Bright white-grey ice, smoothed and refrozen by tidal flexing rather than heavily cratered — closer to Europa than to a dead moon. Fracture lines web the surface where tidal stress cracks the shell, some showing faint tan/reddish staining along the cracks from non-ice material welling up from below. No visible surface structures — everything is under the ice.

<a name="4.4"></a>
## 4.4 Safford Danu

### Siting

Sited on a dedicated minor moon of Mannannán — radius 31.5 km, mass ~2.62×10¹⁷ kg (surface gravity negligible, ~0.18% of Earth g — consistent with [Infrastructure §2.1](Infrastructure.md#2.1)'s requirement that every Safford host body have negligible native gravity), orbiting Mannannán at 590,000 km (e = 0.02, i = 0.61°).

### View From the Station

Mannannán is the visual centerpiece, and its ring system is the real thing — bold and Saturnian, inner radius 84,636.3 km / outer radius 148,067.9 km, a genuine banded giant with a dramatic ring plane crossing the sky. Two stars share the view: Danu A (K2V, amber-orange, Teff 4,830K) is the working light source; Danu B (M4V red dwarf, Teff 3,170K) sits ~656 AU out, a small, dim, fixed reddish point that for all practical purposes never moves across a human lifetime. Boann is visible nearby as a companion ice moon. Background: Danu Galaxy is a barred spiral (SBb) — a real band of light crosses the sky, blue-white star-forming knots and dust lanes, a livelier backdrop than Nova Reach's.

<a name="4.5"></a>
## 4.5 Minor and Uncatalogued Bodies

- Danu b — rocky, 0.0509 AU (e = 0.006, i = 0.18°), scorched, tidally locked, airless
- Danu d — rocky, 0.3066 AU (e = 0.035, i = 1.21°), thin atmosphere, unremarkable
- Sparse asteroid belt — ~1–3 AU; two representative bodies serve as orbital-element examples (Danu Belt 1: 1.53 AU, e = 0.081, i = 3.3°; Danu Belt 2: 2.13 AU, e = 0.111, i = 4.07°) rather than the belt being treated as a single undifferentiated feature
- Mannannán II, III — minor uninhabited moons: II is 370.5 km radius / ~1.246×10²¹ kg at 420,000 km (e = 0.02, i = 0.48°); III is 380.0 km radius / ~1.002×10²¹ kg at 460,000 km (e = 0.01, i = 0.13°). **III is Boann's 3:2 resonance partner** (see [§4.3](#4.3)) — its own small eccentricity is consistent with sharing that resonance, though it remains an ordinary uninhabited moon, no different in character from II.
- Danu f — ice giant, 15.37 AU (e = 0.016, i = 1.26°), outer system

<a name="5"></a>
# 5. Obatala System — Yoruba mythology

**Star:** Obatala, G8V–K0V, ~0.9 M☉ (single star, no binary companion)

<a name="5.1"></a>
## 5.1 Yemoja (Obatala c)

### Etymology

Named for the orisha mother of waters.

### Sky and Landscape

Unlike Obatala b (tidally locked, 0.097 AU), Yemoja at 0.452 AU is far enough out that tidal locking never completes — locked working rotation period: **~30 hours**, giving the world a genuine day/night cycle, distinct from Lugh's and Obatala b's permanent terminator geometry.

A dense, high-pressure atmosphere heavy with water vapor and greenhouse gases produces a strong low-level temperature inversion, capping vertical convection — the same basic principle behind Earth's persistent marine stratocumulus decks, just far more extreme and continuous here. Rather than towering, storm-generating convection, Yemoja carries an unbroken, uniform deck of pale grey-white cloud from horizon to horizon. The star (G8V–K0V) never appears as a disc; it's a flat, shadowless glow diffused evenly through the deck, never brighter, never darker, just a smear of pale light shifting position with the ~30-hour rotation. Warm, steady drizzle rather than violent rain; the ocean surface runs glassy-calm most of the time, with little of the wind-driving convective energy a stormier world would have.

As with Lugh's 504.7 K figure, the data grid's 326.4 K is a no-greenhouse blackbody average and understates the real number — this much water vapor and pressure traps real additional heat. Working range: high-40s to low-50s °C at the surface, oppressively humid, comfortably below water's critical point (647 K), so the ocean stays unambiguously liquid rather than supercritical.

Yemoja's lower bulk density (1.28 M⊕ in a 7,293.6 km radius — notably puffier than Earth for its mass) is consistent with a water-rich world with little continental crust: scattered small volcanic islands rather than continents, dark volcanic-rock shorelines, no large landmasses. Islands sit wrapped in constant low mist where warm, saturated air meets the coastline.

### Ocean Chemistry

Hydrothermal vents around the volcanic islands continuously feed dissolved iron and silica into the water — the same real geochemistry behind Earth's Precambrian Banded Iron Formations, except the process never stopped here, because there's no oxygenation event to shut it off, and no biology involved at any step ([§1.1](#1.1)). As vent water cools and mixes with the open ocean, silica precipitates first (its solubility drops sharply with temperature) as pale sinter terraces close to the vent; further out, once the water has cooled and mixed enough, dissolved iron oxidizes out via purely inorganic pathways — trace atmospheric oxidants dissolved in seawater, or high-altitude UV-driven photolysis products raining down from above the permanent cloud deck — precipitating as rust-red ferric bands. The alternating red/white banding is real, actively-forming rock near every vent field, not a geological relic. Away from vent zones, the open ocean runs a murky, opalescent greenish-grey — dissolved iron tinting the water, colloidal silica lending a faint milky cast, never clear.

### Settlement

Iron ore and high-purity hydrothermal silica are both directly useful — silica/glass in particular ties into the network's post-collapse CRT reconstruction arc ([Infrastructure §6.3](Infrastructure.md#6.3)), making Yemoja a plausible source feeding that entire tech-recovery timeline. Mineral scaling on infrastructure (pipes, equipment, hull fittings) is a routine, ongoing maintenance burden — Yemoja's equivalent of Boann's ice-shaft upkeep.

Coastal, sited directly on the volcanic islands' shorelines — sealed, climate-controlled structures built to manage near-constant condensation and humidity rather than cold, dry, or vacuum stress (life support assumed given no confirmation the atmosphere is breathable, same posture as Boann/Olokun/Ereshkigal). Near-shore aquaculture and kelp-analog farming, using Earth-descended organisms brought by the colonists rather than anything native ([§1.1](#1.1)), is the practical basis for Yemoja's role as Obatala's agricultural population center — water-based food production fitting a water-goddess-named ocean world more naturally than domed hydroponics would. Interiors run warmly and artificially lit to compensate for the flat, grey, shadowless exterior light; corrosion- and scale-resistant construction throughout given the permanent damp.

Deliberately the calmest-feeling world in the network — paired with the long comm lag to Safford (61.5–96.5 min one-way, [Infrastructure §5](Infrastructure.md#5)) and its post-collapse local autonomy ([Politics §4.5](Politics.md#4.5)/[Politics §5.1](Politics.md#5.1)), this reads as a real cultural signature: an insular, self-paced, slow-moving colony, in contrast to Lugh's wind-and-light dynamism, Boann's submarine-crew intensity, or Olokun's frozen-coast hardship.

### View From Orbit

A pale grey-white globe wrapped in permanent, uniform overcast — no polar caps, no sharp terminator (it isn't tidally locked), just faint latitudinal banding in the cloud deck from Coriolis effects at its ~30-hour rotation. Calmer and smoother-looking than Earth's cloud patterns, consistent with the world's "oppressive calm" character — no visible storm systems, no surface visible anywhere.

<a name="5.2"></a>
## 5.2 Olokun (Obatala g)

### Etymology

Named for the orisha of ocean depths and unknowable mystery.

### Orbital and Physical Data

~9–10 AU, axial tilt ~22° (moderate, Earth-like), orbital eccentricity ~0.15–0.20 (a second, overlapping source of seasonal variation atop the tilt), orbital period ~27–30 years. Surface gravity 0.8g (7.85 m/s²), implying a mass of ~0.69 M⊕ at a 6,200 km radius and a bulk density of ~5,520 kg/m³ — slightly denser than Earth's average, consistent with a differentiated rocky world with a substantial core. Surface temperature ~90 K, held above methane/ethane's freezing point by a dense (~2–5 bar) methane/ethane-dominant atmosphere and orbital placement rather than by proximity alone.

### Sky and Landscape

A close real-world analog is available: Titan. A dense (2–5 bar) methane/ethane atmosphere at ~90K produces the same kind of opaque, hazy orange-brown sky Titan is known for, diffusing what little light reaches it — Obatala's star, at ~9–10 AU, is already faint (comparable to Saturn's remove from Sol, ~7–9 W/m²), and the haze further reduces it to a dim smudge rather than a sharp disc; no hard shadows anywhere. Landscape: dark, oily-looking methane/ethane seas; frozen permafrost coastline; anchored extraction platforms; underground coastal habitation/processing bases; and — the one genuinely bright, warm-colored thing anywhere on the moon — the sunlamp-lit hydroponic domes, glowing against an otherwise dim, hazy world. Seasons run in multi-year swings (27–30-year orbit, moderate tilt plus real eccentricity), so the mood of the landscape shifts on a generational rather than annual clock.

### View From Orbit

Essentially featureless from orbit: a smooth, hazy orange-tan globe, Titan-style, with the dense methane/ethane atmosphere hiding every surface detail. At most, the faintest tonal variation hints at sea versus permafrost coast beneath the haze. No extraction platforms visible — the haze swallows everything.

<a name="5.3"></a>
## 5.3 Safford Obatala

### Siting

Co-orbital with Olokun, Phobos/Deimos-style, rather than sited on a dedicated moon of its own — a deliberate departure from the station's original asteroid-belt siting, and the reason Olokun sits in near-instant comm contact with Safford while Yemoja, ~9 AU further out, does not. Full architectural detail lives in [Infrastructure §2.1](Infrastructure.md#2.1).

### View From the Station

No gas giant here — Safford Obatala co-orbits Olokun itself (a terrestrial-scale ocean world, not a giant), Phobos/Deimos-style, so what looms large is a hazy orange-brown sphere at close range rather than a banded giant. The star (G8V–K0V, Teff 5,240K) is dim here — Olokun sits ~9–10 AU out, roughly Saturn's remove from Sol — so it reads as a modest, pale-yellow point. No rings, no companion star. Background: Obatala Galaxy is an Sc spiral — the most "textbook Milky Way" sky of the four, with a bright structured band, visible O/B stars, and pink-tinged HII regions.

<a name="5.4"></a>
## 5.4 Minor and Uncatalogued Bodies

- Obatala b — rocky, molten, tidally locked, ~0.1 AU
- Obatala d, e — unremarkable rocky worlds, ~0.7–1.2 AU
- Asteroid belt — ~2–4 AU (source of imported ice for Olokun's agriculture)
- Obatala f — gas giant, ~8 AU. A minor Trelium source at best, nothing like Goibniu's rich helium enrichment ([§3.1](#3.1)) — not presently worth the infrastructure to exploit.
- Obatala f I, II — minor moons

<a name="6"></a>
# 6. Enlil System — Mesopotamian mythology

Structurally distinct from the other two: this is a post-red-giant system. The primary has already died and become a white dwarf; everything else in the system is wreckage.

**Star(s):** Binary. Enlil A: white dwarf, ~0.6 M☉, Earth-sized, DA-type (hydrogen-dominated atmosphere), still relatively hot as white dwarfs go. Enlil B: surviving K5V or M0V main-sequence companion, ~0.6–0.7 M☉, separated by roughly 20–40 AU.

Causal chain: Enlil A swelled into a red giant → Enlil B's gravity destabilized the original planets' orbits via Kozai–Lidov-type perturbation → planets were shredded/scattered/partially consumed → the white dwarf shows a real "polluted white dwarf" signature from accreted rocky, phosphorus-rich debris — a genuine, observed astrophysical phenomenon used here as the in-world basis for Ereshkigal's phosphorus enrichment.

<a name="6.1"></a>
## 6.1 Ereshkigal (Enlil A b)

### Etymology

Named for the Mesopotamian queen of the underworld — ruling a dead, hollowed-out realm.

### Orbital Data

Phosphorus-rich rocky world, orbits the white dwarf directly at roughly 0.01–0.02 AU. Tidally locked. One face in permanent, brilliant white-dwarf light; the other in permanent dark. No natural warmth or agriculture to speak of beyond the tight orbit — an industrial/extraction outpost, not a residential colony. Likely small, purpose-built, rotational population given the harsh conditions.

*Ereshkigal's status as the network's key phosphorus/starvation-leverage chokepoint (see [Politics §2](Politics.md#2)) is reinforced by its harsh, small-population character — a resource stranglehold held by very few people.*

### Sky and Landscape

Airless and tidally locked directly around the white dwarf. At ~0.0125 AU with Enlil A's actual radius, the white dwarf's angular diameter works out to roughly 0.4° — close to our own Sun's apparent size from Earth (0.53°) — but at Teff 15,140K, blue-white and far more intense, not a gentle amber disc. For anyone topside on the dayside, that's a genuinely dangerous, eye-searing presence in an otherwise jet-black vacuum sky with unblinking stars. Enlil B is visible as an ordinary point far off; the debris ring may show as a faint band if aligned. Population lives in a deep-shielded terminator habitat ([Travel §1.4](Travel.md#1.4)) rather than under open sky routinely — topside exposure is for robotic-quarrying oversight and EVA maintenance work, not casual daylight. Landscape: blasted, phosphorus-rich rock, robotic dayside quarrying scars, the mass-driver track running toward the horizon, and buried/bermed habitat structures rather than anything resembling Lugh's open domes.

### View From Orbit

A stark, knife-edge contrast: a blazingly lit, heavily cratered dayside (phosphorus-rich rock giving it a faint pale yellow-green cast) scarred by robotic quarrying and the long linear gash of the mass-driver track, against a nightside so black it nearly vanishes against space — no atmosphere to soften the line between them at all. Enlil A's debris ring is sometimes visible as a faint arc in the background sky.

<a name="6.2"></a>
## 6.2 Safford Enlil

### Siting

Sited on a rubble-pile remnant beyond Ereshkigal, at roughly 0.05 AU (versus Ereshkigal's ~0.01–0.02 AU) — a deliberately close placement, only ~0.035 AU of separation. Full architectural detail lives in [Infrastructure §2.1](Infrastructure.md#2.1).

### View From the Station

Enlil A, the white dwarf (Teff 15,140K), is a tiny but ferociously blue-white point — the one genuinely alien-colored primary light source in the network. Enlil B, the surviving K5V companion, sits 14.24 AU out as an ordinary warm secondary star. The shattered debris ring around Enlil A is faintly visible as an arc — the graveyard of the original planets, and an acknowledged ongoing collision hazard. Ereshkigal itself is close enough (~0.035 AU separation) to be a notable nearby body. Background: Enlil Galaxy is lenticular (S0) — smooth, muted, no active star formation, matching the system's "already dead" character; a quiet backdrop under a violent-looking foreground light source.

<a name="6.3"></a>
## 6.3 Debris Ring and Minor Bodies

- Debris ring around Enlil A — shattered remains of the original planets, some still slowly accreting onto the white dwarf. Ongoing meteor/radiation hazard for anything nearby.
- Enlil c, d — minor rubble-pile remnants / unstable debris clumps, not true planets
