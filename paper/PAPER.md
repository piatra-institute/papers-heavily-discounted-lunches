---
title: |
  Heavily Discounted Lunches:\
  Structural Subsidies and the Accounting of Competence
author: PIATRA . INSTITUTE
date: July 2026
---

## Abstract

Many complex systems command families of useful behaviour whose explicit design, learning, or evolutionary cost appears small relative to their scope. A single nonlinear switch composes into all of Boolean logic; logarithmic representation yields a full leading-digit distribution; a compliant body walks downhill without a controller; dissociated cells rebuild an anatomy that no genome stores cell by cell. Levin groups such cases as free lunches drawn from a Platonic space of patterns. We retain the phenomena and treat each as a heavily discounted lunch: the world supplies a pre-existing regularity, the system pays to build an interface to it, and a family of consequences follows at low marginal cost. This violates neither thermodynamics nor the No-Free-Lunch theorems, which equalize optimizers only under uniform averaging over an unrestricted problem class. We formalize the discount as a vector across search, samples, description length, computation, energy, control, communication, construction, and repair, measured against a matched baseline within an explicit accounting boundary that records who paid and when. A two-axis taxonomy separates the source of a subsidy from its mechanism, and the mechanisms reduce to seven operations: entailment, equivalence, compression, delegation, amortization, externalization, and protection. Four case studies (functional completeness, Benford's law, morphological computation, and morphogenesis) each identify a regime in which the interface becomes a penalty. A seven-level inference ladder separates the existence of a regularity from access to it, cost reduction from adaptive competency, and competency from claims of new ontology. The resulting question for any apparently disproportionate competence is which structure supplied the discount and where the remaining cost was paid.

## 1. Introduction

A reliable NAND gate suffices for all of logic. Every Boolean function of every arity can be assembled from it by composition, and no further logical fact has to be discovered, encoded, or paid for. Functional completeness is a property of Boolean algebra, established by Sheffer (1913) and inherited by any device that can switch. One primitive is purchased, and the space of finite logical circuits comes with it.

The same pattern appears outside logic. A quantity that ranges over several orders of magnitude and is read on a logarithmic scale has a fixed distribution of leading digits, so a system operating in that regime holds a usable prior over first digits without estimating nine probabilities separately (Berger and Hill, 2011). A two-legged machine with an appropriate mass distribution walks down a shallow slope with no motor, controller, or feedback, its gait supplied by gravity and its own geometry (McGeer, 1990). A soft silicone arm driven at its base performs enough nonlinear filtering in its material that a trained linear readout of its deformations computes functions the base signal alone does not (Nakajima et al., 2015). A flatworm cut into pieces regenerates whole worms, each fragment restoring an anatomy that no single cell holds as an explicit plan (Durant et al., 2017).

Levin groups these cases under one heading. On his account, physical systems are interfaces onto a latent space of mathematical and agential patterns that are discovered and not authored, and evolution draws competence from that space at a discount he calls a free lunch: once a voltage-gated ion channel exists, truth tables come for free, and once two angles of a triangle are fixed, the third needs no separate determination (Levin, 2026, 2022). The examples are well chosen. The word free, however, implies that something was obtained for nothing, and it sets aside the question that makes the examples scientific: what was paid, and by whom.

We retain the phenomena under a different name. A heavily discounted lunch is a case in which coupling a system to a structured substrate sharply lowers the effective cost of obtaining a reusable family of outcomes, relative to a matched alternative that must construct or search for those outcomes more independently. The term discounted imposes a ledger. A discount is defined against a price, in a currency, relative to a baseline, and paid by someone, and each of these four must be specified: the price the system would otherwise have paid, the currency of the saving, the baseline it outperformed, and the party that covered the remainder.

The disproportion between explicit cost and accessible competence is general, takes a small number of forms, and can be measured. The world offers no universal free lunches. It offers domain-specific structural subsidies, regularities already present in mathematics, in environmental statistics, in physical dynamics, in developmental and evolutionary architecture, in collectives, and in accumulated history. A system pays to build an interface to one of these and then draws a family of consequences from it at low marginal cost. For every case the accounting question is the same: which structure supplied the discount, which interface accessed it, in what currency the saving was made, and where the remaining cost was paid and stored.

## 2. Conservation constraints

The immediate objection is conservation: if a system does more than its explicit budget seems to allow, the budget must be misstated. Three conservation results bound what a discount claim can mean.

The first bound is thermodynamic. A passive walker, a self-assembling crystal, and a regenerating tissue create no energy. Each draws on gravity, a chemical gradient, metabolism, an applied field, or ambient temperature, and its discount is in another currency, such as control effort, specification, or search, underwritten in part by an energy source that belongs in the ledger. A discount in one column is compatible with an equal or larger bill in another.

The second bound is informational. A closed deterministic program cannot produce algorithmic information beyond that present in its program, inputs, and initial conditions, up to a fixed additive constant (Li and Vitányi, 2008). A three-line rule can generate an image of unbounded visual intricacy, and the image compresses back to the three lines; the intricacy lies in the rendering. Randomness can add algorithmic information, but random bits do not by themselves add competence at a specific task. A claim that a system produced adaptive capability from nothing either concerns a currency other than algorithmic information or is false.

The third bound, the No-Free-Lunch theorem, is the most often misread. Wolpert and Macready (1997) proved that when performance is averaged with equal weight over all objective functions, every optimizer performs identically, and superiority on one class of problems is offset by inferiority on its complement. The theorem concerns uniform averaging over an unrestricted problem space. It places no constraint on a system that performs well on a structured, nonuniform distribution of problems and poorly on the rest. Organisms and machines do not face uniformly random tasks. They inhabit a world with pervasive continuity, locality, symmetry, conservation, modularity, and correlation, and a system whose built-in assumptions match that structure has an advantage because the world's task distribution differs from the uniform average the theorem assumes. A matched prior, in the minimum-description-length sense (Rissanen, 1978), converts that structure into shorter search. The discount and the theorem are therefore consistent, and the theorem adds a constraint: the discount must be conditional, and a prior that buys competence on the matched distribution must cost competence elsewhere. A structural subsidy with no penalty region would violate the theorem. The framework accordingly predicts that every real subsidy has such a region.

These bounds restrict what "more out than in" can mean. It cannot mean net energy, algorithmic information beyond the additive constant, or an optimizer that is superior on average over all problems. Nor does a surprising output by itself establish memory, goal-direction, intelligence, or a nonphysical cause; each is a separate claim requiring its own evidence (section 6). The admissible meanings are specific: more tasks solved per unit of controller complexity, more functions reachable from a small set of primitives, fewer evolutionary evaluations, fewer training samples, lower marginal construction cost, tolerance without an explicit repair routine, less centralized communication, and reuse across a task family. Each is a discount in a named currency against a matched baseline, and each is measurable.

## 3. Accounting framework

A discount is measured by fixing the task family, the baseline, and the currency, and comparing effective costs. Let $\tau$ be a task drawn from a distribution $P(\tau)$, $S$ a structured substrate, $I$ an interface to it, and $B$ a counterfactual baseline that solves the same task family without that substrate. Setup is amortized over $N$ deployments. For a cost currency $j$, the effective cost of the substrate-and-interface system is

$$C^{\mathrm{eff}}_j(S,I;P,N) = \frac{C^{\mathrm{setup}}_j(S,I)}{N} + \mathbb{E}_{\tau\sim P}\!\left[C^{\mathrm{run}}_j(\tau\mid S,I)\right] + C^{\mathrm{maint}}_j + \mathbb{E}\!\left[C^{\mathrm{fail}}_j\right],$$

with the baseline $B$ costed in the same way. The discount in currency $j$ is the ratio

$$D_j = \frac{C^{\mathrm{eff}}_j(B;P,N)}{C^{\mathrm{eff}}_j(S,I;P,N)}, \qquad H_j = \log_{10} D_j,$$

so that $H_j = 1$ is a tenfold saving, $H_j = 2$ a hundredfold saving, and $H_j = -1$ a tenfold penalty. A ratio below 1 is a negative lunch, an interface that costs more than it saves in that currency.

No single scalar score captures the phenomenon, because costs trade against one another. A compliant robot saves controller computation and spends it again in fabrication and wear. An error-correcting code buys reliability with redundant symbols and decoder complexity. A pretrained model gives its downstream user a large sample discount and carries an upstream training bill that far exceeds it. The appropriate object is a vector,

$$\mathbf{D}=(D_{\mathrm{search}},\, D_{\mathrm{sample}},\, D_{\mathrm{energy}},\, D_{\mathrm{control}},\, D_{\mathrm{comm}},\, D_{\mathrm{constr}},\, D_{\mathrm{repair}},\, D_{\mathrm{descr}}),$$

reported component by component in search evaluations, training samples, joules, controller states or feedback bandwidth, messages, assembly operations, repair interventions, and description length. A leverage claim that reports one favourable component and omits the rest is incomplete.

The priced object is a family of outputs. In the NAND example, crossing a small interface threshold opens a large space of possible behaviours, so the relevant quantity is the breadth of accessible capability,

$$\Gamma_\epsilon(S,I)=\bigl|\{\tau\in\mathcal{T}: U(\tau;S,I)\ge U_{\min},\ \mathrm{error}(\tau)\le\epsilon\}\bigr|,$$

the number of tasks a system built on $S$ through $I$ can perform to tolerance $\epsilon$. Leverage relates this breadth to the cost of the interface,

$$\Lambda_\epsilon=\frac{\log\!\left(1+\Gamma_\epsilon\right)}{C^{\mathrm{setup}}+C^{\mathrm{interface}}}.$$

A gate that performs one useful transformation scores near zero. A gate whose composition closure is all of Boolean logic scores high, because a bounded interface cost supports an unbounded capability family.

Every discount claim must specify its accounting boundary, because a discount for one payer is often a cost transferred to another. The current agent, the full life cycle, the evolutionary or engineering history, the environment, and the whole system are five distinct boundaries, and a lunch can be cheap at one and expensive at the next. The passive walker's control discount is underwritten by gravity, the slope, and the machinist who tuned the mass distribution. The pretrained model's sample discount is underwritten by the compute and data collection that produced it. The embryo's genome holds no explicit map of every cell position, while the cells that build the embryo carry billions of years of evolved molecular machinery and consume metabolic energy to run it. These observations do not cancel a discount. They locate where the cost was moved, over how many uses it was amortized, and whether the discount persists under a wide boundary. For each case the questions are who paid, in what currency, at what time, where the payment is now stored, and how many future outcomes draw on it.

Amortization removes many of these costs from the current agent's view. A cost paid once and reused over $N$ deployments enters the effective ledger as

$$C(N)=C^{\mathrm{setup}}+N\,C^{\mathrm{marginal}},$$

so a high fixed cost with a low marginal cost undercuts repeated construction from scratch once $N$ is large enough, and the crossover point is a measurable prediction. Evolution, development, culture, standardization, and pretraining are amortization processes in this sense: each pays a large structural cost once, and a long series of later tasks draws on it cheaply. A discount that appears anomalous at the margin is often an amortized historical cost.

## 4. Sources and mechanisms of discounts

A flat list of examples is inadequate because one case can involve several mechanisms. NAND combines deductive closure, compositionality, nonlinear switching, and amortized design history. Morphogenesis combines attractors, self-assembly, collective coordination, developmental bias, and repair. Two axes organize the cases. The first is the source of the subsidy, the kind of structure already present: mathematical (logical consequence, symmetry, topology), statistical (sparsity, low dimension, scale invariance), dynamical and material (attractors, resonance, compliance, phase transitions), developmental and evolutionary (genotype-phenotype maps, modularity, canalization, competent cells), collective and ecological (local interaction rules, other agents, environmental scaffolds), and historical and cultural (prior evolution, training, accumulated knowledge, infrastructure). The second axis is the mechanism of the discount, the operation by which the structure lowers a cost.

Across sources, the mechanisms reduce to seven operations. They are not mutually exclusive, and a single biological case can involve all of them; naming them separately allows a case to be decomposed into its components.

Entailment fixes a relation once, so that a family of consequences follows without separate specification. Two angles of a triangle determine the third. A small set of axioms entails a large body of theorems. A single Boolean basis entails all of finite logic (Sheffer, 1913). The saving is in specification and verification. Its limit is that a consequence can be logically determined and still computationally hard to find or prove.

Equivalence shows that many apparently distinct cases are one case under a transformation, and the saving appears as fewer parameters, samples, or experiments. Weight sharing across translations in a convolutional network, group-equivariant architectures, and permutation-invariant set models each convert a symmetry of the task into a smaller hypothesis space (Cohen and Welling, 2016; Zaheer et al., 2017). Its limit is that a false or only approximate symmetry imposes a bias that transfers negatively.

Compression represents many observations economically through a low-dimensional latent structure, a sparse basis, a short generative rule, or a statistical prior. Compressed sensing recovers a sparse signal exactly from far fewer measurements than the naive bound requires, provided the signal is sparse in a basis incoherent with the sampling (Candès, Romberg and Tao, 2006; Donoho, 2006). The saving is in samples, storage, and description length. Its limit is the sparsity or invariance condition the data must satisfy.

Delegation assigns part of an outcome to physical dynamics, local agents, or the environment. Reaction-diffusion kinetics lay down a pattern without a central plan (Turing, 1952). A relaxing physical system settles into a minimum that encodes the answer. Designed staple strands fold a long DNA scaffold into a target shape (Rothemund, 2006). Ant-like agents coordinate through traces left in a shared medium in place of direct messages (Theraulaz and Bonabeau, 1999). The saving is in explicit control and computation. Its limit is that the delegated dynamics may reach only a local solution, which must still be encoded, sensed, and read out.

Amortization pays a large cost once and spreads it over many later uses, as formalized in section 3. Meta-learning tunes an initialization so that new tasks are learned in a few gradient steps, buying a downstream sample discount with a large upstream training cost (Finn, Abbeel and Levine, 2017). Evolution, development, and culture perform the same operation over longer timescales. The saving is in per-task cost. Its limit is that the upstream bill is real and belongs in the wide-boundary ledger.

Externalization moves part of the task into the environment, which then holds state or performs work the system would otherwise pay for internally. Gravity drives the passive walker. A pheromone trail is memory stored outside the animal. Tools, written marks, and infrastructure become working parts of the control loop (Clark and Chalmers, 1998), and organisms that reshape their surroundings alter the selection their descendants face (Odling-Smee, Laland and Feldman, 2003). The saving is in internal actuation, memory, or computation. Its limit is that the capability disappears when the environment changes, and the environment can impose a lock-in cost.

Protection pays once for a mechanism that prevents, absorbs, or corrects errors, ending repeated payment for the same problem. An error-correcting code converts a stream of failures into a fixed redundancy overhead (Hamming, 1950). An attractor basin returns a perturbed state to its target without an explicit repair instruction. Canalization buffers a developmental outcome against genetic and environmental noise (Waddington, 1942). Topological edge modes carry a signal past defects that would scatter an ordinary mode (Lu, Joannopoulos and Soljačić, 2014). The saving is in correction, retransmission, and repair. Its limit is that protection covers only the perturbation class it was built for, and stronger protection tends to reduce flexibility.

Three further mechanisms reduce to the seven. A coarse-graining discount, in which one universal description covers many microscopically different systems that share a large-scale behaviour (Feigenbaum, 1978), is compression applied to models instead of data. Exaptation, the redeployment of an existing part to a new function (Gould and Vrba, 1982), amortizes the part's original construction cost against a use for which it was not built. Polyfunctionality, one substrate carrying several readouts at once (Bongard and Levin, 2023), is an inward form of externalization: several functions are overloaded onto the same material, and the arrangement counts as a discount only when the hardware saved exceeds the added interference and readout cost. The seven operations recur throughout the large set of examples, which consists of these operations in combination.

## 5. Case studies

### 5.1 Functional completeness and switching interfaces

The theorem is old and exact. A single binary operation, the Sheffer stroke, realized physically as a NAND gate, is functionally complete: every truth function of every number of arguments is a composition of NANDs (Sheffer, 1913). A designer with a reliable NAND never needs a physically distinct primitive for any other logical function.

The apparent lunch is that a voltage-gated ion channel, a transistor, or any thresholded switch seems to deliver this universality for the price of one device. The accurate statement is weaker. An ion channel is not a NAND gate. A channel supplies state-dependent nonlinear conductance, a threshold, and sometimes hysteresis, and networks of such elements have been configured in the laboratory as inverters and NAND gates, which shows that the analogy is physically legitimate without being automatic. The gap between a switch and a computer is a list of further requirements, each with a real cost: distinguishable states; sufficient nonlinearity; gain or signal restoration, so that a gate's output can drive another gate without degradation; cascadability; adequate fan-in and fan-out; isolation from unwanted feedback; an energy source or maintained gradient; stable timing; an encoding of inputs and outputs; and, for sequential operation, memory. The universality of Boolean algebra costs nothing. The powered, restored, cascadable switching architecture that reaches it has a substantial cost.

The quantity of interest is how capability grows as these requirements are met, and we propose that it grows by thresholds. As an interface acquires gain, then memory, then cascadability, the reachable family $\Gamma$ can jump,

$$\Gamma(I+\delta I)\gg\Gamma(I),$$

for a small increment $\delta I$ in physical complexity. Some discounted lunches are therefore capability phase transitions, in which a modest addition to the interface produces a disproportionate expansion of what the substrate can be made to do. A switch without gain composes only into a shallow, degrading circuit; the same switch with restoration composes without bound. The discount consists in crossing the threshold beyond which composition closes.

Completeness and efficiency are different properties, and this defines the limit of the case. Functional completeness guarantees that some NAND circuit computes any given function. It bounds neither the size, depth, energy, nor discoverability of that circuit. A universal design space can contain only expensive solutions to a given problem, and finding a compact circuit within it is a separate cost that the completeness theorem does not reduce.

### 5.2 Benford's law as a matched prior

Write a positive quantity as $X = 10^{n+u}$ with $n$ an integer and $0 \le u < 1$. The integer $n$ is the order of magnitude and $u$ fixes the leading digits. If the fractional part of $\log_{10} X$ is approximately uniform on $[0,1)$, the leading digit $D$ obeys

$$P(D=d)=\log_{10}\!\left(1+\tfrac{1}{d}\right),\qquad P(D=1)\approx 0.301,\quad P(D=9)\approx 0.046.$$

Nine digit probabilities are fixed at once, and no process has to estimate them individually. The underlying object is the scale-invariant density $f(s)=1/(s\ln b)$ on the significand, the multiplicative geometry of positive quantities normalized to a single order of magnitude, of which the decimal frequencies are the base-10 projection (Berger and Hill, 2011). A system operating on scale-spanning, multiplicatively generated quantities, with a logarithmic representation and a significand-sensitive readout, inherits the entire distribution as a prior.

The saving is statistical. A Benford-aware estimator needs fewer observations to model a multiplicative signal, detects anomalies against a principled null, and represents multiplicative change directly. The interface that reaches the subsidy is specific: logarithmic encoding, sampling across several orders of magnitude, a generative process that is multiplicative or scale-mixed, and a readout sensitive to the significand.

The case has a sharp and nameable negative regime. Applied to serial numbers, fixed-width identifiers, administratively assigned prices, narrowly bounded measurements, or heavily truncated data, the same prior is wrong, because those generators lack the assumed scale invariance; the estimator's calibration decays and its anomaly flags become false positives. Benford's law therefore illustrates the framework's central conditional most clearly: a structural match yields a discount, and the same structure applied under mismatch yields a penalty. A forensic corollary is often ignored in practice. A deviation from Benford's law is evidence of fraud only after the generative and sampling conditions have been shown to justify the prior; without that step, the deviation is at least as likely to reflect the range of the data.

### 5.3 Morphological computation

McGeer (1990) built a two-legged machine with no actuators and no control system that walks stably down a shallow slope, its gait a limit cycle of its own mechanics under gravity. Soft-body experiments later showed the complementary result: the nonlinear, history-dependent dynamics of a driven silicone arm are rich enough that a trained linear readout of its deformation emulates nonlinear dynamical systems that the input alone does not compute (Nakajima et al., 2015). Together the two results show that computation and control are distributed across a controller, a body, an environment, and a readout, and that a saving in the controller counts only if it persists when the other three are costed.

The appropriate comparison is total life-cycle cost,

$$C_{\mathrm{total}} = C_{\mathrm{fabrication}} + C_{\mathrm{controller}} + C_{\mathrm{sensing}} + C_{\mathrm{environment}} + C_{\mathrm{maintenance}} + C_{\mathrm{energy}},$$

and the discount is real only when this sum falls; a simpler digital controller alone does not establish it. A compliant hand that grasps without computing each contact force has moved the cost of that computation into its material, fabrication, and wear, and whether the shift is a discount is an empirical question about the sum.

This case also requires the framework's strongest methodological caution, because the claim that a body computes is easy to overstate. An arbitrary physical trajectory is not a computation. A defensible claim that a body computes requires a fixed input encoding, a task specified before the readout is chosen, a constrained readout that cannot be retuned per input, comparison against matched controls, generalization to inputs held out of readout training, and perturbation of the physical degrees of freedom that are supposed to perform the work. Without these, an observer can search after the fact for an interpretation under which the trajectory appears meaningful, and that search is an observer-side cost that belongs in the ledger. The reservoir results are persuasive because they meet these conditions; many other claims do not.

### 5.4 Morphogenesis and competent components

The biological case is the richest and the least settled. A gradient of a signalling molecule, read locally by cells that adopt a fate according to their position in it, coordinates pattern across a tissue without any cell holding a map of the whole (Wolpert, 1969), and interacting diffusing substances break an initial uniformity into organized pattern without a central plan (Turing, 1952). Beyond this classical delegation, there is evidence that the pattern is regulated as well as produced. A brief, targeted perturbation of endogenous bioelectric gradients in a regenerating planarian produces a persistent change in the anatomy the fragment rebuilds: a fixed fraction of worms become two-headed and continue to regenerate as two-headed through further rounds of cutting without further intervention (Durant et al., 2017). Adult human airway cells, released from their tissue and cultured, self-construct into motile ciliated multicellular bodies that were never selected for and that heal wounds in a neural sheet (Gumuskaya et al., 2024). A cluster of frog cells of a particular geometry gathers loose cells into new clusters that move and gather in turn (Kriegman et al., 2021).

The potential discount is large. Local cellular policies, intercellular communication, and anatomical constraints together produce large-scale construction and repair that no genome appears to store as an explicit plan specified cell by cell and contingency by contingency. Evolution appears to have paid once for cellular machinery and intercellular interfaces that solve whole classes of morphogenetic problems, and to draw on that investment in every individual and after every injury. Levin interprets the cells as competent agents pursuing anatomical setpoints and treats the setpoint as a pattern reached through a bioelectric interface (Levin, 2022).

The operational evidence is strong, the ontology is open, and the two must be kept separate. Reliable regeneration of a whole from a fragment is consistent with an attractor in a developmental dynamical system, a control loop minimizing error against a stored target, embodied collective computation, an evolved developmental bias that makes the correct form the easiest to reach, and Levin's stronger reading in which a nonphysical pattern is accessed. The data do not yet distinguish these, and the persistent bioelectric edit does not select among them, since it demonstrates distributed pattern control, which every reading predicts. A minimal model makes this underdetermination tractable. Classical sorting algorithms rewritten as populations of autonomous elements, each applying the sort rule locally, show added robustness and non-monotone trajectories that have been described as delayed gratification; because the full code and intervention history are available, the behavioural vocabulary can be tied to perturbation tests (Zhang, Goldstein and Levin, 2024). The morphogenetic discount is among the largest and least resolved in the set of cases, and its size and its interpretation require separate measurements.

## 6. The inference ladder

Six steps separate an interesting pattern from a system that has accessed a nonphysical mind, and the common error in this literature is to take them in one. The ladder makes the steps explicit and assigns each an evidential requirement.

| Level | Claim | Evidence required |
|---|---|---|
| 0 | A pattern exists | Replication and measurement |
| 1 | The pattern is compressible | A model or code shorter than the raw data |
| 2 | A physical interface reliably accesses it | Manipulating interface variables changes the access |
| 3 | Access reduces a specified cost | A matched quantitative baseline in a named currency |
| 4 | The discount transfers across a task family | Held-out tasks and domain variation |
| 5 | The system exhibits adaptive competency | Perturbation, error correction, flexible strategy |
| 6 | The competency requires a new ontology | Failure of the specified physical and computational alternatives |

Most established discounts reach levels 2 to 4. NAND, Benford's law, compressed sensing, passive walking, and error-correcting codes are level-3 or level-4 cases, in which the cost reduction is measured and transfers. Some biological cases plausibly reach level 5 under carefully stated criteria, where perturbation reveals error correction and flexible re-achievement of a target in place of a fixed output. Level 6 is a separate and much stronger inference, reached only by ruling out the physical and computational accounts at level 5, which no case in this area has done. Levin's Platonic-space proposal is a legitimate level-6 hypothesis, but the operational existence of a discount does not entail it, and reading a level-3 measurement as level-6 evidence is the error the ladder is designed to prevent. The framework is strict about the lower levels and agnostic about the top: the discounts are empirical, the ontology is undetermined, and the framework is usable both by readers who reject Platonism and by those who accept it.

An example enters the central account only if it meets a set of admission criteria that operationalize the ladder. There must be an explicit baseline and a specified task family; a single favourable output is insufficient. The substrate structure and the interface must both be named, and the interface must be manipulable. A cost reduction must be measured in at least one currency, and the fuller ledger, including setup, maintenance, energy, and readout, must be attempted. The advantage must transfer beyond the demonstration case, and scrambling or ablating the relevant structure must reduce it. A negative domain must be identified. Two observer-side rules apply: no readout may be chosen after the fact to make a trajectory appear meaningful, and no metaphysical conclusion may be presented as established by operational leverage.

Several familiar candidates fail these tests. Generic emergence, complexity arising from simple rules, is not a discount until a task is solved more cheaply than by a baseline. Criticality can produce scale-free responses, but the claim that a given living system operates at a critical point requires system-specific evidence and does not explain anything by default. The claim that everything computes costs nothing to make: without fixed inputs, fixed outputs, and a constrained readout, almost any physical system can be read as implementing almost any function, so the claim is weakest where it sounds strongest. Anthropomorphic terms such as memory, decision, preference, frustration, and delayed gratification must be tied to operational criteria such as history dependence, policy switching, error correction, and barrier-sensitive detours, or they presuppose the conclusion they are meant to support. The hardest hidden cost to detect is the observer's own search: testing many substrates and reporting the most striking is a selection cost and belongs in the ledger.

## 7. Research program

The measurements the framework requires share one control. In every case, the test of whether a structure supplies a discount is to destroy the structure while holding component count and energy fixed, and to check that the discount disappears. Examples include scrambling the logarithmic mantissas of a Benford signal, randomizing the symmetry a network was built to exploit, shuffling the local communication topology of a swarm, altering the modal structure of a compliant body, and removing the reusable subproblems from an evolutionary task. In each, the parts are unchanged and only the structure is removed, so a genuine subsidy disappears while an artifact of parameter count or energy budget persists. This is the most diagnostic experiment in the program, and it is available in every domain.

Domain-specific benchmarks follow. A switching study varies an interface from linear elements through thresholds, gain, and recurrence, measures the accessible function family at each stage, and tests whether capability breadth jumps when restoration and cascadability appear or only tracks the added parameters. A Benford study trains estimators with raw, logarithmic, and Benford-prior representations on matched multiplicative and non-multiplicative generators, and tests whether the prior helps only where the generator has the matching structure. A morphological-computation study compares a rigid body with a strong controller against a compliant body with a weak one across the full life-cycle ledger, and records a discount only if it survives fabrication, sensing, and maintenance costs. A modularity study reproduces and extends the modularly varying goals result of Kashtan and Alon (2005), mapping the boundary at which reusable structure stops accelerating adaptation and begins to mislead it, which makes evolvability a measurable property of a genotype-phenotype map (Wagner and Altenberg, 1996). A morphogenesis study compares passive particles, locally goal-directed cells, communicating cells, and cells with persistent physiological memory on construction, repair, and rescaling, and tests whether local competency lowers evolutionary search and central specification once the added cellular machinery is counted. A bioelectric study varies channel conductance, coupling, and voltage-state persistence and estimates a map from interface to accessible morphology; a real subsidy predicts that nearby interface changes produce structured changes in form.

These studies share hypotheses stated sharply enough to fail. Discount magnitude should increase as the substrate's low-cost modes align with the task distribution, an alignment expressible as a decreasing cross-entropy between the distribution of useful solutions and the implicit prior of the substrate-interface system,

$$C_{\mathrm{search}}\propto H\!\left(P^\star,\, Q_{S,I}\right)=-\mathbb{E}_{x\sim P^\star}\log Q_{S,I}(x),$$

proposed as a comparative hypothesis across systems and not as a physical law. Some capabilities should appear discontinuously once the interface supplies a minimal set of properties. The discount should grow with reuse and then saturate or decline as maintenance and interference accumulate. Robustness should aid adaptation in some regimes of population size, mutation rate, and landscape and impede it in others, as Draghi et al. (2010) showed for mutational robustness, so the framework must predict regimes and cannot assign a universal sign. Every strong discount must have a demonstrable mismatch region in which it becomes neutral or harmful; by the No-Free-Lunch constraint, a purported subsidy that helps everywhere indicates an accounting error.

## 8. Conclusion

For a system that appears to do more than it paid for, the productive question is an accounting one: which structure supplied the discount, which interface reached it, in what currency the saving was recorded, and where the remaining cost was paid and stored. Posed this way, the disproportionate competence of a NAND network, a scale-aware estimator, a passive walker, and a regenerating worm becomes four entries in one ledger, recorded in different currencies against different baselines, each with an identifiable cost.

## References

Berger, A., and Hill, T. P. (2011). A basic theory of Benford's Law. *Probability Surveys*, 8, 1--126.

Bongard, J., and Levin, M. (2023). There's plenty of room right here: biological systems as evolved, overloaded, multi-scale machines. *Biomimetics*, 8(1), 110.

Candès, E. J., Romberg, J., and Tao, T. (2006). Robust uncertainty principles: exact signal reconstruction from highly incomplete frequency information. *IEEE Transactions on Information Theory*, 52(2), 489--509.

Clark, A., and Chalmers, D. (1998). The extended mind. *Analysis*, 58(1), 7--19.

Cohen, T., and Welling, M. (2016). Group equivariant convolutional networks. In *Proceedings of the 33rd International Conference on Machine Learning*, PMLR 48, 2990--2999.

Donoho, D. L. (2006). Compressed sensing. *IEEE Transactions on Information Theory*, 52(4), 1289--1306.

Draghi, J. A., Parsons, T. L., Wagner, G. P., and Plotkin, J. B. (2010). Mutational robustness can facilitate adaptation. *Nature*, 463(7279), 353--355.

Durant, F., Morokuma, J., Fields, C., Williams, K., Adams, D. S., and Levin, M. (2017). Long-term, stochastic editing of regenerative anatomy via targeting endogenous bioelectric gradients. *Biophysical Journal*, 112(10), 2231--2243.

Feigenbaum, M. J. (1978). Quantitative universality for a class of nonlinear transformations. *Journal of Statistical Physics*, 19(1), 25--52.

Finn, C., Abbeel, P., and Levine, S. (2017). Model-agnostic meta-learning for fast adaptation of deep networks. In *Proceedings of the 34th International Conference on Machine Learning*, PMLR 70, 1126--1135.

Gould, S. J., and Vrba, E. S. (1982). Exaptation, a missing term in the science of form. *Paleobiology*, 8(1), 4--15.

Gumuskaya, G., Srivastava, P., Cooper, B. G., Lesser, H., Semegran, B., Garnier, S., and Levin, M. (2024). Motile living biobots self-construct from adult human somatic progenitor seed cells. *Advanced Science*, 11(4), 2303575.

Hamming, R. W. (1950). Error detecting and error correcting codes. *Bell System Technical Journal*, 29(2), 147--160.

Kashtan, N., and Alon, U. (2005). Spontaneous evolution of modularity and network motifs. *Proceedings of the National Academy of Sciences*, 102(39), 13773--13778.

Kriegman, S., Blackiston, D., Levin, M., and Bongard, J. (2021). Kinematic self-replication in reconfigurable organisms. *Proceedings of the National Academy of Sciences*, 118(49), e2112672118.

Levin, M. (2022). Technological approach to mind everywhere: an experimentally-grounded framework for understanding diverse bodies and minds. *Frontiers in Systems Neuroscience*, 16, 768201.

Levin, M. (2026). A short argument on Platonic Space. Blog post, thoughtforms.life.

Li, M., and Vitányi, P. (2008). *An Introduction to Kolmogorov Complexity and Its Applications* (3rd ed.). Springer.

Lu, L., Joannopoulos, J. D., and Soljačić, M. (2014). Topological photonics. *Nature Photonics*, 8(11), 821--829.

McGeer, T. (1990). Passive dynamic walking. *International Journal of Robotics Research*, 9(2), 62--82.

Nakajima, K., Hauser, H., Li, T., and Pfeifer, R. (2015). Information processing via physical soft body. *Scientific Reports*, 5, 10487.

Odling-Smee, F. J., Laland, K. N., and Feldman, M. W. (2003). *Niche Construction: The Neglected Process in Evolution*. Princeton University Press.

Rissanen, J. (1978). Modeling by shortest data description. *Automatica*, 14(5), 465--471.

Rothemund, P. W. K. (2006). Folding DNA to create nanoscale shapes and patterns. *Nature*, 440(7082), 297--302.

Sheffer, H. M. (1913). A set of five independent postulates for Boolean algebras, with application to logical constants. *Transactions of the American Mathematical Society*, 14(4), 481--488.

Theraulaz, G., and Bonabeau, E. (1999). A brief history of stigmergy. *Artificial Life*, 5(2), 97--116.

Turing, A. M. (1952). The chemical basis of morphogenesis. *Philosophical Transactions of the Royal Society of London B*, 237(641), 37--72.

Waddington, C. H. (1942). Canalization of development and the inheritance of acquired characters. *Nature*, 150(3811), 563--565.

Wagner, G. P., and Altenberg, L. (1996). Complex adaptations and the evolution of evolvability. *Evolution*, 50(3), 967--976.

Wolpert, D. H., and Macready, W. G. (1997). No free lunch theorems for optimization. *IEEE Transactions on Evolutionary Computation*, 1(1), 67--82.

Wolpert, L. (1969). Positional information and the spatial pattern of cellular differentiation. *Journal of Theoretical Biology*, 25(1), 1--47.

Zaheer, M., Kottur, S., Ravanbakhsh, S., Póczos, B., Salakhutdinov, R., and Smola, A. J. (2017). Deep Sets. *Advances in Neural Information Processing Systems*, 30, 3391--3401.

Zhang, T., Goldstein, A., and Levin, M. (2024). Classical sorting algorithms as a model of morphogenesis: self-sorting arrays reveal unexpected competencies in a minimal model of basal intelligence. *arXiv preprint* arXiv:2401.05375.
