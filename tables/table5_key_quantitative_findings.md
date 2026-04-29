| Measure | Observed / model value | Baseline / contrast | Interpretation |
| --- | --- | --- | --- |
| PCS matching rate | 97.02% | Random baseline 5.07% | Structured recombination reproduces observed forms far better than random generation. |
| Token mass coverage | 85.25% | Random baseline 18.50% | Frequent corpus mass is captured by the PCS model. |
| Zipf slope difference | 0.0795 | Random baseline 0.7138 | Generated distribution remains close to real frequency structure. |
| H(suffix/core) | 0.8370 | H(core/prefix) = 5.3205 | Suffix selection is much more constrained by core than core is by prefix. |
| Compression ratio | Real 0.3089; PCS 0.3163 | Shuffled 0.3240 | Real and PCS-generated corpora are more compressible than shuffled text. |
| Bigram entropy | Real 11.7001 | Line-internal shuffle 12.7229 | Real local ordering is more constrained than line-preserving randomization. |
| Next-token prediction | Top-1 0.6917; top-3 0.8168 | Baseline top-1 0.5505; top-3 0.6912 | Observed local sequences improve next-token predictability. |
| Line-position dependence | Chi-square = 46151.0531 | p < .001 | Line position is statistically associated with token distribution. |
| Family clustering | Same-core mean distance 235.93 | Shuffled 442.77 | Related token families cluster locally. |
