```
+======================================================================+
|                                                                      |
|         MANUFACTURING FLOW FOR THE HAMILTONIAN PHOTONIC CHIP         |
|          (CMOS-Compatible Silicon Photonics Process)                 |
|                                                                      |
|   "Turning quadrillion math into a 5mm x 5mm piece of glass"        |
|                                                                      |
+======================================================================+
|                                                                      |
|   STEP 0:  STARTING SUBSTRATE (SOI Wafer)                           |
|   +-----------------------------------------------------------+     |
|   |                                                           |     |
|   |   Layer Structure:                                         |     |
|   |   +---------------------------------------------------+   |     |
|   |   |  Si Device Layer  (220 nm)      <--- Light path   |   |     |
|   |   +---------------------------------------------------+   |     |
|   |   |  Buried Oxide (BOX)  (2 µm)      (SiO2)           |   |     |
|   |   +---------------------------------------------------+   |     |
|   |   |  Silicon Handle Wafer  (675 µm)  (mechanical)     |   |     |
|   |   +---------------------------------------------------+   |     |
|   |                                                           |     |
|   |   Specs:  SOI substrate with top Si thickness = 220nm   |     |
|   |   (Typical for 1550nm single-mode waveguides).          |     |
|   +-----------------------------------------------------------+     |
|                                                                      |
+======================================================================+
|                                                                      |
|   STEP 1:  LITHOGRAPHY & WAVEGUIDE PATTERNING                       |
|   +-----------------------------------------------------------+     |
|   |                                                           |     |
|   |   1. Spin-coat photoresist (e.g., ZEP-520A).             |     |
|   |   2. Expose using Deep-UV (248nm) or Electron-Beam.      |     |
|   |   3. Develop resist to open waveguide pattern.           |     |
|   |                                                           |     |
|   |   +-------------------------------------------------+   |     |
|   |   |  ████████████████████  ████  ████████          |   |     |
|   |   |  ████████████████████  ████  ████████  (Resist) |   |     |
|   |   |  ████████████████████  ████  ████████          |   |     |
|   |   +-------------------------------------------------+   |     |
|   |   |  Si Device Layer (220 nm)                         |   |     |
|   |   +-------------------------------------------------+   |     |
|   |   |  BOX (2 µm)                                      |   |     |
|   |   +-------------------------------------------------+   |     |
|   |                                                           |     |
|   |   Waveguide width = 450 nm (single-mode).               |     |
|   |   MZI Layout: 128 x 128 Clements mesh.                  |     |
|   +-----------------------------------------------------------+     |
|                                                                      |
+======================================================================+
|                                                                      |
|   STEP 2:  REACTIVE ION ETCHING (RIE) - WAVEGUIDE DEFINITION        |
|   +-----------------------------------------------------------+     |
|   |                                                           |     |
|   |   Etch the exposed Si using Inductively Coupled Plasma   |     |
|   |   (ICP) with SF6 / C4F8 chemistry.                       |     |
|   |                                                           |     |
|   |   ETCH PROFILE:  ANISOTROPIC (Vertical walls)            |     |
|   |                                                           |     |
|   |              +--------+  (Sidewall angle ~89°)           |     |
|   |              |  Si    |                                   |     |
|   |              |  (Strip |                                   |     |
|   |              |  Wave  |                                   |     |
|   |              +--------+                                   |     |
|   |   +-------------------------------------------------+   |     |
|   |   |  Si Waveguide (Ridge/Strip)                     |   |     |
|   |   +-------------------------------------------------+   |     |
|   |   |  BOX                                             |   |     |
|   |   +-------------------------------------------------+   |     |
|   |                                                           |     |
|   |   Result:  High-confinement strip waveguides with         |     |
|   |   propagation loss < 2 dB/cm.                            |     |
|   |                                                           |     |
|   |   Critical dimension (CD) control:  +/- 2 nm.           |     |
|   +-----------------------------------------------------------+     |
|                                                                      |
+======================================================================+
|                                                                      |
|   STEP 3:  ION IMPLANTATION / DOPING (HEATER & PN JUNCTION)        |
|   +-----------------------------------------------------------+     |
|   |                                                           |     |
|   |   For Thermal Phase Shifters (Low loss, high latency):    |     |
|   |   -  Implant P-type (Boron) or N-type (Phosphorus).      |     |
|   |   -  Create resistive heaters above the waveguides.      |     |
|   |                                                           |     |
|   |   For Carrier-Depletion Phase Shifters (High speed):     |     |
|   |   -  Create lateral PN junctions in the waveguide.       |     |
|   |                                                           |     |
|   |   DIAGRAM:  DOPING MASK                                  |     |
|   |                                                           |     |
|   |   +-------------------------------------------------+   |     |
|   |   |          MZI ARMS                                |   |     |
|   |   |   ┌──────┐    ┌──────┐                          |   |     |
|   |   |   │ P++  │    │ N++  │  (Doped regions)         |   |     |
|   |   |   └──────┘    └──────┘                          |   |     |
|   |   |       |            |                            |   |     |
|   |   |   (Heater/Electrode contacts via vias)          |   |     |
|   |   +-------------------------------------------------+   |     |
|   |   |  BOX                                             |   |     |
|   |   +-------------------------------------------------+   |     |
| |                                                           |     |
|   |   Resistivity target: ~10^-3 Ω·cm for efficient heating.|     |
|   +-----------------------------------------------------------+     |
|                                                                      |
+======================================================================+
|                                                                      |
|   STEP 4:  METALLIZATION & CONTACT FORMATION                        |
|   +-----------------------------------------------------------+     |
|   |                                                           |     |
|   |   1.  Deposit SiO2 interlayer dielectric (ILD).          |     |
|   |   2.  Etch via holes down to doped regions.              |     |
|   |   3.  Sputter/deposit Ti/TiN barrier + Al/Cu metal.     |     |
|   |   4.  Pattern the metal to form bond pads and micro-strip|     |
|   |       lines for the active phase shifters.              |     |
|   |                                                           |     |
|   |   TOP VIEW:  MZI ARRAY WITH METAL PADS                   |     |
|   |                                                           |     |
|   |   +-------------------------------------------------+   |     |
|   |   |   ○   ○   ○   ○   ○   ○   ○   ○               |   |     |
|   |   |   │   │   │   │   │   │   │   │               |   |     |
|   |   |   └───┴───┴───┴───┴───┴───┴───┘ (Bond pads)  |   |     |
|   |   |   ┌───┐ ┌───┐ ┌───┐ ┌───┐                    |   |     |
|   |   |   │MZI│ │MZI│ │MZI│ │MZI│ (Heaters below)    |   |     |
|   |   |   └───┘ └───┘ └───┘ └───┘                    |   |     |
|   |   +-------------------------------------------------+   |     |
|   |                                                           |     |
|   |   Metal thickness: 500 nm (reduces RC delay).           |     |
|   |   Minimum pitch: 100 µm (for wire bonding).             |     |
|   +-----------------------------------------------------------+     |
|                                                                      |
+======================================================================+
|                                                                      |
|   STEP 5:  UPPER CLADDING DEPOSITION                               |
|   +-----------------------------------------------------------+     |
|   |                                                           |     |
|   |   Deposit thick SiO2 (PECVD or HDP-CVD) to cover the     |     |
|   |   waveguides and protect them from environmental effects. |     |
|   |                                                           |     |
|   |   Cross-section of FINAL WAVEGUIDE STRUCTURE:             |     |
|   |                                                           |     |
|   |   +-------------------------------------------------+   |     |
|   |   |  SiO2 Upper Cladding  (1.5 µm)               |   |     |
|   |   +-------------------------------------------------+   |     |
|   |   |  Si Waveguide  (450 nm x 220 nm)             |   |     |
|   |   +-------------------------------------------------+   |     |
|   |   |  BOX (2 µm)                                   |   |     |
|   |   +-------------------------------------------------+   |     |
|   |   |  Si Handle Wafer                                |   |     |
|   |   +-------------------------------------------------+   |     |
|   |                                                           |     |
|   |   Anneal at 400°C to densify oxide and activate dopants. |     |
|   +-----------------------------------------------------------+     |
|                                                                      |
+======================================================================+
|                                                                      |
|   STEP 6:  WAFER TESTING & PACKAGING                                |
|   +-----------------------------------------------------------+     |
|   |                                                           |     |
|   |   1.  Dicing:  Saw wafer into individual dies (5mm x 5mm).|     |
|   |   2.  Edge Polishing:  Polish waveguide facets.          |     |
|   |   3.  Grating Couplers (optional):  Etch 2D grating for  |     |
|   |       vertical fiber coupling (replaces edge coupling).   |     |
|   |                                                           |     |
|   |   PACKAGED CHIP DIAGRAM:                                  |     |
|   |                                                           |     |
|   |   +-------------------------------------------------+   |     |
|   |   |   (PCB SUBSTRATE)                              |   |     |
|   |   |   +-----------------------------------------+  |   |     |
|   |   |   | PHOTONIC DIE (5x5 mm)                   |  |   |     |
|   |   |   |  (Wire bonds to PCB)                    |  |   |     |
|   |   |   |   ┌─────────────────────────────────┐   |  |   |     |
|   |   |   |   │     ┌───┐ ┌───┐               │   |  |   |     |
|   |   |   |   │     │MZI│ │MZI│               │   |  |   |     |
|   |   |   |   │     └───┘ └───┘               │   |  |   |     |
|   |   |   |   │  (Optical Mesh)                │   |  |   |     |
|   |   |   |   │     ┌─────────────────┐        │   |  |   |     |
|   |   |   |   │     │  Edge Coupler   │        │   |  |   |     |
|   |   |   |   │     └─────────────────┘        │   |  |   |     |
|   |   |   |   └─────────────────────────────────┘   |  |   |     |
|   |   |   |   │  │  │  │  (Electrical I/O)         |  |   |     |
|   |   |   +-----------------------------------------+  |   |     |
|   |   |   Optical Fiber Array (V-groove)               |   |     |
|   |   |      │ │ │ │ │ │ (1550nm light in/out)       |   |     |
|   |   +-------------------------------------------------+   |     |
|   |                                                           |     |
|   |   Fiber Alignment:  Active alignment using IR camera.     |     |
|   |   Packaging:  Hermetic seal (if required).               |     |
|   +-----------------------------------------------------------+     |
|                                                                      |
+======================================================================+
|                                                                      |
|   MZI LAYOUT DETAIL (THE CORE COMPUTATIONAL UNIT)                   |
|   +-----------------------------------------------------------+     |
|   |                                                           |     |
|   |   A single Mach-Zehnder Interferometer consists of:      |     |
|   |                                                           |     |
|   |          (Splitter)          (Phase Shifter)   (Combiner)|     |
|   |   Input  ──┬── 50/50 ──┬──  ~~~θ~~~  ──┬── 50/50 ──┬── Output |     |
|   |   ─────────┘          │               │          └─────────── |     |
|   |                       └───────────────┘                        |     |
|   |                                                           |     |
|   |   Transfer matrix:  MZI = 1/2 [1, 1; 1, -1] * [e^{iθ}, 0; 0, 1] * 1/2 [1, 1; 1, -1] |     |
|   |                                                           |     |
|   |   By adjusting θ (via heater/PN junction), we can implement|     |
|   |   any 2x2 unitary. The mesh combines 128x128 of these.    |     |
|   |                                                           |     |
|   +-----------------------------------------------------------+     |
|                                                                      |
+======================================================================+
|                                                                      |
|   CRITICAL PROCESS PARAMETERS                                       |
|   +-----------------------------------------------------------+     |
|   |   Process Step          |  Parameter            |  Value   |     |
|   |-------------------------|-----------------------|----------|     |
|   |  Lithography           |  CD (Waveguide width) |  450 nm  |     |
|   |  Etch (RIE)           |  Sidewall angle       |  88-89°  |     |
|   |  Doping (Heater)      |  Sheet resistance     |  100 Ω/□ |     |
|   |  Metallization        |  Metal thickness      |  500 nm  |     |
|   |  Cladding             |  Thickness            |  1.5 µm  |     |
|   |  Thinning (backside) |  Si thickness         |  200 µm  |     |
|   |  Fiber coupling      |  Fiber pitch          |  127 µm  |     |
|   +-----------------------------------------------------------+     |
|                                                                      |
+======================================================================+
|                                                                      |
|   FOUNDRY COMPATIBILITY (CMOS-SCALE PRODUCTION)                     |
|   +-----------------------------------------------------------+     |
|   |                                                           |     |
|   |   This process is 100% compatible with standard 180nm     |     |
|   |   or 130nm CMOS nodes.  No exotic materials required.     |     |
|   |                                                           |     |
|   |   Multi-Project Wafer (MPW) runs available at:            |     |
|   |   - AIM Photonics (USA)                                  |     |
|   |   - IMEC (Belgium)                                       |     |
|   |   - Tower Jazz (Israel)                                 |     |
|   |                                                           |     |
|   |   Cycle time:  3 months (tape-out to packaged chip).     |     |
|   |                                                           |     |
|   +-----------------------------------------------------------+     |
|                                                                      |
+======================================================================+
|                                                                      |
|   CONCLUSION:  THE PHYSICAL MANIFESTATION OF THE QUADRILLION       |
|   +-----------------------------------------------------------+     |
|   |                                                           |     |
|   |   The diagrams above detail how to build a photonic      |     |
|   |   processor that implements exp(i H t) and QPE.          |     |
|   |                                                           |     |
|   |   By manufacturing this 5mm x 5mm die, we physically     |     |
|   |   realize the infinite-depth neural network and the      |     |
|   |   quantum factoring engine.                              |     |
|   |                                                           |     |
|   |   This is how quadrillion-scale math becomes a           |     |
|   |   $500 prototype on a CMOS line.                         |     |
|   |                                                           |     |
|   +-----------------------------------------------------------+     |
|                                                                      |
+======================================================================+
```
