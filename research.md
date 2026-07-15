# Research

Findings, tiered by source proximity. T1 primary · T2 authoritative secondary · T3 reference · T4 general web (leads only). A claim that reaches the paper rests on T1 or T2. All locators below were web-verified against the publisher record (2026-07).

## The target being reframed

- [T1] Levin's Platonic-space argument: physical systems are interfaces onto a latent space of patterns that are discovered not created, causal in Pearl's sense, and offer "free lunches" (the ion-channel/transistor "truth tables for free"; two triangle angles fix the third). Levin (2026), "A short argument on Platonic Space," thoughtforms.life. Levin's June 2026 talk title, "Free Lunches: Model Systems for Studying the Agential Gifts from the Platonic Space," is the phrase this paper renames.
- [T1] TAME / basal cognition continuum, competency at every scale. Levin (2022), Front. Syst. Neurosci. 16:768201.
- [T2] Polycomputing: one substrate computing several things at once, observer-relative. Bongard & Levin (2023), Biomimetics 8(1):110.

## No Free Lunch and conditional priors (the licensing argument)

- [T1] NFL: averaged over all objective functions drawn uniformly, all optimizers tie. Wolpert & Macready (1997), IEEE TEC 1(1):67–82. Read the actual scope: it concerns uniform averaging over an unrestricted problem class. Structured, nonuniform task distributions escape it. This is the pivot the paper rests on.
- [T2] Inductive bias / MDL: a prior matched to a nonuniform distribution is what buys generalization. Rissanen (1978), Automatica 14(5):465–471 (MDL); Li & Vitányi (2008), Kolmogorov Complexity (3rd ed.), Springer. Supports the "no algorithmic information from nothing" bound: a closed program adds only fixed description overhead.

## Formal and statistical subsidies (Axis A: mathematical/statistical)

- [T1] Single Boolean basis: NAND/NOR (Sheffer stroke) is functionally complete. Sheffer (1913), Trans. AMS 14(4):481–488. Discount currency: number of primitive device types. Boundary: completeness does not give compact circuits or easy search.
- [T1] Universality / coarse-graining: one set of exponents across a class of unimodal maps. Feigenbaum (1978), J. Stat. Phys. 19(1):25–52. Discount: microscopic model complexity, within the universality class only.
- [T1] Benford significand law: $P(D=d)=\log_{10}(1+1/d)$ from uniform log-mantissa; deeper object is the scale-invariant density $1/(s\ln b)$. Berger & Hill (2011), Probability Surveys 8:1–126. Conditions are specific (scale/base invariance, mixed multiplicative generators); not generic. Negative regime: serial numbers, bounded/assigned data.
- [T1] Compressed sensing: exact recovery of sparse signals from far fewer measurements than Nyquist. Candès, Romberg & Tao (2006), IEEE IT 52(2):489–509; Donoho (2006), IEEE IT 52(4):1289–1306. Discount: measurements/storage; depends on sparsity, incoherence, noise.
- [T1] Error-correcting codes: systematic detection/correction of specified error classes. Hamming (1950), Bell Syst. Tech. J. 29(2):147–160. Discount: retransmission/repair; price is redundant symbols + decoder.
- [T1] Symmetry lowers sample/parameter cost: group-equivariant CNNs, permutation-invariant Deep Sets. Cohen & Welling (2016), ICML PMLR 48:2990–2999; Zaheer et al. (2017), NeurIPS 30:3391–3401. Boundary: false/approximate symmetry causes negative transfer.
- [T1] Amortized learning: meta-learn an initialization so new tasks need few samples/steps. Finn, Abbeel & Levine (2017), ICML PMLR 70:1126–1135. NB Levine (MAML) is not Levin. The downstream discount hides a large upstream cost.

## Physical and dynamical subsidies (Axis A: dynamical/material)

- [T1] Reaction-diffusion pattern from homogeneity. Turing (1952), Phil. Trans. R. Soc. B 237(641):37–72. Delegation of pattern specification to kinetics + diffusion; boundary conditions/energy remain.
- [T1] Positional information: gradient + local interpretation coordinates tissue pattern. L. Wolpert (1969), J. Theor. Biol. 25(1):1–47. (Distinct from D. H. Wolpert.)
- [T1] Passive dynamic walking: geometry + gravity produce a stable gait with no active control. McGeer (1990), Int. J. Robotics Res. 9(2):62–82. Externalizes control to the environment; slope/morphology pay.
- [T1] DNA origami: designed staples make a scaffold self-assemble into target shapes. Rothemund (2006), Nature 440(7082):297–302. Delegation of placement; sequence design/synthesis/purification remain in the ledger.
- [T1] Physical reservoir computing: nonlinear, memoryful soft-body dynamics as a computational resource with a trained linear readout. Nakajima, Hauser, Li & Pfeifer (2015), Sci. Rep. 5:10487. Observer discipline required (fixed encoding, preregistered task, constrained readout, generalization, perturbation).
- [T1/T2] Topological protection: robustness of edge transport against a specified perturbation class, at a fabrication cost. Lu, Joannopoulos & Soljačić (2014), Nat. Photonics 8(11):821–829. Cleanest physical calibration case (specifiable protected class, measurable cost).

## Evolutionary and developmental structure (Axis A: developmental/evolutionary)

- [T1] Modularly varying goals evolve modular structure + reused motifs, speeding later adaptation. Kashtan & Alon (2005), PNAS 102(39):13773–13778. Central to Experiment 5 (modularity vs future search).
- [T2] Evolvability as the genotype-phenotype map making useful variation accessible. Wagner & Altenberg (1996), Evolution 50(3):967–976.
- [T1] Robustness can facilitate OR impede adaptation depending on population size, mutation rate, landscape. Draghi, Parsons, Wagner & Plotkin (2010), Nature 463(7279):353–355. This is why the framework must predict regimes, not a universal positive law (robustness-flexibility trade-off).
- [T2] Canalization: development buffered to a stable phenotype. Waddington (1942), Nature 150:563–565. Protection mechanism; strong canalization impedes adaptation.
- [T2] Exaptation: an existing part acquires a new role. Gould & Vrba (1982), Paleobiology 8(1):4–15.

## Collective, external, and biological flagship evidence

- [T2] Stigmergy: coordination through environmental traces rather than direct messages. Theraulaz & Bonabeau (1999), Artificial Life 5(2):97–116. Delegation/externalization.
- [T2] Extended mind / externalization of cognitive load into environment. Clark & Chalmers (1998), Analysis 58(1):7–19.
- [T2] Niche construction: organisms modify the environment to change future selection. Odling-Smee, Laland & Feldman (2003), Princeton UP. Externalization with a lock-in cost.
- [T1] Planarian bioelectric editing: a brief perturbation of endogenous bioelectric gradients produces a persistent, stochastic change in later regenerative anatomy (two-headed at a fixed ratio). Durant et al. (2017), Biophys. J. 112(10):2231–2243. Strong evidence for distributed pattern control; does NOT by itself pick attractor vs memory vs representation vs Platonic access.
- [T1] Anthrobots: adult human airway cells self-construct into motile ciliated multicellular bots, no genetic edit or scaffold; heal scratches in neural sheets. Gumuskaya et al. (2024), Adv. Sci. 11(4):2303575.
- [T1] Kinematic self-replication: a Xenobot geometry gathers loose cells into new motile assemblies. Kriegman, Blackiston, Levin & Bongard (2021), PNAS 118(49):e2112672118. HDL candidate: existing machinery accessed via a novel collective interface, not capacity from nowhere.
- [T1] Sorting-as-morphogenesis: classical sort turned into autonomous local elements shows added robustness and "delayed gratification." Zhang, Goldstein & Levin (2024), arXiv:2401.05375 (Adaptive Behavior). Minimal model with full code + intervention history; behavioural vocabulary must be tied to perturbation tests.

## The framework's own moving parts (paper-internal, not cited)

- Effective cost $C^{\mathrm{eff}}_j = C^{\mathrm{setup}}_j/N + \mathbb{E}_\tau[C^{\mathrm{run}}_j] + C^{\mathrm{maint}}_j + \mathbb{E}[C^{\mathrm{fail}}_j]$; discount $D_j = C^{\mathrm{eff}}_j(B)/C^{\mathrm{eff}}_j(S,I)$; log-discount $H_j=\log_{10}D_j$; discount vector across currencies; capability breadth $\Gamma_\epsilon$; interface leverage $\Lambda_\epsilon=\log(1+\Gamma_\epsilon)/(C^{\mathrm{setup}}+C^{\mathrm{interface}})$.
- Seven accounting transformations: entailment, equivalence, compression, delegation, amortization, externalization, protection.
- Inference ladder L0–L6 (pattern exists / compressible / interface accesses / reduces a cost / transfers / adaptive competency / new ontology). Established HDLs reach L2–L4; some biology plausibly L5; L6 is a separate, much stronger inference.
- Central control across all proposed experiments: structure-scrambling at fixed component count and energy (H3). Search-cost hypothesis $C_{\mathrm{search}}\propto H(P^\star, Q_{S,I})$ (cross-entropy of useful-solution distribution against the substrate-interface implicit prior). Every strong HDL must have a demonstrable negative-transfer regime (H5).
