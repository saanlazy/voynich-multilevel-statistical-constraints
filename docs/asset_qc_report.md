# Integrated Asset QC Report

## Input Files Used
- integrated_pdf: `/Users/admin/Downloads/Chang_2026f_Voynich_MultiLevel_Integrated_Final.pdf`
- paper3_entropy: `/Users/admin/.gemini/antigravity/codex/voynich-token-explorer/voynich-pcs-repro/results/table1_entropy.csv`
- paper3_prediction: `/Users/admin/.gemini/antigravity/codex/voynich-token-explorer/voynich-pcs-repro/results/table2_prediction.csv`
- paper4_overall: `/Users/admin/.gemini/antigravity/codex/voynich-token-explorer/Chang_2026d_Voynich_PCS_Token_Generation_package/tables/table1_overall.csv`
- paper4_extended: `/Users/admin/.gemini/antigravity/codex/voynich-token-explorer/Chang_2026d_Voynich_PCS_Token_Generation_package/tables/table5_extended.csv`
- paper5_summary: `/Users/admin/.gemini/antigravity/codex/voynich-paper5-intertoken/Chang_2026e_Voynich_InterToken_package/tables/table6_key_results_summary.csv`
- paper5_transition: `/Users/admin/.gemini/antigravity/codex/voynich-paper5-intertoken/Chang_2026e_Voynich_InterToken_package/outputs/transition_metrics.csv`
- paper5_pcs_transition: `/Users/admin/.gemini/antigravity/codex/voynich-paper5-intertoken/Chang_2026e_Voynich_InterToken_package/outputs/pcs_transition_metrics.csv`
- paper5_family: `/Users/admin/.gemini/antigravity/codex/voynich-paper5-intertoken/Chang_2026e_Voynich_InterToken_package/outputs/family_distance_metrics.csv`

## Current Integrated PDF Reference Order
- Detected order: Table 1., Figure 4., Figure 1., Figure 2., Figure 3., Figure 5., Figure 6., Table 2., Table 3.
- Existing issue: the current PDF text mentions Figure 4 before Figures 1-3 because conditional entropy appears first in the Results section.
- Intended final figure asset order: Figure 1 conditional entropy; Figure 2 matching rate; Figure 3 token mass coverage; Figure 4 Zipf slope difference; Figure 5 compression comparison; Figure 6 inter-token structure.
- Table order is already Table 1, Table 2, Table 3.

## Generated Tables
- `table1_study_overview.csv` plus `.md`, `.png`, `.pdf` variants
- `table2_integrated_evidence_matrix.csv` plus `.md`, `.png`, `.pdf` variants
- `table3_key_quantitative_results.csv` plus `.md`, `.png`, `.pdf` variants

## Generated Figures
- `figure1_pcs_conditional_entropy.png` plus `.pdf` variant
- `figure2_pcs_generation_matching_rate.png` plus `.pdf` variant
- `figure3_token_mass_coverage.png` plus `.pdf` variant
- `figure4_zipf_slope_difference.png` plus `.pdf` variant
- `figure5_compression_comparison.png` plus `.pdf` variant
- `figure6_intertoken_structure.png` plus `.pdf` variant

## Source Metrics
- Table 1: component-study PDF/draft synthesis and integrated manuscript summary.
- Table 2: integrated manuscript structure plus component-study outputs listed above.
- Table 3: Paper 3 entropy/prediction CSV, Paper 4 overall/extended tables, and Paper 5 transition/summary tables.
- Figures 1-4: Paper 3 entropy CSV and Paper 4 overall CSV.
- Figure 5: Paper 4 compression values reported in Paper 4 output/reproduction package; shuffled-real gain cross-check from table5_extended.csv.
- Figure 6: Paper 5 transition_metrics.csv and table6_key_results_summary.csv.

## Empty Cell Check
No empty table cells detected.

## Label / Axis / Legend Check
- All figures include titles and y-axis labels.
- Figure 6 includes panel labels and a legend for real vs line-internal baseline.
- Table images include complete cell text and captions; CSV/Markdown variants preserve full values.

## Missing Files
None.

## Resolution of Existing Asset Issues
- Figure numbering issue: resolved in the asset set by assigning numbers according to actual body order, with conditional entropy as Figure 1.
- Empty table cells: resolved; generated CSVs have no blank cells.
- Table layout: regenerated as standalone PNG/PDF assets with wider columns and wrapped text to avoid clipped cells.
- Figure readability: regenerated at high resolution using restrained grayscale styling and larger labels.

## Conservative Interpretation Note
The captions avoid claims of semantic decipherment, translation, or full syntax. They frame the evidence as structured organization and non-random arrangement.
