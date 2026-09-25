# Main prediction table: cell sources

Columns: Capability; Delivered relation; Error; Strongest development baseline; Error; Improvement.
Rendered layout: six columns, with an italic task group line spanning all six columns followed by Mathematics, Code and Question answering rows. Coordinates are zero-based physical body rows and columns, excluding headers and rules: group lines occupy rows 0, 4, 8, 12 and 16 at column 0 with column_span 6; capability rows occupy the following three rows. Every cell is populated. The appendix candidates table prints columns Prediction task; Pre-specified candidate; Candidate error (nats); Delivered relation from the same assembled rows; its recipes follow the main table's.
Development measurements are distinct development configuration measurements per capability for fitting or selecting the tested candidate, excluding dense anchors and held-out measurements. Counts do not describe the post-test delivered predictor. V53 divides recorded scalar rows by the recorded capability-model count; V55/V69 use n_dev_cells; V70 uses development_structure.n_points authenticated by freeze.json. Shared development sets are not additive across rows.
Each capability row has a delivered identity, delivered error, baseline identity, baseline error and signed improvement (baseline minus delivered, computed before rounding). These cells retain their individual frozen JSON recipes. The group line retains the task's configuration numbers and development measurement count. Development or registration selection pointers are recorded in each baseline cell's note/context. Short task labels retain the full state and configuration definitions in their source recipes.
Retrospective appears in the group line only when the stored delivered timing says fixed after test; first predictors were frozen before measurement. Delivered scores reuse the same frozen test cells, not test-error winners. For the earlier bit test the delivered interpolation/median rule has no matching stored score; its development includes those cells. The source surface is not delivered, and the older interpolation's different model and boundary rules cannot supply the missing error.
Stored V70 paired_difference.ci95 endpoints are omitted from Table 1 because they do not fit on the same line as the score. They remain in the appendix tables. The sign is baseline minus candidate; these are not MAE intervals. No refits, resampling or invented intervals.
All indices are zero-based. The numeric inventory identifies the table, physical row/column and recipe part, so appendix and main-table coordinates are distinct. `mean` is equal-weight arithmetic; `weighted_mean` pairs each stored subset MAE with its stored cell count, preserving equal cell weights. No refits or resampling.
Numeric values are formatted directly from the following executable source recipes. Context pointers justify textual labels and freeze identities; incomplete tasks are omitted.
The `label` operation uses the generator's explicit presentation mappings; `expected` preserves the source values and must match before rendering `label`. Counts always use their own JSON fields.
The `shared` operation prints a common value only after checking that all grouped source values are identical.

## Loader reuse and limits

Reused v86_main_table.build_rows, Comparison.number, row_scores and paired_rows; pruning inputs are v53-prune-dev register/predictions/compare and v72-prune-repeat freeze/compare. Did not use test-ranked Row.baselines or post-hoc Row.delivered.
V47 original freeze.json is absent: that original test is omitted here. The registered v5_confirm section is paired with the available V70 freeze.
results/v93-confirm-inputs/pythia-160m--step32000/math/descriptor_bv.json#/aggregates: dense descriptors only; no frozen response prediction or error interval. Not scored as a predictor.
results/v93-confirm-inputs/pythia-160m--step32000/code/descriptor_bv.json#/aggregates: dense descriptors only; no frozen response prediction or error interval. Not scored as a predictor.
results/v93-confirm-inputs/pythia-160m--step32000/qa/descriptor_bv.json#/aggregates: dense descriptors only; no frozen response prediction or error interval. Not scored as a predictor.
results/v93-confirm-inputs/pythia-410m--step32000/math/descriptor_bv.json#/aggregates: dense descriptors only; no frozen response prediction or error interval. Not scored as a predictor.
results/v93-confirm-inputs/pythia-410m--step32000/code/descriptor_bv.json#/aggregates: dense descriptors only; no frozen response prediction or error interval. Not scored as a predictor.
results/v93-confirm-inputs/pythia-410m--step32000/qa/descriptor_bv.json#/aggregates: dense descriptors only; no frozen response prediction or error interval. Not scored as a predictor.
results/v93-confirm-inputs/pythia-1.4b--step32000/math/descriptor_bv.json#/aggregates: dense descriptors only; no frozen response prediction or error interval. Not scored as a predictor.
results/v93-confirm-inputs/pythia-1.4b--step32000/code/descriptor_bv.json#/aggregates: dense descriptors only; no frozen response prediction or error interval. Not scored as a predictor.
results/v93-confirm-inputs/pythia-1.4b--step32000/qa/descriptor_bv.json#/aggregates: dense descriptors only; no frozen response prediction or error interval. Not scored as a predictor.
results/v93-confirm-inputs/pythia-1b--step64000/math/descriptor_bv.json#/aggregates: dense descriptors only; no frozen response prediction or error interval. Not scored as a predictor.
results/v93-confirm-inputs/pythia-1b--step64000/code/descriptor_bv.json#/aggregates: dense descriptors only; no frozen response prediction or error interval. Not scored as a predictor.
results/v93-confirm-inputs/pythia-1b--step64000/qa/descriptor_bv.json#/aggregates: dense descriptors only; no frozen response prediction or error interval. Not scored as a predictor.
V78 is a prospective decision test with frozen configuration predictions; its regret and test oracle are not substituted for relation MAE or a development baseline.
V46 is an earlier new-state test; its freeze identity is checked. Its strongest development baseline is not recorded in the supplied V46 pair, so it is not mixed into the later V53 score.
V70 paired_difference.ci95 is a baseline-minus-candidate interval, never an MAE interval.
Development-only density, budget and data-reuse tasks are outside this frozen-prediction table.
V72 repeats use the same weights; no displayed score uses those repeats.
The earlier unseen-bit-width test moves to the candidate-form appendix: its cells entered the later development grid, so the delivered rule has no independent error on them. Frozen low-order surface: 0.193 / 0.214 / 0.436 nats against 0.553 / 0.726 / 0.537 for the development-selected baseline (development median / development median / development median), from 24 development configuration measurements per capability.

## Fields per cell

- Cell (0, 0): `results/v53-prune-dev/register.json#/selected_candidate`; `results/v53-prune-dev/register.json#/dev_states`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/densities`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/tag`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/tag`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/densities`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/tag`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/densities`; `results/v53-prune-dev/register.json#/n_dev_rows`; `results/v53-prune-dev/register.json#/models`; `results/v86-main-table/summary.json#/main_rows/0/delivered_timing`
- Cell (1, 0): `results/v86-main-table/summary.json#/main_rows/0/capabilities/math/delivered`
- Cell (1, 1): `results/v86-main-table/summary.json#/main_rows/0/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/0/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/0/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/0/capabilities/qa/delivered`
- Cell (1, 2): `results/v86-main-table/summary.json#/main_rows/0/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/0/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/0/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/0/capabilities/qa/delivered`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/math`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/math`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/math`
- Cell (1, 3): `results/v53-prune-dev/register.json#/loso_table`; `results/v53-prune-dev/register.json#/loso_table/2/candidate`
- Cell (1, 4): `results/v53-prune-dev/register.json#/loso_table`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/A2/math`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/A2/math`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/A2/math`
- Cell (1, 5): `results/v86-main-table/summary.json#/main_rows/0/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/0/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/0/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/0/capabilities/qa/delivered`; `results/v53-prune-dev/register.json#/loso_table`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/math`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/math`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/math`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/A2/math`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/A2/math`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/A2/math`
- Cell (2, 0): `results/v86-main-table/summary.json#/main_rows/0/capabilities/code/delivered`
- Cell (2, 1): `results/v86-main-table/summary.json#/main_rows/0/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/0/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/0/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/0/capabilities/qa/delivered`
- Cell (2, 2): `results/v86-main-table/summary.json#/main_rows/0/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/0/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/0/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/0/capabilities/qa/delivered`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/code`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/code`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/code`
- Cell (2, 3): `results/v53-prune-dev/register.json#/loso_table`; `results/v53-prune-dev/register.json#/loso_table/2/candidate`
- Cell (2, 4): `results/v53-prune-dev/register.json#/loso_table`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/A2/code`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/A2/code`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/A2/code`
- Cell (2, 5): `results/v86-main-table/summary.json#/main_rows/0/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/0/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/0/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/0/capabilities/qa/delivered`; `results/v53-prune-dev/register.json#/loso_table`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/code`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/code`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/code`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/A2/code`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/A2/code`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/A2/code`
- Cell (3, 0): `results/v86-main-table/summary.json#/main_rows/0/capabilities/qa/delivered`
- Cell (3, 1): `results/v86-main-table/summary.json#/main_rows/0/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/0/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/0/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/0/capabilities/qa/delivered`
- Cell (3, 2): `results/v86-main-table/summary.json#/main_rows/0/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/0/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/0/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/0/capabilities/qa/delivered`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/qa`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/qa`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/qa`
- Cell (3, 3): `results/v53-prune-dev/register.json#/loso_table`; `results/v53-prune-dev/register.json#/loso_table/5/candidate`
- Cell (3, 4): `results/v53-prune-dev/register.json#/loso_table`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/qa`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/qa`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/qa`
- Cell (3, 5): `results/v86-main-table/summary.json#/main_rows/0/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/0/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/0/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/0/capabilities/qa/delivered`; `results/v53-prune-dev/register.json#/loso_table`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/qa`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/qa`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/qa`
- Cell (4, 0): `results/v69-quant-confirm/freeze.json#/frozen_at_utc`; `results/v69-quant-confirm/compare.json#/rows/0/test_set`; `results/v69-quant-confirm/compare.json#/rows/1/test_set`; `results/v69-quant-confirm/compare.json#/rows/2/test_set`; `results/v69-quant-confirm/compare.json#/rows/3/test_set`; `results/v69-quant-confirm/compare.json#/rows/4/test_set`; `results/v69-quant-confirm/compare.json#/rows/5/test_set`; `results/v69-quant-confirm/compare.json#/rows/6/test_set`; `results/v69-quant-confirm/compare.json#/rows/7/test_set`; `results/v69-quant-confirm/compare.json#/rows/8/test_set`; `results/v69-quant-confirm/compare.json#/rows/9/test_set`; `results/v69-quant-confirm/compare.json#/rows/10/test_set`; `results/v69-quant-confirm/compare.json#/rows/11/test_set`; `results/v69-quant-confirm/compare.json#/rows/12/test_set`; `results/v69-quant-confirm/compare.json#/rows/13/test_set`; `results/v69-quant-confirm/compare.json#/rows/14/test_set`; `results/v69-quant-confirm/compare.json#/rows/15/test_set`; `results/v69-quant-confirm/compare.json#/rows/16/test_set`; `results/v69-quant-confirm/compare.json#/rows/17/test_set`; `results/v69-quant-confirm/compare.json#/rows/18/test_set`; `results/v69-quant-confirm/compare.json#/rows/19/test_set`; `results/v69-quant-confirm/compare.json#/rows/20/test_set`; `results/v69-quant-confirm/compare.json#/rows/21/test_set`; `results/v69-quant-confirm/compare.json#/rows/22/test_set`; `results/v69-quant-confirm/compare.json#/rows/23/test_set`; `results/v69-quant-confirm/compare.json#/rows/24/test_set`; `results/v69-quant-confirm/compare.json#/rows/25/test_set`; `results/v69-quant-confirm/compare.json#/rows/26/test_set`; `results/v69-quant-confirm/compare.json#/rows/27/test_set`; `results/v69-quant-confirm/compare.json#/rows/28/test_set`; `results/v69-quant-confirm/compare.json#/rows/29/test_set`; `results/v69-quant-confirm/compare.json#/rows/30/test_set`; `results/v69-quant-confirm/compare.json#/rows/31/test_set`; `results/v69-quant-confirm/compare.json#/rows/32/test_set`; `results/v69-quant-confirm/compare.json#/rows/33/test_set`; `results/v69-quant-confirm/compare.json#/rows/34/test_set`; `results/v69-quant-confirm/compare.json#/rows/35/test_set`; `results/v69-quant-confirm/develop.json#/dev_states`; `results/v69-quant-confirm/develop.json#/dev_configs`; `results/v69-quant-confirm/develop.json#/selection_rule`; `results/v69-quant-confirm/compare.json#/rows/0/state`; `results/v69-quant-confirm/compare.json#/rows/0/config`; `results/v69-quant-confirm/compare.json#/rows/3/config`; `results/v69-quant-confirm/compare.json#/rows/6/config`; `results/v69-quant-confirm/compare.json#/rows/9/config`; `results/v69-quant-confirm/compare.json#/rows/12/config`; `results/v69-quant-confirm/compare.json#/rows/15/config`; `results/v69-quant-confirm/compare.json#/rows/18/state`; `results/v69-quant-confirm/develop.json#/n_dev_cells`; `results/v86-main-table/summary.json#/main_rows/2/delivered_timing`
- Cell (5, 0): `results/v86-main-table/summary.json#/main_rows/2/capabilities/math/delivered`
- Cell (5, 1): `results/v86-main-table/summary.json#/main_rows/2/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/2/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/2/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/2/capabilities/qa/delivered`; `results/v74-quant-threeway/quant_threeway.json#/recommendation_rule`
- Cell (5, 2): `results/v86-main-table/summary.json#/main_rows/2/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/2/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/2/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/2/capabilities/qa/delivered`; `results/v74-quant-threeway/quant_threeway.json#/recommendation_rule`; `results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/same_input_interpolation/math/mae`
- Cell (5, 3): `results/v69-quant-confirm/develop.json#/loso/scores`; `results/v69-quant-confirm/develop.json#/loso/scores/bilinear/math`
- Cell (5, 4): `results/v69-quant-confirm/develop.json#/loso/scores`; `results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/bilinear/math/mae`
- Cell (5, 5): `results/v86-main-table/summary.json#/main_rows/2/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/2/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/2/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/2/capabilities/qa/delivered`; `results/v74-quant-threeway/quant_threeway.json#/recommendation_rule`; `results/v69-quant-confirm/develop.json#/loso/scores`; `results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/same_input_interpolation/math/mae`; `results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/bilinear/math/mae`
- Cell (6, 0): `results/v86-main-table/summary.json#/main_rows/2/capabilities/code/delivered`
- Cell (6, 1): `results/v86-main-table/summary.json#/main_rows/2/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/2/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/2/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/2/capabilities/qa/delivered`; `results/v74-quant-threeway/quant_threeway.json#/recommendation_rule`
- Cell (6, 2): `results/v86-main-table/summary.json#/main_rows/2/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/2/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/2/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/2/capabilities/qa/delivered`; `results/v74-quant-threeway/quant_threeway.json#/recommendation_rule`; `results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/same_input_interpolation/code/mae`
- Cell (6, 3): `results/v69-quant-confirm/develop.json#/loso/scores`; `results/v69-quant-confirm/develop.json#/loso/scores/zero/code`
- Cell (6, 4): `results/v69-quant-confirm/develop.json#/loso/scores`; `results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/zero/code/mae`
- Cell (6, 5): `results/v86-main-table/summary.json#/main_rows/2/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/2/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/2/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/2/capabilities/qa/delivered`; `results/v74-quant-threeway/quant_threeway.json#/recommendation_rule`; `results/v69-quant-confirm/develop.json#/loso/scores`; `results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/same_input_interpolation/code/mae`; `results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/zero/code/mae`
- Cell (7, 0): `results/v86-main-table/summary.json#/main_rows/2/capabilities/qa/delivered`
- Cell (7, 1): `results/v86-main-table/summary.json#/main_rows/2/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/2/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/2/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/2/capabilities/qa/delivered`; `results/v74-quant-threeway/quant_threeway.json#/recommendation_rule`
- Cell (7, 2): `results/v86-main-table/summary.json#/main_rows/2/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/2/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/2/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/2/capabilities/qa/delivered`; `results/v74-quant-threeway/quant_threeway.json#/recommendation_rule`; `results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/median/qa/mae`
- Cell (7, 3): `results/v69-quant-confirm/develop.json#/loso/scores`; `results/v69-quant-confirm/develop.json#/loso/scores/median/qa`
- Cell (7, 4): `results/v69-quant-confirm/develop.json#/loso/scores`; `results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/median/qa/mae`
- Cell (7, 5): `results/v86-main-table/summary.json#/main_rows/2/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/2/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/2/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/2/capabilities/qa/delivered`; `results/v74-quant-threeway/quant_threeway.json#/recommendation_rule`; `results/v69-quant-confirm/develop.json#/loso/scores`; `results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/median/qa/mae`
- Cell (8, 0): `results/v69-quant-confirm/freeze.json#/frozen_at_utc`; `results/v69-quant-confirm/compare.json#/rows/36/test_set`; `results/v69-quant-confirm/compare.json#/rows/37/test_set`; `results/v69-quant-confirm/compare.json#/rows/38/test_set`; `results/v69-quant-confirm/compare.json#/rows/39/test_set`; `results/v69-quant-confirm/compare.json#/rows/40/test_set`; `results/v69-quant-confirm/compare.json#/rows/41/test_set`; `results/v69-quant-confirm/compare.json#/rows/42/test_set`; `results/v69-quant-confirm/compare.json#/rows/43/test_set`; `results/v69-quant-confirm/compare.json#/rows/44/test_set`; `results/v69-quant-confirm/compare.json#/rows/45/test_set`; `results/v69-quant-confirm/compare.json#/rows/46/test_set`; `results/v69-quant-confirm/compare.json#/rows/47/test_set`; `results/v69-quant-confirm/compare.json#/rows/48/test_set`; `results/v69-quant-confirm/compare.json#/rows/49/test_set`; `results/v69-quant-confirm/compare.json#/rows/50/test_set`; `results/v69-quant-confirm/compare.json#/rows/51/test_set`; `results/v69-quant-confirm/compare.json#/rows/52/test_set`; `results/v69-quant-confirm/compare.json#/rows/53/test_set`; `results/v69-quant-confirm/compare.json#/rows/54/test_set`; `results/v69-quant-confirm/compare.json#/rows/55/test_set`; `results/v69-quant-confirm/compare.json#/rows/56/test_set`; `results/v69-quant-confirm/compare.json#/rows/57/test_set`; `results/v69-quant-confirm/compare.json#/rows/58/test_set`; `results/v69-quant-confirm/compare.json#/rows/59/test_set`; `results/v69-quant-confirm/compare.json#/rows/60/test_set`; `results/v69-quant-confirm/compare.json#/rows/61/test_set`; `results/v69-quant-confirm/compare.json#/rows/62/test_set`; `results/v69-quant-confirm/develop.json#/dev_states`; `results/v69-quant-confirm/develop.json#/dev_configs`; `results/v69-quant-confirm/develop.json#/selection_rule`; `results/v69-quant-confirm/compare.json#/rows/36/state`; `results/v69-quant-confirm/compare.json#/rows/36/config`; `results/v69-quant-confirm/compare.json#/rows/39/config`; `results/v69-quant-confirm/compare.json#/rows/42/config`; `results/v69-quant-confirm/compare.json#/rows/45/config`; `results/v69-quant-confirm/compare.json#/rows/48/config`; `results/v69-quant-confirm/compare.json#/rows/51/config`; `results/v69-quant-confirm/compare.json#/rows/54/config`; `results/v69-quant-confirm/compare.json#/rows/57/config`; `results/v69-quant-confirm/compare.json#/rows/60/config`; `results/v69-quant-confirm/develop.json#/n_dev_cells`; `results/v86-main-table/summary.json#/main_rows/3/delivered_timing`
- Cell (9, 0): `results/v86-main-table/summary.json#/main_rows/3/capabilities/math/delivered`
- Cell (9, 1): `results/v86-main-table/summary.json#/main_rows/3/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/3/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/3/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/3/capabilities/qa/delivered`; `results/v74-quant-threeway/quant_threeway.json#/recommendation_rule`
- Cell (9, 2): `results/v86-main-table/summary.json#/main_rows/3/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/3/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/3/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/3/capabilities/qa/delivered`; `results/v74-quant-threeway/quant_threeway.json#/recommendation_rule`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/math/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/math/n`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/math/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/math/n`
- Cell (9, 3): `results/v69-quant-confirm/develop.json#/loso/scores`; `results/v69-quant-confirm/develop.json#/loso/scores/bilinear/math`
- Cell (9, 4): `results/v69-quant-confirm/develop.json#/loso/scores`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/bilinear/math/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/bilinear/math/n`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/bilinear/math/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/bilinear/math/n`
- Cell (9, 5): `results/v86-main-table/summary.json#/main_rows/3/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/3/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/3/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/3/capabilities/qa/delivered`; `results/v74-quant-threeway/quant_threeway.json#/recommendation_rule`; `results/v69-quant-confirm/develop.json#/loso/scores`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/math/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/math/n`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/math/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/math/n`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/bilinear/math/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/bilinear/math/n`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/bilinear/math/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/bilinear/math/n`
- Cell (10, 0): `results/v86-main-table/summary.json#/main_rows/3/capabilities/code/delivered`
- Cell (10, 1): `results/v86-main-table/summary.json#/main_rows/3/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/3/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/3/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/3/capabilities/qa/delivered`; `results/v74-quant-threeway/quant_threeway.json#/recommendation_rule`
- Cell (10, 2): `results/v86-main-table/summary.json#/main_rows/3/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/3/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/3/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/3/capabilities/qa/delivered`; `results/v74-quant-threeway/quant_threeway.json#/recommendation_rule`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/code/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/code/n`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/code/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/code/n`
- Cell (10, 3): `results/v69-quant-confirm/develop.json#/loso/scores`; `results/v69-quant-confirm/develop.json#/loso/scores/zero/code`
- Cell (10, 4): `results/v69-quant-confirm/develop.json#/loso/scores`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/zero/code/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/zero/code/n`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/zero/code/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/zero/code/n`
- Cell (10, 5): `results/v86-main-table/summary.json#/main_rows/3/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/3/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/3/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/3/capabilities/qa/delivered`; `results/v74-quant-threeway/quant_threeway.json#/recommendation_rule`; `results/v69-quant-confirm/develop.json#/loso/scores`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/code/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/code/n`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/code/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/code/n`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/zero/code/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/zero/code/n`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/zero/code/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/zero/code/n`
- Cell (11, 0): `results/v86-main-table/summary.json#/main_rows/3/capabilities/qa/delivered`
- Cell (11, 1): `results/v86-main-table/summary.json#/main_rows/3/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/3/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/3/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/3/capabilities/qa/delivered`; `results/v74-quant-threeway/quant_threeway.json#/recommendation_rule`
- Cell (11, 2): `results/v86-main-table/summary.json#/main_rows/3/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/3/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/3/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/3/capabilities/qa/delivered`; `results/v74-quant-threeway/quant_threeway.json#/recommendation_rule`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/n`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/n`
- Cell (11, 3): `results/v69-quant-confirm/develop.json#/loso/scores`; `results/v69-quant-confirm/develop.json#/loso/scores/median/qa`
- Cell (11, 4): `results/v69-quant-confirm/develop.json#/loso/scores`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/n`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/n`
- Cell (11, 5): `results/v86-main-table/summary.json#/main_rows/3/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/3/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/3/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/3/capabilities/qa/delivered`; `results/v74-quant-threeway/quant_threeway.json#/recommendation_rule`; `results/v69-quant-confirm/develop.json#/loso/scores`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/n`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/n`
- Cell (12, 0): `results/v70-distill-confirm/freeze.json#/confirmation_register/unused_U_assertion`; `results/v70-distill-confirm/freeze.json#/frozen_at_utc`; `results/v47-p2-register/register.json#/v5_confirm/registered_at_utc`; `results/v70-distill-confirm/develop.json#/development_structure`; `results/v70-distill-confirm/develop.json#/points`; `results/v70-distill-confirm/freeze.json#/inputs_sha256/results~1v70-distill-confirm~1develop.json`; `results/v70-distill-confirm/freeze.json#/confirmation_register/students/0`; `results/v70-distill-confirm/freeze.json#/confirmation_register/pools`; `results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned`; `results/v70-distill-confirm/develop.json#/development_structure/n_points`
- Cell (13, 0): `results/v70-distill-confirm/freeze.json#/selected/math/method`
- Cell (13, 1): `results/v70-distill-confirm/freeze.json#/selected`; `results/v70-distill-confirm/freeze.json#/models`; `results/v70-distill-confirm/freeze.json#/selected/math/method`
- Cell (13, 2): `results/v86-main-table/summary.json#/main_rows/4/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/qa/delivered`; `results/v86-main-table/summary.json#/main_rows/5/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/qa/delivered`; `results/v70-distill-confirm/compare.json#/groups/0/candidate_mae`
- Cell (13, 3): `results/v70-distill-confirm/freeze.json#/baseline_rule`; `results/v70-distill-confirm/freeze.json#/strongest_baseline`; `results/v70-distill-confirm/freeze.json#/strongest_baseline/gemma3-270m/math/method`
- Cell (13, 4): `results/v70-distill-confirm/freeze.json#/baseline_rule`; `results/v70-distill-confirm/freeze.json#/strongest_baseline`; `results/v70-distill-confirm/compare.json#/groups/0/baseline_mae`
- Cell (13, 5): `results/v86-main-table/summary.json#/main_rows/4/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/qa/delivered`; `results/v86-main-table/summary.json#/main_rows/5/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/qa/delivered`; `results/v70-distill-confirm/freeze.json#/baseline_rule`; `results/v70-distill-confirm/freeze.json#/strongest_baseline`; `results/v70-distill-confirm/compare.json#/groups/0/candidate_mae`; `results/v70-distill-confirm/compare.json#/groups/0/baseline_mae`
- Cell (14, 0): `results/v70-distill-confirm/freeze.json#/selected/code/method`
- Cell (14, 1): `results/v70-distill-confirm/freeze.json#/selected`; `results/v70-distill-confirm/freeze.json#/models`; `results/v70-distill-confirm/freeze.json#/selected/code/method`
- Cell (14, 2): `results/v86-main-table/summary.json#/main_rows/4/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/qa/delivered`; `results/v86-main-table/summary.json#/main_rows/5/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/qa/delivered`; `results/v70-distill-confirm/compare.json#/groups/1/candidate_mae`
- Cell (14, 3): `results/v70-distill-confirm/freeze.json#/baseline_rule`; `results/v70-distill-confirm/freeze.json#/strongest_baseline`; `results/v70-distill-confirm/freeze.json#/strongest_baseline/gemma3-270m/code/method`
- Cell (14, 4): `results/v70-distill-confirm/freeze.json#/baseline_rule`; `results/v70-distill-confirm/freeze.json#/strongest_baseline`; `results/v70-distill-confirm/compare.json#/groups/1/baseline_mae`
- Cell (14, 5): `results/v86-main-table/summary.json#/main_rows/4/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/qa/delivered`; `results/v86-main-table/summary.json#/main_rows/5/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/qa/delivered`; `results/v70-distill-confirm/freeze.json#/baseline_rule`; `results/v70-distill-confirm/freeze.json#/strongest_baseline`; `results/v70-distill-confirm/compare.json#/groups/1/candidate_mae`; `results/v70-distill-confirm/compare.json#/groups/1/baseline_mae`
- Cell (15, 0): `results/v70-distill-confirm/freeze.json#/selected/qa/method`
- Cell (15, 1): `results/v70-distill-confirm/freeze.json#/selected`; `results/v70-distill-confirm/freeze.json#/models`; `results/v70-distill-confirm/freeze.json#/selected/qa/method`
- Cell (15, 2): `results/v86-main-table/summary.json#/main_rows/4/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/qa/delivered`; `results/v86-main-table/summary.json#/main_rows/5/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/qa/delivered`; `results/v70-distill-confirm/compare.json#/groups/2/candidate_mae`
- Cell (15, 3): `results/v70-distill-confirm/freeze.json#/baseline_rule`; `results/v70-distill-confirm/freeze.json#/strongest_baseline`; `results/v70-distill-confirm/freeze.json#/strongest_baseline/gemma3-270m/qa/method`
- Cell (15, 4): `results/v70-distill-confirm/freeze.json#/baseline_rule`; `results/v70-distill-confirm/freeze.json#/strongest_baseline`; `results/v70-distill-confirm/compare.json#/groups/2/baseline_mae`
- Cell (15, 5): `results/v86-main-table/summary.json#/main_rows/4/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/qa/delivered`; `results/v86-main-table/summary.json#/main_rows/5/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/qa/delivered`; `results/v70-distill-confirm/freeze.json#/baseline_rule`; `results/v70-distill-confirm/freeze.json#/strongest_baseline`; `results/v70-distill-confirm/compare.json#/groups/2/candidate_mae`; `results/v70-distill-confirm/compare.json#/groups/2/baseline_mae`
- Cell (16, 0): `results/v70-distill-confirm/freeze.json#/confirmation_register/unused_U_assertion`; `results/v70-distill-confirm/freeze.json#/frozen_at_utc`; `results/v47-p2-register/register.json#/v5_confirm/registered_at_utc`; `results/v70-distill-confirm/develop.json#/development_structure`; `results/v70-distill-confirm/develop.json#/points`; `results/v70-distill-confirm/freeze.json#/inputs_sha256/results~1v70-distill-confirm~1develop.json`; `results/v70-distill-confirm/freeze.json#/confirmation_register/students/1`; `results/v70-distill-confirm/freeze.json#/confirmation_register/pools`; `results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned`; `results/v70-distill-confirm/develop.json#/development_structure/n_points`
- Cell (17, 0): `results/v70-distill-confirm/freeze.json#/selected/math/method`
- Cell (17, 1): `results/v70-distill-confirm/freeze.json#/selected`; `results/v70-distill-confirm/freeze.json#/models`; `results/v70-distill-confirm/freeze.json#/selected/math/method`
- Cell (17, 2): `results/v86-main-table/summary.json#/main_rows/4/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/qa/delivered`; `results/v86-main-table/summary.json#/main_rows/5/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/qa/delivered`; `results/v70-distill-confirm/compare.json#/groups/3/candidate_mae`
- Cell (17, 3): `results/v70-distill-confirm/freeze.json#/baseline_rule`; `results/v70-distill-confirm/freeze.json#/strongest_baseline`; `results/v70-distill-confirm/freeze.json#/strongest_baseline/gemma3-1b/math/method`
- Cell (17, 4): `results/v70-distill-confirm/freeze.json#/baseline_rule`; `results/v70-distill-confirm/freeze.json#/strongest_baseline`; `results/v70-distill-confirm/compare.json#/groups/3/baseline_mae`
- Cell (17, 5): `results/v86-main-table/summary.json#/main_rows/4/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/qa/delivered`; `results/v86-main-table/summary.json#/main_rows/5/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/qa/delivered`; `results/v70-distill-confirm/freeze.json#/baseline_rule`; `results/v70-distill-confirm/freeze.json#/strongest_baseline`; `results/v70-distill-confirm/compare.json#/groups/3/candidate_mae`; `results/v70-distill-confirm/compare.json#/groups/3/baseline_mae`
- Cell (18, 0): `results/v70-distill-confirm/freeze.json#/selected/code/method`
- Cell (18, 1): `results/v70-distill-confirm/freeze.json#/selected`; `results/v70-distill-confirm/freeze.json#/models`; `results/v70-distill-confirm/freeze.json#/selected/code/method`
- Cell (18, 2): `results/v86-main-table/summary.json#/main_rows/4/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/qa/delivered`; `results/v86-main-table/summary.json#/main_rows/5/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/qa/delivered`; `results/v70-distill-confirm/compare.json#/groups/4/candidate_mae`
- Cell (18, 3): `results/v70-distill-confirm/freeze.json#/baseline_rule`; `results/v70-distill-confirm/freeze.json#/strongest_baseline`; `results/v70-distill-confirm/freeze.json#/strongest_baseline/gemma3-1b/code/method`
- Cell (18, 4): `results/v70-distill-confirm/freeze.json#/baseline_rule`; `results/v70-distill-confirm/freeze.json#/strongest_baseline`; `results/v70-distill-confirm/compare.json#/groups/4/baseline_mae`
- Cell (18, 5): `results/v86-main-table/summary.json#/main_rows/4/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/qa/delivered`; `results/v86-main-table/summary.json#/main_rows/5/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/qa/delivered`; `results/v70-distill-confirm/freeze.json#/baseline_rule`; `results/v70-distill-confirm/freeze.json#/strongest_baseline`; `results/v70-distill-confirm/compare.json#/groups/4/candidate_mae`; `results/v70-distill-confirm/compare.json#/groups/4/baseline_mae`
- Cell (19, 0): `results/v70-distill-confirm/freeze.json#/selected/qa/method`
- Cell (19, 1): `results/v70-distill-confirm/freeze.json#/selected`; `results/v70-distill-confirm/freeze.json#/models`; `results/v70-distill-confirm/freeze.json#/selected/qa/method`
- Cell (19, 2): `results/v86-main-table/summary.json#/main_rows/4/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/qa/delivered`; `results/v86-main-table/summary.json#/main_rows/5/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/qa/delivered`; `results/v70-distill-confirm/compare.json#/groups/5/candidate_mae`
- Cell (19, 3): `results/v70-distill-confirm/freeze.json#/baseline_rule`; `results/v70-distill-confirm/freeze.json#/strongest_baseline`; `results/v70-distill-confirm/freeze.json#/strongest_baseline/gemma3-1b/qa/method`
- Cell (19, 4): `results/v70-distill-confirm/freeze.json#/baseline_rule`; `results/v70-distill-confirm/freeze.json#/strongest_baseline`; `results/v70-distill-confirm/compare.json#/groups/5/baseline_mae`
- Cell (19, 5): `results/v86-main-table/summary.json#/main_rows/4/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/4/capabilities/qa/delivered`; `results/v86-main-table/summary.json#/main_rows/5/delivered_timing`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/math/delivered`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/code/delivered`; `results/v86-main-table/summary.json#/main_rows/5/capabilities/qa/delivered`; `results/v70-distill-confirm/freeze.json#/baseline_rule`; `results/v70-distill-confirm/freeze.json#/strongest_baseline`; `results/v70-distill-confirm/compare.json#/groups/5/candidate_mae`; `results/v70-distill-confirm/compare.json#/groups/5/baseline_mae`

## Machine-readable cell recipes

```json
[
  {
    "table": "tab:main-prediction-v2",
    "row": 0,
    "column": 0,
    "parts": [
      {
        "sources": [
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/tag",
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/densities",
          "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/tag",
          "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/densities",
          "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/tag",
          "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/densities"
        ],
        "op": "label",
        "format": null,
        "label": "Three unseen checkpoints pruned to densities 0.575, 0.675 and 0.85",
        "expected": [
          "pythia-410m@step48000",
          [
            0.85,
            0.675,
            0.575
          ],
          "pythia-1.4b@step112000",
          [
            0.85,
            0.675,
            0.575
          ],
          "pythia-6.9b@step80000",
          [
            0.85,
            0.675,
            0.575
          ]
        ]
      },
      "; ",
      {
        "sources": [
          "results/v53-prune-dev/register.json#/n_dev_rows",
          "results/v53-prune-dev/register.json#/models"
        ],
        "op": "per_capability",
        "format": null
      },
      " measurements",
      "; ",
      {
        "sources": [
          "results/v86-main-table/summary.json#/main_rows/0/delivered_timing"
        ],
        "op": "label",
        "format": null,
        "label": "Retrospective",
        "expected": [
          "fixed after test; reused frozen in Sec. 5"
        ]
      }
    ],
    "context": [
      "results/v53-prune-dev/register.json#/selected_candidate",
      "results/v53-prune-dev/register.json#/dev_states",
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/densities",
      "results/v53-prune-dev/register.json#/dev_states"
    ],
    "note": "All three test checkpoints are absent from every development fit. The 6.9B size occurs at other stages in the expanded register. 252 recorded scalar rows / three capability models = 84 state-density configurations per capability; cross-checked against dev_states[*].densities. This is the V53 17-state fit, not A9/A11's 36-cell panel. Dense anchors excluded.",
    "compact_scores": "",
    "rendered": "\\multicolumn{6}{@{}>{\\raggedright\\arraybackslash}p{\\dimexpr\\textwidth-0pt\\relax}@{}}{\\textit{Three unseen checkpoints pruned to densities 0.575, 0.675 and 0.85; 84 measurements; Retrospective}}",
    "column_span": 6
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 1,
    "column": 0,
    "parts": [
      "Mathematics"
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/0/capabilities/math/delivered"
    ],
    "note": "",
    "compact_scores": "",
    "rendered": "Mathematics"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 1,
    "column": 1,
    "parts": [
      {
        "sources": [
          "results/v86-main-table/summary.json#/main_rows/0/capabilities/math/delivered"
        ],
        "op": "label",
        "format": null,
        "label": "Source-free median density curve",
        "expected": [
          "median_curve"
        ]
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/0/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/0/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/0/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/0/capabilities/qa/delivered"
    ],
    "note": "New-state source-free median curve, fixed after test; scores use the same three checkpoints and densities as the frozen candidate.",
    "compact_scores": "",
    "rendered": "Source-free median density curve"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 1,
    "column": 2,
    "parts": [
      {
        "sources": [
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/math",
          "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/math",
          "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/math"
        ],
        "op": "mean",
        "format": ".3f"
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/0/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/0/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/0/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/0/capabilities/qa/delivered"
    ],
    "note": "New-state source-free median curve, fixed after test; scores use the same three checkpoints and densities as the frozen candidate.",
    "compact_scores": "",
    "rendered": "0.277"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 1,
    "column": 3,
    "parts": [
      {
        "sources": [
          "results/v53-prune-dev/register.json#/loso_table/2/candidate"
        ],
        "op": "label",
        "format": null,
        "label": "Per-density regression",
        "expected": [
          "A2"
        ]
      }
    ],
    "context": [
      "results/v53-prune-dev/register.json#/loso_table"
    ],
    "note": "Minimum development LOSO MAE excluding power, per capability: per-density regression / per-density regression / development median; no test ranking.",
    "compact_scores": "",
    "rendered": "Per-density regression"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 1,
    "column": 4,
    "parts": [
      {
        "sources": [
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/A2/math",
          "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/A2/math",
          "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/A2/math"
        ],
        "op": "mean",
        "format": ".3f"
      }
    ],
    "context": [
      "results/v53-prune-dev/register.json#/loso_table"
    ],
    "note": "Minimum development LOSO MAE excluding power, per capability: per-density regression / per-density regression / development median; no test ranking.",
    "compact_scores": "",
    "rendered": "0.230"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 1,
    "column": 5,
    "parts": [
      {
        "sources": [
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/math",
          "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/math",
          "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/math",
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/A2/math",
          "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/A2/math",
          "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/A2/math"
        ],
        "op": "difference",
        "parts": [
          {
            "sources": [
              "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/A2/math",
              "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/A2/math",
              "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/A2/math"
            ],
            "op": "mean",
            "format": ".3f"
          },
          {
            "sources": [
              "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/math",
              "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/math",
              "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/math"
            ],
            "op": "mean",
            "format": ".3f"
          }
        ],
        "format": "+.3f"
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/0/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/0/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/0/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/0/capabilities/qa/delivered",
      "results/v53-prune-dev/register.json#/loso_table"
    ],
    "note": "baseline error minus delivered error, per capability",
    "compact_scores": "",
    "rendered": "$-$0.047"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 2,
    "column": 0,
    "parts": [
      "Code"
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/0/capabilities/code/delivered"
    ],
    "note": "",
    "compact_scores": "",
    "rendered": "Code"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 2,
    "column": 1,
    "parts": [
      {
        "sources": [
          "results/v86-main-table/summary.json#/main_rows/0/capabilities/code/delivered"
        ],
        "op": "label",
        "format": null,
        "label": "Source-free median density curve",
        "expected": [
          "median_curve"
        ]
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/0/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/0/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/0/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/0/capabilities/qa/delivered"
    ],
    "note": "New-state source-free median curve, fixed after test; scores use the same three checkpoints and densities as the frozen candidate.",
    "compact_scores": "",
    "rendered": "Source-free median density curve"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 2,
    "column": 2,
    "parts": [
      {
        "sources": [
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/code",
          "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/code",
          "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/code"
        ],
        "op": "mean",
        "format": ".3f"
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/0/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/0/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/0/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/0/capabilities/qa/delivered"
    ],
    "note": "New-state source-free median curve, fixed after test; scores use the same three checkpoints and densities as the frozen candidate.",
    "compact_scores": "",
    "rendered": "0.214"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 2,
    "column": 3,
    "parts": [
      {
        "sources": [
          "results/v53-prune-dev/register.json#/loso_table/2/candidate"
        ],
        "op": "label",
        "format": null,
        "label": "Per-density regression",
        "expected": [
          "A2"
        ]
      }
    ],
    "context": [
      "results/v53-prune-dev/register.json#/loso_table"
    ],
    "note": "Minimum development LOSO MAE excluding power, per capability: per-density regression / per-density regression / development median; no test ranking.",
    "compact_scores": "",
    "rendered": "Per-density regression"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 2,
    "column": 4,
    "parts": [
      {
        "sources": [
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/A2/code",
          "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/A2/code",
          "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/A2/code"
        ],
        "op": "mean",
        "format": ".3f"
      }
    ],
    "context": [
      "results/v53-prune-dev/register.json#/loso_table"
    ],
    "note": "Minimum development LOSO MAE excluding power, per capability: per-density regression / per-density regression / development median; no test ranking.",
    "compact_scores": "",
    "rendered": "0.222"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 2,
    "column": 5,
    "parts": [
      {
        "sources": [
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/code",
          "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/code",
          "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/code",
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/A2/code",
          "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/A2/code",
          "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/A2/code"
        ],
        "op": "difference",
        "parts": [
          {
            "sources": [
              "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/A2/code",
              "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/A2/code",
              "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/A2/code"
            ],
            "op": "mean",
            "format": ".3f"
          },
          {
            "sources": [
              "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/code",
              "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/code",
              "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/code"
            ],
            "op": "mean",
            "format": ".3f"
          }
        ],
        "format": "+.3f"
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/0/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/0/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/0/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/0/capabilities/qa/delivered",
      "results/v53-prune-dev/register.json#/loso_table"
    ],
    "note": "baseline error minus delivered error, per capability",
    "compact_scores": "",
    "rendered": "$+$0.008"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 3,
    "column": 0,
    "parts": [
      "Question answering"
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/0/capabilities/qa/delivered"
    ],
    "note": "",
    "compact_scores": "",
    "rendered": "Question answering"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 3,
    "column": 1,
    "parts": [
      {
        "sources": [
          "results/v86-main-table/summary.json#/main_rows/0/capabilities/qa/delivered"
        ],
        "op": "label",
        "format": null,
        "label": "Source-free median density curve",
        "expected": [
          "median_curve"
        ]
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/0/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/0/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/0/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/0/capabilities/qa/delivered"
    ],
    "note": "New-state source-free median curve, fixed after test; scores use the same three checkpoints and densities as the frozen candidate.",
    "compact_scores": "",
    "rendered": "Source-free median density curve"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 3,
    "column": 2,
    "parts": [
      {
        "sources": [
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/qa",
          "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/qa",
          "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/qa"
        ],
        "op": "mean",
        "format": ".3f"
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/0/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/0/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/0/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/0/capabilities/qa/delivered"
    ],
    "note": "New-state source-free median curve, fixed after test; scores use the same three checkpoints and densities as the frozen candidate.",
    "compact_scores": "",
    "rendered": "0.221"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 3,
    "column": 3,
    "parts": [
      {
        "sources": [
          "results/v53-prune-dev/register.json#/loso_table/5/candidate"
        ],
        "op": "label",
        "format": null,
        "label": "Development median",
        "expected": [
          "median_curve"
        ]
      }
    ],
    "context": [
      "results/v53-prune-dev/register.json#/loso_table"
    ],
    "note": "Minimum development LOSO MAE excluding power, per capability: per-density regression / per-density regression / development median; no test ranking.",
    "compact_scores": "",
    "rendered": "Development median"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 3,
    "column": 4,
    "parts": [
      {
        "sources": [
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/qa",
          "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/qa",
          "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/qa"
        ],
        "op": "mean",
        "format": ".3f"
      }
    ],
    "context": [
      "results/v53-prune-dev/register.json#/loso_table"
    ],
    "note": "Minimum development LOSO MAE excluding power, per capability: per-density regression / per-density regression / development median; no test ranking.",
    "compact_scores": "",
    "rendered": "0.221"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 3,
    "column": 5,
    "parts": [
      {
        "sources": [
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/qa",
          "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/qa",
          "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/qa",
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/qa",
          "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/qa",
          "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/qa"
        ],
        "op": "difference",
        "parts": [
          {
            "sources": [
              "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/qa",
              "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/qa",
              "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/qa"
            ],
            "op": "mean",
            "format": ".3f"
          },
          {
            "sources": [
              "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/qa",
              "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/qa",
              "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/qa"
            ],
            "op": "mean",
            "format": ".3f"
          }
        ],
        "format": "+.3f"
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/0/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/0/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/0/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/0/capabilities/qa/delivered",
      "results/v53-prune-dev/register.json#/loso_table"
    ],
    "note": "baseline error minus delivered error, per capability",
    "compact_scores": "",
    "rendered": "$+$0.000"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 4,
    "column": 0,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/rows/0/state",
          "results/v69-quant-confirm/compare.json#/rows/0/config",
          "results/v69-quant-confirm/compare.json#/rows/3/config",
          "results/v69-quant-confirm/compare.json#/rows/6/config",
          "results/v69-quant-confirm/compare.json#/rows/9/config",
          "results/v69-quant-confirm/compare.json#/rows/12/config",
          "results/v69-quant-confirm/compare.json#/rows/15/config",
          "results/v69-quant-confirm/compare.json#/rows/18/state"
        ],
        "op": "label",
        "format": null,
        "label": "Pythia 410 million and 1.4 billion at unseen group sizes 32 and 512, bit widths 3 to 5",
        "expected": [
          "pythia-410m@step143000",
          "b3_g32",
          "b3_g512",
          "b4_g32",
          "b4_g512",
          "b5_g32",
          "b5_g512",
          "pythia-1.4b@step16000"
        ]
      },
      "; ",
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/n_dev_cells"
        ],
        "op": "identity",
        "format": null
      },
      " measurements",
      "; ",
      {
        "sources": [
          "results/v86-main-table/summary.json#/main_rows/2/delivered_timing"
        ],
        "op": "label",
        "format": null,
        "label": "Retrospective",
        "expected": [
          "fixed after test"
        ]
      }
    ],
    "context": [
      "results/v69-quant-confirm/freeze.json#/frozen_at_utc",
      "results/v69-quant-confirm/compare.json#/rows/0/test_set",
      "results/v69-quant-confirm/compare.json#/rows/1/test_set",
      "results/v69-quant-confirm/compare.json#/rows/2/test_set",
      "results/v69-quant-confirm/compare.json#/rows/3/test_set",
      "results/v69-quant-confirm/compare.json#/rows/4/test_set",
      "results/v69-quant-confirm/compare.json#/rows/5/test_set",
      "results/v69-quant-confirm/compare.json#/rows/6/test_set",
      "results/v69-quant-confirm/compare.json#/rows/7/test_set",
      "results/v69-quant-confirm/compare.json#/rows/8/test_set",
      "results/v69-quant-confirm/compare.json#/rows/9/test_set",
      "results/v69-quant-confirm/compare.json#/rows/10/test_set",
      "results/v69-quant-confirm/compare.json#/rows/11/test_set",
      "results/v69-quant-confirm/compare.json#/rows/12/test_set",
      "results/v69-quant-confirm/compare.json#/rows/13/test_set",
      "results/v69-quant-confirm/compare.json#/rows/14/test_set",
      "results/v69-quant-confirm/compare.json#/rows/15/test_set",
      "results/v69-quant-confirm/compare.json#/rows/16/test_set",
      "results/v69-quant-confirm/compare.json#/rows/17/test_set",
      "results/v69-quant-confirm/compare.json#/rows/18/test_set",
      "results/v69-quant-confirm/compare.json#/rows/19/test_set",
      "results/v69-quant-confirm/compare.json#/rows/20/test_set",
      "results/v69-quant-confirm/compare.json#/rows/21/test_set",
      "results/v69-quant-confirm/compare.json#/rows/22/test_set",
      "results/v69-quant-confirm/compare.json#/rows/23/test_set",
      "results/v69-quant-confirm/compare.json#/rows/24/test_set",
      "results/v69-quant-confirm/compare.json#/rows/25/test_set",
      "results/v69-quant-confirm/compare.json#/rows/26/test_set",
      "results/v69-quant-confirm/compare.json#/rows/27/test_set",
      "results/v69-quant-confirm/compare.json#/rows/28/test_set",
      "results/v69-quant-confirm/compare.json#/rows/29/test_set",
      "results/v69-quant-confirm/compare.json#/rows/30/test_set",
      "results/v69-quant-confirm/compare.json#/rows/31/test_set",
      "results/v69-quant-confirm/compare.json#/rows/32/test_set",
      "results/v69-quant-confirm/compare.json#/rows/33/test_set",
      "results/v69-quant-confirm/compare.json#/rows/34/test_set",
      "results/v69-quant-confirm/compare.json#/rows/35/test_set",
      "results/v69-quant-confirm/develop.json#/dev_states",
      "results/v69-quant-confirm/develop.json#/dev_configs",
      "results/v69-quant-confirm/develop.json#/selection_rule"
    ],
    "note": " Recorded configuration count; six states times nine configurations per capability. Includes development selection of QA's zero rule, which fits no coefficients. The same development panel supports both tests; counts are not additive.",
    "compact_scores": "",
    "rendered": "\\multicolumn{6}{@{}>{\\raggedright\\arraybackslash}p{\\dimexpr\\textwidth-0pt\\relax}@{}}{\\textit{Pythia 410 million and 1.4 billion at unseen group sizes 32 and 512, bit widths 3 to 5; 54 measurements; Retrospective}}",
    "column_span": 6
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 5,
    "column": 0,
    "parts": [
      "Mathematics"
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/2/capabilities/math/delivered"
    ],
    "note": "",
    "compact_scores": "",
    "rendered": "Mathematics"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 5,
    "column": 1,
    "parts": [
      {
        "sources": [
          "results/v86-main-table/summary.json#/main_rows/2/capabilities/math/delivered"
        ],
        "op": "label",
        "format": null,
        "label": "Interpolation",
        "expected": [
          "same_input_interpolation"
        ]
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/2/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/2/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/2/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/2/capabilities/qa/delivered",
      "results/v74-quant-threeway/quant_threeway.json#/recommendation_rule"
    ],
    "note": "Post-test rule on the identical frozen cells, never a test-error minimum. New-state errors pool boundary and interior cells equally per cell.",
    "compact_scores": "",
    "rendered": "Interpolation"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 5,
    "column": 2,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/same_input_interpolation/math/mae"
        ],
        "op": "identity",
        "format": ".3f"
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/2/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/2/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/2/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/2/capabilities/qa/delivered",
      "results/v74-quant-threeway/quant_threeway.json#/recommendation_rule"
    ],
    "note": "Post-test rule on the identical frozen cells, never a test-error minimum. New-state errors pool boundary and interior cells equally per cell.",
    "compact_scores": "",
    "rendered": "0.065"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 5,
    "column": 3,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/loso/scores/bilinear/math"
        ],
        "op": "label",
        "format": null,
        "label": "Bilinear regression",
        "expected": [
          {
            "n": 54,
            "n_states": 6,
            "state_mae": {
              "pythia-1.4b@step143000": 0.18035555432620828,
              "pythia-1.4b@step16000": 0.4042579843558109,
              "pythia-160m@step143000": 3.3985412467109986,
              "pythia-160m@step16000": 0.43688672544116214,
              "pythia-410m@step143000": 0.37784637907436774,
              "pythia-410m@step16000": 0.2598977837534169
            },
            "macro_mae": 0.8429642789436608,
            "mae": 0.8429642789436608
          }
        ]
      }
    ],
    "context": [
      "results/v69-quant-confirm/develop.json#/loso/scores"
    ],
    "note": "Minimum development LOSO macro MAE excluding the selected candidate, per capability: bilinear regression / no change / development median.",
    "compact_scores": "",
    "rendered": "Bilinear regression"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 5,
    "column": 4,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/bilinear/math/mae"
        ],
        "op": "identity",
        "format": ".3f"
      }
    ],
    "context": [
      "results/v69-quant-confirm/develop.json#/loso/scores"
    ],
    "note": "Minimum development LOSO macro MAE excluding the selected candidate, per capability: bilinear regression / no change / development median.",
    "compact_scores": "",
    "rendered": "0.333"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 5,
    "column": 5,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/same_input_interpolation/math/mae",
          "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/bilinear/math/mae"
        ],
        "op": "difference",
        "parts": [
          {
            "sources": [
              "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/bilinear/math/mae"
            ],
            "op": "identity",
            "format": ".3f"
          },
          {
            "sources": [
              "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/same_input_interpolation/math/mae"
            ],
            "op": "identity",
            "format": ".3f"
          }
        ],
        "format": "+.3f"
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/2/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/2/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/2/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/2/capabilities/qa/delivered",
      "results/v74-quant-threeway/quant_threeway.json#/recommendation_rule",
      "results/v69-quant-confirm/develop.json#/loso/scores"
    ],
    "note": "baseline error minus delivered error, per capability",
    "compact_scores": "",
    "rendered": "$+$0.268"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 6,
    "column": 0,
    "parts": [
      "Code"
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/2/capabilities/code/delivered"
    ],
    "note": "",
    "compact_scores": "",
    "rendered": "Code"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 6,
    "column": 1,
    "parts": [
      {
        "sources": [
          "results/v86-main-table/summary.json#/main_rows/2/capabilities/code/delivered"
        ],
        "op": "label",
        "format": null,
        "label": "Interpolation",
        "expected": [
          "same_input_interpolation"
        ]
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/2/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/2/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/2/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/2/capabilities/qa/delivered",
      "results/v74-quant-threeway/quant_threeway.json#/recommendation_rule"
    ],
    "note": "Post-test rule on the identical frozen cells, never a test-error minimum. New-state errors pool boundary and interior cells equally per cell.",
    "compact_scores": "",
    "rendered": "Interpolation"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 6,
    "column": 2,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/same_input_interpolation/code/mae"
        ],
        "op": "identity",
        "format": ".3f"
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/2/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/2/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/2/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/2/capabilities/qa/delivered",
      "results/v74-quant-threeway/quant_threeway.json#/recommendation_rule"
    ],
    "note": "Post-test rule on the identical frozen cells, never a test-error minimum. New-state errors pool boundary and interior cells equally per cell.",
    "compact_scores": "",
    "rendered": "0.116"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 6,
    "column": 3,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/loso/scores/zero/code"
        ],
        "op": "label",
        "format": null,
        "label": "No change",
        "expected": [
          {
            "n": 54,
            "n_states": 6,
            "state_mae": {
              "pythia-1.4b@step143000": 0.5143543829067956,
              "pythia-1.4b@step16000": 0.10937458732799844,
              "pythia-160m@step143000": 6.2735256054723605,
              "pythia-160m@step16000": 0.3426432136914666,
              "pythia-410m@step143000": 1.110008451522595,
              "pythia-410m@step16000": 0.19481419855795895
            },
            "macro_mae": 1.4241200732465291,
            "mae": 1.4241200732465291
          }
        ]
      }
    ],
    "context": [
      "results/v69-quant-confirm/develop.json#/loso/scores"
    ],
    "note": "Minimum development LOSO macro MAE excluding the selected candidate, per capability: bilinear regression / no change / development median.",
    "compact_scores": "",
    "rendered": "No change"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 6,
    "column": 4,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/zero/code/mae"
        ],
        "op": "identity",
        "format": ".3f"
      }
    ],
    "context": [
      "results/v69-quant-confirm/develop.json#/loso/scores"
    ],
    "note": "Minimum development LOSO macro MAE excluding the selected candidate, per capability: bilinear regression / no change / development median.",
    "compact_scores": "",
    "rendered": "0.678"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 6,
    "column": 5,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/same_input_interpolation/code/mae",
          "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/zero/code/mae"
        ],
        "op": "difference",
        "parts": [
          {
            "sources": [
              "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/zero/code/mae"
            ],
            "op": "identity",
            "format": ".3f"
          },
          {
            "sources": [
              "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/same_input_interpolation/code/mae"
            ],
            "op": "identity",
            "format": ".3f"
          }
        ],
        "format": "+.3f"
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/2/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/2/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/2/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/2/capabilities/qa/delivered",
      "results/v74-quant-threeway/quant_threeway.json#/recommendation_rule",
      "results/v69-quant-confirm/develop.json#/loso/scores"
    ],
    "note": "baseline error minus delivered error, per capability",
    "compact_scores": "",
    "rendered": "$+$0.562"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 7,
    "column": 0,
    "parts": [
      "Question answering"
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/2/capabilities/qa/delivered"
    ],
    "note": "",
    "compact_scores": "",
    "rendered": "Question answering"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 7,
    "column": 1,
    "parts": [
      {
        "sources": [
          "results/v86-main-table/summary.json#/main_rows/2/capabilities/qa/delivered"
        ],
        "op": "label",
        "format": null,
        "label": "Development median",
        "expected": [
          "median"
        ]
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/2/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/2/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/2/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/2/capabilities/qa/delivered",
      "results/v74-quant-threeway/quant_threeway.json#/recommendation_rule"
    ],
    "note": "Post-test rule on the identical frozen cells, never a test-error minimum. New-state errors pool boundary and interior cells equally per cell.",
    "compact_scores": "",
    "rendered": "Development median"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 7,
    "column": 2,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/median/qa/mae"
        ],
        "op": "identity",
        "format": ".3f"
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/2/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/2/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/2/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/2/capabilities/qa/delivered",
      "results/v74-quant-threeway/quant_threeway.json#/recommendation_rule"
    ],
    "note": "Post-test rule on the identical frozen cells, never a test-error minimum. New-state errors pool boundary and interior cells equally per cell.",
    "compact_scores": "",
    "rendered": "0.458"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 7,
    "column": 3,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/loso/scores/median/qa"
        ],
        "op": "label",
        "format": null,
        "label": "Development median",
        "expected": [
          {
            "n": 54,
            "n_states": 6,
            "state_mae": {
              "pythia-1.4b@step143000": 0.16258053443177,
              "pythia-1.4b@step16000": 0.2355005016899031,
              "pythia-160m@step143000": 6.541049456062526,
              "pythia-160m@step16000": 0.09769750739332464,
              "pythia-410m@step143000": 0.7294274133924797,
              "pythia-410m@step16000": 0.15231569497253902
            },
            "macro_mae": 1.319761851323757,
            "mae": 1.3197618513237568
          }
        ]
      }
    ],
    "context": [
      "results/v69-quant-confirm/develop.json#/loso/scores"
    ],
    "note": "Minimum development LOSO macro MAE excluding the selected candidate, per capability: bilinear regression / no change / development median.",
    "compact_scores": "",
    "rendered": "Development median"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 7,
    "column": 4,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/median/qa/mae"
        ],
        "op": "identity",
        "format": ".3f"
      }
    ],
    "context": [
      "results/v69-quant-confirm/develop.json#/loso/scores"
    ],
    "note": "Minimum development LOSO macro MAE excluding the selected candidate, per capability: bilinear regression / no change / development median.",
    "compact_scores": "",
    "rendered": "0.458"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 7,
    "column": 5,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/median/qa/mae",
          "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/median/qa/mae"
        ],
        "op": "difference",
        "parts": [
          {
            "sources": [
              "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/median/qa/mae"
            ],
            "op": "identity",
            "format": ".3f"
          },
          {
            "sources": [
              "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/median/qa/mae"
            ],
            "op": "identity",
            "format": ".3f"
          }
        ],
        "format": "+.3f"
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/2/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/2/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/2/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/2/capabilities/qa/delivered",
      "results/v74-quant-threeway/quant_threeway.json#/recommendation_rule",
      "results/v69-quant-confirm/develop.json#/loso/scores"
    ],
    "note": "baseline error minus delivered error, per capability",
    "compact_scores": "",
    "rendered": "$+$0.000"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 8,
    "column": 0,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/rows/36/state",
          "results/v69-quant-confirm/compare.json#/rows/36/config",
          "results/v69-quant-confirm/compare.json#/rows/39/config",
          "results/v69-quant-confirm/compare.json#/rows/42/config",
          "results/v69-quant-confirm/compare.json#/rows/45/config",
          "results/v69-quant-confirm/compare.json#/rows/48/config",
          "results/v69-quant-confirm/compare.json#/rows/51/config",
          "results/v69-quant-confirm/compare.json#/rows/54/config",
          "results/v69-quant-confirm/compare.json#/rows/57/config",
          "results/v69-quant-confirm/compare.json#/rows/60/config"
        ],
        "op": "label",
        "format": null,
        "label": "An unseen 1.4 billion stage at bit widths 3 to 5, group sizes 32 to 512",
        "expected": [
          "pythia-1.4b@step112000",
          "b3_g32",
          "b3_g512",
          "b4_g32",
          "b4_g512",
          "b5_g32",
          "b5_g512",
          "b3_g128",
          "b4_g128",
          "b5_g128"
        ]
      },
      "; ",
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/n_dev_cells"
        ],
        "op": "identity",
        "format": null
      },
      " measurements",
      "; ",
      {
        "sources": [
          "results/v86-main-table/summary.json#/main_rows/3/delivered_timing"
        ],
        "op": "label",
        "format": null,
        "label": "Retrospective",
        "expected": [
          "fixed after test"
        ]
      }
    ],
    "context": [
      "results/v69-quant-confirm/freeze.json#/frozen_at_utc",
      "results/v69-quant-confirm/compare.json#/rows/36/test_set",
      "results/v69-quant-confirm/compare.json#/rows/37/test_set",
      "results/v69-quant-confirm/compare.json#/rows/38/test_set",
      "results/v69-quant-confirm/compare.json#/rows/39/test_set",
      "results/v69-quant-confirm/compare.json#/rows/40/test_set",
      "results/v69-quant-confirm/compare.json#/rows/41/test_set",
      "results/v69-quant-confirm/compare.json#/rows/42/test_set",
      "results/v69-quant-confirm/compare.json#/rows/43/test_set",
      "results/v69-quant-confirm/compare.json#/rows/44/test_set",
      "results/v69-quant-confirm/compare.json#/rows/45/test_set",
      "results/v69-quant-confirm/compare.json#/rows/46/test_set",
      "results/v69-quant-confirm/compare.json#/rows/47/test_set",
      "results/v69-quant-confirm/compare.json#/rows/48/test_set",
      "results/v69-quant-confirm/compare.json#/rows/49/test_set",
      "results/v69-quant-confirm/compare.json#/rows/50/test_set",
      "results/v69-quant-confirm/compare.json#/rows/51/test_set",
      "results/v69-quant-confirm/compare.json#/rows/52/test_set",
      "results/v69-quant-confirm/compare.json#/rows/53/test_set",
      "results/v69-quant-confirm/compare.json#/rows/54/test_set",
      "results/v69-quant-confirm/compare.json#/rows/55/test_set",
      "results/v69-quant-confirm/compare.json#/rows/56/test_set",
      "results/v69-quant-confirm/compare.json#/rows/57/test_set",
      "results/v69-quant-confirm/compare.json#/rows/58/test_set",
      "results/v69-quant-confirm/compare.json#/rows/59/test_set",
      "results/v69-quant-confirm/compare.json#/rows/60/test_set",
      "results/v69-quant-confirm/compare.json#/rows/61/test_set",
      "results/v69-quant-confirm/compare.json#/rows/62/test_set",
      "results/v69-quant-confirm/develop.json#/dev_states",
      "results/v69-quant-confirm/develop.json#/dev_configs",
      "results/v69-quant-confirm/develop.json#/selection_rule"
    ],
    "note": " Recorded configuration count; six states times nine configurations per capability. Includes development selection of QA's zero rule, which fits no coefficients. The same development panel supports both tests; counts are not additive.",
    "compact_scores": "",
    "rendered": "\\multicolumn{6}{@{}>{\\raggedright\\arraybackslash}p{\\dimexpr\\textwidth-0pt\\relax}@{}}{\\textit{An unseen 1.4 billion stage at bit widths 3 to 5, group sizes 32 to 512; 54 measurements; Retrospective}}",
    "column_span": 6
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 9,
    "column": 0,
    "parts": [
      "Mathematics"
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/3/capabilities/math/delivered"
    ],
    "note": "",
    "compact_scores": "",
    "rendered": "Mathematics"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 9,
    "column": 1,
    "parts": [
      {
        "sources": [
          "results/v86-main-table/summary.json#/main_rows/3/capabilities/math/delivered"
        ],
        "op": "label",
        "format": null,
        "label": "Development median",
        "expected": [
          "median"
        ]
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/3/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/3/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/3/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/3/capabilities/qa/delivered",
      "results/v74-quant-threeway/quant_threeway.json#/recommendation_rule"
    ],
    "note": "Post-test rule on the identical frozen cells, never a test-error minimum. New-state errors pool boundary and interior cells equally per cell.",
    "compact_scores": "",
    "rendered": "Development median"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 9,
    "column": 2,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/math/mae",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/math/n",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/math/mae",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/math/n"
        ],
        "op": "weighted_mean",
        "format": ".3f"
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/3/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/3/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/3/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/3/capabilities/qa/delivered",
      "results/v74-quant-threeway/quant_threeway.json#/recommendation_rule"
    ],
    "note": "Post-test rule on the identical frozen cells, never a test-error minimum. New-state errors pool boundary and interior cells equally per cell.",
    "compact_scores": "",
    "rendered": "0.088"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 9,
    "column": 3,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/loso/scores/bilinear/math"
        ],
        "op": "label",
        "format": null,
        "label": "Bilinear regression",
        "expected": [
          {
            "n": 54,
            "n_states": 6,
            "state_mae": {
              "pythia-1.4b@step143000": 0.18035555432620828,
              "pythia-1.4b@step16000": 0.4042579843558109,
              "pythia-160m@step143000": 3.3985412467109986,
              "pythia-160m@step16000": 0.43688672544116214,
              "pythia-410m@step143000": 0.37784637907436774,
              "pythia-410m@step16000": 0.2598977837534169
            },
            "macro_mae": 0.8429642789436608,
            "mae": 0.8429642789436608
          }
        ]
      }
    ],
    "context": [
      "results/v69-quant-confirm/develop.json#/loso/scores"
    ],
    "note": "Minimum development LOSO macro MAE excluding the selected candidate, per capability: bilinear regression / no change / development median.",
    "compact_scores": "",
    "rendered": "Bilinear regression"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 9,
    "column": 4,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/bilinear/math/mae",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/bilinear/math/n",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/bilinear/math/mae",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/bilinear/math/n"
        ],
        "op": "weighted_mean",
        "format": ".3f"
      }
    ],
    "context": [
      "results/v69-quant-confirm/develop.json#/loso/scores"
    ],
    "note": "Minimum development LOSO macro MAE excluding the selected candidate, per capability: bilinear regression / no change / development median.",
    "compact_scores": "",
    "rendered": "0.350"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 9,
    "column": 5,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/math/mae",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/math/n",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/math/mae",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/math/n",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/bilinear/math/mae",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/bilinear/math/n",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/bilinear/math/mae",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/bilinear/math/n"
        ],
        "op": "difference",
        "parts": [
          {
            "sources": [
              "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/bilinear/math/mae",
              "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/bilinear/math/n",
              "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/bilinear/math/mae",
              "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/bilinear/math/n"
            ],
            "op": "weighted_mean",
            "format": ".3f"
          },
          {
            "sources": [
              "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/math/mae",
              "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/math/n",
              "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/math/mae",
              "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/math/n"
            ],
            "op": "weighted_mean",
            "format": ".3f"
          }
        ],
        "format": "+.3f"
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/3/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/3/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/3/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/3/capabilities/qa/delivered",
      "results/v74-quant-threeway/quant_threeway.json#/recommendation_rule",
      "results/v69-quant-confirm/develop.json#/loso/scores"
    ],
    "note": "baseline error minus delivered error, per capability",
    "compact_scores": "",
    "rendered": "$+$0.262"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 10,
    "column": 0,
    "parts": [
      "Code"
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/3/capabilities/code/delivered"
    ],
    "note": "",
    "compact_scores": "",
    "rendered": "Code"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 10,
    "column": 1,
    "parts": [
      {
        "sources": [
          "results/v86-main-table/summary.json#/main_rows/3/capabilities/code/delivered"
        ],
        "op": "label",
        "format": null,
        "label": "Development median",
        "expected": [
          "median"
        ]
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/3/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/3/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/3/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/3/capabilities/qa/delivered",
      "results/v74-quant-threeway/quant_threeway.json#/recommendation_rule"
    ],
    "note": "Post-test rule on the identical frozen cells, never a test-error minimum. New-state errors pool boundary and interior cells equally per cell.",
    "compact_scores": "",
    "rendered": "Development median"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 10,
    "column": 2,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/code/mae",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/code/n",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/code/mae",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/code/n"
        ],
        "op": "weighted_mean",
        "format": ".3f"
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/3/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/3/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/3/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/3/capabilities/qa/delivered",
      "results/v74-quant-threeway/quant_threeway.json#/recommendation_rule"
    ],
    "note": "Post-test rule on the identical frozen cells, never a test-error minimum. New-state errors pool boundary and interior cells equally per cell.",
    "compact_scores": "",
    "rendered": "0.153"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 10,
    "column": 3,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/loso/scores/zero/code"
        ],
        "op": "label",
        "format": null,
        "label": "No change",
        "expected": [
          {
            "n": 54,
            "n_states": 6,
            "state_mae": {
              "pythia-1.4b@step143000": 0.5143543829067956,
              "pythia-1.4b@step16000": 0.10937458732799844,
              "pythia-160m@step143000": 6.2735256054723605,
              "pythia-160m@step16000": 0.3426432136914666,
              "pythia-410m@step143000": 1.110008451522595,
              "pythia-410m@step16000": 0.19481419855795895
            },
            "macro_mae": 1.4241200732465291,
            "mae": 1.4241200732465291
          }
        ]
      }
    ],
    "context": [
      "results/v69-quant-confirm/develop.json#/loso/scores"
    ],
    "note": "Minimum development LOSO macro MAE excluding the selected candidate, per capability: bilinear regression / no change / development median.",
    "compact_scores": "",
    "rendered": "No change"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 10,
    "column": 4,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/zero/code/mae",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/zero/code/n",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/zero/code/mae",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/zero/code/n"
        ],
        "op": "weighted_mean",
        "format": ".3f"
      }
    ],
    "context": [
      "results/v69-quant-confirm/develop.json#/loso/scores"
    ],
    "note": "Minimum development LOSO macro MAE excluding the selected candidate, per capability: bilinear regression / no change / development median.",
    "compact_scores": "",
    "rendered": "0.563"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 10,
    "column": 5,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/code/mae",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/code/n",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/code/mae",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/code/n",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/zero/code/mae",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/zero/code/n",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/zero/code/mae",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/zero/code/n"
        ],
        "op": "difference",
        "parts": [
          {
            "sources": [
              "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/zero/code/mae",
              "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/zero/code/n",
              "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/zero/code/mae",
              "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/zero/code/n"
            ],
            "op": "weighted_mean",
            "format": ".3f"
          },
          {
            "sources": [
              "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/code/mae",
              "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/code/n",
              "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/code/mae",
              "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/code/n"
            ],
            "op": "weighted_mean",
            "format": ".3f"
          }
        ],
        "format": "+.3f"
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/3/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/3/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/3/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/3/capabilities/qa/delivered",
      "results/v74-quant-threeway/quant_threeway.json#/recommendation_rule",
      "results/v69-quant-confirm/develop.json#/loso/scores"
    ],
    "note": "baseline error minus delivered error, per capability",
    "compact_scores": "",
    "rendered": "$+$0.410"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 11,
    "column": 0,
    "parts": [
      "Question answering"
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/3/capabilities/qa/delivered"
    ],
    "note": "",
    "compact_scores": "",
    "rendered": "Question answering"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 11,
    "column": 1,
    "parts": [
      {
        "sources": [
          "results/v86-main-table/summary.json#/main_rows/3/capabilities/qa/delivered"
        ],
        "op": "label",
        "format": null,
        "label": "Development median",
        "expected": [
          "median"
        ]
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/3/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/3/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/3/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/3/capabilities/qa/delivered",
      "results/v74-quant-threeway/quant_threeway.json#/recommendation_rule"
    ],
    "note": "Post-test rule on the identical frozen cells, never a test-error minimum. New-state errors pool boundary and interior cells equally per cell.",
    "compact_scores": "",
    "rendered": "Development median"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 11,
    "column": 2,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/mae",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/n",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/mae",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/n"
        ],
        "op": "weighted_mean",
        "format": ".3f"
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/3/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/3/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/3/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/3/capabilities/qa/delivered",
      "results/v74-quant-threeway/quant_threeway.json#/recommendation_rule"
    ],
    "note": "Post-test rule on the identical frozen cells, never a test-error minimum. New-state errors pool boundary and interior cells equally per cell.",
    "compact_scores": "",
    "rendered": "0.141"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 11,
    "column": 3,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/loso/scores/median/qa"
        ],
        "op": "label",
        "format": null,
        "label": "Development median",
        "expected": [
          {
            "n": 54,
            "n_states": 6,
            "state_mae": {
              "pythia-1.4b@step143000": 0.16258053443177,
              "pythia-1.4b@step16000": 0.2355005016899031,
              "pythia-160m@step143000": 6.541049456062526,
              "pythia-160m@step16000": 0.09769750739332464,
              "pythia-410m@step143000": 0.7294274133924797,
              "pythia-410m@step16000": 0.15231569497253902
            },
            "macro_mae": 1.319761851323757,
            "mae": 1.3197618513237568
          }
        ]
      }
    ],
    "context": [
      "results/v69-quant-confirm/develop.json#/loso/scores"
    ],
    "note": "Minimum development LOSO macro MAE excluding the selected candidate, per capability: bilinear regression / no change / development median.",
    "compact_scores": "",
    "rendered": "Development median"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 11,
    "column": 4,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/mae",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/n",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/mae",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/n"
        ],
        "op": "weighted_mean",
        "format": ".3f"
      }
    ],
    "context": [
      "results/v69-quant-confirm/develop.json#/loso/scores"
    ],
    "note": "Minimum development LOSO macro MAE excluding the selected candidate, per capability: bilinear regression / no change / development median.",
    "compact_scores": "",
    "rendered": "0.141"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 11,
    "column": 5,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/mae",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/n",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/mae",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/n",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/mae",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/n",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/mae",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/n"
        ],
        "op": "difference",
        "parts": [
          {
            "sources": [
              "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/mae",
              "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/n",
              "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/mae",
              "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/n"
            ],
            "op": "weighted_mean",
            "format": ".3f"
          },
          {
            "sources": [
              "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/mae",
              "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/n",
              "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/mae",
              "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/n"
            ],
            "op": "weighted_mean",
            "format": ".3f"
          }
        ],
        "format": "+.3f"
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/3/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/3/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/3/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/3/capabilities/qa/delivered",
      "results/v74-quant-threeway/quant_threeway.json#/recommendation_rule",
      "results/v69-quant-confirm/develop.json#/loso/scores"
    ],
    "note": "baseline error minus delivered error, per capability",
    "compact_scores": "",
    "rendered": "$+$0.000"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 12,
    "column": 0,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/confirmation_register/students/0",
          "results/v70-distill-confirm/freeze.json#/confirmation_register/pools",
          "results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned"
        ],
        "op": "label",
        "format": null,
        "label": "Gemma 270 million distilled on six new pools at 50 to 200 thousand tokens",
        "expected": [
          "gemma3-270m",
          {
            "U200_s31": {
              "U": 200,
              "data_seed": 31,
              "role": "confirmation",
              "n_examples": 597,
              "n_training_examples": 597,
              "pool_processed_tokens": 179688,
              "D_U_completion": 52958,
              "completion_processed_ratio": 0.2947219625128,
              "domain_counts": {
                "code": 198,
                "qa": 199,
                "math": 200
              },
              "id_set_sha256": "248cea90980ec9e921a9d8b2869cfbd558ab6910ba5509996f56d1486d5100a7",
              "data_pool_sha256": "111a5a9e84816cb050c3f7ce921eda2d06cc2581bb22075e1a486714e7801a8e",
              "source_counts": {
                "math": {
                  "source_rows": 200,
                  "training_rows": 200,
                  "coverage_deleted_rows": 0
                },
                "qa": {
                  "source_rows": 200,
                  "training_rows": 199,
                  "coverage_deleted_rows": 1
                },
                "code": {
                  "source_rows": 200,
                  "training_rows": 198,
                  "coverage_deleted_rows": 2
                }
              },
              "planned_milestones": [
                {
                  "planned_T_completion": 50000,
                  "trigger_processed": 169652,
                  "E_completion_convention": 0.9441444163299219
                },
                {
                  "planned_T_completion": 100000,
                  "trigger_processed": 339303,
                  "E_completion_convention": 1.8882888326598437
                },
                {
                  "planned_T_completion": 200000,
                  "trigger_processed": 678606,
                  "E_completion_convention": 3.7765776653196874
                }
              ],
              "schedule_updates": 212,
              "planned_epochs": 6
            },
            "U200_s32": {
              "U": 200,
              "data_seed": 32,
              "role": "confirmation",
              "n_examples": 594,
              "n_training_examples": 594,
              "pool_processed_tokens": 176885,
              "D_U_completion": 52964,
              "completion_processed_ratio": 0.299426180851966,
              "domain_counts": {
                "code": 199,
                "math": 200,
                "qa": 195
              },
              "id_set_sha256": "d7361b13114591e3e246acc73ac57650c5694929659ca7c898a88955c99327bc",
              "data_pool_sha256": "babaee54e739cf5878333cad113ce15a3ddb331f6f133f1a360ae1d22d8e94e3",
              "source_counts": {
                "math": {
                  "source_rows": 200,
                  "training_rows": 200,
                  "coverage_deleted_rows": 0
                },
                "qa": {
                  "source_rows": 200,
                  "training_rows": 195,
                  "coverage_deleted_rows": 5
                },
                "code": {
                  "source_rows": 200,
                  "training_rows": 199,
                  "coverage_deleted_rows": 1
                }
              },
              "planned_milestones": [
                {
                  "planned_T_completion": 50000,
                  "trigger_processed": 166987,
                  "E_completion_convention": 0.9440374594063893
                },
                {
                  "planned_T_completion": 100000,
                  "trigger_processed": 333973,
                  "E_completion_convention": 1.8880749188127786
                },
                {
                  "planned_T_completion": 200000,
                  "trigger_processed": 667945,
                  "E_completion_convention": 3.776149837625557
                }
              ],
              "schedule_updates": 215,
              "planned_epochs": 6
            },
            "U200_s33": {
              "U": 200,
              "data_seed": 33,
              "role": "confirmation",
              "n_examples": 595,
              "n_training_examples": 595,
              "pool_processed_tokens": 176898,
              "D_U_completion": 51800,
              "completion_processed_ratio": 0.292824113330846,
              "domain_counts": {
                "code": 198,
                "math": 200,
                "qa": 197
              },
              "id_set_sha256": "0f2c000781217cd4e671ab4f776cdf4d24405c23ed5c4d080e7c2e158aa38add",
              "data_pool_sha256": "9080a1f0baed5031f2095ff583da9fe720bd341ff79874c51576c266f99cceb0",
              "source_counts": {
                "math": {
                  "source_rows": 200,
                  "training_rows": 200,
                  "coverage_deleted_rows": 0
                },
                "qa": {
                  "source_rows": 200,
                  "training_rows": 197,
                  "coverage_deleted_rows": 3
                },
                "code": {
                  "source_rows": 200,
                  "training_rows": 198,
                  "coverage_deleted_rows": 2
                }
              },
              "planned_milestones": [
                {
                  "planned_T_completion": 50000,
                  "trigger_processed": 170751,
                  "E_completion_convention": 0.9652509652509652
                },
                {
                  "planned_T_completion": 100000,
                  "trigger_processed": 341502,
                  "E_completion_convention": 1.9305019305019304
                },
                {
                  "planned_T_completion": 200000,
                  "trigger_processed": 683004,
                  "E_completion_convention": 3.861003861003861
                }
              ],
              "schedule_updates": 215,
              "planned_epochs": 6
            },
            "U200_s34": {
              "U": 200,
              "data_seed": 34,
              "role": "confirmation",
              "n_examples": 592,
              "n_training_examples": 592,
              "pool_processed_tokens": 178516,
              "D_U_completion": 53528,
              "completion_processed_ratio": 0.29984987340070357,
              "domain_counts": {
                "code": 195,
                "qa": 197,
                "math": 200
              },
              "id_set_sha256": "576e944e2480472b1f1a0676f7c4a16e79c4eb13ee608a33460bde406ece69ba",
              "data_pool_sha256": "d19eb5f62d1f8015b7811f2e52f24efcfb597f41ca00c3cdad1f914ec96050ac",
              "source_counts": {
                "math": {
                  "source_rows": 200,
                  "training_rows": 200,
                  "coverage_deleted_rows": 0
                },
                "qa": {
                  "source_rows": 200,
                  "training_rows": 197,
                  "coverage_deleted_rows": 3
                },
                "code": {
                  "source_rows": 200,
                  "training_rows": 195,
                  "coverage_deleted_rows": 5
                }
              },
              "planned_milestones": [
                {
                  "planned_T_completion": 50000,
                  "trigger_processed": 166751,
                  "E_completion_convention": 0.9340905694216112
                },
                {
                  "planned_T_completion": 100000,
                  "trigger_processed": 333501,
                  "E_completion_convention": 1.8681811388432223
                },
                {
                  "planned_T_completion": 200000,
                  "trigger_processed": 667001,
                  "E_completion_convention": 3.7363622776864447
                }
              ],
              "schedule_updates": 208,
              "planned_epochs": 6
            },
            "U200_s35": {
              "U": 200,
              "data_seed": 35,
              "role": "confirmation",
              "n_examples": 592,
              "n_training_examples": 592,
              "pool_processed_tokens": 178670,
              "D_U_completion": 53332,
              "completion_processed_ratio": 0.2984944310740471,
              "domain_counts": {
                "code": 195,
                "qa": 197,
                "math": 200
              },
              "id_set_sha256": "193e60a043f4a126fe14b75a2aae18b07e919a3e89cba039fb1ad03c6a18db7d",
              "data_pool_sha256": "01742c467573d627517885096f6a984e76f97d76e66460d6874fd2c96154f801",
              "source_counts": {
                "math": {
                  "source_rows": 200,
                  "training_rows": 200,
                  "coverage_deleted_rows": 0
                },
                "qa": {
                  "source_rows": 200,
                  "training_rows": 197,
                  "coverage_deleted_rows": 3
                },
                "code": {
                  "source_rows": 200,
                  "training_rows": 195,
                  "coverage_deleted_rows": 5
                }
              },
              "planned_milestones": [
                {
                  "planned_T_completion": 50000,
                  "trigger_processed": 167508,
                  "E_completion_convention": 0.9375234380859522
                },
                {
                  "planned_T_completion": 100000,
                  "trigger_processed": 335015,
                  "E_completion_convention": 1.8750468761719044
                },
                {
                  "planned_T_completion": 200000,
                  "trigger_processed": 670030,
                  "E_completion_convention": 3.7500937523438087
                }
              ],
              "schedule_updates": 208,
              "planned_epochs": 6
            },
            "U200_s36": {
              "U": 200,
              "data_seed": 36,
              "role": "confirmation",
              "n_examples": 592,
              "n_training_examples": 592,
              "pool_processed_tokens": 178194,
              "D_U_completion": 53411,
              "completion_processed_ratio": 0.2997351201499489,
              "domain_counts": {
                "code": 198,
                "qa": 194,
                "math": 200
              },
              "id_set_sha256": "a7448d221b5d68cf287b65959825d9f2d8d7d0cf93ad787d8bffd2cdff16771e",
              "data_pool_sha256": "c5eca315c67c25841f15d7ca701c7b12a81d28c2b2635b3864c8b748b2cda0b1",
              "source_counts": {
                "math": {
                  "source_rows": 200,
                  "training_rows": 200,
                  "coverage_deleted_rows": 0
                },
                "qa": {
                  "source_rows": 200,
                  "training_rows": 194,
                  "coverage_deleted_rows": 6
                },
                "code": {
                  "source_rows": 200,
                  "training_rows": 198,
                  "coverage_deleted_rows": 2
                }
              },
              "planned_milestones": [
                {
                  "planned_T_completion": 50000,
                  "trigger_processed": 166814,
                  "E_completion_convention": 0.9361367508565651
                },
                {
                  "planned_T_completion": 100000,
                  "trigger_processed": 333628,
                  "E_completion_convention": 1.8722735017131302
                },
                {
                  "planned_T_completion": 200000,
                  "trigger_processed": 667256,
                  "E_completion_convention": 3.7445470034262605
                }
              ],
              "schedule_updates": 208,
              "planned_epochs": 6
            }
          },
          [
            50000,
            100000,
            200000
          ]
        ]
      },
      "; ",
      {
        "sources": [
          "results/v70-distill-confirm/develop.json#/development_structure/n_points"
        ],
        "op": "identity",
        "format": null
      },
      " measurements"
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/confirmation_register/unused_U_assertion",
      "results/v70-distill-confirm/freeze.json#/frozen_at_utc",
      "results/v47-p2-register/register.json#/v5_confirm/registered_at_utc",
      "results/v70-distill-confirm/develop.json#/development_structure",
      "results/v70-distill-confirm/develop.json#/points",
      "results/v70-distill-confirm/freeze.json#/inputs_sha256/results~1v70-distill-confirm~1develop.json"
    ],
    "note": " 100 registered checkpoints (25 trajectories times four) per capability, pooled across development students for the shared fit; not 100 per test student. The freeze authenticates develop.json; dense anchors excluded.",
    "compact_scores": "",
    "rendered": "\\multicolumn{6}{@{}>{\\raggedright\\arraybackslash}p{\\dimexpr\\textwidth-0pt\\relax}@{}}{\\textit{Gemma 270 million distilled on six new pools at 50 to 200 thousand tokens; 100 measurements}}",
    "column_span": 6
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 13,
    "column": 0,
    "parts": [
      "Mathematics"
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/selected/math/method"
    ],
    "note": "",
    "compact_scores": "",
    "rendered": "Mathematics"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 13,
    "column": 1,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/selected/math/method"
        ],
        "op": "label",
        "format": null,
        "label": "Reuse form",
        "expected": [
          "E"
        ]
      }
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/selected",
      "results/v70-distill-confirm/freeze.json#/models"
    ],
    "note": "The frozen and delivered forms are identical: one-coefficient zero-anchored reuse for Math/Code, joint budget/pool for QA; fixed before test.",
    "compact_scores": "",
    "rendered": "Reuse form"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 13,
    "column": 2,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/0/candidate_mae"
        ],
        "op": "identity",
        "format": ".3f"
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/4/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/qa/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/qa/delivered"
    ],
    "note": "Same candidate, same cells; repeat the stored MAEs without the candidate-versus-baseline intervals.",
    "compact_scores": "",
    "rendered": "0.074"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 13,
    "column": 3,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/strongest_baseline/gemma3-270m/math/method"
        ],
        "op": "label",
        "format": null,
        "label": "Budget regression",
        "expected": [
          "T-only"
        ]
      }
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/baseline_rule",
      "results/v70-distill-confirm/freeze.json#/strongest_baseline"
    ],
    "note": "Development-fixed baseline identities for this student: budget regression / reuse regression / reuse regression.",
    "compact_scores": "",
    "rendered": "Budget regression"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 13,
    "column": 4,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/0/baseline_mae"
        ],
        "op": "identity",
        "format": ".3f"
      }
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/baseline_rule",
      "results/v70-distill-confirm/freeze.json#/strongest_baseline"
    ],
    "note": "Development-fixed baseline identities for this student: budget regression / reuse regression / reuse regression.",
    "compact_scores": "",
    "rendered": "0.065"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 13,
    "column": 5,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/0/candidate_mae",
          "results/v70-distill-confirm/compare.json#/groups/0/baseline_mae"
        ],
        "op": "difference",
        "parts": [
          {
            "sources": [
              "results/v70-distill-confirm/compare.json#/groups/0/baseline_mae"
            ],
            "op": "identity",
            "format": ".3f"
          },
          {
            "sources": [
              "results/v70-distill-confirm/compare.json#/groups/0/candidate_mae"
            ],
            "op": "identity",
            "format": ".3f"
          }
        ],
        "format": "+.3f"
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/4/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/qa/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/qa/delivered",
      "results/v70-distill-confirm/freeze.json#/baseline_rule",
      "results/v70-distill-confirm/freeze.json#/strongest_baseline"
    ],
    "note": "baseline error minus delivered error, per capability",
    "compact_scores": "",
    "rendered": "$-$0.009"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 14,
    "column": 0,
    "parts": [
      "Code"
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/selected/code/method"
    ],
    "note": "",
    "compact_scores": "",
    "rendered": "Code"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 14,
    "column": 1,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/selected/code/method"
        ],
        "op": "label",
        "format": null,
        "label": "Reuse form",
        "expected": [
          "E"
        ]
      }
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/selected",
      "results/v70-distill-confirm/freeze.json#/models"
    ],
    "note": "The frozen and delivered forms are identical: one-coefficient zero-anchored reuse for Math/Code, joint budget/pool for QA; fixed before test.",
    "compact_scores": "",
    "rendered": "Reuse form"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 14,
    "column": 2,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/1/candidate_mae"
        ],
        "op": "identity",
        "format": ".3f"
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/4/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/qa/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/qa/delivered"
    ],
    "note": "Same candidate, same cells; repeat the stored MAEs without the candidate-versus-baseline intervals.",
    "compact_scores": "",
    "rendered": "0.019"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 14,
    "column": 3,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/strongest_baseline/gemma3-270m/code/method"
        ],
        "op": "label",
        "format": null,
        "label": "Reuse regression",
        "expected": [
          "E-only"
        ]
      }
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/baseline_rule",
      "results/v70-distill-confirm/freeze.json#/strongest_baseline"
    ],
    "note": "Development-fixed baseline identities for this student: budget regression / reuse regression / reuse regression.",
    "compact_scores": "",
    "rendered": "Reuse regression"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 14,
    "column": 4,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/1/baseline_mae"
        ],
        "op": "identity",
        "format": ".3f"
      }
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/baseline_rule",
      "results/v70-distill-confirm/freeze.json#/strongest_baseline"
    ],
    "note": "Development-fixed baseline identities for this student: budget regression / reuse regression / reuse regression.",
    "compact_scores": "",
    "rendered": "0.023"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 14,
    "column": 5,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/1/candidate_mae",
          "results/v70-distill-confirm/compare.json#/groups/1/baseline_mae"
        ],
        "op": "difference",
        "parts": [
          {
            "sources": [
              "results/v70-distill-confirm/compare.json#/groups/1/baseline_mae"
            ],
            "op": "identity",
            "format": ".3f"
          },
          {
            "sources": [
              "results/v70-distill-confirm/compare.json#/groups/1/candidate_mae"
            ],
            "op": "identity",
            "format": ".3f"
          }
        ],
        "format": "+.3f"
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/4/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/qa/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/qa/delivered",
      "results/v70-distill-confirm/freeze.json#/baseline_rule",
      "results/v70-distill-confirm/freeze.json#/strongest_baseline"
    ],
    "note": "baseline error minus delivered error, per capability",
    "compact_scores": "",
    "rendered": "$+$0.004"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 15,
    "column": 0,
    "parts": [
      "Question answering"
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/selected/qa/method"
    ],
    "note": "",
    "compact_scores": "",
    "rendered": "Question answering"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 15,
    "column": 1,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/selected/qa/method"
        ],
        "op": "label",
        "format": null,
        "label": "Budget and pool form",
        "expected": [
          "joint"
        ]
      }
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/selected",
      "results/v70-distill-confirm/freeze.json#/models"
    ],
    "note": "The frozen and delivered forms are identical: one-coefficient zero-anchored reuse for Math/Code, joint budget/pool for QA; fixed before test.",
    "compact_scores": "",
    "rendered": "Budget and pool form"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 15,
    "column": 2,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/2/candidate_mae"
        ],
        "op": "identity",
        "format": ".3f"
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/4/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/qa/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/qa/delivered"
    ],
    "note": "Same candidate, same cells; repeat the stored MAEs without the candidate-versus-baseline intervals.",
    "compact_scores": "",
    "rendered": "0.515"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 15,
    "column": 3,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/strongest_baseline/gemma3-270m/qa/method"
        ],
        "op": "label",
        "format": null,
        "label": "Reuse regression",
        "expected": [
          "E-only"
        ]
      }
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/baseline_rule",
      "results/v70-distill-confirm/freeze.json#/strongest_baseline"
    ],
    "note": "Development-fixed baseline identities for this student: budget regression / reuse regression / reuse regression.",
    "compact_scores": "",
    "rendered": "Reuse regression"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 15,
    "column": 4,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/2/baseline_mae"
        ],
        "op": "identity",
        "format": ".3f"
      }
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/baseline_rule",
      "results/v70-distill-confirm/freeze.json#/strongest_baseline"
    ],
    "note": "Development-fixed baseline identities for this student: budget regression / reuse regression / reuse regression.",
    "compact_scores": "",
    "rendered": "0.610"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 15,
    "column": 5,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/2/candidate_mae",
          "results/v70-distill-confirm/compare.json#/groups/2/baseline_mae"
        ],
        "op": "difference",
        "parts": [
          {
            "sources": [
              "results/v70-distill-confirm/compare.json#/groups/2/baseline_mae"
            ],
            "op": "identity",
            "format": ".3f"
          },
          {
            "sources": [
              "results/v70-distill-confirm/compare.json#/groups/2/candidate_mae"
            ],
            "op": "identity",
            "format": ".3f"
          }
        ],
        "format": "+.3f"
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/4/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/qa/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/qa/delivered",
      "results/v70-distill-confirm/freeze.json#/baseline_rule",
      "results/v70-distill-confirm/freeze.json#/strongest_baseline"
    ],
    "note": "baseline error minus delivered error, per capability",
    "compact_scores": "",
    "rendered": "$+$0.095"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 16,
    "column": 0,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/confirmation_register/students/1",
          "results/v70-distill-confirm/freeze.json#/confirmation_register/pools",
          "results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned"
        ],
        "op": "label",
        "format": null,
        "label": "Gemma 1 billion distilled on six new pools at 50 to 200 thousand tokens",
        "expected": [
          "gemma3-1b",
          {
            "U200_s31": {
              "U": 200,
              "data_seed": 31,
              "role": "confirmation",
              "n_examples": 597,
              "n_training_examples": 597,
              "pool_processed_tokens": 179688,
              "D_U_completion": 52958,
              "completion_processed_ratio": 0.2947219625128,
              "domain_counts": {
                "code": 198,
                "qa": 199,
                "math": 200
              },
              "id_set_sha256": "248cea90980ec9e921a9d8b2869cfbd558ab6910ba5509996f56d1486d5100a7",
              "data_pool_sha256": "111a5a9e84816cb050c3f7ce921eda2d06cc2581bb22075e1a486714e7801a8e",
              "source_counts": {
                "math": {
                  "source_rows": 200,
                  "training_rows": 200,
                  "coverage_deleted_rows": 0
                },
                "qa": {
                  "source_rows": 200,
                  "training_rows": 199,
                  "coverage_deleted_rows": 1
                },
                "code": {
                  "source_rows": 200,
                  "training_rows": 198,
                  "coverage_deleted_rows": 2
                }
              },
              "planned_milestones": [
                {
                  "planned_T_completion": 50000,
                  "trigger_processed": 169652,
                  "E_completion_convention": 0.9441444163299219
                },
                {
                  "planned_T_completion": 100000,
                  "trigger_processed": 339303,
                  "E_completion_convention": 1.8882888326598437
                },
                {
                  "planned_T_completion": 200000,
                  "trigger_processed": 678606,
                  "E_completion_convention": 3.7765776653196874
                }
              ],
              "schedule_updates": 212,
              "planned_epochs": 6
            },
            "U200_s32": {
              "U": 200,
              "data_seed": 32,
              "role": "confirmation",
              "n_examples": 594,
              "n_training_examples": 594,
              "pool_processed_tokens": 176885,
              "D_U_completion": 52964,
              "completion_processed_ratio": 0.299426180851966,
              "domain_counts": {
                "code": 199,
                "math": 200,
                "qa": 195
              },
              "id_set_sha256": "d7361b13114591e3e246acc73ac57650c5694929659ca7c898a88955c99327bc",
              "data_pool_sha256": "babaee54e739cf5878333cad113ce15a3ddb331f6f133f1a360ae1d22d8e94e3",
              "source_counts": {
                "math": {
                  "source_rows": 200,
                  "training_rows": 200,
                  "coverage_deleted_rows": 0
                },
                "qa": {
                  "source_rows": 200,
                  "training_rows": 195,
                  "coverage_deleted_rows": 5
                },
                "code": {
                  "source_rows": 200,
                  "training_rows": 199,
                  "coverage_deleted_rows": 1
                }
              },
              "planned_milestones": [
                {
                  "planned_T_completion": 50000,
                  "trigger_processed": 166987,
                  "E_completion_convention": 0.9440374594063893
                },
                {
                  "planned_T_completion": 100000,
                  "trigger_processed": 333973,
                  "E_completion_convention": 1.8880749188127786
                },
                {
                  "planned_T_completion": 200000,
                  "trigger_processed": 667945,
                  "E_completion_convention": 3.776149837625557
                }
              ],
              "schedule_updates": 215,
              "planned_epochs": 6
            },
            "U200_s33": {
              "U": 200,
              "data_seed": 33,
              "role": "confirmation",
              "n_examples": 595,
              "n_training_examples": 595,
              "pool_processed_tokens": 176898,
              "D_U_completion": 51800,
              "completion_processed_ratio": 0.292824113330846,
              "domain_counts": {
                "code": 198,
                "math": 200,
                "qa": 197
              },
              "id_set_sha256": "0f2c000781217cd4e671ab4f776cdf4d24405c23ed5c4d080e7c2e158aa38add",
              "data_pool_sha256": "9080a1f0baed5031f2095ff583da9fe720bd341ff79874c51576c266f99cceb0",
              "source_counts": {
                "math": {
                  "source_rows": 200,
                  "training_rows": 200,
                  "coverage_deleted_rows": 0
                },
                "qa": {
                  "source_rows": 200,
                  "training_rows": 197,
                  "coverage_deleted_rows": 3
                },
                "code": {
                  "source_rows": 200,
                  "training_rows": 198,
                  "coverage_deleted_rows": 2
                }
              },
              "planned_milestones": [
                {
                  "planned_T_completion": 50000,
                  "trigger_processed": 170751,
                  "E_completion_convention": 0.9652509652509652
                },
                {
                  "planned_T_completion": 100000,
                  "trigger_processed": 341502,
                  "E_completion_convention": 1.9305019305019304
                },
                {
                  "planned_T_completion": 200000,
                  "trigger_processed": 683004,
                  "E_completion_convention": 3.861003861003861
                }
              ],
              "schedule_updates": 215,
              "planned_epochs": 6
            },
            "U200_s34": {
              "U": 200,
              "data_seed": 34,
              "role": "confirmation",
              "n_examples": 592,
              "n_training_examples": 592,
              "pool_processed_tokens": 178516,
              "D_U_completion": 53528,
              "completion_processed_ratio": 0.29984987340070357,
              "domain_counts": {
                "code": 195,
                "qa": 197,
                "math": 200
              },
              "id_set_sha256": "576e944e2480472b1f1a0676f7c4a16e79c4eb13ee608a33460bde406ece69ba",
              "data_pool_sha256": "d19eb5f62d1f8015b7811f2e52f24efcfb597f41ca00c3cdad1f914ec96050ac",
              "source_counts": {
                "math": {
                  "source_rows": 200,
                  "training_rows": 200,
                  "coverage_deleted_rows": 0
                },
                "qa": {
                  "source_rows": 200,
                  "training_rows": 197,
                  "coverage_deleted_rows": 3
                },
                "code": {
                  "source_rows": 200,
                  "training_rows": 195,
                  "coverage_deleted_rows": 5
                }
              },
              "planned_milestones": [
                {
                  "planned_T_completion": 50000,
                  "trigger_processed": 166751,
                  "E_completion_convention": 0.9340905694216112
                },
                {
                  "planned_T_completion": 100000,
                  "trigger_processed": 333501,
                  "E_completion_convention": 1.8681811388432223
                },
                {
                  "planned_T_completion": 200000,
                  "trigger_processed": 667001,
                  "E_completion_convention": 3.7363622776864447
                }
              ],
              "schedule_updates": 208,
              "planned_epochs": 6
            },
            "U200_s35": {
              "U": 200,
              "data_seed": 35,
              "role": "confirmation",
              "n_examples": 592,
              "n_training_examples": 592,
              "pool_processed_tokens": 178670,
              "D_U_completion": 53332,
              "completion_processed_ratio": 0.2984944310740471,
              "domain_counts": {
                "code": 195,
                "qa": 197,
                "math": 200
              },
              "id_set_sha256": "193e60a043f4a126fe14b75a2aae18b07e919a3e89cba039fb1ad03c6a18db7d",
              "data_pool_sha256": "01742c467573d627517885096f6a984e76f97d76e66460d6874fd2c96154f801",
              "source_counts": {
                "math": {
                  "source_rows": 200,
                  "training_rows": 200,
                  "coverage_deleted_rows": 0
                },
                "qa": {
                  "source_rows": 200,
                  "training_rows": 197,
                  "coverage_deleted_rows": 3
                },
                "code": {
                  "source_rows": 200,
                  "training_rows": 195,
                  "coverage_deleted_rows": 5
                }
              },
              "planned_milestones": [
                {
                  "planned_T_completion": 50000,
                  "trigger_processed": 167508,
                  "E_completion_convention": 0.9375234380859522
                },
                {
                  "planned_T_completion": 100000,
                  "trigger_processed": 335015,
                  "E_completion_convention": 1.8750468761719044
                },
                {
                  "planned_T_completion": 200000,
                  "trigger_processed": 670030,
                  "E_completion_convention": 3.7500937523438087
                }
              ],
              "schedule_updates": 208,
              "planned_epochs": 6
            },
            "U200_s36": {
              "U": 200,
              "data_seed": 36,
              "role": "confirmation",
              "n_examples": 592,
              "n_training_examples": 592,
              "pool_processed_tokens": 178194,
              "D_U_completion": 53411,
              "completion_processed_ratio": 0.2997351201499489,
              "domain_counts": {
                "code": 198,
                "qa": 194,
                "math": 200
              },
              "id_set_sha256": "a7448d221b5d68cf287b65959825d9f2d8d7d0cf93ad787d8bffd2cdff16771e",
              "data_pool_sha256": "c5eca315c67c25841f15d7ca701c7b12a81d28c2b2635b3864c8b748b2cda0b1",
              "source_counts": {
                "math": {
                  "source_rows": 200,
                  "training_rows": 200,
                  "coverage_deleted_rows": 0
                },
                "qa": {
                  "source_rows": 200,
                  "training_rows": 194,
                  "coverage_deleted_rows": 6
                },
                "code": {
                  "source_rows": 200,
                  "training_rows": 198,
                  "coverage_deleted_rows": 2
                }
              },
              "planned_milestones": [
                {
                  "planned_T_completion": 50000,
                  "trigger_processed": 166814,
                  "E_completion_convention": 0.9361367508565651
                },
                {
                  "planned_T_completion": 100000,
                  "trigger_processed": 333628,
                  "E_completion_convention": 1.8722735017131302
                },
                {
                  "planned_T_completion": 200000,
                  "trigger_processed": 667256,
                  "E_completion_convention": 3.7445470034262605
                }
              ],
              "schedule_updates": 208,
              "planned_epochs": 6
            }
          },
          [
            50000,
            100000,
            200000
          ]
        ]
      },
      "; ",
      {
        "sources": [
          "results/v70-distill-confirm/develop.json#/development_structure/n_points"
        ],
        "op": "identity",
        "format": null
      },
      " measurements"
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/confirmation_register/unused_U_assertion",
      "results/v70-distill-confirm/freeze.json#/frozen_at_utc",
      "results/v47-p2-register/register.json#/v5_confirm/registered_at_utc",
      "results/v70-distill-confirm/develop.json#/development_structure",
      "results/v70-distill-confirm/develop.json#/points",
      "results/v70-distill-confirm/freeze.json#/inputs_sha256/results~1v70-distill-confirm~1develop.json"
    ],
    "note": " 100 registered checkpoints (25 trajectories times four) per capability, pooled across development students for the shared fit; not 100 per test student. The freeze authenticates develop.json; dense anchors excluded.",
    "compact_scores": "",
    "rendered": "\\multicolumn{6}{@{}>{\\raggedright\\arraybackslash}p{\\dimexpr\\textwidth-0pt\\relax}@{}}{\\textit{Gemma 1 billion distilled on six new pools at 50 to 200 thousand tokens; 100 measurements}}",
    "column_span": 6
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 17,
    "column": 0,
    "parts": [
      "Mathematics"
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/selected/math/method"
    ],
    "note": "",
    "compact_scores": "",
    "rendered": "Mathematics"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 17,
    "column": 1,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/selected/math/method"
        ],
        "op": "label",
        "format": null,
        "label": "Reuse form",
        "expected": [
          "E"
        ]
      }
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/selected",
      "results/v70-distill-confirm/freeze.json#/models"
    ],
    "note": "The frozen and delivered forms are identical: one-coefficient zero-anchored reuse for Math/Code, joint budget/pool for QA; fixed before test.",
    "compact_scores": "",
    "rendered": "Reuse form"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 17,
    "column": 2,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/3/candidate_mae"
        ],
        "op": "identity",
        "format": ".3f"
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/4/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/qa/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/qa/delivered"
    ],
    "note": "Same candidate, same cells; repeat the stored MAEs without the candidate-versus-baseline intervals.",
    "compact_scores": "",
    "rendered": "0.057"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 17,
    "column": 3,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/strongest_baseline/gemma3-1b/math/method"
        ],
        "op": "label",
        "format": null,
        "label": "Loss regression",
        "expected": [
          "surface:L0"
        ]
      }
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/baseline_rule",
      "results/v70-distill-confirm/freeze.json#/strongest_baseline"
    ],
    "note": "Development-fixed baseline identities for this student: loss regression / reuse regression / size regression.",
    "compact_scores": "",
    "rendered": "Loss regression"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 17,
    "column": 4,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/3/baseline_mae"
        ],
        "op": "identity",
        "format": ".3f"
      }
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/baseline_rule",
      "results/v70-distill-confirm/freeze.json#/strongest_baseline"
    ],
    "note": "Development-fixed baseline identities for this student: loss regression / reuse regression / size regression.",
    "compact_scores": "",
    "rendered": "0.033"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 17,
    "column": 5,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/3/candidate_mae",
          "results/v70-distill-confirm/compare.json#/groups/3/baseline_mae"
        ],
        "op": "difference",
        "parts": [
          {
            "sources": [
              "results/v70-distill-confirm/compare.json#/groups/3/baseline_mae"
            ],
            "op": "identity",
            "format": ".3f"
          },
          {
            "sources": [
              "results/v70-distill-confirm/compare.json#/groups/3/candidate_mae"
            ],
            "op": "identity",
            "format": ".3f"
          }
        ],
        "format": "+.3f"
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/4/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/qa/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/qa/delivered",
      "results/v70-distill-confirm/freeze.json#/baseline_rule",
      "results/v70-distill-confirm/freeze.json#/strongest_baseline"
    ],
    "note": "baseline error minus delivered error, per capability",
    "compact_scores": "",
    "rendered": "$-$0.023"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 18,
    "column": 0,
    "parts": [
      "Code"
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/selected/code/method"
    ],
    "note": "",
    "compact_scores": "",
    "rendered": "Code"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 18,
    "column": 1,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/selected/code/method"
        ],
        "op": "label",
        "format": null,
        "label": "Reuse form",
        "expected": [
          "E"
        ]
      }
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/selected",
      "results/v70-distill-confirm/freeze.json#/models"
    ],
    "note": "The frozen and delivered forms are identical: one-coefficient zero-anchored reuse for Math/Code, joint budget/pool for QA; fixed before test.",
    "compact_scores": "",
    "rendered": "Reuse form"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 18,
    "column": 2,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/4/candidate_mae"
        ],
        "op": "identity",
        "format": ".3f"
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/4/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/qa/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/qa/delivered"
    ],
    "note": "Same candidate, same cells; repeat the stored MAEs without the candidate-versus-baseline intervals.",
    "compact_scores": "",
    "rendered": "0.049"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 18,
    "column": 3,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/strongest_baseline/gemma3-1b/code/method"
        ],
        "op": "label",
        "format": null,
        "label": "Reuse regression",
        "expected": [
          "E-only"
        ]
      }
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/baseline_rule",
      "results/v70-distill-confirm/freeze.json#/strongest_baseline"
    ],
    "note": "Development-fixed baseline identities for this student: loss regression / reuse regression / size regression.",
    "compact_scores": "",
    "rendered": "Reuse regression"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 18,
    "column": 4,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/4/baseline_mae"
        ],
        "op": "identity",
        "format": ".3f"
      }
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/baseline_rule",
      "results/v70-distill-confirm/freeze.json#/strongest_baseline"
    ],
    "note": "Development-fixed baseline identities for this student: loss regression / reuse regression / size regression.",
    "compact_scores": "",
    "rendered": "0.053"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 18,
    "column": 5,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/4/candidate_mae",
          "results/v70-distill-confirm/compare.json#/groups/4/baseline_mae"
        ],
        "op": "difference",
        "parts": [
          {
            "sources": [
              "results/v70-distill-confirm/compare.json#/groups/4/baseline_mae"
            ],
            "op": "identity",
            "format": ".3f"
          },
          {
            "sources": [
              "results/v70-distill-confirm/compare.json#/groups/4/candidate_mae"
            ],
            "op": "identity",
            "format": ".3f"
          }
        ],
        "format": "+.3f"
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/4/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/qa/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/qa/delivered",
      "results/v70-distill-confirm/freeze.json#/baseline_rule",
      "results/v70-distill-confirm/freeze.json#/strongest_baseline"
    ],
    "note": "baseline error minus delivered error, per capability",
    "compact_scores": "",
    "rendered": "$+$0.005"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 19,
    "column": 0,
    "parts": [
      "Question answering"
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/selected/qa/method"
    ],
    "note": "",
    "compact_scores": "",
    "rendered": "Question answering"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 19,
    "column": 1,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/selected/qa/method"
        ],
        "op": "label",
        "format": null,
        "label": "Budget and pool form",
        "expected": [
          "joint"
        ]
      }
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/selected",
      "results/v70-distill-confirm/freeze.json#/models"
    ],
    "note": "The frozen and delivered forms are identical: one-coefficient zero-anchored reuse for Math/Code, joint budget/pool for QA; fixed before test.",
    "compact_scores": "",
    "rendered": "Budget and pool form"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 19,
    "column": 2,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/5/candidate_mae"
        ],
        "op": "identity",
        "format": ".3f"
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/4/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/qa/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/qa/delivered"
    ],
    "note": "Same candidate, same cells; repeat the stored MAEs without the candidate-versus-baseline intervals.",
    "compact_scores": "",
    "rendered": "0.463"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 19,
    "column": 3,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/strongest_baseline/gemma3-1b/qa/method"
        ],
        "op": "label",
        "format": null,
        "label": "Size regression",
        "expected": [
          "surface:logN"
        ]
      }
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/baseline_rule",
      "results/v70-distill-confirm/freeze.json#/strongest_baseline"
    ],
    "note": "Development-fixed baseline identities for this student: loss regression / reuse regression / size regression.",
    "compact_scores": "",
    "rendered": "Size regression"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 19,
    "column": 4,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/5/baseline_mae"
        ],
        "op": "identity",
        "format": ".3f"
      }
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/baseline_rule",
      "results/v70-distill-confirm/freeze.json#/strongest_baseline"
    ],
    "note": "Development-fixed baseline identities for this student: loss regression / reuse regression / size regression.",
    "compact_scores": "",
    "rendered": "0.450"
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 19,
    "column": 5,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/5/candidate_mae",
          "results/v70-distill-confirm/compare.json#/groups/5/baseline_mae"
        ],
        "op": "difference",
        "parts": [
          {
            "sources": [
              "results/v70-distill-confirm/compare.json#/groups/5/baseline_mae"
            ],
            "op": "identity",
            "format": ".3f"
          },
          {
            "sources": [
              "results/v70-distill-confirm/compare.json#/groups/5/candidate_mae"
            ],
            "op": "identity",
            "format": ".3f"
          }
        ],
        "format": "+.3f"
      }
    ],
    "context": [
      "results/v86-main-table/summary.json#/main_rows/4/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/4/capabilities/qa/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/delivered_timing",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/math/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/code/delivered",
      "results/v86-main-table/summary.json#/main_rows/5/capabilities/qa/delivered",
      "results/v70-distill-confirm/freeze.json#/baseline_rule",
      "results/v70-distill-confirm/freeze.json#/strongest_baseline"
    ],
    "note": "baseline error minus delivered error, per capability",
    "compact_scores": "",
    "rendered": "$-$0.013"
  }
]
```

## Caption recipe

```json
{
  "table": "tab:main-prediction-v2",
  "parts": [
    "Delivered relations versus baselines at equal budget, by capability. Errors are mean absolute errors in nats per token; improvement is baseline minus delivered. Group lines give the task, development configuration measurements per capability, and Retrospective for a relation chosen after seeing the result. The baseline was chosen inside the development folds and scored on the same cells. Distillation students: ",
    {
      "sources": [
        "results/v70-distill-confirm/freeze.json#/confirmation_register/students"
      ],
      "op": "label",
      "format": null,
      "label": "270 million and 1 billion",
      "expected": [
        [
          "gemma3-270m",
          "gemma3-1b"
        ]
      ]
    },
    ". Appendix Table~\\ref{tab:main-prediction-candidates} lists each task's pre-specified candidate; Fig.~\\ref{fig:generalization} compares each row with its baseline."
  ],
  "context": [
    "results/v53-prune-dev/register.json#/feature_names",
    "results/v55-quant-group/register.json#/feature_names",
    "results/v70-distill-confirm/freeze.json#/reference_rule",
    "results/v53-prune-dev/register.json#/candidate_definitions/power",
    "results/v55-quant-group/register.json#/candidate_definitions/low_order_2d",
    "results/v70-distill-confirm/freeze.json#/models"
  ],
  "note": "",
  "compact_scores": "",
  "rendered": "Delivered relations versus baselines at equal budget, by capability. Errors are mean absolute errors in nats per token; improvement is baseline minus delivered. Group lines give the task, development configuration measurements per capability, and Retrospective for a relation chosen after seeing the result. The baseline was chosen inside the development folds and scored on the same cells. Distillation students: 270 million and 1 billion. Appendix Table~\\ref{tab:main-prediction-candidates} lists each task's pre-specified candidate; Fig.~\\ref{fig:generalization} compares each row with its baseline."
}
```

## Candidates table cell recipes

```json
[
  {
    "table": "tab:main-prediction-candidates",
    "row": 0,
    "column": 0,
    "parts": [
      {
        "sources": [
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/tag",
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/densities",
          "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/tag",
          "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/densities",
          "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/tag",
          "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/densities"
        ],
        "op": "label",
        "format": null,
        "label": "Three unseen checkpoints pruned to densities 0.575, 0.675 and 0.85",
        "expected": [
          "pythia-410m@step48000",
          [
            0.85,
            0.675,
            0.575
          ],
          "pythia-1.4b@step112000",
          [
            0.85,
            0.675,
            0.575
          ],
          "pythia-6.9b@step80000",
          [
            0.85,
            0.675,
            0.575
          ]
        ]
      }
    ],
    "context": [
      "results/v53-prune-dev/register.json#/selected_candidate",
      "results/v53-prune-dev/register.json#/dev_states",
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/densities"
    ],
    "note": "All three test checkpoints are absent from every development fit. The 6.9B size occurs at other stages in the expanded register.",
    "compact_scores": "",
    "rendered": "Three unseen checkpoints pruned to densities 0.575, 0.675 and 0.85"
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 0,
    "column": 1,
    "parts": [
      {
        "sources": [
          "results/v53-prune-dev/register.json#/candidate_definitions/power",
          "results/v53-prune-dev/register.json#/n_params_per_capability/power",
          "results/v53-prune-dev/register.json#/n_dev_states"
        ],
        "op": "label",
        "format": null,
        "label": "Five-parameter power form",
        "expected": [
          "(beta.phi) * ((1-d)/0.3)**gamma",
          5,
          17
        ]
      }
    ],
    "context": [
      "results/v53-prune-dev/register.json#/feature_names"
    ],
    "note": "",
    "compact_scores": "",
    "rendered": "Five-parameter power form"
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 0,
    "column": 2,
    "parts": [
      {
        "sources": [
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/power/math",
          "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/power/math",
          "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/power/math"
        ],
        "op": "mean",
        "format": ".3f"
      },
      "\n",
      {
        "sources": [
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/power/code",
          "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/power/code",
          "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/power/code"
        ],
        "op": "mean",
        "format": ".3f"
      },
      "\n",
      {
        "sources": [
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/power/qa",
          "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/power/qa",
          "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/power/qa"
        ],
        "op": "mean",
        "format": ".3f"
      }
    ],
    "context": [],
    "note": "",
    "compact_scores": "ordered",
    "rendered": "\\TableOneErrors{0.243}{0.236}{0.678}"
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 0,
    "column": 3,
    "parts": [
      {
        "sources": [
          "results/v86-main-table/summary.json#/main_rows/0/delivered_timing",
          "results/v86-main-table/summary.json#/main_rows/0/capabilities/math/delivered",
          "results/v86-main-table/summary.json#/main_rows/0/capabilities/code/delivered",
          "results/v86-main-table/summary.json#/main_rows/0/capabilities/qa/delivered"
        ],
        "op": "label",
        "format": null,
        "label": "Source-free median density curve",
        "expected": [
          "fixed after test; reused frozen in Sec. 5",
          "median_curve",
          "median_curve",
          "median_curve"
        ]
      },
      "\n",
      {
        "sources": [
          "results/v86-main-table/summary.json#/main_rows/0/delivered_timing"
        ],
        "op": "label",
        "format": null,
        "label": "Retrospective",
        "expected": [
          "fixed after test; reused frozen in Sec. 5"
        ]
      }
    ],
    "context": [],
    "note": "New-state source-free median curve, fixed after test; scores use the same three checkpoints and densities as the frozen candidate.",
    "compact_scores": "",
    "rendered": "Source-free median density curve\\newline Retrospective"
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 1,
    "column": 0,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/rows/0/state",
          "results/v69-quant-confirm/compare.json#/rows/0/config",
          "results/v69-quant-confirm/compare.json#/rows/3/config",
          "results/v69-quant-confirm/compare.json#/rows/6/config",
          "results/v69-quant-confirm/compare.json#/rows/9/config",
          "results/v69-quant-confirm/compare.json#/rows/12/config",
          "results/v69-quant-confirm/compare.json#/rows/15/config",
          "results/v69-quant-confirm/compare.json#/rows/18/state"
        ],
        "op": "label",
        "format": null,
        "label": "Pythia 410 million and 1.4 billion at unseen group sizes 32 and 512, bit widths 3 to 5",
        "expected": [
          "pythia-410m@step143000",
          "b3_g32",
          "b3_g512",
          "b4_g32",
          "b4_g512",
          "b5_g32",
          "b5_g512",
          "pythia-1.4b@step16000"
        ]
      }
    ],
    "context": [
      "results/v69-quant-confirm/freeze.json#/frozen_at_utc",
      "results/v69-quant-confirm/compare.json#/rows/0/test_set",
      "results/v69-quant-confirm/compare.json#/rows/1/test_set",
      "results/v69-quant-confirm/compare.json#/rows/2/test_set",
      "results/v69-quant-confirm/compare.json#/rows/3/test_set",
      "results/v69-quant-confirm/compare.json#/rows/4/test_set",
      "results/v69-quant-confirm/compare.json#/rows/5/test_set",
      "results/v69-quant-confirm/compare.json#/rows/6/test_set",
      "results/v69-quant-confirm/compare.json#/rows/7/test_set",
      "results/v69-quant-confirm/compare.json#/rows/8/test_set",
      "results/v69-quant-confirm/compare.json#/rows/9/test_set",
      "results/v69-quant-confirm/compare.json#/rows/10/test_set",
      "results/v69-quant-confirm/compare.json#/rows/11/test_set",
      "results/v69-quant-confirm/compare.json#/rows/12/test_set",
      "results/v69-quant-confirm/compare.json#/rows/13/test_set",
      "results/v69-quant-confirm/compare.json#/rows/14/test_set",
      "results/v69-quant-confirm/compare.json#/rows/15/test_set",
      "results/v69-quant-confirm/compare.json#/rows/16/test_set",
      "results/v69-quant-confirm/compare.json#/rows/17/test_set",
      "results/v69-quant-confirm/compare.json#/rows/18/test_set",
      "results/v69-quant-confirm/compare.json#/rows/19/test_set",
      "results/v69-quant-confirm/compare.json#/rows/20/test_set",
      "results/v69-quant-confirm/compare.json#/rows/21/test_set",
      "results/v69-quant-confirm/compare.json#/rows/22/test_set",
      "results/v69-quant-confirm/compare.json#/rows/23/test_set",
      "results/v69-quant-confirm/compare.json#/rows/24/test_set",
      "results/v69-quant-confirm/compare.json#/rows/25/test_set",
      "results/v69-quant-confirm/compare.json#/rows/26/test_set",
      "results/v69-quant-confirm/compare.json#/rows/27/test_set",
      "results/v69-quant-confirm/compare.json#/rows/28/test_set",
      "results/v69-quant-confirm/compare.json#/rows/29/test_set",
      "results/v69-quant-confirm/compare.json#/rows/30/test_set",
      "results/v69-quant-confirm/compare.json#/rows/31/test_set",
      "results/v69-quant-confirm/compare.json#/rows/32/test_set",
      "results/v69-quant-confirm/compare.json#/rows/33/test_set",
      "results/v69-quant-confirm/compare.json#/rows/34/test_set",
      "results/v69-quant-confirm/compare.json#/rows/35/test_set"
    ],
    "note": "",
    "compact_scores": "",
    "rendered": "Pythia 410 million and 1.4 billion at unseen group sizes 32 and 512, bit widths 3 to 5"
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 1,
    "column": 1,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/selected/math/candidate",
          "results/v69-quant-confirm/develop.json#/selected/code/candidate",
          "results/v69-quant-confirm/develop.json#/selected/qa/candidate"
        ],
        "op": "label",
        "format": null,
        "label": "Source regression, the median and no change",
        "expected": [
          "low_order_2d",
          "median",
          "zero"
        ]
      }
    ],
    "context": [
      "results/v55-quant-group/register.json#/candidate_definitions/low_order_2d",
      "results/v69-quant-confirm/develop.json#/models",
      "results/v69-quant-confirm/develop.json#/feature_names",
      "results/v69-quant-confirm/develop.json#/dev_configs"
    ],
    "note": "Frozen candidates unchanged: Math uses the source surface, Code the per-configuration median, QA zero. Median interpolation is source-free and differs from the delivered same-input interpolation.",
    "compact_scores": "",
    "rendered": "Source regression, the median and no change"
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 1,
    "column": 2,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/low_order_2d/math/mae"
        ],
        "op": "identity",
        "format": ".3f"
      },
      "\n",
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/median/code/mae"
        ],
        "op": "identity",
        "format": ".3f"
      },
      "\n",
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/zero/qa/mae"
        ],
        "op": "identity",
        "format": ".3f"
      }
    ],
    "context": [],
    "note": "",
    "compact_scores": "ordered",
    "rendered": "\\TableOneErrors{0.215}{0.557}{0.457}"
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 1,
    "column": 3,
    "parts": [
      {
        "sources": [
          "results/v86-main-table/summary.json#/main_rows/2/delivered_timing",
          "results/v86-main-table/summary.json#/main_rows/2/capabilities/math/delivered",
          "results/v86-main-table/summary.json#/main_rows/2/capabilities/code/delivered",
          "results/v86-main-table/summary.json#/main_rows/2/capabilities/qa/delivered",
          "results/v74-quant-threeway/quant_threeway.json#/recommendation_rule"
        ],
        "op": "label",
        "format": null,
        "label": "Interpolate math and code; use the median for question answering",
        "expected": [
          "fixed after test",
          "same_input_interpolation",
          "same_input_interpolation",
          "median",
          "R: piecewise interpolation for math/code on development states; per-configuration median for QA and for all capabilities on new states. Specified post-test rule, not the minimum error in each test panel."
        ]
      },
      "\n",
      {
        "sources": [
          "results/v86-main-table/summary.json#/main_rows/2/delivered_timing"
        ],
        "op": "label",
        "format": null,
        "label": "Retrospective",
        "expected": [
          "fixed after test"
        ]
      }
    ],
    "context": [],
    "note": "Post-test rule on the identical frozen cells, never a test-error minimum. New-state errors pool boundary and interior cells equally per cell.",
    "compact_scores": "",
    "rendered": "Interpolate math and code; use the median for question answering\\newline Retrospective"
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 2,
    "column": 0,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/rows/36/state",
          "results/v69-quant-confirm/compare.json#/rows/36/config",
          "results/v69-quant-confirm/compare.json#/rows/39/config",
          "results/v69-quant-confirm/compare.json#/rows/42/config",
          "results/v69-quant-confirm/compare.json#/rows/45/config",
          "results/v69-quant-confirm/compare.json#/rows/48/config",
          "results/v69-quant-confirm/compare.json#/rows/51/config",
          "results/v69-quant-confirm/compare.json#/rows/54/config",
          "results/v69-quant-confirm/compare.json#/rows/57/config",
          "results/v69-quant-confirm/compare.json#/rows/60/config"
        ],
        "op": "label",
        "format": null,
        "label": "An unseen 1.4 billion stage at bit widths 3 to 5, group sizes 32 to 512",
        "expected": [
          "pythia-1.4b@step112000",
          "b3_g32",
          "b3_g512",
          "b4_g32",
          "b4_g512",
          "b5_g32",
          "b5_g512",
          "b3_g128",
          "b4_g128",
          "b5_g128"
        ]
      }
    ],
    "context": [
      "results/v69-quant-confirm/freeze.json#/frozen_at_utc",
      "results/v69-quant-confirm/compare.json#/rows/36/test_set",
      "results/v69-quant-confirm/compare.json#/rows/37/test_set",
      "results/v69-quant-confirm/compare.json#/rows/38/test_set",
      "results/v69-quant-confirm/compare.json#/rows/39/test_set",
      "results/v69-quant-confirm/compare.json#/rows/40/test_set",
      "results/v69-quant-confirm/compare.json#/rows/41/test_set",
      "results/v69-quant-confirm/compare.json#/rows/42/test_set",
      "results/v69-quant-confirm/compare.json#/rows/43/test_set",
      "results/v69-quant-confirm/compare.json#/rows/44/test_set",
      "results/v69-quant-confirm/compare.json#/rows/45/test_set",
      "results/v69-quant-confirm/compare.json#/rows/46/test_set",
      "results/v69-quant-confirm/compare.json#/rows/47/test_set",
      "results/v69-quant-confirm/compare.json#/rows/48/test_set",
      "results/v69-quant-confirm/compare.json#/rows/49/test_set",
      "results/v69-quant-confirm/compare.json#/rows/50/test_set",
      "results/v69-quant-confirm/compare.json#/rows/51/test_set",
      "results/v69-quant-confirm/compare.json#/rows/52/test_set",
      "results/v69-quant-confirm/compare.json#/rows/53/test_set",
      "results/v69-quant-confirm/compare.json#/rows/54/test_set",
      "results/v69-quant-confirm/compare.json#/rows/55/test_set",
      "results/v69-quant-confirm/compare.json#/rows/56/test_set",
      "results/v69-quant-confirm/compare.json#/rows/57/test_set",
      "results/v69-quant-confirm/compare.json#/rows/58/test_set",
      "results/v69-quant-confirm/compare.json#/rows/59/test_set",
      "results/v69-quant-confirm/compare.json#/rows/60/test_set",
      "results/v69-quant-confirm/compare.json#/rows/61/test_set",
      "results/v69-quant-confirm/compare.json#/rows/62/test_set"
    ],
    "note": "",
    "compact_scores": "",
    "rendered": "An unseen 1.4 billion stage at bit widths 3 to 5, group sizes 32 to 512"
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 2,
    "column": 1,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/selected/math/candidate",
          "results/v69-quant-confirm/develop.json#/selected/code/candidate",
          "results/v69-quant-confirm/develop.json#/selected/qa/candidate"
        ],
        "op": "label",
        "format": null,
        "label": "Source regression, the median and no change",
        "expected": [
          "low_order_2d",
          "median",
          "zero"
        ]
      }
    ],
    "context": [
      "results/v55-quant-group/register.json#/candidate_definitions/low_order_2d",
      "results/v69-quant-confirm/develop.json#/models",
      "results/v69-quant-confirm/develop.json#/feature_names",
      "results/v69-quant-confirm/develop.json#/dev_configs"
    ],
    "note": "Frozen candidates unchanged: Math uses the source surface, Code the per-configuration median, QA zero. Median interpolation is source-free and differs from the delivered same-input interpolation.",
    "compact_scores": "",
    "rendered": "Source regression, the median and no change"
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 2,
    "column": 2,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/low_order_2d/math/mae",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/low_order_2d/math/n",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/low_order_2d/math/mae",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/low_order_2d/math/n"
        ],
        "op": "weighted_mean",
        "format": ".3f"
      },
      "\n",
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/code/mae",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/code/n",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/code/mae",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/code/n"
        ],
        "op": "weighted_mean",
        "format": ".3f"
      },
      "\n",
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/zero/qa/mae",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/zero/qa/n",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/zero/qa/mae",
          "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/zero/qa/n"
        ],
        "op": "weighted_mean",
        "format": ".3f"
      }
    ],
    "context": [],
    "note": "",
    "compact_scores": "ordered",
    "rendered": "\\TableOneErrors{0.303}{0.153}{0.222}"
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 2,
    "column": 3,
    "parts": [
      {
        "sources": [
          "results/v86-main-table/summary.json#/main_rows/3/delivered_timing",
          "results/v86-main-table/summary.json#/main_rows/3/capabilities/math/delivered",
          "results/v86-main-table/summary.json#/main_rows/3/capabilities/code/delivered",
          "results/v86-main-table/summary.json#/main_rows/3/capabilities/qa/delivered",
          "results/v74-quant-threeway/quant_threeway.json#/recommendation_rule"
        ],
        "op": "label",
        "format": null,
        "label": "Development median",
        "expected": [
          "fixed after test",
          "median",
          "median",
          "median",
          "R: piecewise interpolation for math/code on development states; per-configuration median for QA and for all capabilities on new states. Specified post-test rule, not the minimum error in each test panel."
        ]
      },
      "\n",
      {
        "sources": [
          "results/v86-main-table/summary.json#/main_rows/3/delivered_timing"
        ],
        "op": "label",
        "format": null,
        "label": "Retrospective",
        "expected": [
          "fixed after test"
        ]
      }
    ],
    "context": [],
    "note": "Post-test rule on the identical frozen cells, never a test-error minimum. New-state errors pool boundary and interior cells equally per cell.",
    "compact_scores": "",
    "rendered": "Development median\\newline Retrospective"
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 3,
    "column": 0,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/confirmation_register/students/0",
          "results/v70-distill-confirm/freeze.json#/confirmation_register/pools",
          "results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned"
        ],
        "op": "label",
        "format": null,
        "label": "Gemma 270 million distilled on six new pools at 50 to 200 thousand tokens",
        "expected": [
          "gemma3-270m",
          {
            "U200_s31": {
              "U": 200,
              "data_seed": 31,
              "role": "confirmation",
              "n_examples": 597,
              "n_training_examples": 597,
              "pool_processed_tokens": 179688,
              "D_U_completion": 52958,
              "completion_processed_ratio": 0.2947219625128,
              "domain_counts": {
                "code": 198,
                "qa": 199,
                "math": 200
              },
              "id_set_sha256": "248cea90980ec9e921a9d8b2869cfbd558ab6910ba5509996f56d1486d5100a7",
              "data_pool_sha256": "111a5a9e84816cb050c3f7ce921eda2d06cc2581bb22075e1a486714e7801a8e",
              "source_counts": {
                "math": {
                  "source_rows": 200,
                  "training_rows": 200,
                  "coverage_deleted_rows": 0
                },
                "qa": {
                  "source_rows": 200,
                  "training_rows": 199,
                  "coverage_deleted_rows": 1
                },
                "code": {
                  "source_rows": 200,
                  "training_rows": 198,
                  "coverage_deleted_rows": 2
                }
              },
              "planned_milestones": [
                {
                  "planned_T_completion": 50000,
                  "trigger_processed": 169652,
                  "E_completion_convention": 0.9441444163299219
                },
                {
                  "planned_T_completion": 100000,
                  "trigger_processed": 339303,
                  "E_completion_convention": 1.8882888326598437
                },
                {
                  "planned_T_completion": 200000,
                  "trigger_processed": 678606,
                  "E_completion_convention": 3.7765776653196874
                }
              ],
              "schedule_updates": 212,
              "planned_epochs": 6
            },
            "U200_s32": {
              "U": 200,
              "data_seed": 32,
              "role": "confirmation",
              "n_examples": 594,
              "n_training_examples": 594,
              "pool_processed_tokens": 176885,
              "D_U_completion": 52964,
              "completion_processed_ratio": 0.299426180851966,
              "domain_counts": {
                "code": 199,
                "math": 200,
                "qa": 195
              },
              "id_set_sha256": "d7361b13114591e3e246acc73ac57650c5694929659ca7c898a88955c99327bc",
              "data_pool_sha256": "babaee54e739cf5878333cad113ce15a3ddb331f6f133f1a360ae1d22d8e94e3",
              "source_counts": {
                "math": {
                  "source_rows": 200,
                  "training_rows": 200,
                  "coverage_deleted_rows": 0
                },
                "qa": {
                  "source_rows": 200,
                  "training_rows": 195,
                  "coverage_deleted_rows": 5
                },
                "code": {
                  "source_rows": 200,
                  "training_rows": 199,
                  "coverage_deleted_rows": 1
                }
              },
              "planned_milestones": [
                {
                  "planned_T_completion": 50000,
                  "trigger_processed": 166987,
                  "E_completion_convention": 0.9440374594063893
                },
                {
                  "planned_T_completion": 100000,
                  "trigger_processed": 333973,
                  "E_completion_convention": 1.8880749188127786
                },
                {
                  "planned_T_completion": 200000,
                  "trigger_processed": 667945,
                  "E_completion_convention": 3.776149837625557
                }
              ],
              "schedule_updates": 215,
              "planned_epochs": 6
            },
            "U200_s33": {
              "U": 200,
              "data_seed": 33,
              "role": "confirmation",
              "n_examples": 595,
              "n_training_examples": 595,
              "pool_processed_tokens": 176898,
              "D_U_completion": 51800,
              "completion_processed_ratio": 0.292824113330846,
              "domain_counts": {
                "code": 198,
                "math": 200,
                "qa": 197
              },
              "id_set_sha256": "0f2c000781217cd4e671ab4f776cdf4d24405c23ed5c4d080e7c2e158aa38add",
              "data_pool_sha256": "9080a1f0baed5031f2095ff583da9fe720bd341ff79874c51576c266f99cceb0",
              "source_counts": {
                "math": {
                  "source_rows": 200,
                  "training_rows": 200,
                  "coverage_deleted_rows": 0
                },
                "qa": {
                  "source_rows": 200,
                  "training_rows": 197,
                  "coverage_deleted_rows": 3
                },
                "code": {
                  "source_rows": 200,
                  "training_rows": 198,
                  "coverage_deleted_rows": 2
                }
              },
              "planned_milestones": [
                {
                  "planned_T_completion": 50000,
                  "trigger_processed": 170751,
                  "E_completion_convention": 0.9652509652509652
                },
                {
                  "planned_T_completion": 100000,
                  "trigger_processed": 341502,
                  "E_completion_convention": 1.9305019305019304
                },
                {
                  "planned_T_completion": 200000,
                  "trigger_processed": 683004,
                  "E_completion_convention": 3.861003861003861
                }
              ],
              "schedule_updates": 215,
              "planned_epochs": 6
            },
            "U200_s34": {
              "U": 200,
              "data_seed": 34,
              "role": "confirmation",
              "n_examples": 592,
              "n_training_examples": 592,
              "pool_processed_tokens": 178516,
              "D_U_completion": 53528,
              "completion_processed_ratio": 0.29984987340070357,
              "domain_counts": {
                "code": 195,
                "qa": 197,
                "math": 200
              },
              "id_set_sha256": "576e944e2480472b1f1a0676f7c4a16e79c4eb13ee608a33460bde406ece69ba",
              "data_pool_sha256": "d19eb5f62d1f8015b7811f2e52f24efcfb597f41ca00c3cdad1f914ec96050ac",
              "source_counts": {
                "math": {
                  "source_rows": 200,
                  "training_rows": 200,
                  "coverage_deleted_rows": 0
                },
                "qa": {
                  "source_rows": 200,
                  "training_rows": 197,
                  "coverage_deleted_rows": 3
                },
                "code": {
                  "source_rows": 200,
                  "training_rows": 195,
                  "coverage_deleted_rows": 5
                }
              },
              "planned_milestones": [
                {
                  "planned_T_completion": 50000,
                  "trigger_processed": 166751,
                  "E_completion_convention": 0.9340905694216112
                },
                {
                  "planned_T_completion": 100000,
                  "trigger_processed": 333501,
                  "E_completion_convention": 1.8681811388432223
                },
                {
                  "planned_T_completion": 200000,
                  "trigger_processed": 667001,
                  "E_completion_convention": 3.7363622776864447
                }
              ],
              "schedule_updates": 208,
              "planned_epochs": 6
            },
            "U200_s35": {
              "U": 200,
              "data_seed": 35,
              "role": "confirmation",
              "n_examples": 592,
              "n_training_examples": 592,
              "pool_processed_tokens": 178670,
              "D_U_completion": 53332,
              "completion_processed_ratio": 0.2984944310740471,
              "domain_counts": {
                "code": 195,
                "qa": 197,
                "math": 200
              },
              "id_set_sha256": "193e60a043f4a126fe14b75a2aae18b07e919a3e89cba039fb1ad03c6a18db7d",
              "data_pool_sha256": "01742c467573d627517885096f6a984e76f97d76e66460d6874fd2c96154f801",
              "source_counts": {
                "math": {
                  "source_rows": 200,
                  "training_rows": 200,
                  "coverage_deleted_rows": 0
                },
                "qa": {
                  "source_rows": 200,
                  "training_rows": 197,
                  "coverage_deleted_rows": 3
                },
                "code": {
                  "source_rows": 200,
                  "training_rows": 195,
                  "coverage_deleted_rows": 5
                }
              },
              "planned_milestones": [
                {
                  "planned_T_completion": 50000,
                  "trigger_processed": 167508,
                  "E_completion_convention": 0.9375234380859522
                },
                {
                  "planned_T_completion": 100000,
                  "trigger_processed": 335015,
                  "E_completion_convention": 1.8750468761719044
                },
                {
                  "planned_T_completion": 200000,
                  "trigger_processed": 670030,
                  "E_completion_convention": 3.7500937523438087
                }
              ],
              "schedule_updates": 208,
              "planned_epochs": 6
            },
            "U200_s36": {
              "U": 200,
              "data_seed": 36,
              "role": "confirmation",
              "n_examples": 592,
              "n_training_examples": 592,
              "pool_processed_tokens": 178194,
              "D_U_completion": 53411,
              "completion_processed_ratio": 0.2997351201499489,
              "domain_counts": {
                "code": 198,
                "qa": 194,
                "math": 200
              },
              "id_set_sha256": "a7448d221b5d68cf287b65959825d9f2d8d7d0cf93ad787d8bffd2cdff16771e",
              "data_pool_sha256": "c5eca315c67c25841f15d7ca701c7b12a81d28c2b2635b3864c8b748b2cda0b1",
              "source_counts": {
                "math": {
                  "source_rows": 200,
                  "training_rows": 200,
                  "coverage_deleted_rows": 0
                },
                "qa": {
                  "source_rows": 200,
                  "training_rows": 194,
                  "coverage_deleted_rows": 6
                },
                "code": {
                  "source_rows": 200,
                  "training_rows": 198,
                  "coverage_deleted_rows": 2
                }
              },
              "planned_milestones": [
                {
                  "planned_T_completion": 50000,
                  "trigger_processed": 166814,
                  "E_completion_convention": 0.9361367508565651
                },
                {
                  "planned_T_completion": 100000,
                  "trigger_processed": 333628,
                  "E_completion_convention": 1.8722735017131302
                },
                {
                  "planned_T_completion": 200000,
                  "trigger_processed": 667256,
                  "E_completion_convention": 3.7445470034262605
                }
              ],
              "schedule_updates": 208,
              "planned_epochs": 6
            }
          },
          [
            50000,
            100000,
            200000
          ]
        ]
      }
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/confirmation_register/unused_U_assertion",
      "results/v70-distill-confirm/freeze.json#/frozen_at_utc",
      "results/v47-p2-register/register.json#/v5_confirm/registered_at_utc"
    ],
    "note": "",
    "compact_scores": "",
    "rendered": "Gemma 270 million distilled on six new pools at 50 to 200 thousand tokens"
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 3,
    "column": 1,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/selected/math/method",
          "results/v70-distill-confirm/freeze.json#/selected/math/n_params",
          "results/v70-distill-confirm/freeze.json#/selected/code/method",
          "results/v70-distill-confirm/freeze.json#/selected/code/n_params",
          "results/v70-distill-confirm/freeze.json#/selected/qa/method",
          "results/v70-distill-confirm/freeze.json#/selected/qa/n_params"
        ],
        "op": "label",
        "format": null,
        "label": "Reuse forms, with a budget and pool form for question answering",
        "expected": [
          "E",
          1,
          "E",
          1,
          "joint",
          3
        ]
      }
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/selected",
      "results/v70-distill-confirm/freeze.json#/models"
    ],
    "note": "The frozen and delivered forms are identical: one-coefficient zero-anchored reuse for Math/Code, joint budget/pool for QA; fixed before test.",
    "compact_scores": "",
    "rendered": "Reuse forms, with a budget and pool form for question answering"
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 3,
    "column": 2,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/0/candidate_mae"
        ],
        "op": "identity",
        "format": ".3f"
      },
      "\n",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/1/candidate_mae"
        ],
        "op": "identity",
        "format": ".3f"
      },
      "\n",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/2/candidate_mae"
        ],
        "op": "identity",
        "format": ".3f"
      }
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/confirmation_register/students",
      "results/v70-distill-confirm/freeze.json#/bootstrap"
    ],
    "note": "Scores of one student, 270M; no student averaging. Stored paired baseline-minus-candidate intervals do not fit beside these scores and remain in the frozen record.",
    "compact_scores": "ordered",
    "rendered": "\\TableOneErrors{0.074}{0.019}{0.515}"
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 3,
    "column": 3,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/selected/math/method",
          "results/v70-distill-confirm/freeze.json#/selected/math/n_params",
          "results/v70-distill-confirm/freeze.json#/selected/code/method",
          "results/v70-distill-confirm/freeze.json#/selected/code/n_params",
          "results/v70-distill-confirm/freeze.json#/selected/qa/method",
          "results/v70-distill-confirm/freeze.json#/selected/qa/n_params"
        ],
        "op": "label",
        "format": null,
        "label": "The same predictor",
        "expected": [
          "E",
          1,
          "E",
          1,
          "joint",
          3
        ]
      }
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/selected",
      "results/v70-distill-confirm/freeze.json#/models"
    ],
    "note": "The frozen and delivered forms are identical: one-coefficient zero-anchored reuse for Math/Code, joint budget/pool for QA; fixed before test.",
    "compact_scores": "",
    "rendered": "The same predictor"
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 4,
    "column": 0,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/confirmation_register/students/1",
          "results/v70-distill-confirm/freeze.json#/confirmation_register/pools",
          "results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned"
        ],
        "op": "label",
        "format": null,
        "label": "Gemma 1 billion distilled on six new pools at 50 to 200 thousand tokens",
        "expected": [
          "gemma3-1b",
          {
            "U200_s31": {
              "U": 200,
              "data_seed": 31,
              "role": "confirmation",
              "n_examples": 597,
              "n_training_examples": 597,
              "pool_processed_tokens": 179688,
              "D_U_completion": 52958,
              "completion_processed_ratio": 0.2947219625128,
              "domain_counts": {
                "code": 198,
                "qa": 199,
                "math": 200
              },
              "id_set_sha256": "248cea90980ec9e921a9d8b2869cfbd558ab6910ba5509996f56d1486d5100a7",
              "data_pool_sha256": "111a5a9e84816cb050c3f7ce921eda2d06cc2581bb22075e1a486714e7801a8e",
              "source_counts": {
                "math": {
                  "source_rows": 200,
                  "training_rows": 200,
                  "coverage_deleted_rows": 0
                },
                "qa": {
                  "source_rows": 200,
                  "training_rows": 199,
                  "coverage_deleted_rows": 1
                },
                "code": {
                  "source_rows": 200,
                  "training_rows": 198,
                  "coverage_deleted_rows": 2
                }
              },
              "planned_milestones": [
                {
                  "planned_T_completion": 50000,
                  "trigger_processed": 169652,
                  "E_completion_convention": 0.9441444163299219
                },
                {
                  "planned_T_completion": 100000,
                  "trigger_processed": 339303,
                  "E_completion_convention": 1.8882888326598437
                },
                {
                  "planned_T_completion": 200000,
                  "trigger_processed": 678606,
                  "E_completion_convention": 3.7765776653196874
                }
              ],
              "schedule_updates": 212,
              "planned_epochs": 6
            },
            "U200_s32": {
              "U": 200,
              "data_seed": 32,
              "role": "confirmation",
              "n_examples": 594,
              "n_training_examples": 594,
              "pool_processed_tokens": 176885,
              "D_U_completion": 52964,
              "completion_processed_ratio": 0.299426180851966,
              "domain_counts": {
                "code": 199,
                "math": 200,
                "qa": 195
              },
              "id_set_sha256": "d7361b13114591e3e246acc73ac57650c5694929659ca7c898a88955c99327bc",
              "data_pool_sha256": "babaee54e739cf5878333cad113ce15a3ddb331f6f133f1a360ae1d22d8e94e3",
              "source_counts": {
                "math": {
                  "source_rows": 200,
                  "training_rows": 200,
                  "coverage_deleted_rows": 0
                },
                "qa": {
                  "source_rows": 200,
                  "training_rows": 195,
                  "coverage_deleted_rows": 5
                },
                "code": {
                  "source_rows": 200,
                  "training_rows": 199,
                  "coverage_deleted_rows": 1
                }
              },
              "planned_milestones": [
                {
                  "planned_T_completion": 50000,
                  "trigger_processed": 166987,
                  "E_completion_convention": 0.9440374594063893
                },
                {
                  "planned_T_completion": 100000,
                  "trigger_processed": 333973,
                  "E_completion_convention": 1.8880749188127786
                },
                {
                  "planned_T_completion": 200000,
                  "trigger_processed": 667945,
                  "E_completion_convention": 3.776149837625557
                }
              ],
              "schedule_updates": 215,
              "planned_epochs": 6
            },
            "U200_s33": {
              "U": 200,
              "data_seed": 33,
              "role": "confirmation",
              "n_examples": 595,
              "n_training_examples": 595,
              "pool_processed_tokens": 176898,
              "D_U_completion": 51800,
              "completion_processed_ratio": 0.292824113330846,
              "domain_counts": {
                "code": 198,
                "math": 200,
                "qa": 197
              },
              "id_set_sha256": "0f2c000781217cd4e671ab4f776cdf4d24405c23ed5c4d080e7c2e158aa38add",
              "data_pool_sha256": "9080a1f0baed5031f2095ff583da9fe720bd341ff79874c51576c266f99cceb0",
              "source_counts": {
                "math": {
                  "source_rows": 200,
                  "training_rows": 200,
                  "coverage_deleted_rows": 0
                },
                "qa": {
                  "source_rows": 200,
                  "training_rows": 197,
                  "coverage_deleted_rows": 3
                },
                "code": {
                  "source_rows": 200,
                  "training_rows": 198,
                  "coverage_deleted_rows": 2
                }
              },
              "planned_milestones": [
                {
                  "planned_T_completion": 50000,
                  "trigger_processed": 170751,
                  "E_completion_convention": 0.9652509652509652
                },
                {
                  "planned_T_completion": 100000,
                  "trigger_processed": 341502,
                  "E_completion_convention": 1.9305019305019304
                },
                {
                  "planned_T_completion": 200000,
                  "trigger_processed": 683004,
                  "E_completion_convention": 3.861003861003861
                }
              ],
              "schedule_updates": 215,
              "planned_epochs": 6
            },
            "U200_s34": {
              "U": 200,
              "data_seed": 34,
              "role": "confirmation",
              "n_examples": 592,
              "n_training_examples": 592,
              "pool_processed_tokens": 178516,
              "D_U_completion": 53528,
              "completion_processed_ratio": 0.29984987340070357,
              "domain_counts": {
                "code": 195,
                "qa": 197,
                "math": 200
              },
              "id_set_sha256": "576e944e2480472b1f1a0676f7c4a16e79c4eb13ee608a33460bde406ece69ba",
              "data_pool_sha256": "d19eb5f62d1f8015b7811f2e52f24efcfb597f41ca00c3cdad1f914ec96050ac",
              "source_counts": {
                "math": {
                  "source_rows": 200,
                  "training_rows": 200,
                  "coverage_deleted_rows": 0
                },
                "qa": {
                  "source_rows": 200,
                  "training_rows": 197,
                  "coverage_deleted_rows": 3
                },
                "code": {
                  "source_rows": 200,
                  "training_rows": 195,
                  "coverage_deleted_rows": 5
                }
              },
              "planned_milestones": [
                {
                  "planned_T_completion": 50000,
                  "trigger_processed": 166751,
                  "E_completion_convention": 0.9340905694216112
                },
                {
                  "planned_T_completion": 100000,
                  "trigger_processed": 333501,
                  "E_completion_convention": 1.8681811388432223
                },
                {
                  "planned_T_completion": 200000,
                  "trigger_processed": 667001,
                  "E_completion_convention": 3.7363622776864447
                }
              ],
              "schedule_updates": 208,
              "planned_epochs": 6
            },
            "U200_s35": {
              "U": 200,
              "data_seed": 35,
              "role": "confirmation",
              "n_examples": 592,
              "n_training_examples": 592,
              "pool_processed_tokens": 178670,
              "D_U_completion": 53332,
              "completion_processed_ratio": 0.2984944310740471,
              "domain_counts": {
                "code": 195,
                "qa": 197,
                "math": 200
              },
              "id_set_sha256": "193e60a043f4a126fe14b75a2aae18b07e919a3e89cba039fb1ad03c6a18db7d",
              "data_pool_sha256": "01742c467573d627517885096f6a984e76f97d76e66460d6874fd2c96154f801",
              "source_counts": {
                "math": {
                  "source_rows": 200,
                  "training_rows": 200,
                  "coverage_deleted_rows": 0
                },
                "qa": {
                  "source_rows": 200,
                  "training_rows": 197,
                  "coverage_deleted_rows": 3
                },
                "code": {
                  "source_rows": 200,
                  "training_rows": 195,
                  "coverage_deleted_rows": 5
                }
              },
              "planned_milestones": [
                {
                  "planned_T_completion": 50000,
                  "trigger_processed": 167508,
                  "E_completion_convention": 0.9375234380859522
                },
                {
                  "planned_T_completion": 100000,
                  "trigger_processed": 335015,
                  "E_completion_convention": 1.8750468761719044
                },
                {
                  "planned_T_completion": 200000,
                  "trigger_processed": 670030,
                  "E_completion_convention": 3.7500937523438087
                }
              ],
              "schedule_updates": 208,
              "planned_epochs": 6
            },
            "U200_s36": {
              "U": 200,
              "data_seed": 36,
              "role": "confirmation",
              "n_examples": 592,
              "n_training_examples": 592,
              "pool_processed_tokens": 178194,
              "D_U_completion": 53411,
              "completion_processed_ratio": 0.2997351201499489,
              "domain_counts": {
                "code": 198,
                "qa": 194,
                "math": 200
              },
              "id_set_sha256": "a7448d221b5d68cf287b65959825d9f2d8d7d0cf93ad787d8bffd2cdff16771e",
              "data_pool_sha256": "c5eca315c67c25841f15d7ca701c7b12a81d28c2b2635b3864c8b748b2cda0b1",
              "source_counts": {
                "math": {
                  "source_rows": 200,
                  "training_rows": 200,
                  "coverage_deleted_rows": 0
                },
                "qa": {
                  "source_rows": 200,
                  "training_rows": 194,
                  "coverage_deleted_rows": 6
                },
                "code": {
                  "source_rows": 200,
                  "training_rows": 198,
                  "coverage_deleted_rows": 2
                }
              },
              "planned_milestones": [
                {
                  "planned_T_completion": 50000,
                  "trigger_processed": 166814,
                  "E_completion_convention": 0.9361367508565651
                },
                {
                  "planned_T_completion": 100000,
                  "trigger_processed": 333628,
                  "E_completion_convention": 1.8722735017131302
                },
                {
                  "planned_T_completion": 200000,
                  "trigger_processed": 667256,
                  "E_completion_convention": 3.7445470034262605
                }
              ],
              "schedule_updates": 208,
              "planned_epochs": 6
            }
          },
          [
            50000,
            100000,
            200000
          ]
        ]
      }
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/confirmation_register/unused_U_assertion",
      "results/v70-distill-confirm/freeze.json#/frozen_at_utc",
      "results/v47-p2-register/register.json#/v5_confirm/registered_at_utc"
    ],
    "note": "",
    "compact_scores": "",
    "rendered": "Gemma 1 billion distilled on six new pools at 50 to 200 thousand tokens"
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 4,
    "column": 1,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/selected/math/method",
          "results/v70-distill-confirm/freeze.json#/selected/math/n_params",
          "results/v70-distill-confirm/freeze.json#/selected/code/method",
          "results/v70-distill-confirm/freeze.json#/selected/code/n_params",
          "results/v70-distill-confirm/freeze.json#/selected/qa/method",
          "results/v70-distill-confirm/freeze.json#/selected/qa/n_params"
        ],
        "op": "label",
        "format": null,
        "label": "Reuse forms, with a budget and pool form for question answering",
        "expected": [
          "E",
          1,
          "E",
          1,
          "joint",
          3
        ]
      }
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/selected",
      "results/v70-distill-confirm/freeze.json#/models"
    ],
    "note": "The frozen and delivered forms are identical: one-coefficient zero-anchored reuse for Math/Code, joint budget/pool for QA; fixed before test.",
    "compact_scores": "",
    "rendered": "Reuse forms, with a budget and pool form for question answering"
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 4,
    "column": 2,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/3/candidate_mae"
        ],
        "op": "identity",
        "format": ".3f"
      },
      "\n",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/4/candidate_mae"
        ],
        "op": "identity",
        "format": ".3f"
      },
      "\n",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/5/candidate_mae"
        ],
        "op": "identity",
        "format": ".3f"
      }
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/confirmation_register/students",
      "results/v70-distill-confirm/freeze.json#/bootstrap"
    ],
    "note": "Scores of one student, 1B; no student averaging. Stored paired baseline-minus-candidate intervals do not fit beside these scores and remain in the frozen record.",
    "compact_scores": "ordered",
    "rendered": "\\TableOneErrors{0.057}{0.049}{0.463}"
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 4,
    "column": 3,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/selected/math/method",
          "results/v70-distill-confirm/freeze.json#/selected/math/n_params",
          "results/v70-distill-confirm/freeze.json#/selected/code/method",
          "results/v70-distill-confirm/freeze.json#/selected/code/n_params",
          "results/v70-distill-confirm/freeze.json#/selected/qa/method",
          "results/v70-distill-confirm/freeze.json#/selected/qa/n_params"
        ],
        "op": "label",
        "format": null,
        "label": "The same predictor",
        "expected": [
          "E",
          1,
          "E",
          1,
          "joint",
          3
        ]
      }
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/selected",
      "results/v70-distill-confirm/freeze.json#/models"
    ],
    "note": "The frozen and delivered forms are identical: one-coefficient zero-anchored reuse for Math/Code, joint budget/pool for QA; fixed before test.",
    "compact_scores": "",
    "rendered": "The same predictor"
  }
]
```

## Candidates table caption recipe

```json
{
  "table": "tab:main-prediction-candidates",
  "parts": [
    "Pre-specified candidate of each prediction task in Table~\\ref{tab:main-prediction-v2}, its error on the same cells, and the relation delivered after the test. Errors are mean absolute errors in nats per token, in math, code and question answering order; the two distillation rows are the ",
    {
      "sources": [
        "results/v70-distill-confirm/freeze.json#/confirmation_register/students"
      ],
      "op": "label",
      "format": null,
      "label": "270 million and 1 billion",
      "expected": [
        [
          "gemma3-270m",
          "gemma3-1b"
        ]
      ]
    },
    " students."
  ],
  "context": [
    "results/v53-prune-dev/register.json#/feature_names",
    "results/v55-quant-group/register.json#/feature_names",
    "results/v70-distill-confirm/freeze.json#/reference_rule",
    "results/v53-prune-dev/register.json#/candidate_definitions/power",
    "results/v55-quant-group/register.json#/candidate_definitions/low_order_2d",
    "results/v70-distill-confirm/freeze.json#/models"
  ],
  "note": "",
  "compact_scores": "",
  "rendered": "Pre-specified candidate of each prediction task in Table~\\ref{tab:main-prediction-v2}, its error on the same cells, and the relation delivered after the test. Errors are mean absolute errors in nats per token, in math, code and question answering order; the two distillation rows are the 270 million and 1 billion students."
}
```

## Every printed number

- tab:main-prediction-v2: Cell (0, 0), `Three` (label): `results/v53-prune-dev/compare_pythia-410m@step48000.json#/tag`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/densities`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/tag`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/densities`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/tag`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/densities`
- tab:main-prediction-v2: Cell (0, 0), `0.575` (label): `results/v53-prune-dev/compare_pythia-410m@step48000.json#/tag`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/densities`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/tag`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/densities`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/tag`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/densities`
- tab:main-prediction-v2: Cell (0, 0), `0.675` (label): `results/v53-prune-dev/compare_pythia-410m@step48000.json#/tag`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/densities`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/tag`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/densities`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/tag`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/densities`
- tab:main-prediction-v2: Cell (0, 0), `0.85` (label): `results/v53-prune-dev/compare_pythia-410m@step48000.json#/tag`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/densities`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/tag`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/densities`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/tag`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/densities`
- tab:main-prediction-v2: Cell (0, 0), `84` (per_capability): `results/v53-prune-dev/register.json#/n_dev_rows`; `results/v53-prune-dev/register.json#/models`
- tab:main-prediction-v2: Cell (1, 2), `0.277` (mean): `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/math`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/math`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/math`
- tab:main-prediction-v2: Cell (1, 4), `0.230` (mean): `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/A2/math`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/A2/math`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/A2/math`
- tab:main-prediction-v2: Cell (1, 5), `-0.047` (difference): `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/math`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/math`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/math`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/A2/math`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/A2/math`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/A2/math`
- tab:main-prediction-v2: Cell (2, 2), `0.214` (mean): `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/code`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/code`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/code`
- tab:main-prediction-v2: Cell (2, 4), `0.222` (mean): `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/A2/code`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/A2/code`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/A2/code`
- tab:main-prediction-v2: Cell (2, 5), `+0.008` (difference): `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/code`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/code`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/code`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/A2/code`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/A2/code`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/A2/code`
- tab:main-prediction-v2: Cell (3, 2), `0.221` (mean): `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/qa`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/qa`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/qa`
- tab:main-prediction-v2: Cell (3, 4), `0.221` (mean): `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/qa`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/qa`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/qa`
- tab:main-prediction-v2: Cell (3, 5), `+0.000` (difference): `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/qa`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/qa`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/qa`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/qa`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/qa`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/qa`
- tab:main-prediction-v2: Cell (4, 0), `410` (label): `results/v69-quant-confirm/compare.json#/rows/0/state`; `results/v69-quant-confirm/compare.json#/rows/0/config`; `results/v69-quant-confirm/compare.json#/rows/3/config`; `results/v69-quant-confirm/compare.json#/rows/6/config`; `results/v69-quant-confirm/compare.json#/rows/9/config`; `results/v69-quant-confirm/compare.json#/rows/12/config`; `results/v69-quant-confirm/compare.json#/rows/15/config`; `results/v69-quant-confirm/compare.json#/rows/18/state`
- tab:main-prediction-v2: Cell (4, 0), `1.4` (label): `results/v69-quant-confirm/compare.json#/rows/0/state`; `results/v69-quant-confirm/compare.json#/rows/0/config`; `results/v69-quant-confirm/compare.json#/rows/3/config`; `results/v69-quant-confirm/compare.json#/rows/6/config`; `results/v69-quant-confirm/compare.json#/rows/9/config`; `results/v69-quant-confirm/compare.json#/rows/12/config`; `results/v69-quant-confirm/compare.json#/rows/15/config`; `results/v69-quant-confirm/compare.json#/rows/18/state`
- tab:main-prediction-v2: Cell (4, 0), `32` (label): `results/v69-quant-confirm/compare.json#/rows/0/state`; `results/v69-quant-confirm/compare.json#/rows/0/config`; `results/v69-quant-confirm/compare.json#/rows/3/config`; `results/v69-quant-confirm/compare.json#/rows/6/config`; `results/v69-quant-confirm/compare.json#/rows/9/config`; `results/v69-quant-confirm/compare.json#/rows/12/config`; `results/v69-quant-confirm/compare.json#/rows/15/config`; `results/v69-quant-confirm/compare.json#/rows/18/state`
- tab:main-prediction-v2: Cell (4, 0), `512` (label): `results/v69-quant-confirm/compare.json#/rows/0/state`; `results/v69-quant-confirm/compare.json#/rows/0/config`; `results/v69-quant-confirm/compare.json#/rows/3/config`; `results/v69-quant-confirm/compare.json#/rows/6/config`; `results/v69-quant-confirm/compare.json#/rows/9/config`; `results/v69-quant-confirm/compare.json#/rows/12/config`; `results/v69-quant-confirm/compare.json#/rows/15/config`; `results/v69-quant-confirm/compare.json#/rows/18/state`
- tab:main-prediction-v2: Cell (4, 0), `3` (label): `results/v69-quant-confirm/compare.json#/rows/0/state`; `results/v69-quant-confirm/compare.json#/rows/0/config`; `results/v69-quant-confirm/compare.json#/rows/3/config`; `results/v69-quant-confirm/compare.json#/rows/6/config`; `results/v69-quant-confirm/compare.json#/rows/9/config`; `results/v69-quant-confirm/compare.json#/rows/12/config`; `results/v69-quant-confirm/compare.json#/rows/15/config`; `results/v69-quant-confirm/compare.json#/rows/18/state`
- tab:main-prediction-v2: Cell (4, 0), `5` (label): `results/v69-quant-confirm/compare.json#/rows/0/state`; `results/v69-quant-confirm/compare.json#/rows/0/config`; `results/v69-quant-confirm/compare.json#/rows/3/config`; `results/v69-quant-confirm/compare.json#/rows/6/config`; `results/v69-quant-confirm/compare.json#/rows/9/config`; `results/v69-quant-confirm/compare.json#/rows/12/config`; `results/v69-quant-confirm/compare.json#/rows/15/config`; `results/v69-quant-confirm/compare.json#/rows/18/state`
- tab:main-prediction-v2: Cell (4, 0), `54` (identity): `results/v69-quant-confirm/develop.json#/n_dev_cells`
- tab:main-prediction-v2: Cell (5, 2), `0.065` (identity): `results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/same_input_interpolation/math/mae`
- tab:main-prediction-v2: Cell (5, 4), `0.333` (identity): `results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/bilinear/math/mae`
- tab:main-prediction-v2: Cell (5, 5), `+0.268` (difference): `results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/same_input_interpolation/math/mae`; `results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/bilinear/math/mae`
- tab:main-prediction-v2: Cell (6, 2), `0.116` (identity): `results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/same_input_interpolation/code/mae`
- tab:main-prediction-v2: Cell (6, 4), `0.678` (identity): `results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/zero/code/mae`
- tab:main-prediction-v2: Cell (6, 5), `+0.562` (difference): `results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/same_input_interpolation/code/mae`; `results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/zero/code/mae`
- tab:main-prediction-v2: Cell (7, 2), `0.458` (identity): `results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/median/qa/mae`
- tab:main-prediction-v2: Cell (7, 4), `0.458` (identity): `results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/median/qa/mae`
- tab:main-prediction-v2: Cell (7, 5), `+0.000` (difference): `results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/median/qa/mae`; `results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/median/qa/mae`
- tab:main-prediction-v2: Cell (8, 0), `1.4` (label): `results/v69-quant-confirm/compare.json#/rows/36/state`; `results/v69-quant-confirm/compare.json#/rows/36/config`; `results/v69-quant-confirm/compare.json#/rows/39/config`; `results/v69-quant-confirm/compare.json#/rows/42/config`; `results/v69-quant-confirm/compare.json#/rows/45/config`; `results/v69-quant-confirm/compare.json#/rows/48/config`; `results/v69-quant-confirm/compare.json#/rows/51/config`; `results/v69-quant-confirm/compare.json#/rows/54/config`; `results/v69-quant-confirm/compare.json#/rows/57/config`; `results/v69-quant-confirm/compare.json#/rows/60/config`
- tab:main-prediction-v2: Cell (8, 0), `3` (label): `results/v69-quant-confirm/compare.json#/rows/36/state`; `results/v69-quant-confirm/compare.json#/rows/36/config`; `results/v69-quant-confirm/compare.json#/rows/39/config`; `results/v69-quant-confirm/compare.json#/rows/42/config`; `results/v69-quant-confirm/compare.json#/rows/45/config`; `results/v69-quant-confirm/compare.json#/rows/48/config`; `results/v69-quant-confirm/compare.json#/rows/51/config`; `results/v69-quant-confirm/compare.json#/rows/54/config`; `results/v69-quant-confirm/compare.json#/rows/57/config`; `results/v69-quant-confirm/compare.json#/rows/60/config`
- tab:main-prediction-v2: Cell (8, 0), `5` (label): `results/v69-quant-confirm/compare.json#/rows/36/state`; `results/v69-quant-confirm/compare.json#/rows/36/config`; `results/v69-quant-confirm/compare.json#/rows/39/config`; `results/v69-quant-confirm/compare.json#/rows/42/config`; `results/v69-quant-confirm/compare.json#/rows/45/config`; `results/v69-quant-confirm/compare.json#/rows/48/config`; `results/v69-quant-confirm/compare.json#/rows/51/config`; `results/v69-quant-confirm/compare.json#/rows/54/config`; `results/v69-quant-confirm/compare.json#/rows/57/config`; `results/v69-quant-confirm/compare.json#/rows/60/config`
- tab:main-prediction-v2: Cell (8, 0), `32` (label): `results/v69-quant-confirm/compare.json#/rows/36/state`; `results/v69-quant-confirm/compare.json#/rows/36/config`; `results/v69-quant-confirm/compare.json#/rows/39/config`; `results/v69-quant-confirm/compare.json#/rows/42/config`; `results/v69-quant-confirm/compare.json#/rows/45/config`; `results/v69-quant-confirm/compare.json#/rows/48/config`; `results/v69-quant-confirm/compare.json#/rows/51/config`; `results/v69-quant-confirm/compare.json#/rows/54/config`; `results/v69-quant-confirm/compare.json#/rows/57/config`; `results/v69-quant-confirm/compare.json#/rows/60/config`
- tab:main-prediction-v2: Cell (8, 0), `512` (label): `results/v69-quant-confirm/compare.json#/rows/36/state`; `results/v69-quant-confirm/compare.json#/rows/36/config`; `results/v69-quant-confirm/compare.json#/rows/39/config`; `results/v69-quant-confirm/compare.json#/rows/42/config`; `results/v69-quant-confirm/compare.json#/rows/45/config`; `results/v69-quant-confirm/compare.json#/rows/48/config`; `results/v69-quant-confirm/compare.json#/rows/51/config`; `results/v69-quant-confirm/compare.json#/rows/54/config`; `results/v69-quant-confirm/compare.json#/rows/57/config`; `results/v69-quant-confirm/compare.json#/rows/60/config`
- tab:main-prediction-v2: Cell (8, 0), `54` (identity): `results/v69-quant-confirm/develop.json#/n_dev_cells`
- tab:main-prediction-v2: Cell (9, 2), `0.088` (weighted_mean): `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/math/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/math/n`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/math/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/math/n`
- tab:main-prediction-v2: Cell (9, 4), `0.350` (weighted_mean): `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/bilinear/math/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/bilinear/math/n`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/bilinear/math/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/bilinear/math/n`
- tab:main-prediction-v2: Cell (9, 5), `+0.262` (difference): `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/math/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/math/n`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/math/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/math/n`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/bilinear/math/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/bilinear/math/n`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/bilinear/math/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/bilinear/math/n`
- tab:main-prediction-v2: Cell (10, 2), `0.153` (weighted_mean): `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/code/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/code/n`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/code/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/code/n`
- tab:main-prediction-v2: Cell (10, 4), `0.563` (weighted_mean): `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/zero/code/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/zero/code/n`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/zero/code/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/zero/code/n`
- tab:main-prediction-v2: Cell (10, 5), `+0.410` (difference): `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/code/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/code/n`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/code/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/code/n`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/zero/code/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/zero/code/n`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/zero/code/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/zero/code/n`
- tab:main-prediction-v2: Cell (11, 2), `0.141` (weighted_mean): `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/n`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/n`
- tab:main-prediction-v2: Cell (11, 4), `0.141` (weighted_mean): `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/n`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/n`
- tab:main-prediction-v2: Cell (11, 5), `+0.000` (difference): `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/n`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/n`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/n`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/n`
- tab:main-prediction-v2: Cell (12, 0), `270` (label): `results/v70-distill-confirm/freeze.json#/confirmation_register/students/0`; `results/v70-distill-confirm/freeze.json#/confirmation_register/pools`; `results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned`
- tab:main-prediction-v2: Cell (12, 0), `six` (label): `results/v70-distill-confirm/freeze.json#/confirmation_register/students/0`; `results/v70-distill-confirm/freeze.json#/confirmation_register/pools`; `results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned`
- tab:main-prediction-v2: Cell (12, 0), `50` (label): `results/v70-distill-confirm/freeze.json#/confirmation_register/students/0`; `results/v70-distill-confirm/freeze.json#/confirmation_register/pools`; `results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned`
- tab:main-prediction-v2: Cell (12, 0), `200` (label): `results/v70-distill-confirm/freeze.json#/confirmation_register/students/0`; `results/v70-distill-confirm/freeze.json#/confirmation_register/pools`; `results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned`
- tab:main-prediction-v2: Cell (12, 0), `100` (identity): `results/v70-distill-confirm/develop.json#/development_structure/n_points`
- tab:main-prediction-v2: Cell (13, 2), `0.074` (identity): `results/v70-distill-confirm/compare.json#/groups/0/candidate_mae`
- tab:main-prediction-v2: Cell (13, 4), `0.065` (identity): `results/v70-distill-confirm/compare.json#/groups/0/baseline_mae`
- tab:main-prediction-v2: Cell (13, 5), `-0.009` (difference): `results/v70-distill-confirm/compare.json#/groups/0/candidate_mae`; `results/v70-distill-confirm/compare.json#/groups/0/baseline_mae`
- tab:main-prediction-v2: Cell (14, 2), `0.019` (identity): `results/v70-distill-confirm/compare.json#/groups/1/candidate_mae`
- tab:main-prediction-v2: Cell (14, 4), `0.023` (identity): `results/v70-distill-confirm/compare.json#/groups/1/baseline_mae`
- tab:main-prediction-v2: Cell (14, 5), `+0.004` (difference): `results/v70-distill-confirm/compare.json#/groups/1/candidate_mae`; `results/v70-distill-confirm/compare.json#/groups/1/baseline_mae`
- tab:main-prediction-v2: Cell (15, 2), `0.515` (identity): `results/v70-distill-confirm/compare.json#/groups/2/candidate_mae`
- tab:main-prediction-v2: Cell (15, 4), `0.610` (identity): `results/v70-distill-confirm/compare.json#/groups/2/baseline_mae`
- tab:main-prediction-v2: Cell (15, 5), `+0.095` (difference): `results/v70-distill-confirm/compare.json#/groups/2/candidate_mae`; `results/v70-distill-confirm/compare.json#/groups/2/baseline_mae`
- tab:main-prediction-v2: Cell (16, 0), `1` (label): `results/v70-distill-confirm/freeze.json#/confirmation_register/students/1`; `results/v70-distill-confirm/freeze.json#/confirmation_register/pools`; `results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned`
- tab:main-prediction-v2: Cell (16, 0), `six` (label): `results/v70-distill-confirm/freeze.json#/confirmation_register/students/1`; `results/v70-distill-confirm/freeze.json#/confirmation_register/pools`; `results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned`
- tab:main-prediction-v2: Cell (16, 0), `50` (label): `results/v70-distill-confirm/freeze.json#/confirmation_register/students/1`; `results/v70-distill-confirm/freeze.json#/confirmation_register/pools`; `results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned`
- tab:main-prediction-v2: Cell (16, 0), `200` (label): `results/v70-distill-confirm/freeze.json#/confirmation_register/students/1`; `results/v70-distill-confirm/freeze.json#/confirmation_register/pools`; `results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned`
- tab:main-prediction-v2: Cell (16, 0), `100` (identity): `results/v70-distill-confirm/develop.json#/development_structure/n_points`
- tab:main-prediction-v2: Cell (17, 2), `0.057` (identity): `results/v70-distill-confirm/compare.json#/groups/3/candidate_mae`
- tab:main-prediction-v2: Cell (17, 4), `0.033` (identity): `results/v70-distill-confirm/compare.json#/groups/3/baseline_mae`
- tab:main-prediction-v2: Cell (17, 5), `-0.023` (difference): `results/v70-distill-confirm/compare.json#/groups/3/candidate_mae`; `results/v70-distill-confirm/compare.json#/groups/3/baseline_mae`
- tab:main-prediction-v2: Cell (18, 2), `0.049` (identity): `results/v70-distill-confirm/compare.json#/groups/4/candidate_mae`
- tab:main-prediction-v2: Cell (18, 4), `0.053` (identity): `results/v70-distill-confirm/compare.json#/groups/4/baseline_mae`
- tab:main-prediction-v2: Cell (18, 5), `+0.005` (difference): `results/v70-distill-confirm/compare.json#/groups/4/candidate_mae`; `results/v70-distill-confirm/compare.json#/groups/4/baseline_mae`
- tab:main-prediction-v2: Cell (19, 2), `0.463` (identity): `results/v70-distill-confirm/compare.json#/groups/5/candidate_mae`
- tab:main-prediction-v2: Cell (19, 4), `0.450` (identity): `results/v70-distill-confirm/compare.json#/groups/5/baseline_mae`
- tab:main-prediction-v2: Cell (19, 5), `-0.013` (difference): `results/v70-distill-confirm/compare.json#/groups/5/candidate_mae`; `results/v70-distill-confirm/compare.json#/groups/5/baseline_mae`
- tab:main-prediction-v2: Caption, `270` (label): `results/v70-distill-confirm/freeze.json#/confirmation_register/students`
- tab:main-prediction-v2: Caption, `1` (label): `results/v70-distill-confirm/freeze.json#/confirmation_register/students`
- tab:main-prediction-candidates: Cell (0, 0), `Three` (label): `results/v53-prune-dev/compare_pythia-410m@step48000.json#/tag`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/densities`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/tag`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/densities`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/tag`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/densities`
- tab:main-prediction-candidates: Cell (0, 0), `0.575` (label): `results/v53-prune-dev/compare_pythia-410m@step48000.json#/tag`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/densities`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/tag`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/densities`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/tag`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/densities`
- tab:main-prediction-candidates: Cell (0, 0), `0.675` (label): `results/v53-prune-dev/compare_pythia-410m@step48000.json#/tag`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/densities`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/tag`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/densities`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/tag`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/densities`
- tab:main-prediction-candidates: Cell (0, 0), `0.85` (label): `results/v53-prune-dev/compare_pythia-410m@step48000.json#/tag`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/densities`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/tag`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/densities`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/tag`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/densities`
- tab:main-prediction-candidates: Cell (0, 1), `Five` (label): `results/v53-prune-dev/register.json#/candidate_definitions/power`; `results/v53-prune-dev/register.json#/n_params_per_capability/power`; `results/v53-prune-dev/register.json#/n_dev_states`
- tab:main-prediction-candidates: Cell (0, 2), `0.243` (mean): `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/power/math`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/power/math`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/power/math`
- tab:main-prediction-candidates: Cell (0, 2), `0.236` (mean): `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/power/code`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/power/code`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/power/code`
- tab:main-prediction-candidates: Cell (0, 2), `0.678` (mean): `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/power/qa`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/power/qa`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/power/qa`
- tab:main-prediction-candidates: Cell (1, 0), `410` (label): `results/v69-quant-confirm/compare.json#/rows/0/state`; `results/v69-quant-confirm/compare.json#/rows/0/config`; `results/v69-quant-confirm/compare.json#/rows/3/config`; `results/v69-quant-confirm/compare.json#/rows/6/config`; `results/v69-quant-confirm/compare.json#/rows/9/config`; `results/v69-quant-confirm/compare.json#/rows/12/config`; `results/v69-quant-confirm/compare.json#/rows/15/config`; `results/v69-quant-confirm/compare.json#/rows/18/state`
- tab:main-prediction-candidates: Cell (1, 0), `1.4` (label): `results/v69-quant-confirm/compare.json#/rows/0/state`; `results/v69-quant-confirm/compare.json#/rows/0/config`; `results/v69-quant-confirm/compare.json#/rows/3/config`; `results/v69-quant-confirm/compare.json#/rows/6/config`; `results/v69-quant-confirm/compare.json#/rows/9/config`; `results/v69-quant-confirm/compare.json#/rows/12/config`; `results/v69-quant-confirm/compare.json#/rows/15/config`; `results/v69-quant-confirm/compare.json#/rows/18/state`
- tab:main-prediction-candidates: Cell (1, 0), `32` (label): `results/v69-quant-confirm/compare.json#/rows/0/state`; `results/v69-quant-confirm/compare.json#/rows/0/config`; `results/v69-quant-confirm/compare.json#/rows/3/config`; `results/v69-quant-confirm/compare.json#/rows/6/config`; `results/v69-quant-confirm/compare.json#/rows/9/config`; `results/v69-quant-confirm/compare.json#/rows/12/config`; `results/v69-quant-confirm/compare.json#/rows/15/config`; `results/v69-quant-confirm/compare.json#/rows/18/state`
- tab:main-prediction-candidates: Cell (1, 0), `512` (label): `results/v69-quant-confirm/compare.json#/rows/0/state`; `results/v69-quant-confirm/compare.json#/rows/0/config`; `results/v69-quant-confirm/compare.json#/rows/3/config`; `results/v69-quant-confirm/compare.json#/rows/6/config`; `results/v69-quant-confirm/compare.json#/rows/9/config`; `results/v69-quant-confirm/compare.json#/rows/12/config`; `results/v69-quant-confirm/compare.json#/rows/15/config`; `results/v69-quant-confirm/compare.json#/rows/18/state`
- tab:main-prediction-candidates: Cell (1, 0), `3` (label): `results/v69-quant-confirm/compare.json#/rows/0/state`; `results/v69-quant-confirm/compare.json#/rows/0/config`; `results/v69-quant-confirm/compare.json#/rows/3/config`; `results/v69-quant-confirm/compare.json#/rows/6/config`; `results/v69-quant-confirm/compare.json#/rows/9/config`; `results/v69-quant-confirm/compare.json#/rows/12/config`; `results/v69-quant-confirm/compare.json#/rows/15/config`; `results/v69-quant-confirm/compare.json#/rows/18/state`
- tab:main-prediction-candidates: Cell (1, 0), `5` (label): `results/v69-quant-confirm/compare.json#/rows/0/state`; `results/v69-quant-confirm/compare.json#/rows/0/config`; `results/v69-quant-confirm/compare.json#/rows/3/config`; `results/v69-quant-confirm/compare.json#/rows/6/config`; `results/v69-quant-confirm/compare.json#/rows/9/config`; `results/v69-quant-confirm/compare.json#/rows/12/config`; `results/v69-quant-confirm/compare.json#/rows/15/config`; `results/v69-quant-confirm/compare.json#/rows/18/state`
- tab:main-prediction-candidates: Cell (1, 2), `0.215` (identity): `results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/low_order_2d/math/mae`
- tab:main-prediction-candidates: Cell (1, 2), `0.557` (identity): `results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/median/code/mae`
- tab:main-prediction-candidates: Cell (1, 2), `0.457` (identity): `results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/zero/qa/mae`
- tab:main-prediction-candidates: Cell (2, 0), `1.4` (label): `results/v69-quant-confirm/compare.json#/rows/36/state`; `results/v69-quant-confirm/compare.json#/rows/36/config`; `results/v69-quant-confirm/compare.json#/rows/39/config`; `results/v69-quant-confirm/compare.json#/rows/42/config`; `results/v69-quant-confirm/compare.json#/rows/45/config`; `results/v69-quant-confirm/compare.json#/rows/48/config`; `results/v69-quant-confirm/compare.json#/rows/51/config`; `results/v69-quant-confirm/compare.json#/rows/54/config`; `results/v69-quant-confirm/compare.json#/rows/57/config`; `results/v69-quant-confirm/compare.json#/rows/60/config`
- tab:main-prediction-candidates: Cell (2, 0), `3` (label): `results/v69-quant-confirm/compare.json#/rows/36/state`; `results/v69-quant-confirm/compare.json#/rows/36/config`; `results/v69-quant-confirm/compare.json#/rows/39/config`; `results/v69-quant-confirm/compare.json#/rows/42/config`; `results/v69-quant-confirm/compare.json#/rows/45/config`; `results/v69-quant-confirm/compare.json#/rows/48/config`; `results/v69-quant-confirm/compare.json#/rows/51/config`; `results/v69-quant-confirm/compare.json#/rows/54/config`; `results/v69-quant-confirm/compare.json#/rows/57/config`; `results/v69-quant-confirm/compare.json#/rows/60/config`
- tab:main-prediction-candidates: Cell (2, 0), `5` (label): `results/v69-quant-confirm/compare.json#/rows/36/state`; `results/v69-quant-confirm/compare.json#/rows/36/config`; `results/v69-quant-confirm/compare.json#/rows/39/config`; `results/v69-quant-confirm/compare.json#/rows/42/config`; `results/v69-quant-confirm/compare.json#/rows/45/config`; `results/v69-quant-confirm/compare.json#/rows/48/config`; `results/v69-quant-confirm/compare.json#/rows/51/config`; `results/v69-quant-confirm/compare.json#/rows/54/config`; `results/v69-quant-confirm/compare.json#/rows/57/config`; `results/v69-quant-confirm/compare.json#/rows/60/config`
- tab:main-prediction-candidates: Cell (2, 0), `32` (label): `results/v69-quant-confirm/compare.json#/rows/36/state`; `results/v69-quant-confirm/compare.json#/rows/36/config`; `results/v69-quant-confirm/compare.json#/rows/39/config`; `results/v69-quant-confirm/compare.json#/rows/42/config`; `results/v69-quant-confirm/compare.json#/rows/45/config`; `results/v69-quant-confirm/compare.json#/rows/48/config`; `results/v69-quant-confirm/compare.json#/rows/51/config`; `results/v69-quant-confirm/compare.json#/rows/54/config`; `results/v69-quant-confirm/compare.json#/rows/57/config`; `results/v69-quant-confirm/compare.json#/rows/60/config`
- tab:main-prediction-candidates: Cell (2, 0), `512` (label): `results/v69-quant-confirm/compare.json#/rows/36/state`; `results/v69-quant-confirm/compare.json#/rows/36/config`; `results/v69-quant-confirm/compare.json#/rows/39/config`; `results/v69-quant-confirm/compare.json#/rows/42/config`; `results/v69-quant-confirm/compare.json#/rows/45/config`; `results/v69-quant-confirm/compare.json#/rows/48/config`; `results/v69-quant-confirm/compare.json#/rows/51/config`; `results/v69-quant-confirm/compare.json#/rows/54/config`; `results/v69-quant-confirm/compare.json#/rows/57/config`; `results/v69-quant-confirm/compare.json#/rows/60/config`
- tab:main-prediction-candidates: Cell (2, 2), `0.303` (weighted_mean): `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/low_order_2d/math/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/low_order_2d/math/n`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/low_order_2d/math/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/low_order_2d/math/n`
- tab:main-prediction-candidates: Cell (2, 2), `0.153` (weighted_mean): `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/code/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/code/n`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/code/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/code/n`
- tab:main-prediction-candidates: Cell (2, 2), `0.222` (weighted_mean): `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/zero/qa/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/zero/qa/n`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/zero/qa/mae`; `results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/zero/qa/n`
- tab:main-prediction-candidates: Cell (3, 0), `270` (label): `results/v70-distill-confirm/freeze.json#/confirmation_register/students/0`; `results/v70-distill-confirm/freeze.json#/confirmation_register/pools`; `results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned`
- tab:main-prediction-candidates: Cell (3, 0), `six` (label): `results/v70-distill-confirm/freeze.json#/confirmation_register/students/0`; `results/v70-distill-confirm/freeze.json#/confirmation_register/pools`; `results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned`
- tab:main-prediction-candidates: Cell (3, 0), `50` (label): `results/v70-distill-confirm/freeze.json#/confirmation_register/students/0`; `results/v70-distill-confirm/freeze.json#/confirmation_register/pools`; `results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned`
- tab:main-prediction-candidates: Cell (3, 0), `200` (label): `results/v70-distill-confirm/freeze.json#/confirmation_register/students/0`; `results/v70-distill-confirm/freeze.json#/confirmation_register/pools`; `results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned`
- tab:main-prediction-candidates: Cell (3, 2), `0.074` (identity): `results/v70-distill-confirm/compare.json#/groups/0/candidate_mae`
- tab:main-prediction-candidates: Cell (3, 2), `0.019` (identity): `results/v70-distill-confirm/compare.json#/groups/1/candidate_mae`
- tab:main-prediction-candidates: Cell (3, 2), `0.515` (identity): `results/v70-distill-confirm/compare.json#/groups/2/candidate_mae`
- tab:main-prediction-candidates: Cell (4, 0), `1` (label): `results/v70-distill-confirm/freeze.json#/confirmation_register/students/1`; `results/v70-distill-confirm/freeze.json#/confirmation_register/pools`; `results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned`
- tab:main-prediction-candidates: Cell (4, 0), `six` (label): `results/v70-distill-confirm/freeze.json#/confirmation_register/students/1`; `results/v70-distill-confirm/freeze.json#/confirmation_register/pools`; `results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned`
- tab:main-prediction-candidates: Cell (4, 0), `50` (label): `results/v70-distill-confirm/freeze.json#/confirmation_register/students/1`; `results/v70-distill-confirm/freeze.json#/confirmation_register/pools`; `results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned`
- tab:main-prediction-candidates: Cell (4, 0), `200` (label): `results/v70-distill-confirm/freeze.json#/confirmation_register/students/1`; `results/v70-distill-confirm/freeze.json#/confirmation_register/pools`; `results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned`
- tab:main-prediction-candidates: Cell (4, 2), `0.057` (identity): `results/v70-distill-confirm/compare.json#/groups/3/candidate_mae`
- tab:main-prediction-candidates: Cell (4, 2), `0.049` (identity): `results/v70-distill-confirm/compare.json#/groups/4/candidate_mae`
- tab:main-prediction-candidates: Cell (4, 2), `0.463` (identity): `results/v70-distill-confirm/compare.json#/groups/5/candidate_mae`
- tab:main-prediction-candidates: Caption, `270` (label): `results/v70-distill-confirm/freeze.json#/confirmation_register/students`
- tab:main-prediction-candidates: Caption, `1` (label): `results/v70-distill-confirm/freeze.json#/confirmation_register/students`

## Machine-readable numeric inventory

```json
[
  {
    "table": "tab:main-prediction-v2",
    "row": 0,
    "column": 0,
    "part": 0,
    "number": "Three",
    "displayed": "Three unseen checkpoints pruned to densities 0.575, 0.675 and 0.85",
    "op": "label",
    "sources": [
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/tag",
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/densities",
      "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/tag",
      "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/densities",
      "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/tag",
      "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/densities"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 0,
    "column": 0,
    "part": 0,
    "number": "0.575",
    "displayed": "Three unseen checkpoints pruned to densities 0.575, 0.675 and 0.85",
    "op": "label",
    "sources": [
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/tag",
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/densities",
      "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/tag",
      "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/densities",
      "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/tag",
      "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/densities"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 0,
    "column": 0,
    "part": 0,
    "number": "0.675",
    "displayed": "Three unseen checkpoints pruned to densities 0.575, 0.675 and 0.85",
    "op": "label",
    "sources": [
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/tag",
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/densities",
      "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/tag",
      "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/densities",
      "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/tag",
      "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/densities"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 0,
    "column": 0,
    "part": 0,
    "number": "0.85",
    "displayed": "Three unseen checkpoints pruned to densities 0.575, 0.675 and 0.85",
    "op": "label",
    "sources": [
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/tag",
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/densities",
      "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/tag",
      "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/densities",
      "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/tag",
      "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/densities"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 0,
    "column": 0,
    "part": 2,
    "number": "84",
    "displayed": "84",
    "op": "per_capability",
    "sources": [
      "results/v53-prune-dev/register.json#/n_dev_rows",
      "results/v53-prune-dev/register.json#/models"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 1,
    "column": 2,
    "part": 0,
    "number": "0.277",
    "displayed": "0.277",
    "op": "mean",
    "sources": [
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/math",
      "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/math",
      "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/math"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 1,
    "column": 4,
    "part": 0,
    "number": "0.230",
    "displayed": "0.230",
    "op": "mean",
    "sources": [
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/A2/math",
      "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/A2/math",
      "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/A2/math"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 1,
    "column": 5,
    "part": 0,
    "number": "-0.047",
    "displayed": "-0.047",
    "op": "difference",
    "sources": [
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/math",
      "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/math",
      "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/math",
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/A2/math",
      "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/A2/math",
      "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/A2/math"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 2,
    "column": 2,
    "part": 0,
    "number": "0.214",
    "displayed": "0.214",
    "op": "mean",
    "sources": [
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/code",
      "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/code",
      "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/code"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 2,
    "column": 4,
    "part": 0,
    "number": "0.222",
    "displayed": "0.222",
    "op": "mean",
    "sources": [
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/A2/code",
      "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/A2/code",
      "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/A2/code"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 2,
    "column": 5,
    "part": 0,
    "number": "+0.008",
    "displayed": "+0.008",
    "op": "difference",
    "sources": [
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/code",
      "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/code",
      "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/code",
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/A2/code",
      "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/A2/code",
      "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/A2/code"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 3,
    "column": 2,
    "part": 0,
    "number": "0.221",
    "displayed": "0.221",
    "op": "mean",
    "sources": [
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/qa",
      "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/qa",
      "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/qa"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 3,
    "column": 4,
    "part": 0,
    "number": "0.221",
    "displayed": "0.221",
    "op": "mean",
    "sources": [
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/qa",
      "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/qa",
      "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/qa"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 3,
    "column": 5,
    "part": 0,
    "number": "+0.000",
    "displayed": "+0.000",
    "op": "difference",
    "sources": [
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/qa",
      "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/qa",
      "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/qa",
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/qa",
      "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/qa",
      "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/qa"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 4,
    "column": 0,
    "part": 0,
    "number": "410",
    "displayed": "Pythia 410 million and 1.4 billion at unseen group sizes 32 and 512, bit widths 3 to 5",
    "op": "label",
    "sources": [
      "results/v69-quant-confirm/compare.json#/rows/0/state",
      "results/v69-quant-confirm/compare.json#/rows/0/config",
      "results/v69-quant-confirm/compare.json#/rows/3/config",
      "results/v69-quant-confirm/compare.json#/rows/6/config",
      "results/v69-quant-confirm/compare.json#/rows/9/config",
      "results/v69-quant-confirm/compare.json#/rows/12/config",
      "results/v69-quant-confirm/compare.json#/rows/15/config",
      "results/v69-quant-confirm/compare.json#/rows/18/state"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 4,
    "column": 0,
    "part": 0,
    "number": "1.4",
    "displayed": "Pythia 410 million and 1.4 billion at unseen group sizes 32 and 512, bit widths 3 to 5",
    "op": "label",
    "sources": [
      "results/v69-quant-confirm/compare.json#/rows/0/state",
      "results/v69-quant-confirm/compare.json#/rows/0/config",
      "results/v69-quant-confirm/compare.json#/rows/3/config",
      "results/v69-quant-confirm/compare.json#/rows/6/config",
      "results/v69-quant-confirm/compare.json#/rows/9/config",
      "results/v69-quant-confirm/compare.json#/rows/12/config",
      "results/v69-quant-confirm/compare.json#/rows/15/config",
      "results/v69-quant-confirm/compare.json#/rows/18/state"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 4,
    "column": 0,
    "part": 0,
    "number": "32",
    "displayed": "Pythia 410 million and 1.4 billion at unseen group sizes 32 and 512, bit widths 3 to 5",
    "op": "label",
    "sources": [
      "results/v69-quant-confirm/compare.json#/rows/0/state",
      "results/v69-quant-confirm/compare.json#/rows/0/config",
      "results/v69-quant-confirm/compare.json#/rows/3/config",
      "results/v69-quant-confirm/compare.json#/rows/6/config",
      "results/v69-quant-confirm/compare.json#/rows/9/config",
      "results/v69-quant-confirm/compare.json#/rows/12/config",
      "results/v69-quant-confirm/compare.json#/rows/15/config",
      "results/v69-quant-confirm/compare.json#/rows/18/state"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 4,
    "column": 0,
    "part": 0,
    "number": "512",
    "displayed": "Pythia 410 million and 1.4 billion at unseen group sizes 32 and 512, bit widths 3 to 5",
    "op": "label",
    "sources": [
      "results/v69-quant-confirm/compare.json#/rows/0/state",
      "results/v69-quant-confirm/compare.json#/rows/0/config",
      "results/v69-quant-confirm/compare.json#/rows/3/config",
      "results/v69-quant-confirm/compare.json#/rows/6/config",
      "results/v69-quant-confirm/compare.json#/rows/9/config",
      "results/v69-quant-confirm/compare.json#/rows/12/config",
      "results/v69-quant-confirm/compare.json#/rows/15/config",
      "results/v69-quant-confirm/compare.json#/rows/18/state"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 4,
    "column": 0,
    "part": 0,
    "number": "3",
    "displayed": "Pythia 410 million and 1.4 billion at unseen group sizes 32 and 512, bit widths 3 to 5",
    "op": "label",
    "sources": [
      "results/v69-quant-confirm/compare.json#/rows/0/state",
      "results/v69-quant-confirm/compare.json#/rows/0/config",
      "results/v69-quant-confirm/compare.json#/rows/3/config",
      "results/v69-quant-confirm/compare.json#/rows/6/config",
      "results/v69-quant-confirm/compare.json#/rows/9/config",
      "results/v69-quant-confirm/compare.json#/rows/12/config",
      "results/v69-quant-confirm/compare.json#/rows/15/config",
      "results/v69-quant-confirm/compare.json#/rows/18/state"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 4,
    "column": 0,
    "part": 0,
    "number": "5",
    "displayed": "Pythia 410 million and 1.4 billion at unseen group sizes 32 and 512, bit widths 3 to 5",
    "op": "label",
    "sources": [
      "results/v69-quant-confirm/compare.json#/rows/0/state",
      "results/v69-quant-confirm/compare.json#/rows/0/config",
      "results/v69-quant-confirm/compare.json#/rows/3/config",
      "results/v69-quant-confirm/compare.json#/rows/6/config",
      "results/v69-quant-confirm/compare.json#/rows/9/config",
      "results/v69-quant-confirm/compare.json#/rows/12/config",
      "results/v69-quant-confirm/compare.json#/rows/15/config",
      "results/v69-quant-confirm/compare.json#/rows/18/state"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 4,
    "column": 0,
    "part": 2,
    "number": "54",
    "displayed": "54",
    "op": "identity",
    "sources": [
      "results/v69-quant-confirm/develop.json#/n_dev_cells"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 5,
    "column": 2,
    "part": 0,
    "number": "0.065",
    "displayed": "0.065",
    "op": "identity",
    "sources": [
      "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/same_input_interpolation/math/mae"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 5,
    "column": 4,
    "part": 0,
    "number": "0.333",
    "displayed": "0.333",
    "op": "identity",
    "sources": [
      "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/bilinear/math/mae"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 5,
    "column": 5,
    "part": 0,
    "number": "+0.268",
    "displayed": "+0.268",
    "op": "difference",
    "sources": [
      "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/same_input_interpolation/math/mae",
      "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/bilinear/math/mae"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 6,
    "column": 2,
    "part": 0,
    "number": "0.116",
    "displayed": "0.116",
    "op": "identity",
    "sources": [
      "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/same_input_interpolation/code/mae"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 6,
    "column": 4,
    "part": 0,
    "number": "0.678",
    "displayed": "0.678",
    "op": "identity",
    "sources": [
      "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/zero/code/mae"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 6,
    "column": 5,
    "part": 0,
    "number": "+0.562",
    "displayed": "+0.562",
    "op": "difference",
    "sources": [
      "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/same_input_interpolation/code/mae",
      "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/zero/code/mae"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 7,
    "column": 2,
    "part": 0,
    "number": "0.458",
    "displayed": "0.458",
    "op": "identity",
    "sources": [
      "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/median/qa/mae"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 7,
    "column": 4,
    "part": 0,
    "number": "0.458",
    "displayed": "0.458",
    "op": "identity",
    "sources": [
      "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/median/qa/mae"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 7,
    "column": 5,
    "part": 0,
    "number": "+0.000",
    "displayed": "+0.000",
    "op": "difference",
    "sources": [
      "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/median/qa/mae",
      "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/median/qa/mae"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 8,
    "column": 0,
    "part": 0,
    "number": "1.4",
    "displayed": "An unseen 1.4 billion stage at bit widths 3 to 5, group sizes 32 to 512",
    "op": "label",
    "sources": [
      "results/v69-quant-confirm/compare.json#/rows/36/state",
      "results/v69-quant-confirm/compare.json#/rows/36/config",
      "results/v69-quant-confirm/compare.json#/rows/39/config",
      "results/v69-quant-confirm/compare.json#/rows/42/config",
      "results/v69-quant-confirm/compare.json#/rows/45/config",
      "results/v69-quant-confirm/compare.json#/rows/48/config",
      "results/v69-quant-confirm/compare.json#/rows/51/config",
      "results/v69-quant-confirm/compare.json#/rows/54/config",
      "results/v69-quant-confirm/compare.json#/rows/57/config",
      "results/v69-quant-confirm/compare.json#/rows/60/config"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 8,
    "column": 0,
    "part": 0,
    "number": "3",
    "displayed": "An unseen 1.4 billion stage at bit widths 3 to 5, group sizes 32 to 512",
    "op": "label",
    "sources": [
      "results/v69-quant-confirm/compare.json#/rows/36/state",
      "results/v69-quant-confirm/compare.json#/rows/36/config",
      "results/v69-quant-confirm/compare.json#/rows/39/config",
      "results/v69-quant-confirm/compare.json#/rows/42/config",
      "results/v69-quant-confirm/compare.json#/rows/45/config",
      "results/v69-quant-confirm/compare.json#/rows/48/config",
      "results/v69-quant-confirm/compare.json#/rows/51/config",
      "results/v69-quant-confirm/compare.json#/rows/54/config",
      "results/v69-quant-confirm/compare.json#/rows/57/config",
      "results/v69-quant-confirm/compare.json#/rows/60/config"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 8,
    "column": 0,
    "part": 0,
    "number": "5",
    "displayed": "An unseen 1.4 billion stage at bit widths 3 to 5, group sizes 32 to 512",
    "op": "label",
    "sources": [
      "results/v69-quant-confirm/compare.json#/rows/36/state",
      "results/v69-quant-confirm/compare.json#/rows/36/config",
      "results/v69-quant-confirm/compare.json#/rows/39/config",
      "results/v69-quant-confirm/compare.json#/rows/42/config",
      "results/v69-quant-confirm/compare.json#/rows/45/config",
      "results/v69-quant-confirm/compare.json#/rows/48/config",
      "results/v69-quant-confirm/compare.json#/rows/51/config",
      "results/v69-quant-confirm/compare.json#/rows/54/config",
      "results/v69-quant-confirm/compare.json#/rows/57/config",
      "results/v69-quant-confirm/compare.json#/rows/60/config"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 8,
    "column": 0,
    "part": 0,
    "number": "32",
    "displayed": "An unseen 1.4 billion stage at bit widths 3 to 5, group sizes 32 to 512",
    "op": "label",
    "sources": [
      "results/v69-quant-confirm/compare.json#/rows/36/state",
      "results/v69-quant-confirm/compare.json#/rows/36/config",
      "results/v69-quant-confirm/compare.json#/rows/39/config",
      "results/v69-quant-confirm/compare.json#/rows/42/config",
      "results/v69-quant-confirm/compare.json#/rows/45/config",
      "results/v69-quant-confirm/compare.json#/rows/48/config",
      "results/v69-quant-confirm/compare.json#/rows/51/config",
      "results/v69-quant-confirm/compare.json#/rows/54/config",
      "results/v69-quant-confirm/compare.json#/rows/57/config",
      "results/v69-quant-confirm/compare.json#/rows/60/config"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 8,
    "column": 0,
    "part": 0,
    "number": "512",
    "displayed": "An unseen 1.4 billion stage at bit widths 3 to 5, group sizes 32 to 512",
    "op": "label",
    "sources": [
      "results/v69-quant-confirm/compare.json#/rows/36/state",
      "results/v69-quant-confirm/compare.json#/rows/36/config",
      "results/v69-quant-confirm/compare.json#/rows/39/config",
      "results/v69-quant-confirm/compare.json#/rows/42/config",
      "results/v69-quant-confirm/compare.json#/rows/45/config",
      "results/v69-quant-confirm/compare.json#/rows/48/config",
      "results/v69-quant-confirm/compare.json#/rows/51/config",
      "results/v69-quant-confirm/compare.json#/rows/54/config",
      "results/v69-quant-confirm/compare.json#/rows/57/config",
      "results/v69-quant-confirm/compare.json#/rows/60/config"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 8,
    "column": 0,
    "part": 2,
    "number": "54",
    "displayed": "54",
    "op": "identity",
    "sources": [
      "results/v69-quant-confirm/develop.json#/n_dev_cells"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 9,
    "column": 2,
    "part": 0,
    "number": "0.088",
    "displayed": "0.088",
    "op": "weighted_mean",
    "sources": [
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/math/mae",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/math/n",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/math/mae",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/math/n"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 9,
    "column": 4,
    "part": 0,
    "number": "0.350",
    "displayed": "0.350",
    "op": "weighted_mean",
    "sources": [
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/bilinear/math/mae",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/bilinear/math/n",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/bilinear/math/mae",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/bilinear/math/n"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 9,
    "column": 5,
    "part": 0,
    "number": "+0.262",
    "displayed": "+0.262",
    "op": "difference",
    "sources": [
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/math/mae",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/math/n",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/math/mae",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/math/n",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/bilinear/math/mae",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/bilinear/math/n",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/bilinear/math/mae",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/bilinear/math/n"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 10,
    "column": 2,
    "part": 0,
    "number": "0.153",
    "displayed": "0.153",
    "op": "weighted_mean",
    "sources": [
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/code/mae",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/code/n",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/code/mae",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/code/n"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 10,
    "column": 4,
    "part": 0,
    "number": "0.563",
    "displayed": "0.563",
    "op": "weighted_mean",
    "sources": [
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/zero/code/mae",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/zero/code/n",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/zero/code/mae",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/zero/code/n"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 10,
    "column": 5,
    "part": 0,
    "number": "+0.410",
    "displayed": "+0.410",
    "op": "difference",
    "sources": [
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/code/mae",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/code/n",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/code/mae",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/code/n",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/zero/code/mae",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/zero/code/n",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/zero/code/mae",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/zero/code/n"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 11,
    "column": 2,
    "part": 0,
    "number": "0.141",
    "displayed": "0.141",
    "op": "weighted_mean",
    "sources": [
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/mae",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/n",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/mae",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/n"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 11,
    "column": 4,
    "part": 0,
    "number": "0.141",
    "displayed": "0.141",
    "op": "weighted_mean",
    "sources": [
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/mae",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/n",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/mae",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/n"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 11,
    "column": 5,
    "part": 0,
    "number": "+0.000",
    "displayed": "+0.000",
    "op": "difference",
    "sources": [
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/mae",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/n",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/mae",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/n",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/mae",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/qa/n",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/mae",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/qa/n"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 12,
    "column": 0,
    "part": 0,
    "number": "270",
    "displayed": "Gemma 270 million distilled on six new pools at 50 to 200 thousand tokens",
    "op": "label",
    "sources": [
      "results/v70-distill-confirm/freeze.json#/confirmation_register/students/0",
      "results/v70-distill-confirm/freeze.json#/confirmation_register/pools",
      "results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 12,
    "column": 0,
    "part": 0,
    "number": "six",
    "displayed": "Gemma 270 million distilled on six new pools at 50 to 200 thousand tokens",
    "op": "label",
    "sources": [
      "results/v70-distill-confirm/freeze.json#/confirmation_register/students/0",
      "results/v70-distill-confirm/freeze.json#/confirmation_register/pools",
      "results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 12,
    "column": 0,
    "part": 0,
    "number": "50",
    "displayed": "Gemma 270 million distilled on six new pools at 50 to 200 thousand tokens",
    "op": "label",
    "sources": [
      "results/v70-distill-confirm/freeze.json#/confirmation_register/students/0",
      "results/v70-distill-confirm/freeze.json#/confirmation_register/pools",
      "results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 12,
    "column": 0,
    "part": 0,
    "number": "200",
    "displayed": "Gemma 270 million distilled on six new pools at 50 to 200 thousand tokens",
    "op": "label",
    "sources": [
      "results/v70-distill-confirm/freeze.json#/confirmation_register/students/0",
      "results/v70-distill-confirm/freeze.json#/confirmation_register/pools",
      "results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 12,
    "column": 0,
    "part": 2,
    "number": "100",
    "displayed": "100",
    "op": "identity",
    "sources": [
      "results/v70-distill-confirm/develop.json#/development_structure/n_points"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 13,
    "column": 2,
    "part": 0,
    "number": "0.074",
    "displayed": "0.074",
    "op": "identity",
    "sources": [
      "results/v70-distill-confirm/compare.json#/groups/0/candidate_mae"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 13,
    "column": 4,
    "part": 0,
    "number": "0.065",
    "displayed": "0.065",
    "op": "identity",
    "sources": [
      "results/v70-distill-confirm/compare.json#/groups/0/baseline_mae"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 13,
    "column": 5,
    "part": 0,
    "number": "-0.009",
    "displayed": "-0.009",
    "op": "difference",
    "sources": [
      "results/v70-distill-confirm/compare.json#/groups/0/candidate_mae",
      "results/v70-distill-confirm/compare.json#/groups/0/baseline_mae"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 14,
    "column": 2,
    "part": 0,
    "number": "0.019",
    "displayed": "0.019",
    "op": "identity",
    "sources": [
      "results/v70-distill-confirm/compare.json#/groups/1/candidate_mae"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 14,
    "column": 4,
    "part": 0,
    "number": "0.023",
    "displayed": "0.023",
    "op": "identity",
    "sources": [
      "results/v70-distill-confirm/compare.json#/groups/1/baseline_mae"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 14,
    "column": 5,
    "part": 0,
    "number": "+0.004",
    "displayed": "+0.004",
    "op": "difference",
    "sources": [
      "results/v70-distill-confirm/compare.json#/groups/1/candidate_mae",
      "results/v70-distill-confirm/compare.json#/groups/1/baseline_mae"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 15,
    "column": 2,
    "part": 0,
    "number": "0.515",
    "displayed": "0.515",
    "op": "identity",
    "sources": [
      "results/v70-distill-confirm/compare.json#/groups/2/candidate_mae"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 15,
    "column": 4,
    "part": 0,
    "number": "0.610",
    "displayed": "0.610",
    "op": "identity",
    "sources": [
      "results/v70-distill-confirm/compare.json#/groups/2/baseline_mae"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 15,
    "column": 5,
    "part": 0,
    "number": "+0.095",
    "displayed": "+0.095",
    "op": "difference",
    "sources": [
      "results/v70-distill-confirm/compare.json#/groups/2/candidate_mae",
      "results/v70-distill-confirm/compare.json#/groups/2/baseline_mae"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 16,
    "column": 0,
    "part": 0,
    "number": "1",
    "displayed": "Gemma 1 billion distilled on six new pools at 50 to 200 thousand tokens",
    "op": "label",
    "sources": [
      "results/v70-distill-confirm/freeze.json#/confirmation_register/students/1",
      "results/v70-distill-confirm/freeze.json#/confirmation_register/pools",
      "results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 16,
    "column": 0,
    "part": 0,
    "number": "six",
    "displayed": "Gemma 1 billion distilled on six new pools at 50 to 200 thousand tokens",
    "op": "label",
    "sources": [
      "results/v70-distill-confirm/freeze.json#/confirmation_register/students/1",
      "results/v70-distill-confirm/freeze.json#/confirmation_register/pools",
      "results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 16,
    "column": 0,
    "part": 0,
    "number": "50",
    "displayed": "Gemma 1 billion distilled on six new pools at 50 to 200 thousand tokens",
    "op": "label",
    "sources": [
      "results/v70-distill-confirm/freeze.json#/confirmation_register/students/1",
      "results/v70-distill-confirm/freeze.json#/confirmation_register/pools",
      "results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 16,
    "column": 0,
    "part": 0,
    "number": "200",
    "displayed": "Gemma 1 billion distilled on six new pools at 50 to 200 thousand tokens",
    "op": "label",
    "sources": [
      "results/v70-distill-confirm/freeze.json#/confirmation_register/students/1",
      "results/v70-distill-confirm/freeze.json#/confirmation_register/pools",
      "results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 16,
    "column": 0,
    "part": 2,
    "number": "100",
    "displayed": "100",
    "op": "identity",
    "sources": [
      "results/v70-distill-confirm/develop.json#/development_structure/n_points"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 17,
    "column": 2,
    "part": 0,
    "number": "0.057",
    "displayed": "0.057",
    "op": "identity",
    "sources": [
      "results/v70-distill-confirm/compare.json#/groups/3/candidate_mae"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 17,
    "column": 4,
    "part": 0,
    "number": "0.033",
    "displayed": "0.033",
    "op": "identity",
    "sources": [
      "results/v70-distill-confirm/compare.json#/groups/3/baseline_mae"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 17,
    "column": 5,
    "part": 0,
    "number": "-0.023",
    "displayed": "-0.023",
    "op": "difference",
    "sources": [
      "results/v70-distill-confirm/compare.json#/groups/3/candidate_mae",
      "results/v70-distill-confirm/compare.json#/groups/3/baseline_mae"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 18,
    "column": 2,
    "part": 0,
    "number": "0.049",
    "displayed": "0.049",
    "op": "identity",
    "sources": [
      "results/v70-distill-confirm/compare.json#/groups/4/candidate_mae"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 18,
    "column": 4,
    "part": 0,
    "number": "0.053",
    "displayed": "0.053",
    "op": "identity",
    "sources": [
      "results/v70-distill-confirm/compare.json#/groups/4/baseline_mae"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 18,
    "column": 5,
    "part": 0,
    "number": "+0.005",
    "displayed": "+0.005",
    "op": "difference",
    "sources": [
      "results/v70-distill-confirm/compare.json#/groups/4/candidate_mae",
      "results/v70-distill-confirm/compare.json#/groups/4/baseline_mae"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 19,
    "column": 2,
    "part": 0,
    "number": "0.463",
    "displayed": "0.463",
    "op": "identity",
    "sources": [
      "results/v70-distill-confirm/compare.json#/groups/5/candidate_mae"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 19,
    "column": 4,
    "part": 0,
    "number": "0.450",
    "displayed": "0.450",
    "op": "identity",
    "sources": [
      "results/v70-distill-confirm/compare.json#/groups/5/baseline_mae"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "row": 19,
    "column": 5,
    "part": 0,
    "number": "-0.013",
    "displayed": "-0.013",
    "op": "difference",
    "sources": [
      "results/v70-distill-confirm/compare.json#/groups/5/candidate_mae",
      "results/v70-distill-confirm/compare.json#/groups/5/baseline_mae"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "location": "caption",
    "part": 1,
    "number": "270",
    "displayed": "270 million and 1 billion",
    "op": "label",
    "sources": [
      "results/v70-distill-confirm/freeze.json#/confirmation_register/students"
    ]
  },
  {
    "table": "tab:main-prediction-v2",
    "location": "caption",
    "part": 1,
    "number": "1",
    "displayed": "270 million and 1 billion",
    "op": "label",
    "sources": [
      "results/v70-distill-confirm/freeze.json#/confirmation_register/students"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 0,
    "column": 0,
    "part": 0,
    "number": "Three",
    "displayed": "Three unseen checkpoints pruned to densities 0.575, 0.675 and 0.85",
    "op": "label",
    "sources": [
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/tag",
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/densities",
      "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/tag",
      "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/densities",
      "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/tag",
      "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/densities"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 0,
    "column": 0,
    "part": 0,
    "number": "0.575",
    "displayed": "Three unseen checkpoints pruned to densities 0.575, 0.675 and 0.85",
    "op": "label",
    "sources": [
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/tag",
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/densities",
      "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/tag",
      "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/densities",
      "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/tag",
      "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/densities"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 0,
    "column": 0,
    "part": 0,
    "number": "0.675",
    "displayed": "Three unseen checkpoints pruned to densities 0.575, 0.675 and 0.85",
    "op": "label",
    "sources": [
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/tag",
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/densities",
      "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/tag",
      "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/densities",
      "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/tag",
      "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/densities"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 0,
    "column": 0,
    "part": 0,
    "number": "0.85",
    "displayed": "Three unseen checkpoints pruned to densities 0.575, 0.675 and 0.85",
    "op": "label",
    "sources": [
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/tag",
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/densities",
      "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/tag",
      "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/densities",
      "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/tag",
      "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/densities"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 0,
    "column": 1,
    "part": 0,
    "number": "Five",
    "displayed": "Five-parameter power form",
    "op": "label",
    "sources": [
      "results/v53-prune-dev/register.json#/candidate_definitions/power",
      "results/v53-prune-dev/register.json#/n_params_per_capability/power",
      "results/v53-prune-dev/register.json#/n_dev_states"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 0,
    "column": 2,
    "part": 0,
    "number": "0.243",
    "displayed": "0.243",
    "op": "mean",
    "sources": [
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/power/math",
      "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/power/math",
      "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/power/math"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 0,
    "column": 2,
    "part": 2,
    "number": "0.236",
    "displayed": "0.236",
    "op": "mean",
    "sources": [
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/power/code",
      "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/power/code",
      "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/power/code"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 0,
    "column": 2,
    "part": 4,
    "number": "0.678",
    "displayed": "0.678",
    "op": "mean",
    "sources": [
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/power/qa",
      "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/power/qa",
      "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/power/qa"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 1,
    "column": 0,
    "part": 0,
    "number": "410",
    "displayed": "Pythia 410 million and 1.4 billion at unseen group sizes 32 and 512, bit widths 3 to 5",
    "op": "label",
    "sources": [
      "results/v69-quant-confirm/compare.json#/rows/0/state",
      "results/v69-quant-confirm/compare.json#/rows/0/config",
      "results/v69-quant-confirm/compare.json#/rows/3/config",
      "results/v69-quant-confirm/compare.json#/rows/6/config",
      "results/v69-quant-confirm/compare.json#/rows/9/config",
      "results/v69-quant-confirm/compare.json#/rows/12/config",
      "results/v69-quant-confirm/compare.json#/rows/15/config",
      "results/v69-quant-confirm/compare.json#/rows/18/state"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 1,
    "column": 0,
    "part": 0,
    "number": "1.4",
    "displayed": "Pythia 410 million and 1.4 billion at unseen group sizes 32 and 512, bit widths 3 to 5",
    "op": "label",
    "sources": [
      "results/v69-quant-confirm/compare.json#/rows/0/state",
      "results/v69-quant-confirm/compare.json#/rows/0/config",
      "results/v69-quant-confirm/compare.json#/rows/3/config",
      "results/v69-quant-confirm/compare.json#/rows/6/config",
      "results/v69-quant-confirm/compare.json#/rows/9/config",
      "results/v69-quant-confirm/compare.json#/rows/12/config",
      "results/v69-quant-confirm/compare.json#/rows/15/config",
      "results/v69-quant-confirm/compare.json#/rows/18/state"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 1,
    "column": 0,
    "part": 0,
    "number": "32",
    "displayed": "Pythia 410 million and 1.4 billion at unseen group sizes 32 and 512, bit widths 3 to 5",
    "op": "label",
    "sources": [
      "results/v69-quant-confirm/compare.json#/rows/0/state",
      "results/v69-quant-confirm/compare.json#/rows/0/config",
      "results/v69-quant-confirm/compare.json#/rows/3/config",
      "results/v69-quant-confirm/compare.json#/rows/6/config",
      "results/v69-quant-confirm/compare.json#/rows/9/config",
      "results/v69-quant-confirm/compare.json#/rows/12/config",
      "results/v69-quant-confirm/compare.json#/rows/15/config",
      "results/v69-quant-confirm/compare.json#/rows/18/state"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 1,
    "column": 0,
    "part": 0,
    "number": "512",
    "displayed": "Pythia 410 million and 1.4 billion at unseen group sizes 32 and 512, bit widths 3 to 5",
    "op": "label",
    "sources": [
      "results/v69-quant-confirm/compare.json#/rows/0/state",
      "results/v69-quant-confirm/compare.json#/rows/0/config",
      "results/v69-quant-confirm/compare.json#/rows/3/config",
      "results/v69-quant-confirm/compare.json#/rows/6/config",
      "results/v69-quant-confirm/compare.json#/rows/9/config",
      "results/v69-quant-confirm/compare.json#/rows/12/config",
      "results/v69-quant-confirm/compare.json#/rows/15/config",
      "results/v69-quant-confirm/compare.json#/rows/18/state"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 1,
    "column": 0,
    "part": 0,
    "number": "3",
    "displayed": "Pythia 410 million and 1.4 billion at unseen group sizes 32 and 512, bit widths 3 to 5",
    "op": "label",
    "sources": [
      "results/v69-quant-confirm/compare.json#/rows/0/state",
      "results/v69-quant-confirm/compare.json#/rows/0/config",
      "results/v69-quant-confirm/compare.json#/rows/3/config",
      "results/v69-quant-confirm/compare.json#/rows/6/config",
      "results/v69-quant-confirm/compare.json#/rows/9/config",
      "results/v69-quant-confirm/compare.json#/rows/12/config",
      "results/v69-quant-confirm/compare.json#/rows/15/config",
      "results/v69-quant-confirm/compare.json#/rows/18/state"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 1,
    "column": 0,
    "part": 0,
    "number": "5",
    "displayed": "Pythia 410 million and 1.4 billion at unseen group sizes 32 and 512, bit widths 3 to 5",
    "op": "label",
    "sources": [
      "results/v69-quant-confirm/compare.json#/rows/0/state",
      "results/v69-quant-confirm/compare.json#/rows/0/config",
      "results/v69-quant-confirm/compare.json#/rows/3/config",
      "results/v69-quant-confirm/compare.json#/rows/6/config",
      "results/v69-quant-confirm/compare.json#/rows/9/config",
      "results/v69-quant-confirm/compare.json#/rows/12/config",
      "results/v69-quant-confirm/compare.json#/rows/15/config",
      "results/v69-quant-confirm/compare.json#/rows/18/state"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 1,
    "column": 2,
    "part": 0,
    "number": "0.215",
    "displayed": "0.215",
    "op": "identity",
    "sources": [
      "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/low_order_2d/math/mae"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 1,
    "column": 2,
    "part": 2,
    "number": "0.557",
    "displayed": "0.557",
    "op": "identity",
    "sources": [
      "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/median/code/mae"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 1,
    "column": 2,
    "part": 4,
    "number": "0.457",
    "displayed": "0.457",
    "op": "identity",
    "sources": [
      "results/v69-quant-confirm/compare.json#/test_sets/development_state_boundary/scores/zero/qa/mae"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 2,
    "column": 0,
    "part": 0,
    "number": "1.4",
    "displayed": "An unseen 1.4 billion stage at bit widths 3 to 5, group sizes 32 to 512",
    "op": "label",
    "sources": [
      "results/v69-quant-confirm/compare.json#/rows/36/state",
      "results/v69-quant-confirm/compare.json#/rows/36/config",
      "results/v69-quant-confirm/compare.json#/rows/39/config",
      "results/v69-quant-confirm/compare.json#/rows/42/config",
      "results/v69-quant-confirm/compare.json#/rows/45/config",
      "results/v69-quant-confirm/compare.json#/rows/48/config",
      "results/v69-quant-confirm/compare.json#/rows/51/config",
      "results/v69-quant-confirm/compare.json#/rows/54/config",
      "results/v69-quant-confirm/compare.json#/rows/57/config",
      "results/v69-quant-confirm/compare.json#/rows/60/config"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 2,
    "column": 0,
    "part": 0,
    "number": "3",
    "displayed": "An unseen 1.4 billion stage at bit widths 3 to 5, group sizes 32 to 512",
    "op": "label",
    "sources": [
      "results/v69-quant-confirm/compare.json#/rows/36/state",
      "results/v69-quant-confirm/compare.json#/rows/36/config",
      "results/v69-quant-confirm/compare.json#/rows/39/config",
      "results/v69-quant-confirm/compare.json#/rows/42/config",
      "results/v69-quant-confirm/compare.json#/rows/45/config",
      "results/v69-quant-confirm/compare.json#/rows/48/config",
      "results/v69-quant-confirm/compare.json#/rows/51/config",
      "results/v69-quant-confirm/compare.json#/rows/54/config",
      "results/v69-quant-confirm/compare.json#/rows/57/config",
      "results/v69-quant-confirm/compare.json#/rows/60/config"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 2,
    "column": 0,
    "part": 0,
    "number": "5",
    "displayed": "An unseen 1.4 billion stage at bit widths 3 to 5, group sizes 32 to 512",
    "op": "label",
    "sources": [
      "results/v69-quant-confirm/compare.json#/rows/36/state",
      "results/v69-quant-confirm/compare.json#/rows/36/config",
      "results/v69-quant-confirm/compare.json#/rows/39/config",
      "results/v69-quant-confirm/compare.json#/rows/42/config",
      "results/v69-quant-confirm/compare.json#/rows/45/config",
      "results/v69-quant-confirm/compare.json#/rows/48/config",
      "results/v69-quant-confirm/compare.json#/rows/51/config",
      "results/v69-quant-confirm/compare.json#/rows/54/config",
      "results/v69-quant-confirm/compare.json#/rows/57/config",
      "results/v69-quant-confirm/compare.json#/rows/60/config"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 2,
    "column": 0,
    "part": 0,
    "number": "32",
    "displayed": "An unseen 1.4 billion stage at bit widths 3 to 5, group sizes 32 to 512",
    "op": "label",
    "sources": [
      "results/v69-quant-confirm/compare.json#/rows/36/state",
      "results/v69-quant-confirm/compare.json#/rows/36/config",
      "results/v69-quant-confirm/compare.json#/rows/39/config",
      "results/v69-quant-confirm/compare.json#/rows/42/config",
      "results/v69-quant-confirm/compare.json#/rows/45/config",
      "results/v69-quant-confirm/compare.json#/rows/48/config",
      "results/v69-quant-confirm/compare.json#/rows/51/config",
      "results/v69-quant-confirm/compare.json#/rows/54/config",
      "results/v69-quant-confirm/compare.json#/rows/57/config",
      "results/v69-quant-confirm/compare.json#/rows/60/config"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 2,
    "column": 0,
    "part": 0,
    "number": "512",
    "displayed": "An unseen 1.4 billion stage at bit widths 3 to 5, group sizes 32 to 512",
    "op": "label",
    "sources": [
      "results/v69-quant-confirm/compare.json#/rows/36/state",
      "results/v69-quant-confirm/compare.json#/rows/36/config",
      "results/v69-quant-confirm/compare.json#/rows/39/config",
      "results/v69-quant-confirm/compare.json#/rows/42/config",
      "results/v69-quant-confirm/compare.json#/rows/45/config",
      "results/v69-quant-confirm/compare.json#/rows/48/config",
      "results/v69-quant-confirm/compare.json#/rows/51/config",
      "results/v69-quant-confirm/compare.json#/rows/54/config",
      "results/v69-quant-confirm/compare.json#/rows/57/config",
      "results/v69-quant-confirm/compare.json#/rows/60/config"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 2,
    "column": 2,
    "part": 0,
    "number": "0.303",
    "displayed": "0.303",
    "op": "weighted_mean",
    "sources": [
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/low_order_2d/math/mae",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/low_order_2d/math/n",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/low_order_2d/math/mae",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/low_order_2d/math/n"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 2,
    "column": 2,
    "part": 2,
    "number": "0.153",
    "displayed": "0.153",
    "op": "weighted_mean",
    "sources": [
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/code/mae",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/median/code/n",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/code/mae",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/median/code/n"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 2,
    "column": 2,
    "part": 4,
    "number": "0.222",
    "displayed": "0.222",
    "op": "weighted_mean",
    "sources": [
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/zero/qa/mae",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_boundary/scores/zero/qa/n",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/zero/qa/mae",
      "results/v69-quant-confirm/compare.json#/test_sets/new_state_interior/scores/zero/qa/n"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 3,
    "column": 0,
    "part": 0,
    "number": "270",
    "displayed": "Gemma 270 million distilled on six new pools at 50 to 200 thousand tokens",
    "op": "label",
    "sources": [
      "results/v70-distill-confirm/freeze.json#/confirmation_register/students/0",
      "results/v70-distill-confirm/freeze.json#/confirmation_register/pools",
      "results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 3,
    "column": 0,
    "part": 0,
    "number": "six",
    "displayed": "Gemma 270 million distilled on six new pools at 50 to 200 thousand tokens",
    "op": "label",
    "sources": [
      "results/v70-distill-confirm/freeze.json#/confirmation_register/students/0",
      "results/v70-distill-confirm/freeze.json#/confirmation_register/pools",
      "results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 3,
    "column": 0,
    "part": 0,
    "number": "50",
    "displayed": "Gemma 270 million distilled on six new pools at 50 to 200 thousand tokens",
    "op": "label",
    "sources": [
      "results/v70-distill-confirm/freeze.json#/confirmation_register/students/0",
      "results/v70-distill-confirm/freeze.json#/confirmation_register/pools",
      "results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 3,
    "column": 0,
    "part": 0,
    "number": "200",
    "displayed": "Gemma 270 million distilled on six new pools at 50 to 200 thousand tokens",
    "op": "label",
    "sources": [
      "results/v70-distill-confirm/freeze.json#/confirmation_register/students/0",
      "results/v70-distill-confirm/freeze.json#/confirmation_register/pools",
      "results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 3,
    "column": 2,
    "part": 0,
    "number": "0.074",
    "displayed": "0.074",
    "op": "identity",
    "sources": [
      "results/v70-distill-confirm/compare.json#/groups/0/candidate_mae"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 3,
    "column": 2,
    "part": 2,
    "number": "0.019",
    "displayed": "0.019",
    "op": "identity",
    "sources": [
      "results/v70-distill-confirm/compare.json#/groups/1/candidate_mae"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 3,
    "column": 2,
    "part": 4,
    "number": "0.515",
    "displayed": "0.515",
    "op": "identity",
    "sources": [
      "results/v70-distill-confirm/compare.json#/groups/2/candidate_mae"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 4,
    "column": 0,
    "part": 0,
    "number": "1",
    "displayed": "Gemma 1 billion distilled on six new pools at 50 to 200 thousand tokens",
    "op": "label",
    "sources": [
      "results/v70-distill-confirm/freeze.json#/confirmation_register/students/1",
      "results/v70-distill-confirm/freeze.json#/confirmation_register/pools",
      "results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 4,
    "column": 0,
    "part": 0,
    "number": "six",
    "displayed": "Gemma 1 billion distilled on six new pools at 50 to 200 thousand tokens",
    "op": "label",
    "sources": [
      "results/v70-distill-confirm/freeze.json#/confirmation_register/students/1",
      "results/v70-distill-confirm/freeze.json#/confirmation_register/pools",
      "results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 4,
    "column": 0,
    "part": 0,
    "number": "50",
    "displayed": "Gemma 1 billion distilled on six new pools at 50 to 200 thousand tokens",
    "op": "label",
    "sources": [
      "results/v70-distill-confirm/freeze.json#/confirmation_register/students/1",
      "results/v70-distill-confirm/freeze.json#/confirmation_register/pools",
      "results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 4,
    "column": 0,
    "part": 0,
    "number": "200",
    "displayed": "Gemma 1 billion distilled on six new pools at 50 to 200 thousand tokens",
    "op": "label",
    "sources": [
      "results/v70-distill-confirm/freeze.json#/confirmation_register/students/1",
      "results/v70-distill-confirm/freeze.json#/confirmation_register/pools",
      "results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 4,
    "column": 2,
    "part": 0,
    "number": "0.057",
    "displayed": "0.057",
    "op": "identity",
    "sources": [
      "results/v70-distill-confirm/compare.json#/groups/3/candidate_mae"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 4,
    "column": 2,
    "part": 2,
    "number": "0.049",
    "displayed": "0.049",
    "op": "identity",
    "sources": [
      "results/v70-distill-confirm/compare.json#/groups/4/candidate_mae"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "row": 4,
    "column": 2,
    "part": 4,
    "number": "0.463",
    "displayed": "0.463",
    "op": "identity",
    "sources": [
      "results/v70-distill-confirm/compare.json#/groups/5/candidate_mae"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "location": "caption",
    "part": 1,
    "number": "270",
    "displayed": "270 million and 1 billion",
    "op": "label",
    "sources": [
      "results/v70-distill-confirm/freeze.json#/confirmation_register/students"
    ]
  },
  {
    "table": "tab:main-prediction-candidates",
    "location": "caption",
    "part": 1,
    "number": "1",
    "displayed": "270 million and 1 billion",
    "op": "label",
    "sources": [
      "results/v70-distill-confirm/freeze.json#/confirmation_register/students"
    ]
  }
]
```

## Input hashes

- `results/a5-corner-second-difference/summary.json`: `05de90f078ea37d760f256eb9b9cfe37bea734827b2c8099e25f66a689a1bc75`
- `results/a7-closeout-audit/summary.json`: `14d698bc5348bee38fe593632f421fa64d794ad2a2687a70532bae935a078c9e`
- `results/v40-prune-strength/register.json`: `2080fb5ddf606f3a0ba8f4af6096ee4044c3bfb370d710c8abd6f04438265c93`
- `results/v46-p1-newsource/compare.json`: `8e6a4b910b06038ef35f10a96e512d0cc29bfc1d2ed97471bba680cc9cb9d6f0`
- `results/v46-p1-newsource/predictions_frozen.json`: `c33b03950f0a649db07d0406e751e6890e2319e852c2d6fd2ffc4a1ff3d57445`
- `results/v47-p2-register/register.json`: `c12167d4b12b9c18e5983239573868ea4a7dfe3f62c8b638f3a10f99970e4757`
- `results/v50-p2v2/compare_test.json`: `4c07abf0f940e95992a3f46d79b6d9a3ef9524ba55adaefa824b0cdec8a601aa`
- `results/v53-prune-dev/compare_pythia-1.4b@step112000.json`: `23dd3cd34588ea33666f0158fc05004b6bc8273ab8947bb43aad954085857406`
- `results/v53-prune-dev/compare_pythia-410m@step48000.json`: `6cbfcff19a7196a5377e83417538159b86797996d3045c976fcb3e29dd321399`
- `results/v53-prune-dev/compare_pythia-6.9b@step80000.json`: `288af4793219be8325a33fcaa0d2dbc0dd96defff4890de040aea0723e177eb9`
- `results/v53-prune-dev/predictions_pythia-1.4b@step112000.json`: `862e299cc30a55672c785de418b0c184c204e3d5c2b222fb6174351e507489f4`
- `results/v53-prune-dev/predictions_pythia-410m@step48000.json`: `6a3e987278dcb2d59d37eb72161bc0a062dd5cbe67116087b9fe7374bf426d6a`
- `results/v53-prune-dev/predictions_pythia-6.9b@step80000.json`: `c14ec20711138aa57d7ae4d394c97ba8b08c05ed65926c537473e6ec499558d3`
- `results/v53-prune-dev/register.json`: `7498103830f139f6bea16ee440b717a05dee41e45b9835fdac6a2251b833974d`
- `results/v55-quant-group/compare.json`: `aa7101b5a060d9cc89aa7ebd8322bfc0146e49ece9b96006d7b95a0afd607421`
- `results/v55-quant-group/register.json`: `d5e36301651d4627923bb95cf4e23f86600c9eeeea6bb60fd603da8e77b91e3d`
- `results/v69-quant-confirm/compare.json`: `12944c61ed42c61f1beaf8f84ef5c87d900b3b1a38d65d175976e27d3d4e6bac`
- `results/v69-quant-confirm/develop.json`: `9f035cb37a94d425064f37d822490b52dcad4c669e62864f27cba4ffa5e5643d`
- `results/v69-quant-confirm/freeze.json`: `6ade0a3ff576781cf286978519b6a922500d37e3bc72cef4e3e635e826cccdc2`
- `results/v70-distill-confirm/compare.json`: `983f53033b07e035b1cb552429b8ce6ab23f8d6aee4365237970e2b46b0a829b`
- `results/v70-distill-confirm/develop.json`: `a3a3da1c66fdc9a4b21f314316c76c52f0d382afa8e9f65b9c6b0cb16a6bb86d`
- `results/v70-distill-confirm/freeze.json`: `d7b28c7251dbc6113c3de7c957560827e603d4e77a48010f99835a8468db0c24`
- `results/v72-prune-repeat/compare.json`: `639eef759655038f393e0451b4d7471883dae31d4da08ffe32a6277eaec76fb9`
- `results/v72-prune-repeat/freeze.json`: `3f4e45d0bd505b7d65815f2246a5c3b343f3a49be465aedf724aaa208b0de8b9`
- `results/v74-quant-threeway/quant_threeway.json`: `56041ef7efd14235121cc158267abeaecb0f382241ecbea12569cb4f3029b060`
- `results/v78-rule-confirm/compare.json`: `601669be112c5dd7c016e859423700a98f6a916dcd12c838bb5cd9c8c09686a8`
- `results/v78-rule-confirm/freeze.json`: `78dd229d7131f485b3a0651eac6978d2671ad139c02fcc2ea753d3420d5f129f`
- `results/v86-main-table/summary.json`: `15e7c95b6125956e211656a2539db06a0212ec9169b03c09cd0921cc76589e04`
- `results/v93-confirm-inputs/pythia-1.4b--step32000/code/descriptor_bv.json`: `6dd768ff28a612cb7ccc4bcc89defac8c71bb633934fc66af644563f01273aea`
- `results/v93-confirm-inputs/pythia-1.4b--step32000/math/descriptor_bv.json`: `15bc1a6e545228cdc8825e624f768418ce7f36e468c7fe1a9f60785539ead4a7`
- `results/v93-confirm-inputs/pythia-1.4b--step32000/qa/descriptor_bv.json`: `f123b81cda60b9ce7190160e74bc5977c9dcb15fea000ae5f0f8355a2e6f4b66`
- `results/v93-confirm-inputs/pythia-160m--step32000/code/descriptor_bv.json`: `2b1c20e57e1b0ee76bda36f7f2a2e91fa70c1a52676ae55ed296ec242e9281c0`
- `results/v93-confirm-inputs/pythia-160m--step32000/math/descriptor_bv.json`: `0566eec067fb501fd4c2d0b86428480170ea652ff13709bef2c9722c9262082e`
- `results/v93-confirm-inputs/pythia-160m--step32000/qa/descriptor_bv.json`: `b40f0bb31343b37d3c8015ae03958474618d7c30b79f573dcf00712a116a6c44`
- `results/v93-confirm-inputs/pythia-1b--step64000/code/descriptor_bv.json`: `dd2f57d6959ba03218477acb2fc192cf1490bf96010298329c2b64bac7788fb3`
- `results/v93-confirm-inputs/pythia-1b--step64000/math/descriptor_bv.json`: `53de72d512bcc6eebea402eb9e127581c7be7c0263b961c4a4c71ae181e7b494`
- `results/v93-confirm-inputs/pythia-1b--step64000/qa/descriptor_bv.json`: `37a3d9706623b886f17fa2d6fbeafadb7192a1cfe4ce770b41f5be839988de0c`
- `results/v93-confirm-inputs/pythia-410m--step32000/code/descriptor_bv.json`: `01c2ca20d2143a928711724c8a361451ab8d501c607e8a739e97b64fb3076331`
- `results/v93-confirm-inputs/pythia-410m--step32000/math/descriptor_bv.json`: `93faed2ce68844cef1a769dee652bf8bb0cfad9207bd905ffa637a178302feda`
- `results/v93-confirm-inputs/pythia-410m--step32000/qa/descriptor_bv.json`: `fb5267ce8820982968b8971dd9f077cb39e22aa96d87ea2e63bcfdc788160ae6`
