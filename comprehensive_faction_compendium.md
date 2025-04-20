# Comprehensive Faction Compendium – Gameplay‑Ready Version

## Terran Legacy Directorate

### High‑Level Profile

| Home‑space | Snapshot Identity | Strategic Edge |
|---|---|---|
| Earth–Moon system | Guardian bureaucracy of baseline humanity | Launch‑tariff chokehold & veteran fleet |

### Internal Structure
* **Orbital Customs Office** – licenses launches & scans cargo
* **Lunar Shipyard Command** – builds conservative hulls
* **Ministry of Culture** – polices genome & cyberware
* **Off‑World Affairs** – runs proxy ops

### Systems & Mechanics (Godot‑friendly)
| System | Node / Field | Gameplay Effect |
|---|---|---|
| Tariff Gate | TariffGate2D | adds cost or smuggling event |
| Launch Quota | global launch_permits | 0 permits doubles fuel costs |
| Customs Scan | ContrabandCheck | flags illegal cargo & fine |

### Relationships & Drama
* Political brinkmanship with Red Frontier
* Backs Calyx immunity

### Mission Seeds
1. **Launch Window Closed** – Forge permit before intercept mission
2. **Contraband Classics** – Smuggle banned literature
3. **Refugee Pod Dilemma** – Return or protect pods

### Real Science → Design Decisions
| Science Fact | Design Choice | Implementation |
|---|---|---|
| Costly 1g launches | Monetize permits | TariffGate |
| Regolith shielding | Cheap repairs on Luna | Shipyard discount |
| Crowded GEO | Database transponders | Stealth beacon item |

---

## Sunwright Guild

### High‑Level Profile

| Home‑space | Snapshot Identity | Strategic Edge |
|---|---|---|
| Mercury megastruts | Solar‑engineer techno‑priests | Beamed power & solar alloys |

### Internal Structure
* **Heliologians** – maintain mirrors
* **Shade‑Tower Crews** – mobile city
* **Solar Forgers** – cast alloys
* **Luminary Guard** – sail frigates

### Systems & Mechanics (Godot‑friendly)
| System | Node / Field | Gameplay Effect |
|---|---|---|
| Solar Flare Cycle | HeatShaderTimer | scorch outdoor tiles |
| Power PPA | PowerContract | fuel −50% |
| Terminator Rail Dock | RailMover | dock every 90 s |

### Relationships & Drama
* Cold war with Helios
* Ceramic trade with Io

### Mission Seeds
1. **Mirror Alignment** – EVA fix heliostat
2. **Shade Code Theft** – Track saboteur

### Real Science → Design Decisions
| Science Fact | Design Choice | Implementation |
|---|---|---|
| High solar flux | Microwave grid | PowerContract |
| Extreme heat | Heat hazard | Scorch tiles |
| Metal‑rich crust | Alloy exclusivity | Item tag guild_alloy |

---

## Aphrodite Aerostat Republic

### High‑Level Profile

| Home‑space | Snapshot Identity | Strategic Edge |
|---|---|---|
| Venus cloud layer | Glam‑chem aerostat states | Acid monopoly & fast couriers |

### Internal Structure
* **Sky‑Barons Council** – CEO oligarchy
* **Sirocco Guard** – jet fighters
* **Chem Guilds** – catalyst patents
* **Mannerist Academy** – couture authority

### Systems & Mechanics (Godot‑friendly)
| System | Node / Field | Gameplay Effect |
|---|---|---|
| Acid Mist | CorrosiveTile | armor decay |
| Jet‑Stream Drift | WindVector | push entities |
| Style Reputation | rep score | NPC price modifier |

### Relationships & Drama
* Patent wars with Directorate pharma
* Bioexchange with Titan

### Mission Seeds
1. **Runway Heist** – Steal photonic fabric
2. **Acid Rain Escort** – Protect convoy

### Real Science → Design Decisions
| Science Fact | Design Choice | Implementation |
|---|---|---|
| Earth‑like 55km layer | Aerostat habitats | Wind drift |
| Sulfuric acid clouds | Acid hazard | Corrosive tiles |
| Super‑rotation | Fast jets | Courier intercept chance - |

---

## Red Frontier Confederacy

### High‑Level Profile

| Home‑space | Snapshot Identity | Strategic Edge |
|---|---|---|
| Mars & Phobos ring | Syndicalist terraformers | Agri domes & mass‑drivers |

### Internal Structure
* **Clans‑Council** – greenhouse reps
* **Terraform Corps** – hydro mercs
* **Phobos Gunners** – ring artillery

### Systems & Mechanics (Godot‑friendly)
| System | Node / Field | Gameplay Effect |
|---|---|---|
| Dome Integrity | integrity var | crop fail & CO2 fog |
| Orbital Strike | Ability | shell each 5 turns |
| Dust Storm | Hazard | solar & accuracy − |

### Relationships & Drama
* Food‑ice exchange with Belt
* Phobos gun vs Directorate

### Mission Seeds
1. **Patch the Dome** – Repair before storm
2. **Gun Hijack** – Bombard blockade

### Real Science → Design Decisions
| Science Fact | Design Choice | Implementation |
|---|---|---|
| 0.38g | Cheap launcher | Mass‑driver ability |
| Dust storms | Vision penalty | Hazard |
| CO2 caps | Terraform bombs | Questline |

---

## Ceres Aquifer Syndicate

### High‑Level Profile

| Home‑space | Snapshot Identity | Strategic Edge |
|---|---|---|
| Ceres | Water cartel mafia | Ice price control & illicit refits |

### Internal Structure
* **Don Families** – ice mines
* **Dry‑Docks** – truss yards
* **Convoy Wardens** – escort

### Systems & Mechanics (Godot‑friendly)
| System | Node / Field | Gameplay Effect |
|---|---|---|
| Water Price | ice_price var | affects fuel token cost |
| Protection Fee | TollArea | non-pay spawns pirates |
| Refit Yard | ShipRepairFast | quick repair & suspicion |

### Relationships & Drama
* Extorts Belt convoys
* Rival Triton nitrogen

### Mission Seeds
1. **Ice Ransom** – Escort tanker
2. **Dock Double‑Cross** – Upgrade or sabotage

### Real Science → Design Decisions
| Science Fact | Design Choice | Implementation |
|---|---|---|
| Huge ice reserves | Water currency | ice_price var |
| Micro‑g | Large docks | fast repair |
| Legal grey zone | Mob rule | intimidation dialogues |

---

## Belt Free Assembly

### High‑Level Profile

| Home‑space | Snapshot Identity | Strategic Edge |
|---|---|---|
| Main belt | Unionised Belters | Ice convoy leverage & strike power |

### Internal Structure
* **Convoy Guild** – routes ice
* **Vac Phys Council** – protects low‑g rights
* **Strike Committee** – organises stoppages

### Systems & Mechanics (Godot‑friendly)
| System | Node / Field | Gameplay Effect |
|---|---|---|
| Ice Convoy | MovingFleet | escort/raid event |
| Strike Meter | global int | port shutdown |
| Creole Dialog | dialect tag | miscomm chance |

### Relationships & Drama
* Labor tension with Ceres
* Sympathy with Mars

### Mission Seeds
1. **Convoy Rescue** – Protect hauler
2. **Strikebreaker** – Smuggle scabs

### Real Science → Design Decisions
| Science Fact | Design Choice | Implementation |
|---|---|---|
| Micro‑g | Physio trait | EVA buff |
| Ice vital | Convoy gameplay | escort |
| Language drift | Creole | dialog system |

---

## Europa Ocean Collective

### High‑Level Profile

| Home‑space | Snapshot Identity | Strategic Edge |
|---|---|---|
| Europa under‑ice | Dream‑commune transhumans | Superconductive organics & fortress caverns |

### Internal Structure
* **Dream Lagoon** – VR cloud
* **Bathypawn Corps** – pressure explorers
* **Vent Harvesters** – enzyme extractors

### Systems & Mechanics (Godot‑friendly)
| System | Node / Field | Gameplay Effect |
|---|---|---|
| Submersible Mode | VehicleSwitch | alt movement |
| Shared Dream | morale buff | if linked |
| Optic Relay | structure hp | cut disables comm |

### Relationships & Drama
* Embargo by Directorate
* Alliance with Titan

### Mission Seeds
1. **Vent Expedition** – Harvest enzymes
2. **Dream Heist** – Steal memory

### Real Science → Design Decisions
| Science Fact | Design Choice | Implementation |
|---|---|---|
| Ocean & vents | Bathypawn bodies | Submersible mode |
| High surface rad | Under‑ice living | safe maps |
| Conductive ocean | Organic supercon | item upgrade |

---

## Hydromagnetic Commonwealth of Ganymede

### High‑Level Profile

| Home‑space | Snapshot Identity | Strategic Edge |
|---|---|---|
| Ganymede shield | Guild engineer haven | Hydrogen bank & radiation shelter |

### Internal Structure
* **Induction Canopy Guild** – mesh upkeep
* **Hydro‑Refinery** – LH2 plants
* **Surface Council** – merit rotation

### Systems & Mechanics (Godot‑friendly)
| System | Node / Field | Gameplay Effect |
|---|---|---|
| Canopy Segment | Structure hp | broken -> map rad Major |
| Fuel Contract | LH2Token | cheap fuel; sabotage price spike |
| Mag‑Storm Minigame | QTE event | success stabilizes, fail arcs |

### Relationships & Drama
* Helios toll disputes
* Tech share with Europa

### Mission Seeds
1. **Radiation Leak** – Repair canopy
2. **Fuel Panic** – Protect refinery

### Real Science → Design Decisions
| Science Fact | Design Choice | Implementation |
|---|---|---|
| Magnetosphere | Safe pocket | Radiation flag |
| Low gravity | Cheap LH2 launch | Fuel economy |
| Induction current | Power source | Mag-Storm gameplay |

---

## Volcanic Forge Communion

### High‑Level Profile

| Home‑space | Snapshot Identity | Strategic Edge |
|---|---|---|
| Io lava skimmers | Forge monks | Refractory alloys & power bricks |

### Internal Structure
* **Monastic Foundry** – lava hovers
* **Induction Priors** – flux power
* **Pilgrim Escorts** – guide traders

### Systems & Mechanics (Godot‑friendly)
| System | Node / Field | Gameplay Effect |
|---|---|---|
| Induction Surge | Hazard | EMP stun 2 turns |
| Radiation Timer | rad Major | stack per 15s |
| Lava River | InstantKillTile | death |

### Relationships & Drama
* Trade with Sunwright
* Hates Threshold

### Mission Seeds
1. **Pilgrim Escort** – Guide through eruption window
2. **Flux Overload** – Dump charge or melt

### Real Science → Design Decisions
| Science Fact | Design Choice | Implementation |
|---|---|---|
| Volcanism | Natural furnace | Alloy loot |
| Flux tube current | Power bricks | Hazard surge |
| Radiation high | Risk timer | Rad stacks |

---

## Helios Consortium

### High‑Level Profile

| Home‑space | Snapshot Identity | Strategic Edge |
|---|---|---|
| Jovian/Saturn skies | He‑3 merchant princes | Fuel monopoly & beam navy |

### Internal Structure
* **He‑3 Board** – lords
* **Sky‑Carrier Fleet** – mobile plants
* **Private Court** – charter law

### Systems & Mechanics (Godot‑friendly)
| System | Node / Field | Gameplay Effect |
|---|---|---|
| Fuel Index | fuel_price var | reactor cost mod |
| Beam Lance | WeaponSweep | long range |
| Carrier Deck | ConveyorTiles | boarding |

### Relationships & Drama
* Espionage war with Sunwright
* Contracts with Nexus

### Mission Seeds
1. **Fuel Embargo** – Sneak fuel
2. **Carrier Heist** – Board carrier

### Real Science → Design Decisions
| Science Fact | Design Choice | Implementation |
|---|---|---|
| He‑3 rich | Fuel monopoly | fuel_price var |
| High ascent | Carriers stay aloft | unique map |
| Historical precedent | Private courts | Bounty |

---

## Titan Cloud Alchemists

### High‑Level Profile

| Home‑space | Snapshot Identity | Strategic Edge |
|---|---|---|
| Titan methane | Biopunk eco cult | Living hydrocarbon factories |

### Internal Structure
* **Bio‑Lakes Guild** – harvest
* **Luminescent Order** – lighting
* **Cryo Wardens** – cold tech

### Systems & Mechanics (Godot‑friendly)
| System | Node / Field | Gameplay Effect |
|---|---|---|
| Cold Meter | env cryo | warmth drain |
| Living Armor | item regen | flammable |
| Balloon Relay | CommNode | hack snoop |

### Relationships & Drama
* Clash with Helios
* Gene pact with Europa

### Mission Seeds
1. **Spill Cleanup** – Contain toxic lake
2. **Gene Heist** – Steal enzyme

### Real Science → Design Decisions
| Science Fact | Design Choice | Implementation |
|---|---|---|
| Methane lakes | Cryo bioware | Cold meter |
| Haze blocks radio | Relay balloons | Comm gameplay |
| Organic atmosphere | Living plastic | Item regen |

---

## Cryo‑Cartel of Triton

### High‑Level Profile

| Home‑space | Snapshot Identity | Strategic Edge |
|---|---|---|
| Triton glaciers | Frontier cartel | Stealth nitrogen & catapult toll |

### Internal Structure
* **Glacier Dons** – mine N2
* **Catapult Masters** – rail launch
* **Freezer Vaults** – contraband

### Systems & Mechanics (Godot‑friendly)
| System | Node / Field | Gameplay Effect |
|---|---|---|
| Rail Launch | FastTravel | teleport w/ hull stress |
| Cryo Vault | ColdTile | freeze damage |
| Lag Contract | DelayedAction | outcome hours later |

### Relationships & Drama
* Broker for Ghost Fleet
* Price war with Ceres

### Mission Seeds
1. **Catapult Sabotage** – Strand expedition
2. **Vault Heist** – Retrieve xenotech

### Real Science → Design Decisions
| Science Fact | Design Choice | Implementation |
|---|---|---|
| -235C | Natural freezer | ColdTile |
| Geysers | Rail power | FastTravel |
| Light lag | Async deals | DelayedAction |

---

## Calyx Archive Compact

### High‑Level Profile

| Home‑space | Snapshot Identity | Strategic Edge |
|---|---|---|
| Callisto vaults | Neutral data bank | Immutable pods & insurance sanctions |

### Internal Structure
* **Archivum** – data
* **Custodia** – cryo wardens
* **Legatus** – diplomats

### Systems & Mechanics (Godot‑friendly)
| System | Node / Field | Gameplay Effect |
|---|---|---|
| Immutable Pod | DataPod | destroy -> outrage |
| Neutrality Token | ShipFlag | AI cost ×5 |
| Checksum Drift | Timer event | requires spin-glass |

### Relationships & Drama
* Depends on Ganymede hydrogen
* Targeted by Threshold

### Mission Seeds
1. **Frozen Testament** – Recover will
2. **Token Breach** – Extradite pirate sanctuary

### Real Science → Design Decisions
| Science Fact | Design Choice | Implementation |
|---|---|---|
| Low rad/cryogenic | Cheap storage | DataPod |
| Ice crust stable | Vault safety | Map persist |
| Neutral hub | Insurance market | Token system |

---

## Threshold Dominion

### High‑Level Profile

| Home‑space | Snapshot Identity | Strategic Edge |
|---|---|---|
| Charon terminator | Cosmic horror choir | Flash gate & sanity fog |

### Internal Structure
* **Choir Wrought** – entangled minds
* **Null Altar Keepers** – well operators
* **Prophecy Arks** – AI couriers

### Systems & Mechanics (Godot‑friendly)
| System | Node / Field | Gameplay Effect |
|---|---|---|
| Null Hymn Aura | MapAura | sanity drain & sensor jam |
| Flash Gate | Teleport | instant ambush |
| Corruption Meter | pawn stat | mutations |

### Relationships & Drama
* Feared by all; Directorate spies seek tech
* Infiltrates Belters

### Mission Seeds
1. **Gate Crash** – Stop altar
2. **Whisper Pods** – Quarantine crew

### Real Science → Design Decisions
| Science Fact | Design Choice | Implementation |
|---|---|---|
| Micro black holes | Sensor noise | MapAura |
| Quantum echo voices | Polyvoice | Audio overlay |
| Charon vacuum | Safe test site | Home map |

---

## Nexus Shipworks Collective

### High‑Level Profile

| Home‑space | Snapshot Identity | Strategic Edge |
|---|---|---|
| Mobile Tycho yard | Worker‑owned arms dealer | Stealth prototypes & moving market |

### Internal Structure
* **Shareholders Assembly** – votes work
* **Prototype Line** – test hulls
* **Strike Guards** – security

### Systems & Mechanics (Godot‑friendly)
| System | Node / Field | Gameplay Effect |
|---|---|---|
| Hull Prototype | ExplodeOnFail | test hazard |
| Market Relocate | yard_pos | vendors move |
| Labor Strike | global bool | services halt |

### Relationships & Drama
* Supplies Helios, Mars, Directorate
* Espionage battleground

### Mission Seeds
1. **Prototype Rescue** – Save crew
2. **Vote Rigging** – Buy shares

### Real Science → Design Decisions
| Science Fact | Design Choice | Implementation |
|---|---|---|
| Zero‑g fab | Huge hulls | Prototype Line |
| Drum rotation | Coriolis combat | accuracy mod |
| Private station | Treaty dodge | Relocate |

---
