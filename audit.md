# Audit

Dated log of editorial passes and verification runs. Newest first.
See the workspace docs (run `papers docs`): writing-pipeline.md §7 and refresh-pipeline.md.

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
