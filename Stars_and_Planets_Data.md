All projects
Fallen Branch
I want to craft a hard science fiction setting about a beach of star systems connected by wormholes that becomes permanently cut off from the rest of the network, including Earth.


How can I help you today?
Recents
Daily life on Sanford station before collapse
3 minutes ago
Star system diagram creation
14 hours ago
Exploring open questions about Sat-39's collapse
16 hours ago
Wormhole extraction pipeline viability calculation
16 hours ago
Farfields exploration
23 hours ago
Fairfield's planetary colonization strategy
2 days ago
Settlement population estimates
2 days ago
Wormhole diameter standards and mining
5 days ago
Immediate Aftermath
5 days ago
Primordial wormholes and detection methods
5 days ago
Wormhole network hard science fiction
5 days ago
Memory
Only you

Project memory will show here after a few chats.
Instructions

Add instructions to tailor Claude’s responses
Files
2% of project capacity used

Nova_Reach_Stars_and_Planets_Data.md
# Nova Reach Network — Stars & Planets Data Grid
 
*Companion reference to the Worldbuilding Bible. Values pulled directly from the SpaceEngine addon configs where established; other fields are computed from real physics; anything neither established nor cleanly computable is marked **TBD** rather than invented.*
 
## Methodology & assumptions
 
- **Mass / Radius / Semi-major axis / Eccentricity**: taken directly from the current SpaceEngine addon scripts (single source of truth — matches what's actually in-game).
- **Surface gravity**: computed directly, g = GM/r².
- **Solar day**: for tidally-locked bodies, solar day = orbital period exactly (real physics, not an estimate). For gas/ice giants, given as a *typical estimate* (~10–16 hr) based on real solar-system giants — angular momentum conservation during formation makes fast rotation near-universal for giants regardless of orbital distance, but this specific number isn't locked-in canon. For non-tidally-locked rocky worlds, no rotation period has been established — marked TBD.
- **Equilibrium temperature**: computed via T = T_eff × √(R_star / 2a) × (1 − albedo)^0.25, assuming albedo = 0.3 (Earth-like default) and simple blackbody physics — **no greenhouse effect, no atmosphere, whole-planet average**. For tidally-locked "eyeball" worlds (Danu b, Lugh, Obatala b, Ereshkigal) this average is hotter than the actual habitable terminator zone people would live at — treat these as an upper-bound/global-average number, not the temperature where anyone actually lives.
- **Atmospheric pressure**: for the three gas giants, SpaceEngine defines a planet's `Radius` as the 1-bar reference level by convention — so "1 bar (by definition, at stated radius)" is a real fact, not a guess. No pressure has been established for any rocky world **except Lugh**, whose thick cometary-delivered CO2 atmosphere (1.8 bar) is now bible-established (see Worldbuilding Bible discussion) precisely because it's narratively load-bearing — it distinguishes Lugh from Boann, enables surface settlement and low-gravity/thick-air flight, and isn't just decorative.
- **Atmospheric composition**: only Goibniu has an explicit scripted composition. Everything else is either SpaceEngine-procedural (not fixed in our script) or only described qualitatively in the bible — noted where the bible says something, TBD otherwise.
- **Comm delay from Safford**: only computed for worlds with an actual settlement the bible discusses coordinating with (Lugh, Yemoja, Olokun, Ereshkigal). Uninhabited/unvisited bodies are marked N/A rather than given a meaningless number.
- **Population**: only Ereshkigal has a bible-stated number (2,000–4,000, rotational). Everything else is TBD — the bible describes Lugh/Yemoja/Olokun/Boann qualitatively (e.g. "primary agricultural hub") without hard population figures. Station (Safford) populations are noted separately per system since they're bible-established but describe the *station*, not the planet.
Units: stellar mass/radius in solar units (M☉/R☉); planetary mass/radius in Earth units (M⊕) and km. Temperatures in Kelvin. Distances in AU.
 
---
 
## Nova Reach System
 
**Safford station population (bible-established): ≈25,000–35,000** (largest in the network, hosts all three branch mouths)
 
| Body | Type | Mass | Radius | Surface Gravity | Semi-Major Axis | Atm. Pressure | Eq. Temperature | Atm. Composition | Solar Day | Comm Delay from Safford | Population |
|---|---|---|---|---|---|---|---|---|---|---|---|
| Nova Reach | K4V star | 0.71 M☉ | 0.733 R☉ | 362.1 m/s² (36.9× Earth) | — | — | Teff 4,460 K | — | TBD | — | — |
| Nova Reach I | Rocky planet | 0.391 M⊕ | 4,144.8 km | 9.07 m/s² (0.92× Earth) | 0.289 AU | TBD | 313.5 K | TBD (uncatalogued) | TBD | N/A (uninhabited) | TBD |
| Nova Reach II | Rocky planet | 0.615 M⊕ | 4,803.3 km | 10.63 m/s² (1.08× Earth) | 0.606 AU | TBD | 216.4 K | TBD (uncatalogued) | TBD | N/A (uninhabited) | TBD |
| Nova Reach Goibniu | Gas giant | 299.0 M⊕ | 73,424.5 km | 22.11 m/s² (2.25× Earth) | 5.13 AU | 1 bar (by definition, at stated radius) | 74.4 K | H₂ 74.72%, He 20.00%, CH₄ 4.00%, NH₃ 0.25%, H₂S 0.03% | ~10–16 hr (typical giant, estimate) | N/A (Safford orbits Goibniu directly) | — |
 
---
 
## Danu System
 
**Safford Danu station population (bible-established): 150 rotational crew** (short arc-module, 66.1 m arc/33.9°, network-standard 111.8 m/2.000 rpm/0.5g design — Nova Reach personnel, not counted toward Danu's population)
 
| Body | Type | Mass | Radius | Surface Gravity | Semi-Major Axis | Atm. Pressure | Eq. Temperature | Atm. Composition | Solar Day | Comm Delay from Safford | Population |
|---|---|---|---|---|---|---|---|---|---|---|---|
| Danu A | K2V star | 0.80 M☉ | 0.822 R☉ | 324.5 m/s² (33.1× Earth) | 148.78 AU (barycentric) | — | Teff 4,830 K | — | TBD | — | — |
| Danu B | M4V star | 0.25 M☉ | 0.315 R☉ | 690.4 m/s² (70.4× Earth) | 507.28 AU (barycentric) | — | Teff 3,170 K | — | TBD | — | — |
| Danu b | Rocky planet | 0.301 M⊕ | 4,044.9 km | 7.33 m/s² (0.75× Earth) | 0.051 AU | TBD | 856.4 K | TBD | 4.69 days (= orbital period, tidally locked) | N/A (uninhabited) | TBD |
| Danu Lugh | Rocky planet, eyeball world, thick CO2 atmosphere (cometary-delivered) | 0.665 M⊕ | 6,213.3 km | 6.87 m/s² (0.70× Earth) | 0.147 AU | 1.8 bar, CO2-dominant (~95%+), trace N₂/inerts | 504.7 K (global avg, blackbody calc only — **no greenhouse term**; real terminator-zone surface temp runs warmer than this given CO2's radiative properties, not yet computed) | ~95%+ CO₂, trace N₂ and inert gases; cometary-delivery origin, no free O₂ | 22.90 days (= orbital period, tidally locked) | 49.0–51.5 min one-way | TBD (primary agricultural hub, no hard figure) |
| Danu d | Rocky planet | 0.491 M⊕ | 4,709.7 km | 8.82 m/s² (0.90× Earth) | 0.307 AU | TBD | 348.9 K | Thin (bible-qualitative) | TBD | N/A (uninhabited) | TBD |
| Danu Mannannán | Gas giant | 253.0 M⊕ | 68,725.3 km | 21.35 m/s² (2.18× Earth) | 6.04 AU | 1 bar (by definition) | 78.6 K | TBD | ~10–16 hr (estimate) | N/A (Safford orbits it directly) | — |
| Danu f | Ice giant | 14.24 M⊕ | 22,303.7 km | 11.41 m/s² (1.16× Earth) | 15.37 AU | 1 bar (by definition) | 49.3 K | TBD | ~14–18 hr (estimate) | N/A (uninhabited) | TBD |
 
*Eccentricity and inclination are now locked for every body above but, like Olokun's axial tilt/eccentricity, aren't columns in this grid yet: Danu A and Danu B share a single, physically consistent e=0.014/i=0.19° (barycentric orbits — both stars trace geometrically similar ellipses around the shared barycenter, so a single e/i applies to both, unlike an earlier pass that mismatched them); Danu b e=0.006/i=0.18°; Lugh e=0.024/i=0.19°; Danu d e=0.035/i=1.21°; Mannannán e=0.012/i=0.28°; Danu f e=0.016/i=1.26°. Mannannán also now has a locked ring system (inner radius 84,636.3 km, outer radius 148,067.9 km) — decorative/setting detail only so far.*

### Danu Moons (Mannannán system)

| Body | Mass | Radius | Surface Gravity | Orbital Radius | Eccentricity / Inclination | Comm Delay from Safford | Notes |
|---|---|---|---|---|---|---|---|
| Boann | ~8.9 × 10²⁰ kg (~0.00015 M⊕) | 550 km | 0.02g (0.196 m/s²) | 350,000 km | e = 0.008, i = 1.26° | <10 sec (co-orbital) | Populated water-operations site; bulk density ~1,275 kg/m³ (cf. Rhea, 1,236 kg/m³). Ice shell ~3–5 km thick at the borehole site. Eccentricity locked in the Europa/Enceladus range (e≈0.009/0.005) specifically to sustain the tidal heating the settlement depends on. Still open (lower priority): whether a resonance with Mannannán II/III/Safford's host moon is what maintains this eccentricity long-term. |
| Mannannán II | ~1.246 × 10²¹ kg | 370.5 km | TBD | 420,000 km | e = 0.02, i = 0.48° | N/A (uninhabited) | Minor uninhabited moon |
| Mannannán III | ~1.002 × 10²¹ kg | 380.0 km | TBD | 460,000 km | e = 0.01, i = 0.13° | N/A (uninhabited) | Minor uninhabited moon |
| Safford Danu's host moon | ~2.62 × 10¹⁷ kg | 31.5 km | ~0.018 m/s² (~0.18% Earth g, negligible) | 590,000 km | e = 0.02, i = 0.61° | — (Safford wing itself) | Dedicated station-siting body, distinct from Mannannán II/III; negligible native gravity consistent with §4.1's Safford siting requirement |

*Two representative asteroid-belt bodies are also now locked as examples of the ~1–3 AU sparse belt (not an exhaustive catalog): Danu Belt 1 at 1.53 AU (e = 0.081, i = 3.3°, ~5.4 × 10¹⁸ kg, 75.80 km radius) and Danu Belt 2 at 2.13 AU (e = 0.111, i = 4.07°, ~4.8 × 10¹⁸ kg, 71.52 km radius).*

---
 
## Obatala System
 
**Safford Obatala station population (bible-established): 90 rotational crew** (short arc-module, 39.7 m arc/20.3°, network-standard 111.8 m/2.000 rpm/0.5g design — Nova Reach personnel, not counted toward Obatala's population). **Relocated** (this session) from the 2–4 AU asteroid belt to a minor moon co-orbital with Olokun, Phobos/Deimos-style — see Olokun's row below and the Worldbuilding Bible §7.2.
 
| Body | Type | Mass | Radius | Surface Gravity | Semi-Major Axis | Atm. Pressure | Eq. Temperature | Atm. Composition | Solar Day | Comm Delay from Safford | Population |
|---|---|---|---|---|---|---|---|---|---|---|---|
| Obatala | G8V star | 0.87 M☉ | 0.901 R☉ | 293.7 m/s² (29.9× Earth) | — | — | Teff 5,240 K | — | TBD | — | — |
| Obatala b | Rocky planet | 0.338 M⊕ | 4,088.0 km | 8.07 m/s² (0.82× Earth) | 0.097 AU | TBD | 703.7 K | TBD | 11.87 days (= orbital period, tidally locked) | N/A (uninhabited) | TBD |
| Obatala Yemoja | Ocean world | 1.28 M⊕ | 7,293.6 km | 9.59 m/s² (0.98× Earth) | 0.452 AU | TBD | 326.4 K | Thick (bible-qualitative, traps heat) | TBD | **61.5–96.5 min one-way** (revised — now the isolated, slow-coupled world following Safford's relocation to Olokun) | TBD (agricultural population center, no hard figure) |
| Obatala d | Rocky planet | 0.555 M⊕ | 4,724.7 km | 9.90 m/s² (1.01× Earth) | 0.870 AU | TBD | 235.2 K | TBD | TBD | N/A (uninhabited) | TBD |
| Obatala e | Rocky planet | 0.678 M⊕ | 5,539.9 km | 8.80 m/s² (0.90× Earth) | 1.14 AU | TBD | 205.5 K | TBD | TBD | N/A (uninhabited) | TBD |
| Obatala f | Gas giant | 214.0 M⊕ | 59,496.4 km | 24.10 m/s² (2.46× Earth) | 8.07 AU | 1 bar (by definition) | 77.2 K | TBD | ~10–16 hr (estimate) | N/A (uninhabited) | Minor Trelium source only — not worth developing (bible §7.2) |
| Obatala Olokun | Liquid methane/ethane ocean world | **0.69 M⊕** (revised) | **6,200 km** (revised) | **7.85 m/s² (0.80× Earth)** (revised — locked this session) | **~9–10 AU** (revised inward from 18.76 AU) | **~2–5 bar, methane/ethane-dominant** (revised) | **~90 K** (revised — held above methane/ethane freezing point by dense atmosphere + orbital placement; supports a liquid ocean) | Methane/ethane-dominant, dense | TBD | **under ~10 sec one-way** (revised — Safford now co-orbital, Phobos/Deimos-style) | TBD (hydrocarbon extraction + growing post-collapse hydroponic-agriculture workforce, bible §7.2) |
| Obatala h | Icy dwarf | 0.021 M⊕ | 1,348.7 km | 4.60 m/s² (0.47× Earth) | 26.13 AU | TBD | 42.9 K | TBD | TBD | N/A (uninhabited) | TBD |
| Obatala i | Icy dwarf | 0.015 M⊕ | 1,212.1 km | 4.13 m/s² (0.42× Earth) | 32.67 AU | TBD | 38.4 K | TBD | TBD | N/A (uninhabited) | TBD |
 
*Olokun's revised values (0.8g, 0.69 M⊕, 6,200 km radius, bulk density ~5,520 kg/m³, 22° axial tilt, ~0.15–0.20 eccentricity, ~27–30 year orbital period) supersede the earlier 18.76 AU / 1.43g / near-90° tilt entry. Axial tilt and eccentricity aren't columns in this grid yet — noted here and in the bible §7.2 pending a possible grid restructure. Eq. temperature (~90 K) is a target value consistent with a liquid ocean, not a blackbody calc — a proper greenhouse/albedo pass is still owed, same caveat as Lugh's stale 504.7 K figure.*
 
---
 
## Enlil System
 
**Safford Enlil station population (bible-established): 50 rotational crew** (short arc-module, 22.0 m arc/11.3°, network-standard 111.8 m/2.000 rpm/0.5g design — Nova Reach personnel, not counted toward Ereshkigal's population)
 
| Body | Type | Mass | Radius | Surface Gravity | Semi-Major Axis | Atm. Pressure | Eq. Temperature | Atm. Composition | Solar Day | Comm Delay from Safford | Population |
|---|---|---|---|---|---|---|---|---|---|---|---|
| Enlil A | White dwarf (DA4) | 0.62 M☉ | 0.009 R☉ | 2,097,535 m/s² (~213,900× Earth) | 15.32 AU (barycentric) | — | Teff 15,140 K | — | TBD | — | — |
| Enlil B | K5V star | 0.68 M☉ | 0.701 R☉ | 379.2 m/s² (38.7× Earth) | 14.24 AU (barycentric) | — | Teff 4,390 K | — | TBD | — | — |
| Enlil Ereshkigal | Phosphorus-rich rocky world | 0.400 M⊕ | 4,142.5 km | 9.29 m/s² (0.95× Earth) | 0.015 AU | TBD | 517.4 K (global avg — permanent day/night split, not uniform) | TBD | 0.85 days / ~20.4 hr (= orbital period, tidally locked) | 0.31–0.56 min (18–34 sec) one-way | **2,000–4,000 (bible-established, rotational)** |
 
*Note: Enlil c/d (rubble remnants) and the debris ring are not true planets, so excluded per your request.*
 
---
 
## Summary: comm delay from Safford, settled worlds only
 
| World | System | One-way delay | Round-trip delay |
|---|---|---|---|
| Ereshkigal | Enlil | 18–34 sec | 35–65 sec |
| Boann *(moon, for reference)* | Danu | <10 sec | <15 sec |
| Olokun *(moon-scale; Safford relocated here, revised this session)* | Obatala | under ~10 sec | under ~15 sec |
| Lugh | Danu | 49.0–51.5 min | 1.63–1.72 hr |
| Yemoja *(revised this session — now the isolated world)* | Obatala | 61.5–96.5 min | 2.05–3.22 hr |
 
*Yemoja and Olokun swapped roles this session: Safford Obatala relocated from the asteroid belt to a minor moon co-orbital with Olokun (bible §7.2), making Olokun the fast-coupled, tightly-controlled world and Yemoja the slow-coupled, autonomous one — the reverse of the original table above.*
 
