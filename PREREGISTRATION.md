# Pre-registration: two out-of-sample tests (written 27 Nov 2026, before any of these runs)

Everything below was fixed before the runs in notebooks PK1 to PK4 were started. The commit that adds this file is the timestamp.
Design file: `configs/exposure_design.json` (sha256 533a7c0548cfa50a...). Predictions file: `configs/validation_predictions.json`.

## Test 1: replication on the untouched SLAKE validation split

The 96 validation images (1,053 questions, 631 open) were never used for training, tuning or analysis. We evaluate the existing models on them unchanged.

**Exposure model (built after the coverage test, fitted only on the 8 SLAKE test-set runs):** P(correct) for an open question = answer effect (shrunk towards its question-type mean) + effect of how many times the answer appears in the training subset (bins 0, 1, 2-4, 5-19, 20+). Leave-one-run-out error on the test set: 0.010.

| Run | Validation open coverage | Predicted open accuracy (exposure model) | Coverage rule (0.69 x C) |
|---|---|---|---|
| img5_s42 | 0.772 | 0.565 | 0.533 |
| img10_s42 | 0.835 | 0.620 | 0.576 |
| img25_s42 | 0.951 | 0.674 | 0.656 |
| img50_s42 | 0.978 | 0.711 | 0.675 |
| covhigh10_s42 | 0.962 | 0.615 | 0.664 |
| covhigh10_s123 | 0.962 | 0.615 | 0.664 |
| covlow10_s42 | 0.658 | 0.593 | 0.454 |
| covlow10_s123 | 0.658 | 0.593 | 0.454 |

**Hypotheses (validation, open questions, exact match, 95% intervals by resampling validation images):**
- V1. Mean absolute error of the exposure model over the 8 runs is below 0.03, and below that of the coverage rule.
- V2. The gain over zero-shot on answers absent from the training subset has an interval that includes zero in every run.
- V3. Gain on answers present in the training subset is positive in every run (interval above zero).
- V4. Open accuracy rises with budget: 22 < 45 < 112 < 225 images.

## Test 2: randomised exposure (causal test of "about five examples per answer")

**Design.** 70 open answers that occur at least 8 times in SLAKE training and appear in test or validation. Each answer is assigned a dose of 0, 1, 2, 4 or 8 training examples (stratified by question type, Latin square), so across 5 runs every answer receives every dose exactly once and every run has 14 answers at each dose. Examples per answer are nested (dose 2 contains dose 1's example, and so on). Every run also contains the same 300 closed (yes/no) training questions. Each run therefore has exactly 510 training questions; model, LoRA settings, seed (42) and 3 epochs are identical to the earlier runs. Only the dose assignment differs.

**Outcome.** For each answer and run: open accuracy on the test and validation questions with that answer (1,094 questions). Analysis: linear probability model with answer and run fixed effects; 95% intervals by bootstrap over answers (2,000 resamples).

**Hypotheses.**
- E1 (primary). Accuracy at dose 8 minus dose 0 is positive (interval above zero).
- E2. Point estimates rise with dose: 0 < 1 < 2 < 4 < 8.
- E3. Dose 1 gives less than half of the dose-8 gain.
- E4 (size, from the observational estimates +0.08, +0.18, +0.30): dose 1 between 0.00 and +0.15; dose 8 at least +0.20.

Any result, including a failure, will be reported.
