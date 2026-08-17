# Culture

*Each file numbers its own sections independently starting at §1. Cross-references elsewhere in the bible take the form `[File §X.Y](File.md#X.Y)`, naming the target file before the section number.*

<a name="1"></a>
## 1 Historical colonist strata
 
- First-wave colonists: white-collar administrators plus idealists who believed the corporate "libertarian frontier" sales pitch.
- Second-wave colonists: pragmatists who knew the reality and emigrated out of economic desperation on Earth.
- Older colonies skew more idealist (now disillusioned); newer colonies skew more pragmatist.
<a name="2"></a>
## 2 Three ideological groups post-founding
 
- Pragmatists — want stability and wages, will work with any system that keeps them fed.
- Disillusioned idealists — angry about the corporate lie, want genuine change, potential revolutionary drivers.
- White-collar administrators — invested in the corporate hierarchy, will leverage institutional legitimacy during crisis.
<a name="3"></a>
## 3 Labor classes (Nova Reach extraction pipeline)
 
- Remote drone operators/monitors — station-based technicians overseeing automated sweeper and scoop fleets (not "pilots" — more like air-traffic control for a robotic swarm).
- Maintenance/retrieval technicians — smaller, specialized trade; physically service and recover malfunctioning drones.
- Wormhole inspectors/engineers — rare, physics-literate specialists who judge seed viability by charge-to-mass ratio and threading-field response, and who stabilize/expand viable seeds into gates. Irreplaceable; the only people who can repair or create gates. Enormous post-collapse leverage.
- Hazard/maintenance crews — present on every station network-wide. EVA/vacuum work, gate machinery tuning, emergency response. Tradesperson culture, tight-knit, informal experience-based hierarchy, high status despite blue-collar pay. Likely present (dead, or heroic) at the moment any given gate fails — natural candidates for post-collapse mythology.
### Lugh: Culture and Belief

Three constant material facts of life on Lugh — the slowness of its light, the routine closeness of a fast, mechanical death just outside a dome, and decades of practiced self-governance — shape a culture that reads as distinct from anywhere else in the network, Safford included.

**Time is read, not measured.** The 22.9-day light cycle shifts too gradually for a clock to matter the way it does elsewhere; Lugh colonists track the cycle the way a farmer tracks a season rather than the way a shift worker tracks an hour. This plausibly produces something closer to an agrarian or maritime relationship with time than an industrial one, potentially including its own informal calendar of rituals or festivals tied to the light's peak and trough within each cycle — a lived, secular liturgical rhythm that stands in sharp contrast to Safford's flat, arbitrary, always-identical fluorescent day. A Lugh colonist visiting Safford would likely find its constant artificial light faintly unsettling — disconnected from anything real outside.

**Death is close and mundane, which produces competence-worship rather than fatalism.** A failed seal check kills in minutes (§ above), and every child learns this fact before they're old enough to understand much else. Real-world communities that live with routine, mechanical, high-consequence risk — commercial diving, wildland firefighting, high-altitude mountaineering towns — tend not to turn morbid about it; they ritualize competence instead. The mandatory safety-officer gear check at every dome exit is experienced less as bureaucratic friction and more as a small daily ceremony everyone willingly participates in, because everyone has heard the story of the one time it wasn't done properly. Skill with one's own equipment is a genuine point of pride, and a visitor who treats the check carelessly — an unfamiliar Safford administrator, say — reads as dangerously naive rather than merely rude.

**Self-reliance here is lived history, not ideology.** Long before the eventual severance, Lugh has already been operating on local decision-making by necessity — the ~49-minute one-way comm lag to Safford makes real-time corporate micromanagement structurally impossible ([Politics §5.1](Politics.md#5.1)). That means Farfield's original "libertarian frontier" recruitment pitch ([§1](#1)) may feel *less* like a broken promise on Lugh than it does at Safford, even though both are nominally under the same corporate umbrella: Lugh's people have genuine, decades-deep lived experience of making real decisions that actually stick. This is a meaningfully different psychological inheritance from Safford's disillusioned-idealist strand ([§1](#1)–10.2), who watched that same promise collapse up close. On Lugh, the founding idealism had somewhere real to go.

**Cultivation versus extraction is the deepest value-level split between Lugh and the rest of the network.** Nova Reach's economy is built entirely on extraction — sweeping ring particles, harvesting seeds, refining trelium, tracking children into labor pipelines ([Infrastructure §2.2](Infrastructure.md#2.2)). Lugh's economy is built entirely on cultivation — tending, waiting, nurturing something across a full cycle before it's ready to harvest. This is not merely an economic difference; it plausibly shapes work ethic, parenting philosophy, and even conflict resolution on Lugh toward something closer to "tend it and give it time" rather than "extract value and move on." A Lugh colonist encountering Nova Reach's extraction pipeline firsthand might find its underlying logic — take, process, ship, repeat, nothing given time to grow — faintly alien or even quietly grotesque.

**Aviation is a shared literacy, not a specialist trade, and it is where all of the above crystallizes culturally.** Growing up around small aircraft the way people elsewhere grow up around bicycles or boats plausibly produces real folk heroes — legendary pilots who flew rescue missions through a dust storm, a first solo flight functioning as an informal coming-of-age marker, art and music built around wind and thermals the way maritime cultures build songs around the sea. "The wind off the line" (the terminator's thermal updrafts, §above) is both a practical piece of flying knowledge and, plausibly, a piece of local poetry.

**Underneath all of this: a quiet, specific resentment of being unseen.** Lugh feeds the 25,000–35,000 people on Safford, and by rights that should command real respect — but the people eating that food never meet the people who grew it, thanks to distance and a corporate culture that treats Lugh as a resource line item rather than a place with a name and a face. This is a different flavor of grievance from Safford's own direct, felt corporate control ([Infrastructure §2.2](Infrastructure.md#2.2)) — less about being controlled, more about being taken for granted by people who have never once watched the light shift across a twenty-two-day cycle, or checked a neighbor's seal before stepping outside.

<a name="4"></a>
## 4 Post-Collapse Software and Information Culture

The pre-collapse assumption that hardware always improves — already an established working principle in ITV spin-gravity engineering ([Travel §1](Travel.md#1)) — breaks for the first time in the network's history after Year 92 ([History §4.1](History.md#4.1)): hardware stops improving and starts getting scarcer, for roughly a century. Software culture reorganizes itself completely around that reversal.

**A two-tier culture emerges.** Dwindling pre-collapse Earth-chip hardware keeps running whatever software was already controlling life-critical systems — gate monitoring, life support — largely untouched, since nobody dares risk rewriting code nobody living fully understands anymore. This legacy software becomes something closer to sacred, guarded rather than modernized. Everything built fresh on locally-fabbed, low-density chips ([Infrastructure §6.2](Infrastructure.md#6.2)) demands a genuinely new toolchain, since old general-purpose software habits waste cycles and memory this hardware can't spare.

**A new language lineage.** Descended from C's philosophy of direct hardware control and minimal runtime overhead, but with compile-time enforced memory safety and resource budgeting built in from the start — the colonies' engineers have the benefit of decades of hindsight about exactly how C-era memory bugs kill systems, and on hardware where a crash in gate-adjacent code is existential rather than inconvenient, that hindsight gets written into the language itself rather than left as a lesson learned the hard way twice.

**A new network protocol.** A dense, binary, schema-first data format (structurally closer to Protocol Buffers or CBOR than to text-based formats like JSON or HTML) replaces anything requiring on-the-wire text parsing — every byte and every CPU cycle spent decoding data is a real cost on megahertz-tier hardware, and fixed, pre-agreed schemas let fields go across the wire as raw typed values with no names attached at all.

**Efficiency becomes a form of status**, the same way hazard-crew work is blue-collar but genuinely respected ([§3](#3) above) — a programmer who can shave a routine's power draw or cycle budget isn't just skilled, they're keeping something alive.

**A distributed, swarm-native computing paradigm.** Given locally-fabbed chips are individually weak, and given Safford's drone-operations education track already trains systems thinking and swarm-behavior control theory ([Infrastructure §2.2](Infrastructure.md#2.2)), the culture's dominant paradigm becomes coordinating many small, cheap processors rather than building toward one powerful machine — a genuinely new invention shaped by necessity, not a retro throwback to pre-collapse computing.

**Color as institutional hope.** Even through the long decades when displays are monochrome or, at best, field-sequential ([Infrastructure §6.3](Infrastructure.md#6.3)), the network's data formats preserve full color information losslessly rather than discarding it — a deliberate act of faith that color-capable hardware will eventually be common again. When three-phosphor color displays finally do reach ordinary people, old archives and images are seen in true color for the first time by anyone still alive to see them.
