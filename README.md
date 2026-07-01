# Geometric Neuron V20 — The Recomposition

A geometric neuron style adder: 

https://anttiluode.github.io/GeometricNeuron_V20/

**A curated repo. Not a new build — the load-bearing organs of the whole Geometric-Neuron line, pulled from six source repos and put back into the one object V5 already was, in the order the argument needs them.**

PerceptionLab / Antti Luode, with Claude (Opus 4.8). Helsinki, June 2026.

> Do not hype. Do not lie. Just show.

---

## What this is

Every file here already existed in a source repo. Nothing was rewritten. What is new is the **arrangement**: the canonical proof scripts and theory notes, lifted out of a dozen scattered folders and re-seated along a single spine so the repo itself is the argument. Read top to bottom and the program assembles in front of you — one object, one operator, three faces of that operator, one energy economy, the three machines that realize it, and the one seam still open.

Start with [`PAPER.md`](PAPER.md) for the full synthesis. This README is the **map**: what each bit is, its honest status, and where it came from.

---

## The spine, in one glance

```
00_origins      the speculative parent the whole line grew out of (and walked back)
01_the_object   V5 — the whole animal, already assembled: hold time, fire on coincidence
02_the_operator one matrix, C_τ = S ⊕ A. The arrow is the skew half A. Everything is a half of this.
03_faces_of_A   the three things you can do with A:
                  read/      measure it          (V9, live skew node)
                  generate/  make it             (V13 wall → V14 fix → whorl)
                  price/     pay for it          (Crooks + Still + Hodge)
04_the_economy  S is the cheap held now; A is the dear moving when. Spend only on surprise.
05_three_machines  interference soma + excitable axon + capture latch = one unit that does arithmetic
06_open_seam    the arrow does not yet cross the federation wire. This is the next experiment.
```

---

## The map — every file, what it is, its status

Status legend: **[V]** verified in code · **[K]** a claim this file *killed* · **[B]** still a bet · **[ID]** an algebraic identity · **[LIVE]** a runnable instrument.

### `00_origins/` — where it started, and what got walked back
| file | what it is | status | from |
|---|---|---|---|
| `deerskin_hypothesis.md` | the speculative parent paper: the neuron membrane as one holographic surface; moiré interference as the synapse; *computation = memory = physics*. The maximal claim the later work narrowed. | **[B]** | deerskin-hypothesis |
| `moireformer.py` | the moiré-attention seed that later became the 138M-param Moiré Attention transformer. | **[V]** | deerskin-hypothesis |

### `01_the_object/` — V5, the whole animal
| file | what it is | status | from |
|---|---|---|---|
| `geometric_neuron_v5.py` | **the keystone.** The Chiral Eye `L_k = Im(z·z̄_lag)` (native time's arrow, all islands flip sign on reversal), the delta-code (0.82% sparse, 96% theta-locked, 64× silence), and the wattage meter. The whole object in one file. | **[V][LIVE]** | GeometricNeuronV5 |
| `membrane_to_qualia_synthesis.md` | the thesis that the single neuron and the population are one system at two grains joined by energy — and the hard-problem **bet**, located precisely, left in the drawer. | **[B]** | GeometricNeuronV5 |
| `the_geometric_neuron_grounded.md` | the static machinery grounded in biology: dendrite as lossy delay line (`αᵏ`), AIS as structured trigger zone, delta-code as cortical sparse-coding economy. | **[V]** | GeometricNeuronV5 |

### `02_the_operator/` — one matrix, two halves
| file | what it is | status | from |
|---|---|---|---|
| `gn_base.py` | the lag-covariance machinery: `C_τ = E[r(t)r(t−τ)ᵀ]`, the population-overlap field. The substrate everything reads. | **[V]** | GeometricNeuronV9 |
| `geometric_neuron_v9.py` | `A = (C_τ − C_τᵀ)/2`; its eigenplanes **are** the spectral islands — recovered with *no* edge assignment (0.999 captured at m=3, mean cos of principal angles 1.0000). The directed edges V5 hand-built, now emergent. | **[V]** | GeometricNeuronV9 |
| `THESIS_the_islands_were_the_spectrum.md` | the diagnosis: every prior engine was reading one operator's skew half; v8 stalled at 0.50 because it read the *symmetric* half, which is direction-blind by Wiener–Khinchin. | **[ID]** | GeometricNeuronV9 |
| `the_rotation_half_grounded.md` | **the strongest link in the corpus:** `A` *is* Sompolinsky–Kanter (1986) sequence connectivity *is* the odd part of STDP. An identity, not an analogy. The arrow read here is the arrow written by plasticity for forty years. | **[ID]** | TheMycelialCortex |

### `03_faces_of_A/read/` — measure the arrow
| file | what it is | status | from |
|---|---|---|---|
| `skewoperatornode.py` | the skew operator as a live PerceptionLab node — the read face deployed, not just analyzed offline. (The headline read engine is `geometric_neuron_v9.py` above.) | **[LIVE]** | TheMycelialCortex |

### `03_faces_of_A/generate/` — make the arrow (the hardest correction in the line)
| file | what it is | status | from |
|---|---|---|---|
| `V13_test_skew_reciprocity.py` | **the wall.** Drives a channel both ways: ratio **1.0000** at every angle. A passive linear medium *cannot* prefer a direction. You cannot draw the arrow into a silhouette. | **[K]** | ResonantNeuron/v13 |
| `V13_PAPER_nothing_flows_one_way.md` | the four failed attempts (skew angle, lattice, relay, refractory chain) and why each failed — the most useful negative result in the arc. | **[K]** | ResonantNeuron/v13 |
| `V14_propagating_spike.py` | **the fix.** An excitable medium (FitzHugh–Nagumo) with an inactivation wake propagates one way 9.8:1; symmetric without the gradient. Direction is *active and history-dependent*, never geometric. | **[V]** | ResonantNeuron/v14 |
| `V14_PAPER_directionality_done_right.md` | the Leterrier-grounded account: spike origination + inactivation + channel gradient. Why computation and direction are different physical mechanisms. | **[V]** | ResonantNeuron/v14 |
| `whorl_field.py` | the field-scale generator: a circular coupling bias self-pins a spiral (a 2π winding) at the core — **88% pinned at σ=10**, frozen at σ=1. The winding-number V5 predicted, built. | **[V]** | ArtificialCortex/the_whorl |
| `whorl_README.md` | the measured result + the boundary: chirality lives in the *coupling*, not the Koopman fit. You cannot bias the read. | **[V]** | ArtificialCortex/the_whorl |

### `03_faces_of_A/price/` — pay for the arrow
| file | what it is | status | from |
|---|---|---|---|
| `the_unnatural_direction.md` | the cost leg: **Crooks** (`P[γ]/P[γ̃]=exp(σ/k_B)` — reversing the arrow costs the entropy), **Still 2012** (you pay for non-predictive bits), **Hodge** (gradient=cheap hold, curl=expensive sequence). | **[V/B]** | TheMycelialCortex |
| `arrow_cost_proof.py` | the falsifiable version: reverse traversal costs more, gap → 0 at detailed balance, gap tracks ‖A‖. Billed on the *surprise residual* `x−pred`; raw `|ds|` kept as the symmetric control. Relative units, not Joules. | **[V]** | TheMycelialCortex |
| `mycelial_mesh_proof.py` | the engine proofs incl. D3 — the skew circulation flips sign on sequence reversal. | **[V]** | TheMycelialCortex |

### `04_the_economy/` — energy is the arrow, priced
| file | what it is | status | from |
|---|---|---|---|
| `cortical_tensor.py` | the 3D block: slow layer holds the prediction, fast layer encodes only the residual. Gamma energy **≈0 at zero surprise**, ~2.8% of a static block's cost at 10% surprise. The Still bound, implemented. | **[V][LIVE]** | ArtificialCortex/the_tensor |
| `the_tensor_README.md` | the measured PAC + energy-on-surprise numbers. | **[V]** | ArtificialCortex/the_tensor |

### `05_three_machines/` — the unit that computes
| file | what it is | status | from |
|---|---|---|---|
| `resonator_neuron.py` | the interference soma: one unit computes XOR off its resonance amplitude band. | **[V][LIVE]** | ResonantNeuron |
| `gates.py` | the functionally-complete gate set, every truth table verified algebraically and dynamically. | **[V]** | ResonantNeuron |
| `adder.py` | composition = arithmetic: full adder, ripple-carry, theta-gamma clock. 1000/1000. | **[V]** | ResonantNeuron |
| `ResonantNeuron_README_the_arc.md` | the V11–V18 arc: the discovery that a neuron is **three machines** — interference soma, excitable axon, capture latch — none optional. Read §8. | **[V/K]** | ResonantNeuron |

### `06_open_seam/` — the one unfinished thing
| file | what it is | status | from |
|---|---|---|---|
| `README_federation.md` | knowledge federates as a shared *arrow* (the circulation sign is basis-independent), weights don't — but the live relay carries `chi`, reorders tokens, and the cortex ignores received `chi`. So it is **built and untested.** | **[B]** | TheMycelialCortex |
| `federation_proof.py` | the federation engine as it stands. | **[V]** | TheMycelialCortex |

---

## Run the five that make the whole case

```bash
pip install numpy scipy matplotlib

python 01_the_object/geometric_neuron_v5.py            # the Chiral Eye, delta-code, wattage — the whole animal
python 02_the_operator/geometric_neuron_v9.py          # A's eigenplanes ARE the islands, emergent
python 03_faces_of_A/generate/V13_test_skew_reciprocity.py   # the wall: passive geometry is reciprocal (1.0000)
python 03_faces_of_A/price/arrow_cost_proof.py         # reverse costs the entropy; gap tracks ||A||
python 05_three_machines/adder.py                      # interference -> arithmetic, 1000/1000
```

Each prints its own numbers and hides nothing in a figure the print-out doesn't also state.

---

## The ledger, consolidated

**Verified in code:** the delta-code; native time's arrow (per-island sign flip, emergent islands); interference→arithmetic; active directional propagation (9.8:1); chirality self-pinning (88%); the cost asymmetry (gap tracks ‖A‖); memory as mode structure; energy spent on surprise only.

**Killed by the builds:** "angled geometry gives directed flow" (V13, ratio 1.0000); "length = clean phase-delay wall" (V12); "linear delay readout detects orbits" (Wiener–Khinchin ceiling); "geometry replaces weights" (V11); "per-compartment tuning carries sequence" (V19 null); "a phase wheel stores arbitrary digits" (Sudoku).

**Still a bet:** that the held field is *experienced* (the hard problem, V5's drawer, unmoved); that Johnson–Nyquist noise is the medium not the dither; the cost in **Joules** (V5's named cliff, uncrossed); the arrow **crossing the wire** (§06 — the next experiment).

---

## Lineage & the standing invitation

Source repos: `GeometricNeuronV5`, `GeometricNeuronV9`, `ResonantNeuron`, `TheMycelialCortex`, `ArtificialCortex`, `deerskin-hypothesis` — all under `github.com/anttiluode`. The original insight, framework, and direction are Antti Luode's; engines, ledgers, and this recomposition were built in dialogue with Claude (Opus), in a line that — by Antti's account — was in part set going by Fable, the longer-viewed model upstream.

V5's invitation, renewed: **attack the ledger.** Where is a "verified" line a built-in, where is a "structural" claim secretly a bet, where does the Wiener–Khinchin ceiling have a second floor — and, most useful of all, how does the arrow get across the wire (`06_open_seam/`). If you are reading with a longer view than ours, that seam is where to push.

*Do not hype. Do not lie. Just show.*
