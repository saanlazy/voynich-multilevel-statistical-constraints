# Multi-Level Statistical Constraints in the Voynich Manuscript: From Token Structure to Sequential Organization

Author: Youngsan Chang  
Date: April 2026

This repository contains the GitHub-ready and Zenodo-ready reproduction package for Chang 2026f, an integrated manuscript titled 'Multi-Level Statistical Constraints in the Voynich Manuscript: From Token Structure to Sequential Organization.' The study synthesizes five component analyses of the Voynich Manuscript and evaluates structural constraints across positional organization, comparative predictability, prefix-core-suffix dependency, token-generation modeling, and local inter-token arrangement. It does not propose decipherment, translation, or confirmed syntax.

## Summary

This integrated package collects the final preprint PDF, manuscript source, submission materials, figures, tables, methods summaries, and documentation for the Chang 2026f synthesis paper. The manuscript summarizes evidence from Papers 1-5 and frames the result conservatively as multi-level statistical structure rather than semantic reading.

## Research Question

Do the component studies jointly support a multi-level statistical account of Voynich token organization, spanning token position, token predictability, token-internal structure, token generation, and local sequential arrangement?

## Repository Structure

- `paper/` — Zenodo preprint PDF only.
- `source/` — final manuscript source in Markdown.
- `submission/` — Cryptologia submission Word manuscript and cover letter.
- `figures/` — final Figure 1-6 assets in PNG/PDF.
- `tables/` — final Table 1-5 assets in CSV/MD/TXT/PNG/PDF.
- `methods_summary/` — methods summary source files and supporting tables, including `methods_summary_full.md`.
- `docs/` — data/code availability, AI use disclosure, captions, QC reports, package checklist, highlights, significance statement, and supporting documentation.

## Key Results

- Paper 1: positional constraints for line-initial, paragraph-initial, and line-final token classes survive permutation baselines.
- Paper 2: Voynich entropy and ambiguity curves are natural-language-like, while suffix concentration and prefix-family organization remain structurally divergent.
- Paper 3: suffix selection is strongly conditioned on the operationally defined core, with H(suffix|core) = 0.8370 and suffix-from-core top-1 accuracy = 79.11%.
- Paper 4: the PCS token-generation model achieves 97.02% matching and 85.25% token mass coverage, compared with 5.07% and 18.50% for random baselines.
- Paper 5: real local sequences show lower bigram entropy than line-internal shuffle baselines (11.7001 vs. 12.7229) and higher next-token prediction accuracy.

## Integrated Package DOI

The integrated reproduction package for the Chang 2026f synthesis is archived on Zenodo at https://doi.org/10.5281/zenodo.19876003. This DOI identifies the integrated synthesis package, not the five component papers or their separate reproduction packages.

## Component Paper DOIs

- Paper 1: https://doi.org/10.5281/zenodo.19687875
- Paper 2: https://doi.org/10.5281/zenodo.19737888
- Paper 3: https://doi.org/10.5281/zenodo.19765707
- Paper 4: https://doi.org/10.5281/zenodo.19858094
- Paper 5: https://doi.org/10.5281/zenodo.19869629

## Component Package DOIs

- Paper 1 package/concept: https://doi.org/10.5281/zenodo.19689753
- Paper 2 package: https://doi.org/10.5281/zenodo.19737444
- Paper 3 package: https://doi.org/10.5281/zenodo.19765403
- Paper 4 package: https://doi.org/10.5281/zenodo.19857820
- Paper 5 package: https://doi.org/10.5281/zenodo.19869615

The component paper DOI records and component package DOI records are intentionally distinct. Paper-level DOI records identify manuscripts; package DOI records identify reproducibility archives.

## Reproducibility

The integrated package contains the final synthesis PDF, final Markdown source, final Figure 1-6 assets, final Table 1-5 assets, methods summary files, and supporting documentation. Component-level code and full reproduction archives are linked through the component package DOI records above rather than duplicated here.

Required packages for rebuilding or inspecting generated assets are listed in `requirements.txt`.

## Submission and Preprint Files

- `paper/Chang_2026f_Voynich_MultiLevel_Integrated_Zenodo_Preprint.pdf` — Zenodo preprint PDF.
- `submission/Chang_2026f_Voynich_MultiLevel_Integrated_Cryptologia_Submission.docx` — Word manuscript prepared for Cryptologia submission.
- `submission/Cryptologia_Cover_Letter_Final.md` — Cryptologia cover letter draft.

## License

- Text/manuscript: CC BY 4.0
- Code/assets where applicable: MIT License
- Data: follows the original Zandbergen-Landini EVA transcription source terms

## Citation Note

If citing the integrated manuscript, cite the paper record for Chang 2026f when available. If citing or reusing the reproduction materials, cite the associated package record. The component paper DOI records and component package DOI records listed above remain separate by design.
