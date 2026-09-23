# DOC-2-019 - RNA Hallucination Detector

## Summary (from `DOC-2-019-RNA-Hallucination-Detector/PROJECT_SUMMARY.md`)


## R0 verdict
Locked useful negative. A short-range sequence-complexity detector was not strong or precise enough under held-out Rfam-family generalization, even against a controlled first-order Markov surrogate.

## Useful discovery
The study was large and leakage-resistant: 2,110 eligible families, 15,658 authentic sequences and 427 fully held-out test families. Nuisance discrimination from length+GC was at chance (AUROC 0.506), and short/long strata each exceeded 0.70. But primary family-macro AUROC was 0.7043 versus the 0.75 gate, with family-bootstrap lower bound 0.6835 versus 0.70. The negative isolates the limitation to short-range sequence features, not trivial nuisance imbalance.

## What is new and why it matters
The experiment turns the playful "RNA hallucination" idea into a family-level audit estimand with an explicit generative null. It shows that plausible local statistics are not enough for a strong family-general detector and blocks premature claims about named RNA models.

## Application
R0 supplies a reusable surrogate benchmark and family-macro evaluation tool. It can screen future structurally informed detectors for family leakage, nuisance exploitation and length instability. It does not evaluate any named RNA generator and cannot establish structural or functional validity.

## Top-lab/grant next question
A separate locked study should use outputs from multiple named RNA generators, model-held-out plus family-held-out axes, experimental structure/error labels, calibrated abstention and external RNA classes. Grant readiness requires showing that the audit changes experimental-priority decisions and transports beyond the surrogate generator.

## Claim boundary
This is a useful negative result, not a complete sculpted project or deployable detector. It adds one result to the program ledger but does not graduate the topic.

## Contents

- `DOC-2-019-RNA-Hallucination-Detector/` - migrated unchanged from `science-program/projects/DOC-2-019-RNA-Hallucination-Detector` (7 files)
- `DOC-2-019/` - migrated unchanged from `science-program/projects/DOC-2-019` (11 files)

## Provenance

Split out of the `science-program` repository (source commit `028a7141ed5f951a7b6e6517d4e72768d414a560`) on 2026-09-23. Every file is byte-identical to the source; `MIGRATION_MANIFEST.tsv` lists sha256, original path and new path for each of the 18 files.

Part of Udita Phookan's computational science program: every experiment locks its question, validation design, success gate and failure policy before outcome analysis, and negative results are preserved. Program-wide ledgers and standards live in the `science-program-ledger` repository.
