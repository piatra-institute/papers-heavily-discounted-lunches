# Audit

Dated log of editorial passes and verification runs. Newest first.
See the workspace docs (run `papers docs`): writing-pipeline.md §7 and refresh-pipeline.md.

## 2026-09-23 — structured-evidence migration

Structured-evidence migration (references and claims).
- references.yaml: 33 CSL entries. 25 matched in Crossref by title, authors and year; donoho2006, wagner1996 and gumuskaya2024 resolved through doi.org; cohen2016, finn2017 and zaheer2017 entered from PMLR/NeurIPS proceedings pages; li2008 and odlingsmee2003 from publisher details; levin2026 from the blog post (thoughtforms.life, 2026-03-31). In-text citations converted to Pandoc [@id] syntax; legacy reference list replaced by the citeproc-rendered list (Chicago author-date).
- Corrections: gumuskaya2024 automatic match was the journal's cover-image record (10.1002/advs.202470026), replaced by the article (10.1002/advs.202303575); levin2026 title completed to the post's full title ("A Short Argument on Platonic Space: Variable-Agency Patterns That In-Form Physics, Biology, Computer Science, and Cognitive Science"); zhang2024 updated from arXiv:2401.05375 to its published version (Adaptive Behavior 33(1), 25-54, DOI 10.1177/10597123241269740); article numbers/pages added (berger2011 1-126, bongard2023 110, kriegman2021 e2112672118, levin2022 768201, nakajima2015 10487); Candès accent and Waddington title casing restored.
- claims.yaml: 36 claims (16 source, 11 interpretation, 4 definition, 3 assumption, 2 normative). No simulation; the Benford probabilities 0.301 and 0.046 are bound as arithmetic from the stated law.
- Source statements not bound: the triangle example attributed to Levin (not found in the blog post; the ion-channel/truth-table example is confirmed), sheffer1913, li2008 (information bound), rissanen1978, cohen2016/zaheer2017, finn2017, clark1998, odlingsmee2003, hamming1950, waddington1942, lu2014, feigenbaum1978, wolpert1969, draghi2010, wagner1996, levin2022 (no abstract retrieved or abstract not covering the specific statement).
- metadata claims_target: claim-ledger.

## 2026-09-23 — prose revision

Prose rewritten against the house standards. Headings made descriptive (1. Introduction, 2. Conservation constraints, 3. Accounting framework, 4. Sources and mechanisms of discounts, 5. Case studies with 5.1 Functional completeness and switching interfaces, 5.2 Benford's law as a matched prior, 5.3 Morphological computation, 5.4 Morphogenesis and competent components, 6. The inference ladder, 7. Research program, 8. Conclusion). The former closing paragraph of section 7 became section 8.

Tic counts before -> after: 'rather than' 12 -> 0; inline ', not X' 4 -> 0; 'worth' 3 -> 0; 'what follows/here is' 2 -> 0; 'exactly/precisely' 5 -> 1 (the technical "recovers exactly" of compressed sensing); 'merely/simply' 4 -> 0.

Corrections: none needed. Numerical claims rechecked: P(D=1) = log10 2 = 0.30103 -> 0.301 and P(D=9) = log10(10/9) = 0.04576 -> 0.046 are correct; the significand density 1/(s ln b) is correct; H_j = 1, 2, -1 correspond to tenfold saving, hundredfold saving, tenfold penalty. The inference ladder has seven levels (0 to 6) and six steps between them, as stated.

Grid audit: not applicable (has_simulation: false; no computed thresholds).

## 2026-07-15 — first draft through publish

Scope: authored the paper end to end from the seed conversation in `chats/chat.md` (a ChatGPT research exchange proposing the "Heavily Discounted Lunches" framework), through the full pipeline to a built and web-synced PDF.

Kind: synthesis. `has_simulation: false`, `claims_target: none`; the numbers in the prose are cited literature results and framework-internal definitions, so there is no simulation to reconcile against.

Changes:
- `brief.md`, `research.md`, `sources.md` written first (research pipeline). The seed's substance was reorganized into a rigorous cross-disciplinary Perspective and stripped of its AI-slop presentation (bullet dumps, "Takeaway", emoji favicons, table-per-idea).
- Every citation web-verified against the publisher record before freezing the bibliography (33 sources). Confirmed the higher-error recent ones: Gumuskaya et al. Anthrobots (*Advanced Science* 11(4):2303575, 2024), Durant et al. planaria (*Biophys. J.* 112(10):2231--2243, 2017), Kriegman et al. kinematic replication (*PNAS* 118(49):e2112672118, 2021), Nakajima et al. reservoir (*Sci. Rep.* 5:10487, 2015), Bongard & Levin polycomputing (*Biomimetics* 8(1):110, 2023), Berger & Hill Benford (*Probability Surveys* 8:1--126, 2011), Draghi et al. robustness (*Nature* 463:353--355, 2010), Lu et al. topological photonics (*Nat. Photonics* 8:821--829, 2014), Kashtan & Alon modularity (*PNAS* 102(39):13773--13778, 2005). Kept the distinction between D. H. Wolpert (No Free Lunch) and L. Wolpert (positional information), and between Levine (MAML) and Levin.
- `paper/PAPER.md` drafted in the house voice: argument-driven numbered sections, no roadmap paragraph, no ceremonial conclusion, limits folded into the argument (the conservation bounds in section 2, the observer discipline in 5.3, the underdetermination in 5.4, the cautions in 6). Formal spine in display math (effective cost, discount factor and vector, capability breadth, interface leverage, amortization, the Benford significand law, the cross-entropy search-cost hypothesis); inline math throughout, no raw Unicode. The four case studies (NAND switching, Benford, body as coprocessor, morphogenesis) each carry a named negative regime. Ends on the reframed accounting question, not a tagline.
- Voice pass: cleared the one real negate-pivot (the Benford "not about the numeral 1" construction) and trimmed the flagged pet-vocabulary (`carries` 7 -> 3, `the very`, `precisely`, `discipline`, `the move`, `earns a place`).
- `metadata.yaml`: title, header, `date: July 2026`, abstract, `status: published`. `README.md` rewritten from the stub.

Verification:
- voice: 0 errors, 7 review-candidates (inline-contrastive and one bare negation, all developed contrasts inherent to the argument). Advisory tricolon density is high, as expected for a taxonomy paper whose content is enumerations (cost currencies, the seven operations, the source axes, the admission standards).
- refs: 33 in-text keys / 33 entries, 0 missing, 0 unused.
- claims: `none` (manual; no simulation).
- build: 16 pages, 0 missing-character warnings.
- check => PASS. PDF synced to `public/papers/heavily-discounted-lunches.pdf`.

Not done (left for the author): paste the emitted `web-entry` object into `app/papers/page.tsx` `ownPapers[]` with hand-picked `topics`/`kinds`; create the GitHub repo and push (origin is already configured).
