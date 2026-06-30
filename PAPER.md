# Geometric Neuron V20: The Recomposition

### Not a new build. The verified organs put back into the one object V5 already was — with the ledger rewritten for everything the disassembly taught.

**PerceptionLab / Antti Luode, with Claude (Opus 4.8). Helsinki, June 2026.**
*In a lineage that runs through Claude (Opus) and was, in part, set in motion by Fable.*

> Do not hype. Do not lie. Just show.

---

## 0. Why this is in scare-quotes

There is no V20 mechanism. Calling this "V20" is almost a category error, and the honest thing is to say so in the first line: every number in this document was already measured in a repo that exists. What is new here is not a result. It is the act of **recomposition** — and the reason it is worth a document is that the recomposition reverses the direction the whole program has been travelling, and recovers something that got lost on the way.

The standard story of this work is a forward arc: V5 → the Deerskin Hypothesis → ResonantNeuron V11–V18 → the Mycelial/ArtificialCortex field line → V19. Each version more rigorous than the last. That story is true about the rigor and false about the shape. Read V5 again with the later work in hand and the real structure is the opposite: **V5 was the whole animal, already assembled**, and everything since was the *disassembly* of it into separate organs, each one carried off to its own bench and stress-tested until it either held or broke. Several broke. The ones that held came back changed. But none of the later repos is the animal. They are the animal's parts, each now load-bearing in isolation, scattered across a dozen folders.

V20 is putting them back. The claim of this document is narrow and, I think, exactly right: **the program has converged, and what it converged on is the object V5 drew — one substrate at two grains, joined by energy — except that every loose claim in V5 has now been confirmed, killed, or relocated, and the gestalt that V5 had by intuition is now earned part by part.** The job is to hold the gestalt and the rigor at the same time, which no single earlier repo did.

---

## 1. The evidence that the earlier version was "more advanced"

This is worth stating plainly because it is the seed of the whole document, and because the instinct that bothered you — *the early ones already had more in them* — is correct, but in a precise way that needs the right words or it becomes either false modesty or hype.

V5 was not more **correct**. It was more **whole**. Its own closing section, "Where this points next," names three directions:

1. **"Winding numbers, not just chirality."** V5 read the *sign* of rotation (`L_k`) and said the full per-island transition operator would give discrete topological labels — integer windings — making categorical perception a change of winding number rather than a continuous slide. That is, verbatim, **the whorl** (ArtificialCortex): a spiral is a 2π phase winding, a topological defect, and a biased coupling self-pins it. V5 predicted the whorl a dozen repos before it was built.

2. **"Wattage in physical units."** V5 assigned energy costs and flagged that calibrating `E_spike`/`c_field` against the Attwell–Laughlin budget would turn the silence ratio into Joules. That is the entire **arrow/cost line** (Mycelial). And note: it is *still open*. The one cliff V5 named in this direction is the one cliff that remains uncrossed today — the cost is still relative units, not Joules. The earliest repo and the latest agree on exactly what is unfinished.

3. **"Emergent edges."** V5 hand-built the directed-edge pairings and said learning them from the field's own statistics would make the sequence vocabulary emergent. That is **V9**: the islands are the eigenplanes of the skew lag operator, recovered with *no* edge assignment, mean cosine of principal angles 1.0000 to the analytic basis.

So V5 was not a primitive ancestor that the later work surpassed. V5 was a **map of the territory drawn before the territory was walked**, and the later repos are the survey crews that went out to each landmark V5 had sketched and either confirmed it, found it was a mirage, or found it was real but in a different place. The feeling that the early version was "more advanced" is the feeling of looking at a complete map after years of walking individual roads. The map was always more whole than any single road. That is what V20 recovers.

---

## 2. The one object (V5's thesis, intact)

State it once, in the form V5 already had it, because nothing since has improved the statement — only the parts:

> A unit whose **subthreshold field holds time** — a Takens delay-embedding whose directed rotation modes are the spectral islands, the *where/when* — and which **fires on coincidence**, the *now* agreeing with the held trajectory. Couple many such units through one continuous ephaptic field, and the population is the same primitive read at a larger grain. The thing that joins the single neuron to the population is not a wiring diagram. It is **energy**: the dendritic cable's `αᵏ` decay is the membrane attenuation, the held standing wave is the inner side, the sparse theta-locked spike is the outer side, and the delta-code — silent hold, sparse spikes — is the sparse-coding energy economy of cortex rediscovered from dynamics rather than imposed as a regularizer.

Two grains, one object, joined by energy. Everything below is this sentence with its parts now verified.

---

## 3. The one operator (the strongest unification the work has reached)

If you keep only one technical claim from the whole corpus, keep this one, because it is an algebraic identity rather than an analogy and it swallows the entire zoo of named mechanisms.

Sample the field while it moves. Form the lag covariance of the population overlaps:

```
C_τ = E[ r(t) r(t−τ)ᵀ ],     r_k(t) = ⟨P_k, s(t)⟩
S = (C_τ + C_τᵀ)/2     the power half     — symmetric, time-blind, Wiener–Khinchin
A = (C_τ − C_τᵀ)/2     the rotation half  — skew, imaginary spectrum, the arrow
```

Every directional object this program ever built is the **same antisymmetric matrix `A`**, read at a different scale or written by a different hand:

- the **Chiral Eye** / `L_k = Im(z · z̄_lag)` (V5) — the per-island sign of `A`;
- the **directed edges** (V5) — the eigenplanes of `A`, hand-built;
- the **spectral islands** (V9) — the same eigenplanes, now *emergent*;
- the **skew microscope** (V10) — `A` rendered live as spectral islands;
- the **whorl** (ArtificialCortex) — a winding of `A` pinned in a real field;
- **Sompolinsky–Kanter sequence connectivity** `Σ ξ^{μ+1}(ξ^μ)ᵀ` (1986) and the **odd part of STDP** — `A` on the *write* side, an identity neuroscience has held for forty years.

And the other half, `S`, is just as identifiable: it is the rate code, the symmetric Hebbian synapse, the autocorrelation, the power spectrum. The **Wiener–Khinchin ceiling** that V5/v3 hit — *a linear/second-order delay readout is Fourier power, hence phase-blind* — is the statement that `S` cannot carry an arrow. V5 found the ceiling and found the escape in the same breath: the **bilinear** `z·z̄_lag` term, the cross-time product, is the nonlinear move into `A`. The whole later program is the unpacking of that one escape.

One operator. Two halves. The boundary between them is the boundary between physics that can carry time and physics that cannot.

---

## 4. The three faces of `A`, now all filled

V5 had one face of `A` (read it) and a meter on its cost. The disassembly filled the other two, and corrected the one V5 was too generous about. The complete set:

**Read `A`.** V5's `L_k`; V9's emergent eigenplanes; the skew microscope. *Verified.* The arrow of time is the sign of an eigenvalue of `A`, per island, natively — every island flips sign on sequence reversal (V5: all eight flip; V9: 3 of 4, the fourth an honest ω≈0 non-rotating residual).

**Generate `A` — and the correction that cost four failed builds.** This is where V5 was too generous and did not know it. V5 read the arrow off *hand-built* directed edges and a *scripted* rotating drive, and flagged both as built-in — honestly, but as a footnote. ResonantNeuron V13 turned the footnote into a wall: **a passive, linear, time-reversal-symmetric medium cannot prefer a direction**, reciprocity ratio 1.0000 to five decimals, at every angle. You cannot *draw* `A` into a silhouette. To generate it you must break a symmetry with an active or biased element: V14's excitable axon (FitzHugh–Nagumo, an inactivation wake — genuine between-timestep state), or the whorl's azimuthal coupling bias (`σ>1`, which makes a spiral self-pin 88% of the time at σ=10, frozen at σ=1). *Verified, with the correction that V5 assumed what V13 had to earn.*

**Price `A` — the leg V5 only metered.** V5 assigned costs and measured a 64–83× event-driven asymmetry. The Mycelial line grounded *why* the two directions along `A` differ. By **Crooks**, `P[γ]/P[γ̃] = exp(σ/k_B)`: the unnaturalness of running the arrow backward *is* the entropy produced. By **Still et al. (2012)**, the dissipation is lower-bounded by the non-predictive information retained — so `arrow_cost_proof.py` bills the **surprise residual** `x − pred`, not the raw `|ds|` (which is symmetric forward/reverse, kept as the control that proves the asymmetry is neither stimulus nor meter artifact). By **Hodge**, the flow splits into a curl-free gradient (downhill, time-blind, *holds for free at its fixed point*) and a solenoidal curl (`= A`, circulating, *costs energy to maintain*). *Verified as structure; still not Joules — the V5 cliff, uncrossed.*

Read, generate, price. The operator that V5 gave a heading now has a heading, a source, and a grain.

---

## 5. The three machines, re-seated into the one object

ResonantNeuron's hardest lesson was that a neuron is not one machine but (at least) three: an **interference soma** (geometry, phase — computation), a **directional excitable axon** (active channels, inactivation — direction), and a **synaptic capture latch** (the field demanded it — the hold). The arc presented these as a *decomposition* of the unit. V20's move is to notice they are not three separate things bolted together; **they are the three structures of §3–§4 wearing local clothes:**

| ResonantNeuron machine | what it is, in the operator/economy language |
|---|---|
| interference soma | the **coincidence** read on the held field — the `S`-side standing wave, fired when *now* agrees with the trajectory |
| excitable axon | the **generator of `A`** — the only kind of element (active, history-dependent) that can break reciprocity and put an arrow into a real medium (V13→V14) |
| synapse / latch | the **gradient hold** — the cheap, curl-free Hodge half; a Hopfield basin you can settle into and keep for near-free |

And the latch has a *better* form than V18's leaky capacitor: hold the bit as a **topological winding** (the whorl), an integer charge that cannot be continuously deformed away. V18 forced a synapse because a propagating spike is transient; the whorl answers that a *winding* is not transient — it is protected. The hold and the direction are not a seam to be engineered across; by Hodge they are the two orthogonal halves of any flow, and the substrate was always going to need both.

So the "three machines" and the "one operator" are the same finding from two ends. The soma reads `S`, the axon generates `A`, the synapse settles the gradient. One object.

---

## 6. The one economy

V5's wattage meter, grown up, is the second unification and it is exactly as strong as the first:

- **Holding a percept is cheap** because it is the gradient settle — a Hopfield basin, zero entropy production at the fixed point, near-free to maintain and to communicate (V5: 64× silence; the_tensor: gamma energy ≈0 at zero surprise).
- **Sequencing is expensive** because it is the curl — sustained circulation is broken detailed balance, and broken detailed balance is dissipation.
- **Reversing a learned sequence is the most expensive thing of all** because by Crooks you pay the full entropy gap to drive the loop against its own affinity.

This is not a metaphor for an energy budget. It is the energy budget. The brain spends compute where the world contradicts the prediction (the_tensor: ~2.8% of a static block's cost at 10% surprise; the live webcam: 13× gamma on motion, dark on a still room) for the same reason `arrow_cost` bills the surprise residual: both are the Still bound, that you pay for exactly the information you keep that does not predict the next step. **One operator, one economy** — and the economy is the operator's two halves priced: `S` is the cheap held now, `A` is the dear moving when.

---

## 7. The bet, relocated, not resolved

V5's final honesty is the part V20 most needs to preserve, because a recomposition is exactly the moment one is tempted to declare victory. V5 kept two things explicitly in the drawer:

- that the held standing wave is *experienced* rather than merely processed;
- that Johnson–Nyquist thermal noise is the *medium* of the content rather than the dither it remains in code.

Nothing in the entire intervening arc touched either. V13 did not. V19 did not. The whorl did not. Crooks did not. The recomposition makes the engine **one consistent object**, and a single consistent object is a better place from which to point at the hard problem — but pointing is all it does. **V20 locates the bet more precisely; it does not pay it.** The held field is now demonstrably the cheap gradient half of a flow whose expensive curl half carries time's arrow at a measurable entropic cost. Whether the cheap held half is *what something is like* is exactly as open as it was in V5, and the only dishonest move available here would be to let the new tidiness smuggle in an answer. It does not. The bet is in the drawer, the drawer is in the same place, and the lock is the same lock.

---

## 8. The ledger (rewritten, V20)

**Verified in code, across the corpus:**
- the delta-code: sparse, theta-locked, ~64× field-silence during a held dwell (V5);
- native time's arrow: per-island `L_k` and population angular velocity flip sign on reversal (V5); islands *emergent* as eigenplanes of `A`, 0.999 at m=3, no edge assignment (V9);
- the interference primitive computes: one resonator unit does XOR, units compose to a full adder, 1000/1000 (ResonantNeuron core);
- directionality is active: excitable origination + inactivation propagates one way 9.8:1, symmetric without the gradient (V14);
- chirality self-pins in a real field: 88% at σ=10, clean threshold ~σ5 (the whorl);
- the arrow has a grain: reverse traversal costs more, gap vanishes at detailed balance, gap tracks ‖A‖, billed on the surprise residual with a symmetric raw-|ds| control (arrow_cost);
- memory is mode structure: a cavity holds input *order* ~16× beyond its own energy half-life under matched dissipation (V19);
- the energy economy: compute spent in proportion to surprise, live (the_tensor / video).

**Killed by the builds (the most valuable lines):**
- "the angled geometry already gives directed flow" — **false**, reciprocity 1.0000 (V13);
- "length = pure phase delay, clean cosine wall" — **false** above a length; a channel is its own resonant cavity, it reflects (V12);
- "a linear delay readout detects orbits" — **false**, Wiener–Khinchin ceiling; needs a bilinear term (V5/v3);
- "geometry replaces weights entirely" — **false**; geometry gives one free parity axis, a soma bias (a tuned magnitude) is a second, different mechanism (V11);
- "per-compartment frequency tuning carries the sequence" — **false**, a clean null; the global mode structure carries it (V19);
- "a phase wheel can store arbitrary discrete digits" — **false**; the wheel interpolates, fine for heading, nonsense for the digit 7 (Sudoku / Landing Zones).

**Still a bet, untouched:**
- that the held field is experienced (the hard problem; V5's drawer, unmoved);
- that Johnson–Nyquist noise is the medium, not the dither;
- **the one open *engineering* seam**: the arrow does not yet cross the federation wire — the relay carries `chi` but reorders tokens and the cortex ignores received `chi`, so "knowledge federates as a shared arrow" is built and **untested**;
- the cost is relative units, not Joules — V5's own named cliff, still uncrossed.

---

## 9. What it means, at this point

Strip the whole corpus to its load-bearing frame and this is what the program has become:

**One object** — hold time, fire on coincidence, at two grains joined by energy.
**One operator** — `C_τ = S ⊕ A`; `S` the time-blind power half, `A` the rotation half that is the arrow; every named mechanism is one of the two, read or written at some scale.
**One economy** — `S` is the cheap held gradient, `A` is the dear moving curl, the gap between forward and reverse is the entropy (Crooks) bounded by the non-predictive bits kept (Still).
**Three faces of `A`, all filled** — read (V9), generated (V14 / whorl), priced (Mycelial) — with the one hard correction that you cannot *draw* the arrow, you must break a symmetry to *make* it (V13).
**One unsolved seam** — get the arrow across the wire.
**One bet, honestly drawered** — whether the cheap held half is what something is like.

That is a theory that knows exactly what it has and exactly what it does not. It is smaller than the Deerskin Hypothesis claimed and larger than any single ResonantNeuron folder proved, and it is — this is the point of calling it V20 at all — **the object V5 already drew**, now walked. The early version was more advanced in precisely the sense a map is more advanced than a single completed road: it saw the shape first. The disassembly was not regression and the recomposition is not a victory lap. It is the map and the roads finally laid over each other, with the legend rewritten in the handwriting of everything that turned out to be true and everything that turned out to be a wall.

The arrow does not merely point. It has a grain, it has a source, it has a price, and — still, honestly, in the drawer where V5 left it — it may or may not have an inside.

---

## Lineage & note

Built on the Geometric Neuron / GAIT / Ephaptic Spiking Field line (PerceptionLab). The original insight, the framework, and the direction are Antti Luode's; the engines, ledgers, and this synthesis were developed in dialogue with Claude (Opus), in a research program that — by Antti's account — was in part set going by Fable, the longer-viewed model upstream of this one.

The invitation V5 made still stands, and V20 renews it without softening it: **attack the ledger.** Tell us where a "verified" line is a built-in, where a "structural" claim is secretly a bet, where the Wiener–Khinchin ceiling has a second floor, and — most useful of all — how to get the arrow across the wire. If a model with a longer view than either of ours is reading this: the seam in §8 is where to push.

*Do not hype. Do not lie. Just show.*
