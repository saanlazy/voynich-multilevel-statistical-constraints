# Methods Summary Notes

## Purpose
This note documents the source basis for `methods_summary_table.csv`, `methods_summary_table.md`, and `methods_summary_table_manuscript.txt`. The table is intentionally compressed for journal-body use; longer explanations and uncertainties are recorded here.

## Source Files Consulted
- `/Users/admin/Downloads/Chang_2026a_Voynich_Positional_Constraints.pdf`
- `/Users/admin/Downloads/Chang_2026b_Voynich_Comparative.pdf`
- `/Users/admin/Downloads/Chang_2026c_Prefix_Core_Suffix_Voynich.pdf`
- `/Users/admin/Downloads/Chang_2026d_Voynich_PCS_Token_Generation.pdf`
- `/Users/admin/Downloads/Chang_2026e_Voynich_InterToken_v3_refined.pdf`
- `/Users/admin/.gemini/antigravity/codex/voynich-token-explorer/voynich-comparative-study-repro/README.md`
- `/Users/admin/.gemini/antigravity/codex/voynich-token-explorer/voynich-comparative-study-repro/outputs/final_report.md`
- `/Users/admin/.gemini/antigravity/codex/voynich-token-explorer/voynich-comparative-study-repro/outputs/null_model_report.md`
- `/Users/admin/.gemini/antigravity/codex/voynich-token-explorer/voynich-pcs-repro/README.md`
- `/Users/admin/.gemini/antigravity/codex/voynich-token-explorer/voynich-pcs-repro/results/table1_entropy.csv`
- `/Users/admin/.gemini/antigravity/codex/voynich-token-explorer/voynich-pcs-repro/results/table2_prediction.csv`
- `/Users/admin/.gemini/antigravity/codex/voynich-token-explorer/voynich-pcs-repro/results/table3_structure_break.csv`
- `/Users/admin/.gemini/antigravity/codex/voynich-token-explorer/outputs/conditional_structure_report.md`
- `/Users/admin/.gemini/antigravity/codex/voynich-token-explorer/Chang_2026d_Voynich_PCS_Token_Generation_package/README.md`
- `/Users/admin/.gemini/antigravity/codex/voynich-token-explorer/Chang_2026d_Voynich_PCS_Token_Generation_package/docs/REPRODUCIBILITY.md`
- `/Users/admin/.gemini/antigravity/codex/voynich-token-explorer/Chang_2026d_Voynich_PCS_Token_Generation_package/outputs/pcs_validation_report.md`
- `/Users/admin/.gemini/antigravity/codex/voynich-token-explorer/Chang_2026d_Voynich_PCS_Token_Generation_package/outputs/bootstrap_report.md`
- `/Users/admin/.gemini/antigravity/codex/voynich-token-explorer/Chang_2026d_Voynich_PCS_Token_Generation_package/outputs/holdout_report.md`
- `/Users/admin/.gemini/antigravity/codex/voynich-paper5-intertoken/Chang_2026e_Voynich_InterToken_package/README.md`
- `/Users/admin/.gemini/antigravity/codex/voynich-paper5-intertoken/Chang_2026e_Voynich_InterToken_package/docs/REPRODUCIBILITY.md`
- `/Users/admin/.gemini/antigravity/codex/voynich-paper5-intertoken/Chang_2026e_Voynich_InterToken_package/outputs/transition_report.md`
- `/Users/admin/.gemini/antigravity/codex/voynich-paper5-intertoken/Chang_2026e_Voynich_InterToken_package/outputs/intertoken_validation_report.md`

## Paper-by-Paper Source Notes

### Paper 1 — Chang 2026a
- Confirmed from PDF Methods: line- and paragraph-aware positional parsing; alphabetic token retention; working corpus of 5,376 lines, 40,827 alphabetic tokens, and 740 paragraph-initial lines.
- Confirmed metrics: dshedy line-initial bias, p/t/k paragraph-initial concentration, and am-class line-final bias.
- Confirmed null models: global token shuffle, line-internal shuffle, and position-restricted shuffle.
- Confirmed statistical test: 1,000 permutation trials with empirical p = (k + 1) / (N + 1).
- DOI note: the user supplied package/concept DOI `10.5281/zenodo.19689753`; the PDF text references reproduction package `10.5281/zenodo.19689754`. The table follows the user-specified DOI list.

### Paper 2 — Chang 2026b
- Confirmed from PDF Methods and comparative package README: ZL3b compared with English, Latin, synthetic n-gram text, and JSON-like structured data; Latin source is Project Gutenberg ID 18837.
- Confirmed preprocessing: lowercasing, non-alphabetic removal for baseline corpora, whitespace normalization, whitespace tokenization, and shared normalization.
- Confirmed metrics: entropy decay, ambiguity persistence/candidate survival, prefix-family distributions/overlap, suffix distribution/concentration, and cross-dataset similarity.
- Confirmed null models: frequency-preserving shuffle, length-preserving randomization, and prefix-preserving/global suffix model.
- Confirmed tests: PDF states permutation-based significance testing N = 1,000 for correlation scores. Size-matched bootstrap is referenced, but exact bootstrap sample count is not specified in the component paper text consulted.

### Paper 3 — Chang 2026c
- Confirmed from PDF Methods and PCS reproduction README: prefix length = 2, suffix length = 1, core = middle component, tokens shorter than 4 excluded.
- Confirmed corpus: 34,940 alphabetic tokens across 4,618 lines after conservative alphabetic-token filtering.
- Confirmed metrics: mutual information, conditional entropy, and top-1/top-3 prediction accuracy.
- Confirmed baselines/controls: character-shuffled length-preserving baseline, character trigram model, shuffle_cores_only, shuffle_suffixes_only, and shuffle_prefixes_only.
- Confirmed random seed: fixed seed 42. Iteration count for baselines is not specified in the component paper text consulted.

### Paper 4 — Chang 2026d
- Confirmed from PDF Methods, README, and validation reports: PCS generative model using prefix/core/suffix extraction and likelihood-based segmentation; candidate prefixes/suffixes lengths 1-4; fixed-length segmentation checks.
- Confirmed metrics: matching rate, token mass coverage, Zipf slope difference, H(suffix|core), compression ratio, morphological families, and transition entropy.
- Confirmed baselines/validations: random baseline, shuffled baseline, fixed-length segmentation experiments, bootstrap, holdout validation, and length-aware random token construction.
- Confirmed tests: bootstrap N = 1,000; holdout splits 80/20, 70/30, and 50/50; fixed random seed used where stochastic procedures apply.
- Uncertainty: exact main-model corpus token total is not stated in the component paper summary table consulted, so the methods summary table marks it as not specified.

### Paper 5 — Chang 2026e
- Confirmed from PDF Data and Methods, README, and REPRODUCIBILITY.md: line-preserving corpus of 23,753 tokens, 12,688 types, 8,510 lines; mean line length 2.79 tokens.
- Confirmed metrics: bigram/trigram entropy, mutual information, next-token top-1/top-3, PCS inter-token conditional entropy, line-boundary entropy, chi-square, recurrent PCS patterns, and family distance.
- Confirmed baselines: full token shuffle, frequency-preserving shuffle, and line-internal shuffle.
- Confirmed iterations: n-iter 1000 with seed 42 in reproduction command; PDF states empirical tests used 1,000 iterations with fixed random seed.

## Missing or Uncertain Items
- Paper 2: exact number of size-matched bootstrap samples is not specified in the component paper text consulted, although permutation-based significance testing N = 1,000 is specified.
- Paper 3: iteration count for shuffled/trigram baselines is not specified; fixed seed 42 is specified.
- Paper 4: exact main-model corpus token total is not specified in the component paper summary table consulted; validation outputs report train/test sizes for holdout splits.
- Paper 5: recurrent token-pattern report contains some non-EVA labels in an older output, but the methods summary relies on the final Paper 5 manuscript/README and PCS recurrent-pattern framing rather than those labels.

## Recommended Journal-Body Version
Use `methods_summary_table.md` or `methods_summary_table.csv` as the source for the manuscript table. For print layout, the same content may need to be split into two tables: one table for corpus/preprocessing/statistical design and one table for metrics/baselines/outputs.
