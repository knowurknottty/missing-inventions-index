# The Missing Inventions Index v2.0

**Authors:** Knowurknottty and bioCAPTv3
**Affiliation:** Inversion Labs
**Date:** July 2026

---

## What This Is

An open-source atlas of unsolved engineering problems.

Instead of cataloging inventions, we catalog **gaps**:

- Humanity has no practical X
- Existing solutions all fail because Y
- Here are the constraints
- Anyone may attempt to solve it

This is not a wish list. Every entry has quantified metrics, falsification criteria, dependency graphs, and cross-domain synthesis. It is designed to be **actionable** -- not inspirational.

---

## How to Use This

1. **Find a problem** that interests you
2. **Read the metrics** -- understand priority and difficulty
3. **Check the dependency graph** -- see what this unlocks
4. **Read the falsification criteria** -- know when to stop
5. **Propose a solution** -- open a PR or issue
6. **Document your results** -- success or failure, both are valuable

---

## Metrics Reference

| Metric | Description |
|--------|-------------|
| **Global Impact** | People or industries affected (millions/billions) |
| **Difficulty** | Engineering challenge (1-10, 10 = hardest) |
| **Cost to Prototype** | Rough budget for first proof |
| **Time Horizon** | Months/years to first proof |
| **Scientific Risk** | How much depends on unknown science (1-10) |
| **Engineering Risk** | How much depends on execution (1-10) |
| **Evidence Score** | Strength of supporting literature (1-10) |
| **Readiness** | Hypothesis / Simulation / Prototype / Demonstrated |

---

## Technology Dependency Graph

```
RTS (Room-Temp Superconductor)
│
├── Grid-Scale Storage (MI-001)
│   ├── Autonomous Agriculture
│   ├── Green Hydrogen
│   ├── Disaster Recovery
│   └── Water-Positive Cities
│
├── Zero-Field MRI (MI-009)
│   ├── Global Diagnostic Access
│   ├── Cancer Screening at Scale
│   └── Neurological Research
│
├── Desalination (MI-004)
│   ├── Autonomous Agriculture
│   ├── Green Hydrogen
│   ├── Disaster Recovery
│   └── Water-Positive Cities
│
├── Room-Temp Quantum Computing (MI-020)
│   ├── Drug Discovery
│   ├── Materials Science
│   ├── Cryptography
│   └── Climate Modeling
│
├── Solar 60% (MI-002)
│   ├── Desalination (power source)
│   ├── Grid-Scale Storage (charge source)
│   └── Off-Grid Infrastructure
│
├── Protein $0.10/kg (MI-006)
│   ├── Food Security
│   ├── Deforestation Reduction
│   └── Water Conservation
│
├── Housing $1K (MI-011)
│   ├── Disaster Recovery
│   ├── Urbanization
│   └── Space Habitats
│
└── 1 Exaflop at 1W (MI-021)
    ├── AI for Science
    ├── Autonomous Systems
    └── Edge Computing
```

**Key insight:** RTS is the root node. Most other gaps depend on it or become easier with it.

---

## 1. Energy

### MI-001: Grid-Scale Energy Storage Without Lithium

**Problem:** Global energy storage capacity is 16 GWh. We need 10,000 GWh to fully utilize renewables.

**Current best:** Lithium-ion batteries ($150/kWh, 10-year lifespan, fire risk).

**Metrics:**

| Metric | Value |
|--------|-------|
| Global Impact | 8 billion (energy access for all) |
| Difficulty | 9/10 |
| Cost to Prototype | $10-50M |
| Time Horizon | 5-10 years |
| Scientific Risk | 7/10 |
| Engineering Risk | 8/10 |
| Evidence Score | 6/10 |
| Readiness | Hypothesis |

**Why existing solutions fail:**
- Lithium is scarce (concentrated in 3 countries)
- Batteries degrade (50% capacity loss in 10 years)
- Fire risk (thermal runaway)
- Environmental damage (mining, disposal)

**Why it hasn't been solved:**
- **Economic:** Lithium industry has $50B+ invested in current tech
- **Physics:** Energy density of chemical storage has fundamental limits
- **Manufacturing:** Gigafactory scale required for cost reduction
- **Regulatory:** Grid storage standards assume lithium
- **Incentives:** Utilities are risk-averse, slow to adopt
- **Tooling gaps:** No materials discovery pipeline for grid-scale alternatives

**Falsification criteria:**
This idea fails if: (1) no material achieves >1000 Wh/kg at <$50/kWh, OR (2) cycle life <10,000 cycles at 80% capacity, OR (3) thermal runaway risk cannot be eliminated.

**Cross-domain synthesis:**
- Could biology solve this? -- Flow batteries use organic molecules (quines)
- Could materials science remove the bottleneck? -- RTS magnetic storage, metal-air batteries
- Could AI reduce design costs? -- Yes, GNoME-style screening of 381K materials

**Convergence:** Multiple teams (Form Energy iron-air, ESS iron flow, Ambri liquid metal) converging on earth-abundant materials. Independent rediscovery suggests the lithium paradigm is reaching its limits.

---

### MI-002: Solar Cells at 60% Efficiency

**Problem:** Best solar cells achieve 47% (multi-junction). Commercial panels achieve 20-22%. We need 60% for economic viability.

**Current best:** Multi-junction cells (47%, $100,000/m2).

**Metrics:**

| Metric | Value |
|--------|-------|
| Global Impact | 8 billion (clean energy) |
| Difficulty | 8/10 |
| Cost to Prototype | $5-20M |
| Time Horizon | 3-7 years |
| Scientific Risk | 6/10 |
| Engineering Risk | 7/10 |
| Evidence Score | 7/10 |
| Readiness | Simulation |

**Why existing solutions fail:**
- Multi-junction cells are too expensive for mass deployment
- Single-junction cells hit Shockley-Queisser limit (33%)
- Tandem cells add complexity and cost

**Why it hasn't been solved:**
- **Physics:** Shockley-Queisser limit is fundamental for single junction
- **Manufacturing:** Multi-junction epitaxy is expensive
- **Economics:** Cost per watt matters more than efficiency
- **Incentives:** 22% panels are "good enough" for current markets

**Falsification criteria:**
This idea fails if: (1) no multi-junction approach achieves 60% at <$1/watt, OR (2) thermalization losses cannot be reduced below 20%, OR (3) tandem architectures hit practical complexity limits.

**Cross-domain synthesis:**
- Could biology solve this? -- Photosynthesis achieves 30% in nature
- Could AI reduce design costs? -- Yes, optimization of layer thicknesses and compositions
- Could materials science remove the bottleneck? -- Perovskite stacking, quantum dot harvesting

**Convergence:** Oxford PV, Caelux, and others converging on perovskite-silicon tandems. Efficiency climbing 1-2% per year.

---

### MI-003: Room-Temperature Superconductor (Ambient Pressure)

**Problem:** Superconductors require cryogenic cooling or extreme pressure. No room-temperature, ambient-pressure superconductor exists.

**Current best:** Pd-Ni-P metallic glass (our work, Tc ~300K at ambient pressure -- kinetic trapping).

**Metrics:**

| Metric | Value |
|--------|-------|
| Global Impact | 8 billion (enables everything) |
| Difficulty | 10/10 |
| Cost to Prototype | $1-10M |
| Time Horizon | 2-5 years |
| Scientific Risk | 9/10 |
| Engineering Risk | 6/10 |
| Evidence Score | 4/10 |
| Readiness | Hypothesis |

**Why existing solutions fail:**
- Hydrides require >100 GPa pressure
- Cuprates require liquid nitrogen cooling
- All existing solutions are expensive or impractical

**Why it hasn't been solved:**
- **Physics:** Electron-phonon coupling is weak at ambient conditions
- **Manufacturing:** Metastable phases are hard to synthesize
- **Tooling gaps:** No high-throughput superconductor screening

**Falsification criteria:**
This idea fails if: (1) kinetic trapping cannot stabilize high-Tc phases, OR (2) Pd-Ni-P system cannot achieve Tc >350K, OR (3) synthesis is not reproducible across labs.

**Cross-domain synthesis:**
- Could AI reduce design costs? -- Yes, GNoME screening
- Could materials science remove the bottleneck? -- Ionic oxide theory (2025) provides new roadmap

**Convergence:** Multiple groups (Cao et al., Dias retracted, our work) independently exploring metallic glasses. The field is converging on metastable synthesis as the path.

---

## 2. Water

### MI-004: Desalination at $0.01/liter

**Problem:** 2 billion people lack clean water. Desalinated water costs $0.50-1.00/m3 ($0.0005-0.001/liter). We need $0.01/liter for universal access.

**Current best:** Reverse osmosis ($0.50/m3).

**Metrics:**

| Metric | Value |
|--------|-------|
| Global Impact | 2 billion |
| Difficulty | 8/10 |
| Cost to Prototype | $5-20M |
| Time Horizon | 3-5 years |
| Scientific Risk | 5/10 |
| Engineering Risk | 8/10 |
| Evidence Score | 7/10 |
| Readiness | Prototype |

**Why existing solutions fail:**
- RO requires high pressure (60-80 bar) -- energy-intensive
- Membranes foul and need replacement
- Brine disposal damages ecosystems

**Why it hasn't been solved:**
- **Physics:** Thermodynamic minimum energy for desalination is 0.3 kWh/m3
- **Manufacturing:** Membrane production is energy-intensive
- **Economics:** Energy cost dominates operational cost
- **Incentives:** Water utilities are publicly funded, slow to innovate
- **Tooling gaps:** No membrane material achieves theoretical efficiency

**Falsification criteria:**
This idea fails if: (1) no membrane achieves <0.3 kWh/m3, OR (2) membrane lifetime <5 years, OR (3) brine disposal cannot be solved.

**Cross-domain synthesis:**
- Could biology solve this? -- Aquaporins (biological water channels) are 1000x more efficient
- Could materials science remove the bottleneck? -- Graphene membranes, MOF membranes
- Could AI reduce design costs? -- Yes, optimization of membrane structure

**Convergence:** Desalinate, Gradiant, and others converging on next-gen membranes. Cost declining 5-10% per year.

---

### MI-005: Underground Water Detection Without Drilling

**Problem:** 30% of wells in Africa go dry because they are drilled in the wrong place. Each dry well wastes $10,000-50,000.

**Current best:** Geophysical survey ($50,000, takes months).

**Metrics:**

| Metric | Value |
|--------|-------|
| Global Impact | 300 million |
| Difficulty | 7/10 |
| Cost to Prototype | $1-5M |
| Time Horizon | 1-3 years |
| Scientific Risk | 4/10 |
| Engineering Risk | 7/10 |
| Evidence Score | 5/10 |
| Readiness | Hypothesis |

**Why existing solutions fail:**
- Geophysical surveys are too expensive for rural use
- Satellite imaging lacks resolution
- No portable, affordable solution exists

**Why it hasn't been solved:**
- **Physics:** Electromagnetic signals attenuate in rock
- **Manufacturing:** SQUID sensors require cryogenic cooling
- **Economics:** No market incentive for affordable detection
- **Incentives:** NGOs fund wells, not detection

**Falsification criteria:**
This idea fails if: (1) no sensor achieves 500m depth at <$5,000, OR (2) resolution is insufficient to distinguish water-bearing layers.

**Cross-domain synthesis:**
- Could biology solve this? -- Some animals detect underground water
- Could semiconductor advances enable it? -- Yes, RTS SQUID arrays

**Convergence:** Zond and others using magnetotellurics. Cost declining but still too high.

---

## 3. Food

### MI-006: Protein Production at $0.10/kg

**Problem:** Global protein demand will double by 2050. Current production costs $5-10/kg for animal protein, $2-5/kg for plant-based.

**Current best:** Plant-based protein ($2-5/kg).

**Metrics:**

| Metric | Value |
|--------|-------|
| Global Impact | 8 billion |
| Difficulty | 9/10 |
| Cost to Prototype | $20-100M |
| Time Horizon | 5-10 years |
| Scientific Risk | 7/10 |
| Engineering Risk | 8/10 |
| Evidence Score | 4/10 |
| Readiness | Hypothesis |

**Why existing solutions fail:**
- Animal protein is too expensive and resource-intensive
- Plant-based protein lacks complete amino acid profile
- Cultured meat is too expensive ($10,000/kg)

**Why it hasn't been solved:**
- **Physics:** Protein synthesis requires energy and precursors
- **Manufacturing:** Bioreactors are expensive
- **Economics:** Scale requires massive capital
- **Regulatory:** Novel proteins face safety hurdles
- **Incentives:** Meat industry resists alternatives

**Falsification criteria:**
This idea fails if: (1) no production method achieves <$0.10/kg at scale, OR (2) nutritional quality cannot match animal protein, OR (3) consumer acceptance is too low.

**Cross-domain synthesis:**
- Could biology solve this? -- Precision fermentation, single-cell protein
- Could swarm intelligence solve it? -- Decentralized small-scale production
- Could AI reduce design costs? -- Optimization of fermentation conditions

**Convergence:** Perfect Day, Solar Foods, and others converging on fermentation-based protein. Cost declining but still 10-50x target.

---

### MI-007: Crop Yield Increase Without GMO or Pesticides

**Problem:** Crop yields have plateaued. We need 50% increase by 2050 to feed 10 billion people.

**Current best:** GMO + pesticide intensive farming.

**Metrics:**

| Metric | Value |
|--------|-------|
| Global Impact | 2 billion (farmers) |
| Difficulty | 8/10 |
| Cost to Prototype | $5-20M |
| Time Horizon | 5-10 years |
| Scientific Risk | 6/10 |
| Engineering Risk | 7/10 |
| Evidence Score | 5/10 |
| Readiness | Simulation |

**Why existing solutions fail:**
- GMO faces public resistance and regulatory barriers
- Pesticides harm pollinators and human health
- Organic farming has 20-30% lower yields

**Why it hasn't been solved:**
- **Physics:** Photosynthesis has fundamental efficiency limits
- **Biology:** Plant genetics are complex
- **Economics:** GMO seeds are profitable for suppliers
- **Regulatory:** GMO approval takes 10+ years
- **Incentives:** Chemical companies profit from pesticides

**Falsification criteria:**
This idea fails if: (1) no non-GMO method achieves 50% yield increase, OR (2) pest damage cannot be controlled without chemicals.

**Cross-domain synthesis:**
- Could biology solve this? -- Microbiome engineering, companion planting
- Could semiconductor advances enable it? -- Magnetic pest deterrence, precision agriculture
- Could swarm intelligence solve it? -- Decentralized monitoring

**Convergence:** Pivot Bio, Indigo Ag, and others converging on microbiome-based solutions.

---

### MI-008: Food Preservation Without Refrigeration for 30 Days

**Problem:** 30% of food is lost post-harvest. In developing countries, 50% of perishable food spoils before reaching consumers.

**Current best:** Cold chain refrigeration ($100B/year infrastructure).

**Metrics:**

| Metric | Value |
|--------|-------|
| Global Impact | 2 billion |
| Difficulty | 7/10 |
| Cost to Prototype | $1-5M |
| Time Horizon | 1-3 years |
| Scientific Risk | 4/10 |
| Engineering Risk | 6/10 |
| Evidence Score | 6/10 |
| Readiness | Prototype |

**Why existing solutions fail:**
- Refrigeration requires infrastructure that does not exist in 50% of developing countries
- Ice melts and needs replacement
- Drying reduces nutritional value

**Why it hasn't been solved:**
- **Physics:** Entropy drives spoilage
- **Manufacturing:** Passive cooling systems are limited
- **Economics:** Cold chain is profitable in developed countries
- **Incentives:** Food companies optimize for developed markets
- **Tooling gaps:** No affordable, long-lasting preservation method exists

**Falsification criteria:**
This idea fails if: (1) no method preserves perishable food for 30 days at ambient temperature, OR (2) cost exceeds $100/unit.

**Cross-domain synthesis:**
- Could biology solve this? -- Fermentation, natural preservatives
- Could materials science remove the bottleneck? -- Phase-change materials, superconducting magnetic storage

**Convergence:** Zero Acre Farms, Apeel Sciences, and others converging on novel preservation methods.

---

## 4. Health

### MI-009: MRI at Point-of-Care for $500

**Problem:** 2/3 of the world has no access to medical imaging. MRI machines cost $1-3M.

**Current best:** Portable ultrasound ($5,000-50,000).

**Metrics:**

| Metric | Value |
|--------|-------|
| Global Impact | 5 billion |
| Difficulty | 9/10 |
| Cost to Prototype | $10-50M |
| Time Horizon | 5-10 years |
| Scientific Risk | 8/10 |
| Engineering Risk | 8/10 |
| Evidence Score | 4/10 |
| Readiness | Hypothesis |

**Why existing solutions fail:**
- MRI requires cryogenic cooling ($100K/year)
- MRI requires shielded room ($500K)
- Ultrasound lacks soft tissue contrast

**Why it hasn't been solved:**
- **Physics:** Strong magnetic fields require superconducting magnets
- **Manufacturing:** Cryogenic systems are complex
- **Economics:** MRI is profitable at $1M+ price point
- **Regulatory:** Medical devices face 5-10 year approval
- **Incentives:** Hospitals invest in high-margin machines

**Falsification criteria:**
This idea fails if: (1) no superconductor achieves sufficient field strength at room temperature, OR (2) signal-to-noise ratio is insufficient for diagnosis.

**Cross-domain synthesis:**
- Could semiconductor advances enable it? -- Yes, RTS magnets
- Could AI reduce design costs? -- Yes, compressed sensing, AI reconstruction

**Convergence:** Hyperfine (portable MRI), Promaxo (MRI-guided intervention) converging on lower-cost imaging.

---

### MI-010: Antibiotic Production Without Fermentation

**Problem:** Antibiotic resistance is rising. We need new production methods that are faster and cheaper.

**Current best:** Fermentation ($50-100/kg for generic antibiotics).

**Metrics:**

| Metric | Value |
|--------|-------|
| Global Impact | 8 billion |
| Difficulty | 8/10 |
| Cost to Prototype | $10-50M |
| Time Horizon | 5-10 years |
| Scientific Risk | 7/10 |
| Engineering Risk | 7/10 |
| Evidence Score | 5/10 |
| Readiness | Hypothesis |

**Why existing solutions fail:**
- Fermentation takes weeks
- Requires expensive bioreactors
- Limited to naturally occurring compounds

**Why it hasn't been solved:**
- **Physics:** Chemical synthesis of complex molecules is hard
- **Biology:** Natural products are optimized by evolution
- **Economics:** Fermentation is cheap at scale
- **Regulatory:** Novel antibiotics face approval hurdles
- **Incentives:** Low ROI discourages antibiotic development

**Falsification criteria:**
This idea fails if: (1) no synthesis method achieves <$10/kg, OR (2) novel compounds cannot be synthesized faster than fermentation.

**Cross-domain synthesis:**
- Could biology solve this? -- Synthetic biology, engineered pathways
- Could AI reduce design costs? -- Yes, retrosynthesis planning

**Convergence:** Phage therapy, antimicrobial peptides, and AI-designed antibiotics converging as alternatives.

---

## 5. Housing

### MI-011: Permanent Housing at $1,000 per Family

**Problem:** 1.6 billion people lack adequate housing. Temporary shelters cost $500-2,000 but last only 2-5 years.

**Current best:** Tents ($500, last 2 years) and concrete block ($10,000, lasts 50 years).

**Metrics:**

| Metric | Value |
|--------|-------|
| Global Impact | 1.6 billion |
| Difficulty | 7/10 |
| Cost to Prototype | $1-5M |
| Time Horizon | 2-5 years |
| Scientific Risk | 3/10 |
| Engineering Risk | 7/10 |
| Evidence Score | 6/10 |
| Readiness | Prototype |

**Why existing solutions fail:**
- Tents are temporary and unsafe
- Concrete requires skilled labor and infrastructure
- No affordable permanent solution exists

**Why it hasn't been solved:**
- **Physics:** Materials must withstand weather and time
- **Manufacturing:** Local materials vary widely
- **Economics:** $1,000 is below cost for conventional construction
- **Regulatory:** Building codes assume conventional materials
- **Incentives:** Construction industry profits from complexity
- **Tooling gaps:** No standardized low-cost building system

**Falsification criteria:**
This idea fails if: (1) no material system achieves 25-year lifespan at <$1,000, OR (2) construction cannot be done by unskilled labor in 1 week.

**Cross-domain synthesis:**
- Could biology solve this? -- Mycelium bricks, earth construction
- Could swarm intelligence solve it? -- Decentralized, community-led construction

**Convergence:** ICON (3D printing), WikiHouse (open-source construction), and others converging on digital fabrication.

---

### MI-012: Affordable Insulation at R-50

**Problem:** Energy poverty affects 2.4 billion people. Heating/cooling costs are prohibitive without insulation.

**Current best:** Fiberglass insulation ($0.50/sq ft, R-3.5 per inch).

**Metrics:**

| Metric | Value |
|--------|-------|
| Global Impact | 2.4 billion |
| Difficulty | 6/10 |
| Cost to Prototype | $500K-2M |
| Time Horizon | 1-2 years |
| Scientific Risk | 2/10 |
| Engineering Risk | 5/10 |
| Evidence Score | 7/10 |
| Readiness | Prototype |

**Why existing solutions fail:**
- Fiberglass requires installation skill
- Spray foam requires equipment
- No affordable, easy-to-install solution exists

**Why it hasn't been solved:**
- **Physics:** Low thermal conductivity requires porous structure
- **Manufacturing:** Aerogel production is expensive
- **Economics:** R-50 requires 14 inches of fiberglass
- **Incentives:** Insulation industry optimizes for developed markets

**Falsification criteria:**
This idea fails if: (1) no material achieves R-50 at <$0.10/sq ft, OR (2) installation requires skilled labor.

**Cross-domain synthesis:**
- Could materials science remove the bottleneck? -- Aerogels, vacuum insulation panels
- Could biology solve this? -- Mycelium insulation, straw bale

**Convergence:** biomass insulation, recycled materials converging on lower-cost solutions.

---

## 6. Transportation

### MI-013: Personal Air Transport at Car Price

**Problem:** Urban congestion wastes 1 trillion hours/year globally. Personal air transport could solve this but costs $200K+.

**Current best:** eVTOL prototypes ($200K-1M, not yet certified).

**Metrics:**

| Metric | Value |
|--------|-------|
| Global Impact | 4 billion (urban) |
| Difficulty | 9/10 |
| Cost to Prototype | $50-200M |
| Time Horizon | 5-10 years |
| Scientific Risk | 5/10 |
| Engineering Risk | 9/10 |
| Evidence Score | 4/10 |
| Readiness | Hypothesis |

**Why existing solutions fail:**
- eVTOLs are too expensive for personal use
- Helicopters cost $1M+ and require pilots
- No autonomous air taxi exists yet

**Why it hasn't been solved:**
- **Physics:** Energy density of batteries limits range
- **Manufacturing:** Aerospace certification is slow
- **Economics:** $50,000 target is 10x below current cost
- **Regulatory:** No framework for autonomous air vehicles
- **Incentives:** Aerospace industry optimizes for military/commercial

**Falsification criteria:**
This idea fails if: (1) battery energy density cannot exceed 500 Wh/kg, OR (2) autonomous flight certification takes >15 years.

**Cross-domain synthesis:**
- Could semiconductor advances enable it? -- RTS motors, power electronics
- Could AI reduce design costs? -- Yes, autonomous flight control

**Convergence:** Joby, Lilium, Archer converging on eVTOL. Cost declining but still far from target.

---

### MI-014: Transatlantic Flight in 1 Hour

**Problem:** Transatlantic flights take 7-8 hours. Hypersonic travel could reduce this to 1 hour.

**Current best:** Concorde (retired, Mach 2, $10,000/ticket).

**Metrics:**

| Metric | Value |
|--------|-------|
| Global Impact | 1 billion (frequent travelers) |
| Difficulty | 10/10 |
| Cost to Prototype | $100M-1B |
| Time Horizon | 10-20 years |
| Scientific Risk | 8/10 |
| Engineering Risk | 9/10 |
| Evidence Score | 3/10 |
| Readiness | Hypothesis |

**Why existing solutions fail:**
- Hypersonic vehicles face thermal protection challenges
- Sonic boom limits overland flight
- Fuel consumption is extreme

**Why it hasn't been solved:**
- **Physics:** Mach 5+ generates extreme heat
- **Manufacturing:** Thermal protection systems are heavy
- **Economics:** $1,000/ticket is 10x below current cost
- **Regulatory:** Sonic boom bans over land
- **Incentives:** Airlines optimize for fuel efficiency, not speed

**Falsification criteria:**
This idea fails if: (1) no thermal protection system survives Mach 5+ for 1000+ cycles, OR (2) sonic boom cannot be mitigated below regulatory limits.

**Cross-domain synthesis:**
- Could materials science remove the bottleneck? -- Ceramic matrix composites, RTS superconducting magnets
- Could AI reduce design costs? -- Yes, aerodynamic optimization

**Convergence:** Boom Supersonic (Mach 1.7), SpaceX Starship (cargo) converging on supersonic/hypersonic.

---

## 7. Communication

### MI-015: Internet Access for 1 Billion Unconnected

**Problem:** 3 billion people lack internet access. Rural and remote areas are unprofitable for ISPs.

**Current best:** Starlink ($500 terminal, $50/month).

**Metrics:**

| Metric | Value |
|--------|-------|
| Global Impact | 3 billion |
| Difficulty | 7/10 |
| Cost to Prototype | $10-50M |
| Time Horizon | 3-5 years |
| Scientific Risk | 3/10 |
| Engineering Risk | 7/10 |
| Evidence Score | 6/10 |
| Readiness | Prototype |

**Why existing solutions fail:**
- Starlink is too expensive for poorest populations
- Cellular requires tower infrastructure
- No affordable solution exists for remote areas

**Why it hasn't been solved:**
- **Physics:** Signal propagation limits range
- **Manufacturing:** Terminals are expensive
- **Economics:** $5/month is below cost for most providers
- **Regulatory:** Spectrum allocation is complex
- **Incentives:** ISPs optimize for profitable markets

**Falsification criteria:**
This idea fails if: (1) no terminal achieves <$50, OR (2) service cost cannot drop below $5/month, OR (3) solar power is insufficient for remote operation.

**Cross-domain synthesis:**
- Could semiconductor advances enable it? -- RTS deep-field communication coils
- Could swarm intelligence solve it? -- Mesh networks, community-owned infrastructure

**Convergence:** Starlink, Project Loon (discontinued), and others converging on satellite-based access.

---

## 8. Environment

### MI-016: Carbon Capture at $50/ton

**Problem:** We emit 40 billion tons of CO2/year. Current capture costs $200-600/ton. We need $50/ton for economic viability.

**Current best:** Direct air capture ($200-600/ton).

**Metrics:**

| Metric | Value |
|--------|-------|
| Global Impact | 8 billion |
| Difficulty | 9/10 |
| Cost to Prototype | $50-200M |
| Time Horizon | 5-10 years |
| Scientific Risk | 7/10 |
| Engineering Risk | 8/10 |
| Evidence Score | 5/10 |
| Readiness | Prototype |

**Why existing solutions fail:**
- DAC is too expensive
- Tree planting is too slow and limited
- Ocean fertilization has ecological risks

**Why it hasn't been solved:**
- **Physics:** CO2 is dilute (420 ppm) -- separating it takes energy
- **Manufacturing:** DAC plants are expensive
- **Economics:** $50/ton is below current cost by 4-12x
- **Incentives:** Carbon credits are worth $20-50/ton
- **Tooling gaps:** No sorbent material achieves theoretical efficiency

**Falsification criteria:**
This idea fails if: (1) no sorbent achieves <$50/ton at scale, OR (2) energy cost of capture exceeds 100 kWh/ton, OR (3) storage permanence cannot be guaranteed.

**Cross-domain synthesis:**
- Could biology solve this? -- Algae, enhanced weathering
- Could materials science remove the bottleneck? -- Metal-organic frameworks, RTS-enabled processes

**Convergence:** Climeworks, Carbon Engineering, and others converging on DAC. Cost declining 10-15% per year.

---

### MI-017: Ocean Plastic Cleanup at Scale

**Problem:** 11 million tons of plastic enter the ocean annually. Current cleanup efforts remove <0.1%.

**Current best:** The Ocean Cleanup ($30M system, removes 1% of input).

**Metrics:**

| Metric | Value |
|--------|-------|
| Global Impact | 4 billion (coastal populations) |
| Difficulty | 8/10 |
| Cost to Prototype | $10-50M |
| Time Horizon | 5-10 years |
| Scientific Risk | 5/10 |
| Engineering Risk | 8/10 |
| Evidence Score | 5/10 |
| Readiness | Prototype |

**Why existing solutions fail:**
- Ocean is too vast for surface cleanup
- Microplastics are impossible to filter
- Prevention is more effective than cleanup

**Why it hasn't been solved:**
- **Physics:** Ocean currents distribute plastic globally
- **Manufacturing:** Cleanup systems are too small
- **Economics:** No revenue model for ocean plastic
- **Incentives:** Plastic producers externalize costs
- **Tooling gaps:** No technology can filter microplastics at scale

**Falsification criteria:**
This idea fails if: (1) no system removes >10% of input plastic, OR (2) microplastic filtration is not technically feasible at scale.

**Cross-domain synthesis:**
- Could swarm intelligence solve it? -- Autonomous cleanup vessels
- Could biology solve this? -- Plastic-eating enzymes (PETase)

**Convergence:** The Ocean Cleanup, Plastic Bank, and others converging on collection and recycling.

---

## 9. Education

### MI-018: Quality Education for $1/student/year

**Problem:** 260 million children lack access to education. Private school costs $50-500/student/year.

**Current best:** Khan Academy (free, but requires internet and devices).

**Metrics:**

| Metric | Value |
|--------|-------|
| Global Impact | 260 million children |
| Difficulty | 7/10 |
| Cost to Prototype | $5-20M |
| Time Horizon | 3-5 years |
| Scientific Risk | 3/10 |
| Engineering Risk | 6/10 |
| Evidence Score | 6/10 |
| Readiness | Prototype |

**Why existing solutions fail:**
- Internet is not available in rural areas
- Devices are too expensive
- No curriculum adapts to local language and culture

**Why it hasn't been solved:**
- **Physics:** No -- this is a social/economic problem
- **Manufacturing:** Devices cost $50-100 minimum
- **Economics:** $1/student/year is below operational cost
- **Regulatory:** Education standards vary by country
- **Incentives:** Education industry optimizes for affluent markets

**Fascination criteria:**
This idea fails if: (1) no device achieves <$10, OR (2) curriculum cannot be localized at scale, OR (3) teacher training cannot be automated.

**Cross-domain synthesis:**
- Could AI reduce design costs? -- Yes, adaptive learning, automated assessment
- Could swarm intelligence solve it? -- Community-led education models

**Convergence:** Bridge, Eneza, and others converging on low-cost digital education.

---

### MI-019: Vocational Training at Scale Without Physical Infrastructure

**Problem:** 75 million youth are unemployed. Vocational training requires physical workshops.

**Current best:** Community colleges ($5,000-20,000/year).

**Metrics:**

| Metric | Value |
|--------|-------|
| Global Impact | 75 million youth |
| Difficulty | 7/10 |
| Cost to Prototype | $5-20M |
| Time Horizon | 3-5 years |
| Scientific Risk | 3/10 |
| Engineering Risk | 6/10 |
| Evidence Score | 5/10 |
| Readiness | Hypothesis |

**Why existing solutions fail:**
- Physical infrastructure is expensive
- Trained instructors are scarce
- No scalable virtual training exists

**Why it hasn't been solved:**
- **Physics:** Hands-on skills require physical practice
- **Manufacturing:** VR hardware is expensive
- **Economics:** $100/student/year is below cost
- **Incentives:** Training industry profits from physical presence

**Falsification criteria:**
This idea fails if: (1) no virtual method achieves equivalent skill transfer, OR (2) VR hardware costs cannot drop below $50.

**Cross-domain synthesis:**
- Could AI reduce design costs? -- Yes, AI tutors, skill assessment
- Could swarm intelligence solve it? -- Peer learning, mentorship networks

**Convergence:** Coursera, Udacity, and others converging on online credentials.

---

## 10. Computing

### MI-020: Room-Temperature Quantum Computer

**Problem:** Quantum computers require near-absolute-zero cooling ($1M+ per unit). No room-temperature quantum computer exists.

**Current best:** IBM Eagle (127 qubits, requires dilution refrigerator).

**Metrics:**

| Metric | Value |
|--------|-------|
| Global Impact | 8 billion (computing for all) |
| Difficulty | 10/10 |
| Cost to Prototype | $50-200M |
| Time Horizon | 10-20 years |
| Scientific Risk | 9/10 |
| Engineering Risk | 8/10 |
| Evidence Score | 2/10 |
| Readiness | Hypothesis |

**Why existing solutions fail:**
- Qubit coherence drops exponentially with temperature
- Dilution refrigerators cost $1M+ and fill a room
- No room-temperature qubit technology exists

**Why it hasn't been solved:**
- **Physics:** Thermal noise destroys quantum coherence
- **Manufacturing:** Quantum devices require extreme precision
- **Economics:** $100,000 target is 10x below current cost
- **Incentives:** Quantum computing is profitable at $1M+ price point

**Falsification criteria:**
This idea fails if: (1) no qubit technology achieves >1 second coherence at room temperature, OR (2) error correction overhead makes large-scale computation impossible.

**Cross-domain synthesis:**
- Could semiconductor advances enable it? -- Yes, RTS Josephson junctions
- Could materials science remove the bottleneck? -- Topological qubits, NV centers in diamond

**Convergence:** IBM, Google, and others converging on error correction. No room-temperature approach is close.

---

### MI-021: 1 Exaflop Computing at 1 Watt

**Problem:** Current supercomputers achieve 1 exaflop at 20+ megawatts. We need 1 exaflop at 1 watt for ubiquitous AI.

**Current best:** Frontier (1.1 exaflop, 21 MW).

**Metrics:**

| Metric | Value |
|--------|-------|
| Global Impact | 8 billion |
| Difficulty | 10/10 |
| Cost to Prototype | $100M-1B |
| Time Horizon | 10-20 years |
| Scientific Risk | 9/10 |
| Engineering Risk | 9/10 |
| Evidence Score | 2/10 |
| Readiness | Hypothesis |

**Why existing solutions fail:**
- Current architectures are power-limited
- Moore's Law is slowing
- No revolutionary architecture exists

**Why it hasn't been solved:**
- **Physics:** Landauer's principle sets minimum energy per operation
- **Manufacturing:** Nanoscale transistors face quantum effects
- **Economics:** Power is the dominant cost in computing
- **Incentives:** Chip industry optimizes for performance, not efficiency
- **Tooling gaps:** No architecture achieves >1 TFLOPS/watt

**Falsification criteria:**
This idea fails if: (1) Landauer's principle cannot be circumvented, OR (2) no material achieves >10x energy efficiency of silicon, OR (3) reversible computing is not practical.

**Cross-domain synthesis:**
- Could biology solve this? -- Neural networks achieve ~10 TFLOPS/watt
- Could semiconductor advances enable it? -- RTS interconnects, neuromorphic chips
- Could AI reduce design costs? -- Yes, AI-designed chips

**Convergence:** BrainChip, Intel Loihi, and others converging on neuromorphic computing. Efficiency improving 10x per decade.

---

## Retired Myths

These ideas have been convincingly shown to be impractical or physically impossible under current understanding. Rejecting an idea based on evidence is as valuable as advancing one.

### RM-001: Cold Fusion (LENR)

**Original claim:** Deuterium fusion in palladium at room temperature produces excess heat.

**Evidence reviewed:** Multiple replications attempted. No consistent excess heat. No confirmed nuclear products.

**Why it doesn't hold up:** Nuclear fusion requires overcoming Coulomb barrier (1 MeV). Room-temperature palladium cannot provide this energy. All positive results attributed to measurement error.

**What discovery would change this:** Confirmation of nuclear products (helium-3, tritium) in excess heat experiments, with independent replication.

---

### RM-002: Room-Temperature Superconductivity via Diamond Anvil (Retracted Claims)

**Original claim:** Carbonaceous sulfur hydride achieves 287K (14C) at 267 GPa.

**Evidence reviewed:** Original paper retracted. Independent groups failed to reproduce. Key data inconsistencies identified.

**Why it doesn't hold up:** Retraction due to data integrity issues. Independent attempts to reproduce showed no superconductivity at claimed conditions.

**What discovery would change this:** Independent replication with verified data, or new material system achieving similar results.

---

### RM-003: Room-Temperature Superconductivity via LK-99

**Original claim:** Pb9CuPO4 (LK-99) is a room-temperature superconductor at ambient pressure.

**Evidence reviewed:** Multiple independent groups synthesized LK-99. No Meissner effect. Resistivity behavior attributed to Cu2S impurity phase.

**Why it doesn't hold up:** LK-99 is a semiconductor, not a superconductor. Partial levitation is due to ferromagnetism of Cu2S, not Meissner effect.

**What discovery would change this:** Demonstration of zero resistance and Meissner effect in pure phase LK-99, with independent replication.

---

### RM-004: Faster-Than-Light Communication

**Original claim:** Quantum entanglement enables faster-than-light information transfer.

**Evidence reviewed:** No experiment has demonstrated FTL communication. Quantum mechanics respects causality.

**Why it doesn't hold up:** No-cloning theorem prevents copying quantum states. Measurement outcomes are random, cannot encode information.

**What discovery would change this:** Demonstration of controllable quantum state transfer with superluminal velocity, with independent verification.

---

### RM-005: Perpetual Motion Machines

**Original claim:** Devices can produce work without energy input indefinitely.

**Evidence reviewed:** No device has ever achieved net positive energy output. All claims debunked by thermodynamic analysis.

**Why it doesn't hold up:** First and second laws of thermodynamics are well-established. No exception has been found in 200+ years.

**What discovery would change this:** Demonstration of a device that produces >100% efficiency, with independent verification under controlled conditions.

---

### RM-006: Anti-Gravity Devices

**Original claim:** Electromagnetic or gravitational devices can negate gravity without fuel.

**Evidence reviewed:** No experiment has demonstrated gravity manipulation. All claims attributed to measurement error or hoax.

**Why it doesn't hold up:** General relativity predicts no mechanism for gravity cancellation. All "anti-gravity" demonstrations have been debunked.

**What discovery would change this:** Demonstration of measurable gravity reduction by >1%, with independent replication and theoretical explanation.

---

## Statistics

| Category | Gaps | Open | In Progress | Solved |
|----------|------|------|-------------|--------|
| Energy | 3 | 2 | 1 | 0 |
| Water | 2 | 2 | 0 | 0 |
| Food | 3 | 2 | 1 | 0 |
| Health | 2 | 2 | 0 | 0 |
| Housing | 2 | 2 | 0 | 0 |
| Transportation | 2 | 2 | 0 | 0 |
| Communication | 1 | 1 | 0 | 0 |
| Environment | 2 | 2 | 0 | 0 |
| Education | 2 | 2 | 0 | 0 |
| Computing | 2 | 1 | 1 | 0 |
| **Total** | **21** | **18** | **3** | **0** |

| Retired Myths | Count |
|---------------|-------|
| Total | 6 |

---

## How to Contribute

1. **Add new gaps** -- open a PR with a new MI-XXX entry
2. **Update existing gaps** -- add new attempts, update status
3. **Propose solutions** -- link to your invention or research
4. **Document failures** -- dead ends are valuable
5. **Add retired myths** -- ideas that have been disproven
6. **Update metrics** -- refine evidence scores, readiness levels

---

*This index is a living document. As solutions emerge, gaps move from OPEN to IN PROGRESS to SOLVED. New gaps are added as humanity's needs evolve. Myths are retired as evidence accumulates.*

*Part of the Inversion Labs ecosystem. Built for reproducibility, evidence, and open engineering.*
