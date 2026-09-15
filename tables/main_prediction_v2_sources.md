# Main prediction table: cell sources

Columns: task, relation, tested range, error, development baseline, status.
All indices are zero-based JSON pointers. `mean` is equal-weight arithmetic only; no refits or resampling.
Numeric values are formatted directly from the following executable source recipes. Context pointers justify textual labels and missing evidence.
The `label` operation uses the generator's explicit presentation mappings; `expected` preserves the source values and must match before rendering `label`. Counts always use their own JSON fields.

## Loader reuse and limits

Reused v86_main_table.build_rows, Comparison.number, row_scores and paired_rows; pruning inputs are v53-prune-dev register/predictions/compare and v72-prune-repeat freeze/compare. Did not use test-ranked Row.baselines or post-hoc Row.delivered.
V47 original freeze.json is absent: that original test is not tested here. The registered v5_confirm section is paired with the available V70 freeze.
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
Intervals remain attached to their estimand: A2 primary_mae_interval is an error interval; V70 paired_difference.ci95 is a baseline-minus-candidate interval, never an MAE interval.
The requested nine-state leave-density-out DEVELOPMENT evaluation is absent from the supplied V53 files. register.json records n_dev_states=17 and loso_folds/loso_predictions hold out source states, not densities. predictions_<tag>.json contains new-source predictions only. V40 documents the original nine-state panel and its [0.6, 0.9] grid, but does not supply the requested density-holdout errors. No LOSO, training-fit or identical-weight repeat errors are substituted.
V72 repeat: same weights, one state. Legacy identity checks still read it, but no table score uses it.

## Fields per cell

- Cell (0, 0): `results/v53-prune-dev/register.json#/loso_folds`
- Cell (0, 1): `results/v53-prune-dev/register.json#/feature_names`; `results/v53-prune-dev/register.json#/candidate_definitions/power`; `results/v53-prune-dev/register.json#/n_params_per_capability/power`
- Cell (0, 2): `results/v40-prune-strength/register.json#/dev`
- Cell (0, 3): `results/v53-prune-dev/register.json#/loso_predictions`
- Cell (0, 4): `results/v53-prune-dev/register.json#/loso_table`
- Cell (0, 5): `results/v53-prune-dev/register.json#/selection_rule`
- Cell (1, 0): `results/v53-prune-dev/register.json#/selected_candidate`
- Cell (1, 1): `results/v53-prune-dev/register.json#/feature_names`; `results/v53-prune-dev/register.json#/candidate_definitions/power`; `results/v53-prune-dev/register.json#/n_params_per_capability/power`
- Cell (1, 2): `results/v53-prune-dev/compare_pythia-410m@step48000.json#/densities`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/tag`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/tag`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/tag`; `results/v40-prune-strength/register.json#/dev/sizes`
- Cell (1, 3): `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/power/math`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/power/math`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/power/math`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/power/code`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/power/code`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/power/code`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/power/qa`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/power/qa`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/power/qa`
- Cell (1, 4): `results/v53-prune-dev/register.json#/loso_table`; `results/v53-prune-dev/register.json#/loso_table/2/candidate`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/A2/math`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/A2/math`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/A2/math`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/A2/code`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/A2/code`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/A2/code`; `results/v53-prune-dev/register.json#/loso_table/5/candidate`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/qa`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/qa`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/qa`
- Cell (1, 5): `results/v53-prune-dev/register.json#/selected_candidate`
- Cell (2, 0): `results/v55-quant-group/register.json#/test_sets/bit_test`
- Cell (2, 1): `results/v55-quant-group/register.json#/feature_names`; `results/v55-quant-group/register.json#/candidate_definitions/low_order_2d`; `results/v55-quant-group/register.json#/n_params_per_capability/low_order_2d`
- Cell (2, 2): `results/v55-quant-group/register.json#/test_sets/bit_test/states`; `results/v55-quant-group/register.json#/test_sets/bit_test/configs`
- Cell (2, 3): `results/v55-quant-group/compare.json#/test_sets/bit_test/mae_table/1/mae/math`; `results/v55-quant-group/compare.json#/test_sets/bit_test/mae_table/1/mae/code`; `results/v55-quant-group/compare.json#/test_sets/bit_test/mae_table/1/mae/qa`
- Cell (2, 4): `results/v55-quant-group/register.json#/loso_table`; `results/v55-quant-group/register.json#/loso_table/4/candidate`; `results/v55-quant-group/compare.json#/test_sets/bit_test/mae_table/4/mae/math`; `results/v55-quant-group/compare.json#/test_sets/bit_test/mae_table/4/mae/code`; `results/v55-quant-group/compare.json#/test_sets/bit_test/mae_table/4/mae/qa`
- Cell (2, 5): `results/v55-quant-group/register.json#/precommitted_rule`
- Cell (3, 0): `results/v69-quant-confirm/compare.json#/rows/0/test_set`; `results/v69-quant-confirm/compare.json#/rows/1/test_set`; `results/v69-quant-confirm/compare.json#/rows/2/test_set`; `results/v69-quant-confirm/compare.json#/rows/3/test_set`; `results/v69-quant-confirm/compare.json#/rows/4/test_set`; `results/v69-quant-confirm/compare.json#/rows/5/test_set`; `results/v69-quant-confirm/compare.json#/rows/6/test_set`; `results/v69-quant-confirm/compare.json#/rows/7/test_set`; `results/v69-quant-confirm/compare.json#/rows/8/test_set`; `results/v69-quant-confirm/compare.json#/rows/9/test_set`; `results/v69-quant-confirm/compare.json#/rows/10/test_set`; `results/v69-quant-confirm/compare.json#/rows/11/test_set`; `results/v69-quant-confirm/compare.json#/rows/12/test_set`; `results/v69-quant-confirm/compare.json#/rows/13/test_set`; `results/v69-quant-confirm/compare.json#/rows/14/test_set`; `results/v69-quant-confirm/compare.json#/rows/15/test_set`; `results/v69-quant-confirm/compare.json#/rows/16/test_set`; `results/v69-quant-confirm/compare.json#/rows/17/test_set`; `results/v69-quant-confirm/compare.json#/rows/18/test_set`; `results/v69-quant-confirm/compare.json#/rows/19/test_set`; `results/v69-quant-confirm/compare.json#/rows/20/test_set`; `results/v69-quant-confirm/compare.json#/rows/21/test_set`; `results/v69-quant-confirm/compare.json#/rows/22/test_set`; `results/v69-quant-confirm/compare.json#/rows/23/test_set`; `results/v69-quant-confirm/compare.json#/rows/24/test_set`; `results/v69-quant-confirm/compare.json#/rows/25/test_set`; `results/v69-quant-confirm/compare.json#/rows/26/test_set`; `results/v69-quant-confirm/compare.json#/rows/27/test_set`; `results/v69-quant-confirm/compare.json#/rows/28/test_set`; `results/v69-quant-confirm/compare.json#/rows/29/test_set`; `results/v69-quant-confirm/compare.json#/rows/30/test_set`; `results/v69-quant-confirm/compare.json#/rows/31/test_set`; `results/v69-quant-confirm/compare.json#/rows/32/test_set`; `results/v69-quant-confirm/compare.json#/rows/33/test_set`; `results/v69-quant-confirm/compare.json#/rows/34/test_set`; `results/v69-quant-confirm/compare.json#/rows/35/test_set`
- Cell (3, 1): `results/v55-quant-group/register.json#/candidate_definitions/low_order_2d`; `results/v69-quant-confirm/develop.json#/models`; `results/v69-quant-confirm/develop.json#/feature_names`; `results/v69-quant-confirm/develop.json#/dev_configs`; `results/v69-quant-confirm/develop.json#/selected/math/candidate`; `results/v69-quant-confirm/develop.json#/selected/math/n_coefficients`; `results/v69-quant-confirm/develop.json#/selected/code/candidate`; `results/v69-quant-confirm/develop.json#/selected/code/n_coefficients`; `results/v69-quant-confirm/develop.json#/selected/qa/candidate`; `results/v69-quant-confirm/develop.json#/selected/qa/n_coefficients`
- Cell (3, 2): `results/v69-quant-confirm/compare.json#/rows/0/state`; `results/v69-quant-confirm/compare.json#/rows/0/config`; `results/v69-quant-confirm/compare.json#/rows/1/state`; `results/v69-quant-confirm/compare.json#/rows/1/config`; `results/v69-quant-confirm/compare.json#/rows/2/state`; `results/v69-quant-confirm/compare.json#/rows/2/config`; `results/v69-quant-confirm/compare.json#/rows/3/state`; `results/v69-quant-confirm/compare.json#/rows/3/config`; `results/v69-quant-confirm/compare.json#/rows/4/state`; `results/v69-quant-confirm/compare.json#/rows/4/config`; `results/v69-quant-confirm/compare.json#/rows/5/state`; `results/v69-quant-confirm/compare.json#/rows/5/config`; `results/v69-quant-confirm/compare.json#/rows/6/state`; `results/v69-quant-confirm/compare.json#/rows/6/config`; `results/v69-quant-confirm/compare.json#/rows/7/state`; `results/v69-quant-confirm/compare.json#/rows/7/config`; `results/v69-quant-confirm/compare.json#/rows/8/state`; `results/v69-quant-confirm/compare.json#/rows/8/config`; `results/v69-quant-confirm/compare.json#/rows/9/state`; `results/v69-quant-confirm/compare.json#/rows/9/config`; `results/v69-quant-confirm/compare.json#/rows/10/state`; `results/v69-quant-confirm/compare.json#/rows/10/config`; `results/v69-quant-confirm/compare.json#/rows/11/state`; `results/v69-quant-confirm/compare.json#/rows/11/config`; `results/v69-quant-confirm/compare.json#/rows/12/state`; `results/v69-quant-confirm/compare.json#/rows/12/config`; `results/v69-quant-confirm/compare.json#/rows/13/state`; `results/v69-quant-confirm/compare.json#/rows/13/config`; `results/v69-quant-confirm/compare.json#/rows/14/state`; `results/v69-quant-confirm/compare.json#/rows/14/config`; `results/v69-quant-confirm/compare.json#/rows/15/state`; `results/v69-quant-confirm/compare.json#/rows/15/config`; `results/v69-quant-confirm/compare.json#/rows/16/state`; `results/v69-quant-confirm/compare.json#/rows/16/config`; `results/v69-quant-confirm/compare.json#/rows/17/state`; `results/v69-quant-confirm/compare.json#/rows/17/config`; `results/v69-quant-confirm/compare.json#/rows/18/state`; `results/v69-quant-confirm/compare.json#/rows/18/config`; `results/v69-quant-confirm/compare.json#/rows/19/state`; `results/v69-quant-confirm/compare.json#/rows/19/config`; `results/v69-quant-confirm/compare.json#/rows/20/state`; `results/v69-quant-confirm/compare.json#/rows/20/config`; `results/v69-quant-confirm/compare.json#/rows/21/state`; `results/v69-quant-confirm/compare.json#/rows/21/config`; `results/v69-quant-confirm/compare.json#/rows/22/state`; `results/v69-quant-confirm/compare.json#/rows/22/config`; `results/v69-quant-confirm/compare.json#/rows/23/state`; `results/v69-quant-confirm/compare.json#/rows/23/config`; `results/v69-quant-confirm/compare.json#/rows/24/state`; `results/v69-quant-confirm/compare.json#/rows/24/config`; `results/v69-quant-confirm/compare.json#/rows/25/state`; `results/v69-quant-confirm/compare.json#/rows/25/config`; `results/v69-quant-confirm/compare.json#/rows/26/state`; `results/v69-quant-confirm/compare.json#/rows/26/config`; `results/v69-quant-confirm/compare.json#/rows/27/state`; `results/v69-quant-confirm/compare.json#/rows/27/config`; `results/v69-quant-confirm/compare.json#/rows/28/state`; `results/v69-quant-confirm/compare.json#/rows/28/config`; `results/v69-quant-confirm/compare.json#/rows/29/state`; `results/v69-quant-confirm/compare.json#/rows/29/config`; `results/v69-quant-confirm/compare.json#/rows/30/state`; `results/v69-quant-confirm/compare.json#/rows/30/config`; `results/v69-quant-confirm/compare.json#/rows/31/state`; `results/v69-quant-confirm/compare.json#/rows/31/config`; `results/v69-quant-confirm/compare.json#/rows/32/state`; `results/v69-quant-confirm/compare.json#/rows/32/config`; `results/v69-quant-confirm/compare.json#/rows/33/state`; `results/v69-quant-confirm/compare.json#/rows/33/config`; `results/v69-quant-confirm/compare.json#/rows/34/state`; `results/v69-quant-confirm/compare.json#/rows/34/config`; `results/v69-quant-confirm/compare.json#/rows/35/state`; `results/v69-quant-confirm/compare.json#/rows/35/config`
- Cell (3, 3): `results/v69-quant-confirm/compare.json#/rows/0/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/3/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/6/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/9/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/12/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/15/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/18/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/21/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/24/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/27/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/30/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/33/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/1/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/4/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/7/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/10/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/13/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/16/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/19/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/22/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/25/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/28/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/31/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/34/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/2/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/5/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/8/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/11/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/14/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/17/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/20/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/23/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/26/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/29/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/32/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/35/absolute_errors/zero`
- Cell (3, 4): `results/v69-quant-confirm/develop.json#/loso/scores`; `results/v69-quant-confirm/develop.json#/loso/scores/bilinear/math`; `results/v69-quant-confirm/compare.json#/rows/0/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/3/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/6/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/9/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/12/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/15/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/18/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/21/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/24/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/27/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/30/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/33/absolute_errors/bilinear`; `results/v69-quant-confirm/develop.json#/loso/scores/zero/code`; `results/v69-quant-confirm/compare.json#/rows/1/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/4/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/7/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/10/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/13/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/16/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/19/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/22/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/25/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/28/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/31/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/34/absolute_errors/zero`; `results/v69-quant-confirm/develop.json#/loso/scores/median/qa`; `results/v69-quant-confirm/compare.json#/rows/2/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/5/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/8/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/11/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/14/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/17/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/20/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/23/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/26/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/29/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/32/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/35/absolute_errors/median`
- Cell (3, 5): `results/v69-quant-confirm/freeze.json#/frozen_at_utc`
- Cell (4, 0): `results/v69-quant-confirm/compare.json#/rows/36/test_set`; `results/v69-quant-confirm/compare.json#/rows/37/test_set`; `results/v69-quant-confirm/compare.json#/rows/38/test_set`; `results/v69-quant-confirm/compare.json#/rows/39/test_set`; `results/v69-quant-confirm/compare.json#/rows/40/test_set`; `results/v69-quant-confirm/compare.json#/rows/41/test_set`; `results/v69-quant-confirm/compare.json#/rows/42/test_set`; `results/v69-quant-confirm/compare.json#/rows/43/test_set`; `results/v69-quant-confirm/compare.json#/rows/44/test_set`; `results/v69-quant-confirm/compare.json#/rows/45/test_set`; `results/v69-quant-confirm/compare.json#/rows/46/test_set`; `results/v69-quant-confirm/compare.json#/rows/47/test_set`; `results/v69-quant-confirm/compare.json#/rows/48/test_set`; `results/v69-quant-confirm/compare.json#/rows/49/test_set`; `results/v69-quant-confirm/compare.json#/rows/50/test_set`; `results/v69-quant-confirm/compare.json#/rows/51/test_set`; `results/v69-quant-confirm/compare.json#/rows/52/test_set`; `results/v69-quant-confirm/compare.json#/rows/53/test_set`; `results/v69-quant-confirm/compare.json#/rows/54/test_set`; `results/v69-quant-confirm/compare.json#/rows/55/test_set`; `results/v69-quant-confirm/compare.json#/rows/56/test_set`; `results/v69-quant-confirm/compare.json#/rows/57/test_set`; `results/v69-quant-confirm/compare.json#/rows/58/test_set`; `results/v69-quant-confirm/compare.json#/rows/59/test_set`; `results/v69-quant-confirm/compare.json#/rows/60/test_set`; `results/v69-quant-confirm/compare.json#/rows/61/test_set`; `results/v69-quant-confirm/compare.json#/rows/62/test_set`
- Cell (4, 1): `results/v55-quant-group/register.json#/candidate_definitions/low_order_2d`; `results/v69-quant-confirm/develop.json#/models`; `results/v69-quant-confirm/develop.json#/feature_names`; `results/v69-quant-confirm/develop.json#/dev_configs`; `results/v69-quant-confirm/develop.json#/selected/math/candidate`; `results/v69-quant-confirm/develop.json#/selected/math/n_coefficients`; `results/v69-quant-confirm/develop.json#/selected/code/candidate`; `results/v69-quant-confirm/develop.json#/selected/code/n_coefficients`; `results/v69-quant-confirm/develop.json#/selected/qa/candidate`; `results/v69-quant-confirm/develop.json#/selected/qa/n_coefficients`
- Cell (4, 2): `results/v69-quant-confirm/compare.json#/rows/36/state`; `results/v69-quant-confirm/compare.json#/rows/36/config`; `results/v69-quant-confirm/compare.json#/rows/37/state`; `results/v69-quant-confirm/compare.json#/rows/37/config`; `results/v69-quant-confirm/compare.json#/rows/38/state`; `results/v69-quant-confirm/compare.json#/rows/38/config`; `results/v69-quant-confirm/compare.json#/rows/39/state`; `results/v69-quant-confirm/compare.json#/rows/39/config`; `results/v69-quant-confirm/compare.json#/rows/40/state`; `results/v69-quant-confirm/compare.json#/rows/40/config`; `results/v69-quant-confirm/compare.json#/rows/41/state`; `results/v69-quant-confirm/compare.json#/rows/41/config`; `results/v69-quant-confirm/compare.json#/rows/42/state`; `results/v69-quant-confirm/compare.json#/rows/42/config`; `results/v69-quant-confirm/compare.json#/rows/43/state`; `results/v69-quant-confirm/compare.json#/rows/43/config`; `results/v69-quant-confirm/compare.json#/rows/44/state`; `results/v69-quant-confirm/compare.json#/rows/44/config`; `results/v69-quant-confirm/compare.json#/rows/45/state`; `results/v69-quant-confirm/compare.json#/rows/45/config`; `results/v69-quant-confirm/compare.json#/rows/46/state`; `results/v69-quant-confirm/compare.json#/rows/46/config`; `results/v69-quant-confirm/compare.json#/rows/47/state`; `results/v69-quant-confirm/compare.json#/rows/47/config`; `results/v69-quant-confirm/compare.json#/rows/48/state`; `results/v69-quant-confirm/compare.json#/rows/48/config`; `results/v69-quant-confirm/compare.json#/rows/49/state`; `results/v69-quant-confirm/compare.json#/rows/49/config`; `results/v69-quant-confirm/compare.json#/rows/50/state`; `results/v69-quant-confirm/compare.json#/rows/50/config`; `results/v69-quant-confirm/compare.json#/rows/51/state`; `results/v69-quant-confirm/compare.json#/rows/51/config`; `results/v69-quant-confirm/compare.json#/rows/52/state`; `results/v69-quant-confirm/compare.json#/rows/52/config`; `results/v69-quant-confirm/compare.json#/rows/53/state`; `results/v69-quant-confirm/compare.json#/rows/53/config`; `results/v69-quant-confirm/compare.json#/rows/54/state`; `results/v69-quant-confirm/compare.json#/rows/54/config`; `results/v69-quant-confirm/compare.json#/rows/55/state`; `results/v69-quant-confirm/compare.json#/rows/55/config`; `results/v69-quant-confirm/compare.json#/rows/56/state`; `results/v69-quant-confirm/compare.json#/rows/56/config`; `results/v69-quant-confirm/compare.json#/rows/57/state`; `results/v69-quant-confirm/compare.json#/rows/57/config`; `results/v69-quant-confirm/compare.json#/rows/58/state`; `results/v69-quant-confirm/compare.json#/rows/58/config`; `results/v69-quant-confirm/compare.json#/rows/59/state`; `results/v69-quant-confirm/compare.json#/rows/59/config`; `results/v69-quant-confirm/compare.json#/rows/60/state`; `results/v69-quant-confirm/compare.json#/rows/60/config`; `results/v69-quant-confirm/compare.json#/rows/61/state`; `results/v69-quant-confirm/compare.json#/rows/61/config`; `results/v69-quant-confirm/compare.json#/rows/62/state`; `results/v69-quant-confirm/compare.json#/rows/62/config`
- Cell (4, 3): `results/v69-quant-confirm/compare.json#/rows/36/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/39/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/42/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/45/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/48/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/51/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/54/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/57/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/60/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/37/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/40/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/43/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/46/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/49/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/52/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/55/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/58/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/61/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/38/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/41/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/44/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/47/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/50/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/53/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/56/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/59/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/62/absolute_errors/zero`
- Cell (4, 4): `results/v69-quant-confirm/develop.json#/loso/scores`; `results/v69-quant-confirm/develop.json#/loso/scores/bilinear/math`; `results/v69-quant-confirm/compare.json#/rows/36/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/39/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/42/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/45/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/48/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/51/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/54/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/57/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/60/absolute_errors/bilinear`; `results/v69-quant-confirm/develop.json#/loso/scores/zero/code`; `results/v69-quant-confirm/compare.json#/rows/37/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/40/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/43/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/46/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/49/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/52/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/55/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/58/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/61/absolute_errors/zero`; `results/v69-quant-confirm/develop.json#/loso/scores/median/qa`; `results/v69-quant-confirm/compare.json#/rows/38/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/41/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/44/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/47/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/50/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/53/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/56/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/59/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/62/absolute_errors/median`
- Cell (4, 5): `results/v69-quant-confirm/freeze.json#/frozen_at_utc`
- Cell (5, 0): `results/a2-curvature-interaction/summary.json#/decision_table/18/target`; `results/a2-curvature-interaction/summary.json#/decision_table/6/target`; `results/a2-curvature-interaction/summary.json#/decision_table/54/target`
- Cell (5, 1): `results/a2-curvature-interaction/summary.json#/protocol/structures`; `results/a2-curvature-interaction/summary.json#/protocol/descriptors`; `results/a2-curvature-interaction/summary.json#/protocol/descriptor_calibration_cost`; `results/a2-curvature-interaction/summary.json#/protocol/structures/F_log`; `results/a2-curvature-interaction/summary.json#/parameter_intervals/0/fits/F_log/fit/nominal_parameters`; `results/a2-curvature-interaction/summary.json#/protocol/structures/F_curv`; `results/a2-curvature-interaction/summary.json#/parameter_intervals/0/fits/F_curv/fit/nominal_parameters`; `results/a2-curvature-interaction/summary.json#/protocol/structures/F_int`; `results/a2-curvature-interaction/summary.json#/parameter_intervals/0/fits/F_int/fit/nominal_parameters`
- Cell (5, 2): `results/a2-curvature-interaction/summary.json#/decision_table/18/distribution`; `results/a2-curvature-interaction/summary.json#/decision_table/6/distribution`; `results/a2-curvature-interaction/summary.json#/decision_table/54/distribution`; `results/a2-curvature-interaction/summary.json#/parameter_intervals/0/fits/F_log/fit/standardizer/students`; `results/a2-curvature-interaction/summary.json#/protocol/largest_budget`
- Cell (5, 3): `results/a2-curvature-interaction/summary.json#/decision_table/18/primary_mae`; `results/a2-curvature-interaction/summary.json#/decision_table/18/primary_mae_interval/0`; `results/a2-curvature-interaction/summary.json#/decision_table/18/primary_mae_interval/1`; `results/a2-curvature-interaction/summary.json#/decision_table/6/primary_mae`; `results/a2-curvature-interaction/summary.json#/decision_table/6/primary_mae_interval/0`; `results/a2-curvature-interaction/summary.json#/decision_table/6/primary_mae_interval/1`; `results/a2-curvature-interaction/summary.json#/decision_table/54/primary_mae`; `results/a2-curvature-interaction/summary.json#/decision_table/54/primary_mae_interval/0`; `results/a2-curvature-interaction/summary.json#/decision_table/54/primary_mae_interval/1`
- Cell (5, 4): `results/a2-curvature-interaction/summary.json#/decision_table/18/inner_selected_baselines`; `results/a2-curvature-interaction/summary.json#/decision_table/18/baseline_mae`; `results/a2-curvature-interaction/summary.json#/decision_table/6/inner_selected_baselines`; `results/a2-curvature-interaction/summary.json#/decision_table/6/baseline_mae`; `results/a2-curvature-interaction/summary.json#/decision_table/54/inner_selected_baselines`; `results/a2-curvature-interaction/summary.json#/decision_table/54/baseline_mae`
- Cell (5, 5): `results/a2-curvature-interaction/summary.json#/protocol/secondary`; `results/a2-curvature-interaction/summary.json#/protocol/previous_F_int`
- Cell (6, 0): `results/a2-curvature-interaction/summary.json#/decision_table/14/target`; `results/a2-curvature-interaction/summary.json#/decision_table/2/target`; `results/a2-curvature-interaction/summary.json#/decision_table/50/target`
- Cell (6, 1): `results/a2-curvature-interaction/summary.json#/protocol/structures`; `results/a2-curvature-interaction/summary.json#/protocol/descriptors`; `results/a2-curvature-interaction/summary.json#/protocol/descriptor_calibration_cost`; `results/a2-curvature-interaction/summary.json#/protocol/structures/F_log`; `results/a2-curvature-interaction/summary.json#/parameter_intervals/0/fits/F_log/fit/nominal_parameters`; `results/a2-curvature-interaction/summary.json#/protocol/structures/F_curv`; `results/a2-curvature-interaction/summary.json#/parameter_intervals/0/fits/F_curv/fit/nominal_parameters`; `results/a2-curvature-interaction/summary.json#/protocol/structures/F_int`; `results/a2-curvature-interaction/summary.json#/parameter_intervals/0/fits/F_int/fit/nominal_parameters`
- Cell (6, 2): `results/a2-curvature-interaction/summary.json#/decision_table/14/distribution`; `results/a2-curvature-interaction/summary.json#/decision_table/2/distribution`; `results/a2-curvature-interaction/summary.json#/decision_table/50/distribution`; `results/a2-curvature-interaction/summary.json#/parameter_intervals/0/fits/F_curv/fit/standardizer/students`; `results/a2-curvature-interaction/summary.json#/protocol/I_U`
- Cell (6, 3): `results/a2-curvature-interaction/summary.json#/decision_table/14/primary_mae`; `results/a2-curvature-interaction/summary.json#/decision_table/14/primary_mae_interval/0`; `results/a2-curvature-interaction/summary.json#/decision_table/14/primary_mae_interval/1`; `results/a2-curvature-interaction/summary.json#/decision_table/2/primary_mae`; `results/a2-curvature-interaction/summary.json#/decision_table/2/primary_mae_interval/0`; `results/a2-curvature-interaction/summary.json#/decision_table/2/primary_mae_interval/1`; `results/a2-curvature-interaction/summary.json#/decision_table/50/primary_mae`; `results/a2-curvature-interaction/summary.json#/decision_table/50/primary_mae_interval/0`; `results/a2-curvature-interaction/summary.json#/decision_table/50/primary_mae_interval/1`
- Cell (6, 4): `results/a2-curvature-interaction/summary.json#/decision_table/14/inner_selected_baselines`; `results/a2-curvature-interaction/summary.json#/decision_table/14/baseline_mae`; `results/a2-curvature-interaction/summary.json#/decision_table/2/inner_selected_baselines`; `results/a2-curvature-interaction/summary.json#/decision_table/2/baseline_mae`; `results/a2-curvature-interaction/summary.json#/decision_table/50/inner_selected_baselines`; `results/a2-curvature-interaction/summary.json#/decision_table/50/baseline_mae`
- Cell (6, 5): `results/a2-curvature-interaction/summary.json#/protocol/secondary`; `results/a2-curvature-interaction/summary.json#/protocol/previous_F_int`
- Cell (7, 0): `results/v70-distill-confirm/freeze.json#/confirmation_register/unused_U_assertion`
- Cell (7, 1): `results/v70-distill-confirm/freeze.json#/models`; `results/v70-distill-confirm/freeze.json#/reference_rule`; `results/v70-distill-confirm/freeze.json#/prediction_rule`; `results/v70-distill-confirm/freeze.json#/selected/math/method`; `results/v70-distill-confirm/freeze.json#/selected/math/n_params`; `results/v70-distill-confirm/freeze.json#/selected/code/method`; `results/v70-distill-confirm/freeze.json#/selected/code/n_params`; `results/v70-distill-confirm/freeze.json#/selected/qa/method`; `results/v70-distill-confirm/freeze.json#/selected/qa/n_params`
- Cell (7, 2): `results/v70-distill-confirm/freeze.json#/confirmation_register/students`; `results/v70-distill-confirm/freeze.json#/confirmation_register/pools`; `results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned`
- Cell (7, 3): `results/v70-distill-confirm/freeze.json#/confirmation_register/students`; `results/v70-distill-confirm/compare.json#/groups/0/candidate_mae`; `results/v70-distill-confirm/compare.json#/groups/3/candidate_mae`; `results/v70-distill-confirm/compare.json#/groups/1/candidate_mae`; `results/v70-distill-confirm/compare.json#/groups/4/candidate_mae`; `results/v70-distill-confirm/compare.json#/groups/2/candidate_mae`; `results/v70-distill-confirm/compare.json#/groups/5/candidate_mae`
- Cell (7, 4): `results/v70-distill-confirm/freeze.json#/baseline_rule`; `results/v70-distill-confirm/freeze.json#/strongest_baseline`; `results/v70-distill-confirm/compare.json#/groups/0/paired_difference`; `results/v70-distill-confirm/compare.json#/groups/1/paired_difference`; `results/v70-distill-confirm/compare.json#/groups/2/paired_difference`; `results/v70-distill-confirm/compare.json#/groups/3/paired_difference`; `results/v70-distill-confirm/compare.json#/groups/4/paired_difference`; `results/v70-distill-confirm/compare.json#/groups/5/paired_difference`; `results/v70-distill-confirm/compare.json#/groups/0/strongest_baseline`; `results/v70-distill-confirm/compare.json#/groups/3/strongest_baseline`; `results/v70-distill-confirm/compare.json#/groups/0/baseline_mae`; `results/v70-distill-confirm/compare.json#/groups/3/baseline_mae`; `results/v70-distill-confirm/compare.json#/groups/1/strongest_baseline`; `results/v70-distill-confirm/compare.json#/groups/4/strongest_baseline`; `results/v70-distill-confirm/compare.json#/groups/1/baseline_mae`; `results/v70-distill-confirm/compare.json#/groups/4/baseline_mae`; `results/v70-distill-confirm/compare.json#/groups/2/strongest_baseline`; `results/v70-distill-confirm/compare.json#/groups/5/strongest_baseline`; `results/v70-distill-confirm/compare.json#/groups/2/baseline_mae`; `results/v70-distill-confirm/compare.json#/groups/5/baseline_mae`
- Cell (7, 5): `results/v70-distill-confirm/freeze.json#/frozen_at_utc`; `results/v47-p2-register/register.json#/v5_confirm/registered_at_utc`

## Machine-readable cell recipes

```json
[
  {
    "row": 0,
    "column": 0,
    "parts": [
      "Prune: density"
    ],
    "context": [
      "results/v53-prune-dev/register.json#/loso_folds"
    ],
    "note": "The requested nine-state leave-density-out DEVELOPMENT evaluation is absent from the supplied V53 files. register.json records n_dev_states=17 and loso_folds/loso_predictions hold out source states, not densities. predictions_<tag>.json contains new-source predictions only. V40 documents the original nine-state panel and its [0.6, 0.9] grid, but does not supply the requested density-holdout errors. No LOSO, training-fit or identical-weight repeat errors are substituted.",
    "rendered": "Prune: density"
  },
  {
    "row": 0,
    "column": 1,
    "parts": [
      {
        "sources": [
          "results/v53-prune-dev/register.json#/candidate_definitions/power"
        ],
        "op": "label",
        "format": null,
        "label": "$A_c(\\mathbf x)r^{\\gamma_c}$",
        "expected": [
          "(beta.phi) * ((1-d)/0.3)**gamma"
        ]
      },
      " (",
      {
        "sources": [
          "results/v53-prune-dev/register.json#/n_params_per_capability/power"
        ],
        "op": "identity",
        "format": null
      },
      ")"
    ],
    "context": [
      "results/v53-prune-dev/register.json#/feature_names"
    ],
    "note": "",
    "rendered": "$A_c(\\mathbf x)r^{\\gamma_c}$ (5)"
  },
  {
    "row": 0,
    "column": 2,
    "parts": [
      {
        "sources": [
          "results/v40-prune-strength/register.json#/dev"
        ],
        "op": "label",
        "format": null,
        "label": "9 states; d=0.6-0.9",
        "expected": [
          {
            "sizes": [
              "160m",
              "410m",
              "1.4b"
            ],
            "steps": [
              16000,
              64000,
              143000
            ],
            "seen_densities": [
              0.9,
              0.8,
              0.7,
              0.6
            ],
            "n_rows": 108
          }
        ]
      }
    ],
    "context": [],
    "note": "Requested scope, not an assertion that this holdout artifact exists.",
    "rendered": "9 states; d=0.6-0.9"
  },
  {
    "row": 0,
    "column": 3,
    "parts": [
      "not tested"
    ],
    "context": [
      "results/v53-prune-dev/register.json#/loso_predictions"
    ],
    "note": "The requested nine-state leave-density-out DEVELOPMENT evaluation is absent from the supplied V53 files. register.json records n_dev_states=17 and loso_folds/loso_predictions hold out source states, not densities. predictions_<tag>.json contains new-source predictions only. V40 documents the original nine-state panel and its [0.6, 0.9] grid, but does not supply the requested density-holdout errors. No LOSO, training-fit or identical-weight repeat errors are substituted.",
    "rendered": "not tested"
  },
  {
    "row": 0,
    "column": 4,
    "parts": [
      "not tested"
    ],
    "context": [
      "results/v53-prune-dev/register.json#/loso_table"
    ],
    "note": "The requested nine-state leave-density-out DEVELOPMENT evaluation is absent from the supplied V53 files. register.json records n_dev_states=17 and loso_folds/loso_predictions hold out source states, not densities. predictions_<tag>.json contains new-source predictions only. V40 documents the original nine-state panel and its [0.6, 0.9] grid, but does not supply the requested density-holdout errors. No LOSO, training-fit or identical-weight repeat errors are substituted.",
    "rendered": "not tested"
  },
  {
    "row": 0,
    "column": 5,
    "parts": [
      "development"
    ],
    "context": [
      "results/v53-prune-dev/register.json#/selection_rule"
    ],
    "note": "Requested evaluation status; no scores claimed.",
    "rendered": "devel\\-opment"
  },
  {
    "row": 1,
    "column": 0,
    "parts": [
      "Prune: state"
    ],
    "context": [
      "results/v53-prune-dev/register.json#/selected_candidate"
    ],
    "note": "",
    "rendered": "Prune: state"
  },
  {
    "row": 1,
    "column": 1,
    "parts": [
      {
        "sources": [
          "results/v53-prune-dev/register.json#/candidate_definitions/power"
        ],
        "op": "label",
        "format": null,
        "label": "$A_c(\\mathbf x)r^{\\gamma_c}$",
        "expected": [
          "(beta.phi) * ((1-d)/0.3)**gamma"
        ]
      },
      " (",
      {
        "sources": [
          "results/v53-prune-dev/register.json#/n_params_per_capability/power"
        ],
        "op": "identity",
        "format": null
      },
      ")"
    ],
    "context": [
      "results/v53-prune-dev/register.json#/feature_names"
    ],
    "note": "",
    "rendered": "$A_c(\\mathbf x)r^{\\gamma_c}$ (5)"
  },
  {
    "row": 1,
    "column": 2,
    "parts": [
      {
        "sources": [
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/tag",
          "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/tag",
          "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/tag",
          "results/v40-prune-strength/register.json#/dev/sizes"
        ],
        "op": "label",
        "format": null,
        "label": "seen-size stages; 6.9B outside",
        "expected": [
          "pythia-410m@step48000",
          "pythia-1.4b@step112000",
          "pythia-6.9b@step80000",
          [
            "160m",
            "410m",
            "1.4b"
          ]
        ]
      }
    ],
    "context": [
      "results/v53-prune-dev/compare_pythia-410m@step48000.json#/densities"
    ],
    "note": "Outside the size range of the original nine-state panel; V53's expanded register itself includes 6.9B.",
    "rendered": "seen-size stages; 6.9B outside"
  },
  {
    "row": 1,
    "column": 3,
    "parts": [
      "math ",
      {
        "sources": [
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/power/math",
          "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/power/math",
          "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/power/math"
        ],
        "op": "mean",
        "format": ".2f"
      },
      " / ",
      "code ",
      {
        "sources": [
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/power/code",
          "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/power/code",
          "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/power/code"
        ],
        "op": "mean",
        "format": ".2f"
      },
      " / ",
      "QA ",
      {
        "sources": [
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/power/qa",
          "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/power/qa",
          "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/power/qa"
        ],
        "op": "mean",
        "format": ".2f"
      }
    ],
    "context": [],
    "note": "",
    "rendered": "math 0.24/ code 0.24/ QA 0.68"
  },
  {
    "row": 1,
    "column": 4,
    "parts": [
      {
        "sources": [
          "results/v53-prune-dev/register.json#/loso_table/2/candidate"
        ],
        "op": "label",
        "format": null,
        "label": "A2",
        "expected": [
          "A2"
        ]
      },
      " ",
      {
        "sources": [
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/A2/math",
          "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/A2/math",
          "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/A2/math"
        ],
        "op": "mean",
        "format": ".2f"
      },
      " / ",
      {
        "sources": [
          "results/v53-prune-dev/register.json#/loso_table/2/candidate"
        ],
        "op": "label",
        "format": null,
        "label": "A2",
        "expected": [
          "A2"
        ]
      },
      " ",
      {
        "sources": [
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/A2/code",
          "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/A2/code",
          "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/A2/code"
        ],
        "op": "mean",
        "format": ".2f"
      },
      " / ",
      {
        "sources": [
          "results/v53-prune-dev/register.json#/loso_table/5/candidate"
        ],
        "op": "label",
        "format": null,
        "label": "med",
        "expected": [
          "median_curve"
        ]
      },
      " ",
      {
        "sources": [
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/qa",
          "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/qa",
          "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/qa"
        ],
        "op": "mean",
        "format": ".2f"
      }
    ],
    "context": [
      "results/v53-prune-dev/register.json#/loso_table"
    ],
    "note": "Minimum development LOSO MAE excluding power, per capability; no test ranking.",
    "rendered": "A2 0.23/ A2 0.22/ med 0.22"
  },
  {
    "row": 1,
    "column": 5,
    "parts": [
      "frozen prediction"
    ],
    "context": [
      "results/v53-prune-dev/register.json#/selected_candidate"
    ],
    "note": "",
    "rendered": "frozen prediction"
  },
  {
    "row": 2,
    "column": 0,
    "parts": [
      "Quant: bits"
    ],
    "context": [
      "results/v55-quant-group/register.json#/test_sets/bit_test"
    ],
    "note": "",
    "rendered": "Quant: bits"
  },
  {
    "row": 2,
    "column": 1,
    "parts": [
      {
        "sources": [
          "results/v55-quant-group/register.json#/candidate_definitions/low_order_2d"
        ],
        "op": "label",
        "format": null,
        "label": "$\\phi^\\top Q_c$",
        "expected": [
          "phi.[a0 + a1*u + a2*v + a3*u*v + a4*u^2]; coefficients ordered by term then phi"
        ]
      },
      " (",
      {
        "sources": [
          "results/v55-quant-group/register.json#/n_params_per_capability/low_order_2d"
        ],
        "op": "identity",
        "format": null
      },
      ")"
    ],
    "context": [
      "results/v55-quant-group/register.json#/feature_names"
    ],
    "note": "",
    "rendered": "$\\phi^\\top Q_c$ (20)"
  },
  {
    "row": 2,
    "column": 2,
    "parts": [
      {
        "sources": [
          "results/v55-quant-group/register.json#/test_sets/bit_test/states",
          "results/v55-quant-group/register.json#/test_sets/bit_test/configs"
        ],
        "op": "label",
        "format": null,
        "label": "160M-1.4B; b4/g64,256",
        "expected": [
          [
            "pythia-160m@step16000",
            "pythia-160m@step143000",
            "pythia-410m@step16000",
            "pythia-410m@step143000",
            "pythia-1.4b@step16000",
            "pythia-1.4b@step143000"
          ],
          [
            "b4_g64",
            "b4_g256"
          ]
        ]
      }
    ],
    "context": [],
    "note": "",
    "rendered": "160M-1.4B; b4/g64,256"
  },
  {
    "row": 2,
    "column": 3,
    "parts": [
      "math ",
      {
        "sources": [
          "results/v55-quant-group/compare.json#/test_sets/bit_test/mae_table/1/mae/math"
        ],
        "op": "identity",
        "format": ".2f"
      },
      " / ",
      "code ",
      {
        "sources": [
          "results/v55-quant-group/compare.json#/test_sets/bit_test/mae_table/1/mae/code"
        ],
        "op": "identity",
        "format": ".2f"
      },
      " / ",
      "QA ",
      {
        "sources": [
          "results/v55-quant-group/compare.json#/test_sets/bit_test/mae_table/1/mae/qa"
        ],
        "op": "identity",
        "format": ".2f"
      }
    ],
    "context": [],
    "note": "",
    "rendered": "math 0.19/ code 0.21/ QA 0.44"
  },
  {
    "row": 2,
    "column": 4,
    "parts": [
      {
        "sources": [
          "results/v55-quant-group/register.json#/loso_table/4/candidate"
        ],
        "op": "label",
        "format": null,
        "label": "med",
        "expected": [
          "median"
        ]
      },
      " ",
      {
        "sources": [
          "results/v55-quant-group/compare.json#/test_sets/bit_test/mae_table/4/mae/math"
        ],
        "op": "identity",
        "format": ".2f"
      },
      " / ",
      {
        "sources": [
          "results/v55-quant-group/register.json#/loso_table/4/candidate"
        ],
        "op": "label",
        "format": null,
        "label": "med",
        "expected": [
          "median"
        ]
      },
      " ",
      {
        "sources": [
          "results/v55-quant-group/compare.json#/test_sets/bit_test/mae_table/4/mae/code"
        ],
        "op": "identity",
        "format": ".2f"
      },
      " / ",
      {
        "sources": [
          "results/v55-quant-group/register.json#/loso_table/4/candidate"
        ],
        "op": "label",
        "format": null,
        "label": "med",
        "expected": [
          "median"
        ]
      },
      " ",
      {
        "sources": [
          "results/v55-quant-group/compare.json#/test_sets/bit_test/mae_table/4/mae/qa"
        ],
        "op": "identity",
        "format": ".2f"
      }
    ],
    "context": [
      "results/v55-quant-group/register.json#/loso_table"
    ],
    "note": "Development minimum over registered baselines mean/median/zero.",
    "rendered": "med 0.55/ med 0.73/ med 0.54"
  },
  {
    "row": 2,
    "column": 5,
    "parts": [
      "frozen prediction"
    ],
    "context": [
      "results/v55-quant-group/register.json#/precommitted_rule"
    ],
    "note": "",
    "rendered": "frozen prediction"
  },
  {
    "row": 3,
    "column": 0,
    "parts": [
      "Quant: group"
    ],
    "context": [
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
    "rendered": "Quant: group"
  },
  {
    "row": 3,
    "column": 1,
    "parts": [
      "math: ",
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/selected/math/candidate"
        ],
        "op": "label",
        "format": null,
        "label": "$\\phi^\\top Q_c$",
        "expected": [
          "low_order_2d"
        ]
      },
      " (",
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/selected/math/n_coefficients"
        ],
        "op": "identity",
        "format": null
      },
      ")",
      "; ",
      "code: ",
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/selected/code/candidate"
        ],
        "op": "label",
        "format": null,
        "label": "$m_c(b,g)$",
        "expected": [
          "median"
        ]
      },
      " (",
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/selected/code/n_coefficients"
        ],
        "op": "identity",
        "format": null
      },
      ")",
      "; ",
      "QA: ",
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/selected/qa/candidate"
        ],
        "op": "label",
        "format": null,
        "label": "$0$",
        "expected": [
          "zero"
        ]
      },
      " (",
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/selected/qa/n_coefficients"
        ],
        "op": "identity",
        "format": null
      },
      ")"
    ],
    "context": [
      "results/v55-quant-group/register.json#/candidate_definitions/low_order_2d",
      "results/v69-quant-confirm/develop.json#/models",
      "results/v69-quant-confirm/develop.json#/feature_names",
      "results/v69-quant-confirm/develop.json#/dev_configs"
    ],
    "note": "Surface is phi.[a0+a1*u+a2*v+a3*u*v+a4*u^2]; median is per configuration; zero is identically zero.",
    "rendered": "math: $\\phi^\\top Q_c$ (20); code: $m_c(b,g)$ (9); QA: $0$ (0)"
  },
  {
    "row": 3,
    "column": 2,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/rows/0/state",
          "results/v69-quant-confirm/compare.json#/rows/0/config",
          "results/v69-quant-confirm/compare.json#/rows/1/state",
          "results/v69-quant-confirm/compare.json#/rows/1/config",
          "results/v69-quant-confirm/compare.json#/rows/2/state",
          "results/v69-quant-confirm/compare.json#/rows/2/config",
          "results/v69-quant-confirm/compare.json#/rows/3/state",
          "results/v69-quant-confirm/compare.json#/rows/3/config",
          "results/v69-quant-confirm/compare.json#/rows/4/state",
          "results/v69-quant-confirm/compare.json#/rows/4/config",
          "results/v69-quant-confirm/compare.json#/rows/5/state",
          "results/v69-quant-confirm/compare.json#/rows/5/config",
          "results/v69-quant-confirm/compare.json#/rows/6/state",
          "results/v69-quant-confirm/compare.json#/rows/6/config",
          "results/v69-quant-confirm/compare.json#/rows/7/state",
          "results/v69-quant-confirm/compare.json#/rows/7/config",
          "results/v69-quant-confirm/compare.json#/rows/8/state",
          "results/v69-quant-confirm/compare.json#/rows/8/config",
          "results/v69-quant-confirm/compare.json#/rows/9/state",
          "results/v69-quant-confirm/compare.json#/rows/9/config",
          "results/v69-quant-confirm/compare.json#/rows/10/state",
          "results/v69-quant-confirm/compare.json#/rows/10/config",
          "results/v69-quant-confirm/compare.json#/rows/11/state",
          "results/v69-quant-confirm/compare.json#/rows/11/config",
          "results/v69-quant-confirm/compare.json#/rows/12/state",
          "results/v69-quant-confirm/compare.json#/rows/12/config",
          "results/v69-quant-confirm/compare.json#/rows/13/state",
          "results/v69-quant-confirm/compare.json#/rows/13/config",
          "results/v69-quant-confirm/compare.json#/rows/14/state",
          "results/v69-quant-confirm/compare.json#/rows/14/config",
          "results/v69-quant-confirm/compare.json#/rows/15/state",
          "results/v69-quant-confirm/compare.json#/rows/15/config",
          "results/v69-quant-confirm/compare.json#/rows/16/state",
          "results/v69-quant-confirm/compare.json#/rows/16/config",
          "results/v69-quant-confirm/compare.json#/rows/17/state",
          "results/v69-quant-confirm/compare.json#/rows/17/config",
          "results/v69-quant-confirm/compare.json#/rows/18/state",
          "results/v69-quant-confirm/compare.json#/rows/18/config",
          "results/v69-quant-confirm/compare.json#/rows/19/state",
          "results/v69-quant-confirm/compare.json#/rows/19/config",
          "results/v69-quant-confirm/compare.json#/rows/20/state",
          "results/v69-quant-confirm/compare.json#/rows/20/config",
          "results/v69-quant-confirm/compare.json#/rows/21/state",
          "results/v69-quant-confirm/compare.json#/rows/21/config",
          "results/v69-quant-confirm/compare.json#/rows/22/state",
          "results/v69-quant-confirm/compare.json#/rows/22/config",
          "results/v69-quant-confirm/compare.json#/rows/23/state",
          "results/v69-quant-confirm/compare.json#/rows/23/config",
          "results/v69-quant-confirm/compare.json#/rows/24/state",
          "results/v69-quant-confirm/compare.json#/rows/24/config",
          "results/v69-quant-confirm/compare.json#/rows/25/state",
          "results/v69-quant-confirm/compare.json#/rows/25/config",
          "results/v69-quant-confirm/compare.json#/rows/26/state",
          "results/v69-quant-confirm/compare.json#/rows/26/config",
          "results/v69-quant-confirm/compare.json#/rows/27/state",
          "results/v69-quant-confirm/compare.json#/rows/27/config",
          "results/v69-quant-confirm/compare.json#/rows/28/state",
          "results/v69-quant-confirm/compare.json#/rows/28/config",
          "results/v69-quant-confirm/compare.json#/rows/29/state",
          "results/v69-quant-confirm/compare.json#/rows/29/config",
          "results/v69-quant-confirm/compare.json#/rows/30/state",
          "results/v69-quant-confirm/compare.json#/rows/30/config",
          "results/v69-quant-confirm/compare.json#/rows/31/state",
          "results/v69-quant-confirm/compare.json#/rows/31/config",
          "results/v69-quant-confirm/compare.json#/rows/32/state",
          "results/v69-quant-confirm/compare.json#/rows/32/config",
          "results/v69-quant-confirm/compare.json#/rows/33/state",
          "results/v69-quant-confirm/compare.json#/rows/33/config",
          "results/v69-quant-confirm/compare.json#/rows/34/state",
          "results/v69-quant-confirm/compare.json#/rows/34/config",
          "results/v69-quant-confirm/compare.json#/rows/35/state",
          "results/v69-quant-confirm/compare.json#/rows/35/config"
        ],
        "op": "label",
        "format": null,
        "label": "410M/1.4B; bits 3-5, g32/512",
        "expected": [
          "pythia-410m@step143000",
          "b3_g32",
          "pythia-410m@step143000",
          "b3_g32",
          "pythia-410m@step143000",
          "b3_g32",
          "pythia-410m@step143000",
          "b3_g512",
          "pythia-410m@step143000",
          "b3_g512",
          "pythia-410m@step143000",
          "b3_g512",
          "pythia-410m@step143000",
          "b4_g32",
          "pythia-410m@step143000",
          "b4_g32",
          "pythia-410m@step143000",
          "b4_g32",
          "pythia-410m@step143000",
          "b4_g512",
          "pythia-410m@step143000",
          "b4_g512",
          "pythia-410m@step143000",
          "b4_g512",
          "pythia-410m@step143000",
          "b5_g32",
          "pythia-410m@step143000",
          "b5_g32",
          "pythia-410m@step143000",
          "b5_g32",
          "pythia-410m@step143000",
          "b5_g512",
          "pythia-410m@step143000",
          "b5_g512",
          "pythia-410m@step143000",
          "b5_g512",
          "pythia-1.4b@step16000",
          "b3_g32",
          "pythia-1.4b@step16000",
          "b3_g32",
          "pythia-1.4b@step16000",
          "b3_g32",
          "pythia-1.4b@step16000",
          "b3_g512",
          "pythia-1.4b@step16000",
          "b3_g512",
          "pythia-1.4b@step16000",
          "b3_g512",
          "pythia-1.4b@step16000",
          "b4_g32",
          "pythia-1.4b@step16000",
          "b4_g32",
          "pythia-1.4b@step16000",
          "b4_g32",
          "pythia-1.4b@step16000",
          "b4_g512",
          "pythia-1.4b@step16000",
          "b4_g512",
          "pythia-1.4b@step16000",
          "b4_g512",
          "pythia-1.4b@step16000",
          "b5_g32",
          "pythia-1.4b@step16000",
          "b5_g32",
          "pythia-1.4b@step16000",
          "b5_g32",
          "pythia-1.4b@step16000",
          "b5_g512",
          "pythia-1.4b@step16000",
          "b5_g512",
          "pythia-1.4b@step16000",
          "b5_g512"
        ]
      }
    ],
    "context": [],
    "note": "",
    "rendered": "410M/1.4B; bits 3-5, g32/512"
  },
  {
    "row": 3,
    "column": 3,
    "parts": [
      "math ",
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/rows/0/absolute_errors/low_order_2d",
          "results/v69-quant-confirm/compare.json#/rows/3/absolute_errors/low_order_2d",
          "results/v69-quant-confirm/compare.json#/rows/6/absolute_errors/low_order_2d",
          "results/v69-quant-confirm/compare.json#/rows/9/absolute_errors/low_order_2d",
          "results/v69-quant-confirm/compare.json#/rows/12/absolute_errors/low_order_2d",
          "results/v69-quant-confirm/compare.json#/rows/15/absolute_errors/low_order_2d",
          "results/v69-quant-confirm/compare.json#/rows/18/absolute_errors/low_order_2d",
          "results/v69-quant-confirm/compare.json#/rows/21/absolute_errors/low_order_2d",
          "results/v69-quant-confirm/compare.json#/rows/24/absolute_errors/low_order_2d",
          "results/v69-quant-confirm/compare.json#/rows/27/absolute_errors/low_order_2d",
          "results/v69-quant-confirm/compare.json#/rows/30/absolute_errors/low_order_2d",
          "results/v69-quant-confirm/compare.json#/rows/33/absolute_errors/low_order_2d"
        ],
        "op": "mean",
        "format": ".2f"
      },
      " / ",
      "code ",
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/rows/1/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/4/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/7/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/10/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/13/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/16/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/19/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/22/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/25/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/28/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/31/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/34/absolute_errors/median"
        ],
        "op": "mean",
        "format": ".2f"
      },
      " / ",
      "QA ",
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/rows/2/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/5/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/8/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/11/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/14/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/17/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/20/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/23/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/26/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/29/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/32/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/35/absolute_errors/zero"
        ],
        "op": "mean",
        "format": ".2f"
      }
    ],
    "context": [],
    "note": "",
    "rendered": "math 0.21/ code 0.56/ QA 0.46"
  },
  {
    "row": 3,
    "column": 4,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/loso/scores/bilinear/math"
        ],
        "op": "label",
        "format": null,
        "label": "bilin",
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
      },
      " ",
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/rows/0/absolute_errors/bilinear",
          "results/v69-quant-confirm/compare.json#/rows/3/absolute_errors/bilinear",
          "results/v69-quant-confirm/compare.json#/rows/6/absolute_errors/bilinear",
          "results/v69-quant-confirm/compare.json#/rows/9/absolute_errors/bilinear",
          "results/v69-quant-confirm/compare.json#/rows/12/absolute_errors/bilinear",
          "results/v69-quant-confirm/compare.json#/rows/15/absolute_errors/bilinear",
          "results/v69-quant-confirm/compare.json#/rows/18/absolute_errors/bilinear",
          "results/v69-quant-confirm/compare.json#/rows/21/absolute_errors/bilinear",
          "results/v69-quant-confirm/compare.json#/rows/24/absolute_errors/bilinear",
          "results/v69-quant-confirm/compare.json#/rows/27/absolute_errors/bilinear",
          "results/v69-quant-confirm/compare.json#/rows/30/absolute_errors/bilinear",
          "results/v69-quant-confirm/compare.json#/rows/33/absolute_errors/bilinear"
        ],
        "op": "mean",
        "format": ".2f"
      },
      " / ",
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/loso/scores/zero/code"
        ],
        "op": "label",
        "format": null,
        "label": "zero",
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
      },
      " ",
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/rows/1/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/4/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/7/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/10/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/13/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/16/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/19/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/22/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/25/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/28/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/31/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/34/absolute_errors/zero"
        ],
        "op": "mean",
        "format": ".2f"
      },
      " / ",
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/loso/scores/median/qa"
        ],
        "op": "label",
        "format": null,
        "label": "med",
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
      },
      " ",
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/rows/2/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/5/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/8/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/11/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/14/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/17/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/20/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/23/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/26/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/29/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/32/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/35/absolute_errors/median"
        ],
        "op": "mean",
        "format": ".2f"
      }
    ],
    "context": [
      "results/v69-quant-confirm/develop.json#/loso/scores"
    ],
    "note": "Minimum development LOSO macro MAE excluding the selected candidate, per capability.",
    "rendered": "bilin 0.33/ zero 0.68/ med 0.46"
  },
  {
    "row": 3,
    "column": 5,
    "parts": [
      "frozen prediction"
    ],
    "context": [
      "results/v69-quant-confirm/freeze.json#/frozen_at_utc"
    ],
    "note": "",
    "rendered": "frozen prediction"
  },
  {
    "row": 4,
    "column": 0,
    "parts": [
      "Quant: state"
    ],
    "context": [
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
    "rendered": "Quant: state"
  },
  {
    "row": 4,
    "column": 1,
    "parts": [
      "math: ",
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/selected/math/candidate"
        ],
        "op": "label",
        "format": null,
        "label": "$\\phi^\\top Q_c$",
        "expected": [
          "low_order_2d"
        ]
      },
      " (",
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/selected/math/n_coefficients"
        ],
        "op": "identity",
        "format": null
      },
      ")",
      "; ",
      "code: ",
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/selected/code/candidate"
        ],
        "op": "label",
        "format": null,
        "label": "$m_c(b,g)$",
        "expected": [
          "median"
        ]
      },
      " (",
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/selected/code/n_coefficients"
        ],
        "op": "identity",
        "format": null
      },
      ")",
      "; ",
      "QA: ",
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/selected/qa/candidate"
        ],
        "op": "label",
        "format": null,
        "label": "$0$",
        "expected": [
          "zero"
        ]
      },
      " (",
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/selected/qa/n_coefficients"
        ],
        "op": "identity",
        "format": null
      },
      ")"
    ],
    "context": [
      "results/v55-quant-group/register.json#/candidate_definitions/low_order_2d",
      "results/v69-quant-confirm/develop.json#/models",
      "results/v69-quant-confirm/develop.json#/feature_names",
      "results/v69-quant-confirm/develop.json#/dev_configs"
    ],
    "note": "Surface is phi.[a0+a1*u+a2*v+a3*u*v+a4*u^2]; median is per configuration; zero is identically zero.",
    "rendered": "math: $\\phi^\\top Q_c$ (20); code: $m_c(b,g)$ (9); QA: $0$ (0)"
  },
  {
    "row": 4,
    "column": 2,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/rows/36/state",
          "results/v69-quant-confirm/compare.json#/rows/36/config",
          "results/v69-quant-confirm/compare.json#/rows/37/state",
          "results/v69-quant-confirm/compare.json#/rows/37/config",
          "results/v69-quant-confirm/compare.json#/rows/38/state",
          "results/v69-quant-confirm/compare.json#/rows/38/config",
          "results/v69-quant-confirm/compare.json#/rows/39/state",
          "results/v69-quant-confirm/compare.json#/rows/39/config",
          "results/v69-quant-confirm/compare.json#/rows/40/state",
          "results/v69-quant-confirm/compare.json#/rows/40/config",
          "results/v69-quant-confirm/compare.json#/rows/41/state",
          "results/v69-quant-confirm/compare.json#/rows/41/config",
          "results/v69-quant-confirm/compare.json#/rows/42/state",
          "results/v69-quant-confirm/compare.json#/rows/42/config",
          "results/v69-quant-confirm/compare.json#/rows/43/state",
          "results/v69-quant-confirm/compare.json#/rows/43/config",
          "results/v69-quant-confirm/compare.json#/rows/44/state",
          "results/v69-quant-confirm/compare.json#/rows/44/config",
          "results/v69-quant-confirm/compare.json#/rows/45/state",
          "results/v69-quant-confirm/compare.json#/rows/45/config",
          "results/v69-quant-confirm/compare.json#/rows/46/state",
          "results/v69-quant-confirm/compare.json#/rows/46/config",
          "results/v69-quant-confirm/compare.json#/rows/47/state",
          "results/v69-quant-confirm/compare.json#/rows/47/config",
          "results/v69-quant-confirm/compare.json#/rows/48/state",
          "results/v69-quant-confirm/compare.json#/rows/48/config",
          "results/v69-quant-confirm/compare.json#/rows/49/state",
          "results/v69-quant-confirm/compare.json#/rows/49/config",
          "results/v69-quant-confirm/compare.json#/rows/50/state",
          "results/v69-quant-confirm/compare.json#/rows/50/config",
          "results/v69-quant-confirm/compare.json#/rows/51/state",
          "results/v69-quant-confirm/compare.json#/rows/51/config",
          "results/v69-quant-confirm/compare.json#/rows/52/state",
          "results/v69-quant-confirm/compare.json#/rows/52/config",
          "results/v69-quant-confirm/compare.json#/rows/53/state",
          "results/v69-quant-confirm/compare.json#/rows/53/config",
          "results/v69-quant-confirm/compare.json#/rows/54/state",
          "results/v69-quant-confirm/compare.json#/rows/54/config",
          "results/v69-quant-confirm/compare.json#/rows/55/state",
          "results/v69-quant-confirm/compare.json#/rows/55/config",
          "results/v69-quant-confirm/compare.json#/rows/56/state",
          "results/v69-quant-confirm/compare.json#/rows/56/config",
          "results/v69-quant-confirm/compare.json#/rows/57/state",
          "results/v69-quant-confirm/compare.json#/rows/57/config",
          "results/v69-quant-confirm/compare.json#/rows/58/state",
          "results/v69-quant-confirm/compare.json#/rows/58/config",
          "results/v69-quant-confirm/compare.json#/rows/59/state",
          "results/v69-quant-confirm/compare.json#/rows/59/config",
          "results/v69-quant-confirm/compare.json#/rows/60/state",
          "results/v69-quant-confirm/compare.json#/rows/60/config",
          "results/v69-quant-confirm/compare.json#/rows/61/state",
          "results/v69-quant-confirm/compare.json#/rows/61/config",
          "results/v69-quant-confirm/compare.json#/rows/62/state",
          "results/v69-quant-confirm/compare.json#/rows/62/config"
        ],
        "op": "label",
        "format": null,
        "label": "1.4B/112k; g32,128,512",
        "expected": [
          "pythia-1.4b@step112000",
          "b3_g32",
          "pythia-1.4b@step112000",
          "b3_g32",
          "pythia-1.4b@step112000",
          "b3_g32",
          "pythia-1.4b@step112000",
          "b3_g512",
          "pythia-1.4b@step112000",
          "b3_g512",
          "pythia-1.4b@step112000",
          "b3_g512",
          "pythia-1.4b@step112000",
          "b4_g32",
          "pythia-1.4b@step112000",
          "b4_g32",
          "pythia-1.4b@step112000",
          "b4_g32",
          "pythia-1.4b@step112000",
          "b4_g512",
          "pythia-1.4b@step112000",
          "b4_g512",
          "pythia-1.4b@step112000",
          "b4_g512",
          "pythia-1.4b@step112000",
          "b5_g32",
          "pythia-1.4b@step112000",
          "b5_g32",
          "pythia-1.4b@step112000",
          "b5_g32",
          "pythia-1.4b@step112000",
          "b5_g512",
          "pythia-1.4b@step112000",
          "b5_g512",
          "pythia-1.4b@step112000",
          "b5_g512",
          "pythia-1.4b@step112000",
          "b3_g128",
          "pythia-1.4b@step112000",
          "b3_g128",
          "pythia-1.4b@step112000",
          "b3_g128",
          "pythia-1.4b@step112000",
          "b4_g128",
          "pythia-1.4b@step112000",
          "b4_g128",
          "pythia-1.4b@step112000",
          "b4_g128",
          "pythia-1.4b@step112000",
          "b5_g128",
          "pythia-1.4b@step112000",
          "b5_g128",
          "pythia-1.4b@step112000",
          "b5_g128"
        ]
      }
    ],
    "context": [],
    "note": "",
    "rendered": "1.4B/112k; g32,128,512"
  },
  {
    "row": 4,
    "column": 3,
    "parts": [
      "math ",
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/rows/36/absolute_errors/low_order_2d",
          "results/v69-quant-confirm/compare.json#/rows/39/absolute_errors/low_order_2d",
          "results/v69-quant-confirm/compare.json#/rows/42/absolute_errors/low_order_2d",
          "results/v69-quant-confirm/compare.json#/rows/45/absolute_errors/low_order_2d",
          "results/v69-quant-confirm/compare.json#/rows/48/absolute_errors/low_order_2d",
          "results/v69-quant-confirm/compare.json#/rows/51/absolute_errors/low_order_2d",
          "results/v69-quant-confirm/compare.json#/rows/54/absolute_errors/low_order_2d",
          "results/v69-quant-confirm/compare.json#/rows/57/absolute_errors/low_order_2d",
          "results/v69-quant-confirm/compare.json#/rows/60/absolute_errors/low_order_2d"
        ],
        "op": "mean",
        "format": ".2f"
      },
      " / ",
      "code ",
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/rows/37/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/40/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/43/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/46/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/49/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/52/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/55/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/58/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/61/absolute_errors/median"
        ],
        "op": "mean",
        "format": ".2f"
      },
      " / ",
      "QA ",
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/rows/38/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/41/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/44/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/47/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/50/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/53/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/56/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/59/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/62/absolute_errors/zero"
        ],
        "op": "mean",
        "format": ".2f"
      }
    ],
    "context": [],
    "note": "",
    "rendered": "math 0.30/ code 0.15/ QA 0.22"
  },
  {
    "row": 4,
    "column": 4,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/loso/scores/bilinear/math"
        ],
        "op": "label",
        "format": null,
        "label": "bilin",
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
      },
      " ",
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/rows/36/absolute_errors/bilinear",
          "results/v69-quant-confirm/compare.json#/rows/39/absolute_errors/bilinear",
          "results/v69-quant-confirm/compare.json#/rows/42/absolute_errors/bilinear",
          "results/v69-quant-confirm/compare.json#/rows/45/absolute_errors/bilinear",
          "results/v69-quant-confirm/compare.json#/rows/48/absolute_errors/bilinear",
          "results/v69-quant-confirm/compare.json#/rows/51/absolute_errors/bilinear",
          "results/v69-quant-confirm/compare.json#/rows/54/absolute_errors/bilinear",
          "results/v69-quant-confirm/compare.json#/rows/57/absolute_errors/bilinear",
          "results/v69-quant-confirm/compare.json#/rows/60/absolute_errors/bilinear"
        ],
        "op": "mean",
        "format": ".2f"
      },
      " / ",
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/loso/scores/zero/code"
        ],
        "op": "label",
        "format": null,
        "label": "zero",
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
      },
      " ",
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/rows/37/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/40/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/43/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/46/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/49/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/52/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/55/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/58/absolute_errors/zero",
          "results/v69-quant-confirm/compare.json#/rows/61/absolute_errors/zero"
        ],
        "op": "mean",
        "format": ".2f"
      },
      " / ",
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/loso/scores/median/qa"
        ],
        "op": "label",
        "format": null,
        "label": "med",
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
      },
      " ",
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/rows/38/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/41/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/44/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/47/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/50/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/53/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/56/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/59/absolute_errors/median",
          "results/v69-quant-confirm/compare.json#/rows/62/absolute_errors/median"
        ],
        "op": "mean",
        "format": ".2f"
      }
    ],
    "context": [
      "results/v69-quant-confirm/develop.json#/loso/scores"
    ],
    "note": "Minimum development LOSO macro MAE excluding the selected candidate, per capability.",
    "rendered": "bilin 0.35/ zero 0.56/ med 0.14"
  },
  {
    "row": 4,
    "column": 5,
    "parts": [
      "frozen prediction"
    ],
    "context": [
      "results/v69-quant-confirm/freeze.json#/frozen_at_utc"
    ],
    "note": "",
    "rendered": "frozen prediction"
  },
  {
    "row": 5,
    "column": 0,
    "parts": [
      "Distill: budget"
    ],
    "context": [
      "results/a2-curvature-interaction/summary.json#/decision_table/18/target",
      "results/a2-curvature-interaction/summary.json#/decision_table/6/target",
      "results/a2-curvature-interaction/summary.json#/decision_table/54/target"
    ],
    "note": "",
    "rendered": "Distill: budget"
  },
  {
    "row": 5,
    "column": 1,
    "parts": [
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/protocol/structures/F_log"
        ],
        "op": "label",
        "format": null,
        "label": "$Au+Bv$",
        "expected": [
          "(a+a_prime*z)*u+(b+b_prime*z)*v"
        ]
      },
      " (",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/parameter_intervals/0/fits/F_log/fit/nominal_parameters"
        ],
        "op": "identity",
        "format": null
      },
      "); ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/protocol/structures/F_curv"
        ],
        "op": "label",
        "format": null,
        "label": "$Au+Bh_p(E)$",
        "expected": [
          "(a+a_prime*z)*u+(b+b_prime*z)*h_p(E)"
        ]
      },
      " (",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/parameter_intervals/0/fits/F_curv/fit/nominal_parameters"
        ],
        "op": "identity",
        "format": null
      },
      "); ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/protocol/structures/F_int"
        ],
        "op": "label",
        "format": null,
        "label": "$Au+Bv+kuv$",
        "expected": [
          "(a+a_prime*z)*u+(b+b_prime*z)*v+k*u*v"
        ]
      },
      " (",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/parameter_intervals/0/fits/F_int/fit/nominal_parameters"
        ],
        "op": "identity",
        "format": null
      },
      ")"
    ],
    "context": [
      "results/a2-curvature-interaction/summary.json#/protocol/structures",
      "results/a2-curvature-interaction/summary.json#/protocol/descriptors",
      "results/a2-curvature-interaction/summary.json#/protocol/descriptor_calibration_cost"
    ],
    "note": "Fold-selected forms; A=a+a_prime*z and B=b+b_prime*z. Counts are per structure, not summed over folds.",
    "rendered": "$Au+Bv$ (4); $Au+Bh_p(E)$ (5); $Au+Bv+kuv$ (5)"
  },
  {
    "row": 5,
    "column": 2,
    "parts": [
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/parameter_intervals/0/fits/F_log/fit/standardizer/students",
          "results/a2-curvature-interaction/summary.json#/protocol/largest_budget"
        ],
        "op": "label",
        "format": null,
        "label": "3 students; $T\\ge150$k held out",
        "expected": [
          [
            "gemma3-1b",
            "gemma3-270m",
            "gemma3-4b"
          ],
          "All T>=150000 withheld; fit only T<150000. QA scope has only final positive checkpoints and is unscorable here."
        ]
      }
    ],
    "context": [
      "results/a2-curvature-interaction/summary.json#/decision_table/18/distribution",
      "results/a2-curvature-interaction/summary.json#/decision_table/6/distribution",
      "results/a2-curvature-interaction/summary.json#/decision_table/54/distribution"
    ],
    "note": "Only the training-probe rows whose MAEs are printed here; fresh-sample QA rows are not pooled or advertised.",
    "rendered": "3 students; $T\\ge150$k held out"
  },
  {
    "row": 5,
    "column": 3,
    "parts": [
      "math ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/18/primary_mae"
        ],
        "op": "identity",
        "format": ".2f"
      },
      " [",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/18/primary_mae_interval/0"
        ],
        "op": "identity",
        "format": ".2f"
      },
      ",",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/18/primary_mae_interval/1"
        ],
        "op": "identity",
        "format": ".2f"
      },
      "]",
      " / ",
      "code ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/6/primary_mae"
        ],
        "op": "identity",
        "format": ".2f"
      },
      " [",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/6/primary_mae_interval/0"
        ],
        "op": "identity",
        "format": ".2f"
      },
      ",",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/6/primary_mae_interval/1"
        ],
        "op": "identity",
        "format": ".2f"
      },
      "]",
      " / ",
      "QA ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/54/primary_mae"
        ],
        "op": "identity",
        "format": ".2f"
      },
      " [",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/54/primary_mae_interval/0"
        ],
        "op": "identity",
        "format": ".2f"
      },
      ",",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/54/primary_mae_interval/1"
        ],
        "op": "identity",
        "format": ".2f"
      },
      "]"
    ],
    "context": [],
    "note": "Training-probe MAEs; reuse is the recorded tolerance proxy, not an exact intervention. Intervals conditional on frozen fold predictions.",
    "rendered": "math 0.07 [0.05,0.11]/ code 0.07 [0.05,0.09]/ QA 2.18 [1.68,2.88]"
  },
  {
    "row": 5,
    "column": 4,
    "parts": [
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/18/inner_selected_baselines"
        ],
        "op": "label",
        "format": null,
        "label": "const",
        "expected": [
          {
            "constant": 34
          }
        ]
      },
      " ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/18/baseline_mae"
        ],
        "op": "identity",
        "format": ".2f"
      },
      " / ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/6/inner_selected_baselines"
        ],
        "op": "label",
        "format": null,
        "label": "const",
        "expected": [
          {
            "constant": 34
          }
        ]
      },
      " ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/6/baseline_mae"
        ],
        "op": "identity",
        "format": ".2f"
      },
      " / ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/54/inner_selected_baselines"
        ],
        "op": "label",
        "format": null,
        "label": "const",
        "expected": [
          {
            "constant": 34
          }
        ]
      },
      " ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/54/baseline_mae"
        ],
        "op": "identity",
        "format": ".2f"
      }
    ],
    "context": [],
    "note": "Inner-development-selected baselines. Never strongest_observed_baseline or strongest_baseline_mae.",
    "rendered": "const 0.09/ const 0.11/ const 1.44"
  },
  {
    "row": 5,
    "column": 5,
    "parts": [
      "development"
    ],
    "context": [
      "results/a2-curvature-interaction/summary.json#/protocol/secondary",
      "results/a2-curvature-interaction/summary.json#/protocol/previous_F_int"
    ],
    "note": "",
    "rendered": "devel\\-opment"
  },
  {
    "row": 6,
    "column": 0,
    "parts": [
      "Distill: reuse"
    ],
    "context": [
      "results/a2-curvature-interaction/summary.json#/decision_table/14/target",
      "results/a2-curvature-interaction/summary.json#/decision_table/2/target",
      "results/a2-curvature-interaction/summary.json#/decision_table/50/target"
    ],
    "note": "",
    "rendered": "Distill: reuse"
  },
  {
    "row": 6,
    "column": 1,
    "parts": [
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/protocol/structures/F_log"
        ],
        "op": "label",
        "format": null,
        "label": "$Au+Bv$",
        "expected": [
          "(a+a_prime*z)*u+(b+b_prime*z)*v"
        ]
      },
      " (",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/parameter_intervals/0/fits/F_log/fit/nominal_parameters"
        ],
        "op": "identity",
        "format": null
      },
      "); ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/protocol/structures/F_curv"
        ],
        "op": "label",
        "format": null,
        "label": "$Au+Bh_p(E)$",
        "expected": [
          "(a+a_prime*z)*u+(b+b_prime*z)*h_p(E)"
        ]
      },
      " (",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/parameter_intervals/0/fits/F_curv/fit/nominal_parameters"
        ],
        "op": "identity",
        "format": null
      },
      "); ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/protocol/structures/F_int"
        ],
        "op": "label",
        "format": null,
        "label": "$Au+Bv+kuv$",
        "expected": [
          "(a+a_prime*z)*u+(b+b_prime*z)*v+k*u*v"
        ]
      },
      " (",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/parameter_intervals/0/fits/F_int/fit/nominal_parameters"
        ],
        "op": "identity",
        "format": null
      },
      ")"
    ],
    "context": [
      "results/a2-curvature-interaction/summary.json#/protocol/structures",
      "results/a2-curvature-interaction/summary.json#/protocol/descriptors",
      "results/a2-curvature-interaction/summary.json#/protocol/descriptor_calibration_cost"
    ],
    "note": "Fold-selected forms; A=a+a_prime*z and B=b+b_prime*z. Counts are per structure, not summed over folds.",
    "rendered": "$Au+Bv$ (4); $Au+Bh_p(E)$ (5); $Au+Bv+kuv$ (5)"
  },
  {
    "row": 6,
    "column": 2,
    "parts": [
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/parameter_intervals/0/fits/F_curv/fit/standardizer/students",
          "results/a2-curvature-interaction/summary.json#/protocol/I_U"
        ],
        "op": "label",
        "format": null,
        "label": "3 students; 1% budget proxy",
        "expected": [
          [
            "gemma3-1b",
            "gemma3-270m",
            "gemma3-4b"
          ],
          "Exact I_U has no observed positive matched-T pairs. Decision MAEs labelled 1% tolerance proxy use actual endpoints; fixed-T model predictions are stored but not scored against mismatched outcomes. 0.5%/5% separate sensitivity, never pooled."
        ]
      }
    ],
    "context": [
      "results/a2-curvature-interaction/summary.json#/decision_table/14/distribution",
      "results/a2-curvature-interaction/summary.json#/decision_table/2/distribution",
      "results/a2-curvature-interaction/summary.json#/decision_table/50/distribution"
    ],
    "note": "Only the training-probe rows whose MAEs are printed here; fresh-sample QA rows are not pooled or advertised.",
    "rendered": "3 students; 1\\% budget proxy"
  },
  {
    "row": 6,
    "column": 3,
    "parts": [
      "math ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/14/primary_mae"
        ],
        "op": "identity",
        "format": ".2f"
      },
      " [",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/14/primary_mae_interval/0"
        ],
        "op": "identity",
        "format": ".2f"
      },
      ",",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/14/primary_mae_interval/1"
        ],
        "op": "identity",
        "format": ".2f"
      },
      "]",
      " / ",
      "code ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/2/primary_mae"
        ],
        "op": "identity",
        "format": ".2f"
      },
      " [",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/2/primary_mae_interval/0"
        ],
        "op": "identity",
        "format": ".2f"
      },
      ",",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/2/primary_mae_interval/1"
        ],
        "op": "identity",
        "format": ".2f"
      },
      "]",
      " / ",
      "QA ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/50/primary_mae"
        ],
        "op": "identity",
        "format": ".2f"
      },
      " [",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/50/primary_mae_interval/0"
        ],
        "op": "identity",
        "format": ".2f"
      },
      ",",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/50/primary_mae_interval/1"
        ],
        "op": "identity",
        "format": ".2f"
      },
      "]"
    ],
    "context": [],
    "note": "Training-probe MAEs; reuse is the recorded tolerance proxy, not an exact intervention. Intervals conditional on frozen fold predictions.",
    "rendered": "math 0.08 [0.05,0.14]/ code 0.07 [0.04,0.12]/ QA 1.02 [0.72,1.34]"
  },
  {
    "row": 6,
    "column": 4,
    "parts": [
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/14/inner_selected_baselines"
        ],
        "op": "label",
        "format": null,
        "label": "surf/E",
        "expected": [
          {
            "surface": 109,
            "reuse_only": 29
          }
        ]
      },
      " ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/14/baseline_mae"
        ],
        "op": "identity",
        "format": ".2f"
      },
      " / ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/2/inner_selected_baselines"
        ],
        "op": "label",
        "format": null,
        "label": "zero/surf/E",
        "expected": [
          {
            "zero": 38,
            "surface": 71,
            "reuse_only": 29
          }
        ]
      },
      " ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/2/baseline_mae"
        ],
        "op": "identity",
        "format": ".2f"
      },
      " / ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/50/inner_selected_baselines"
        ],
        "op": "label",
        "format": null,
        "label": "surf",
        "expected": [
          {
            "surface": 138
          }
        ]
      },
      " ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/50/baseline_mae"
        ],
        "op": "identity",
        "format": ".2f"
      }
    ],
    "context": [],
    "note": "Inner-development-selected baselines. Never strongest_observed_baseline or strongest_baseline_mae.",
    "rendered": "surf/E 0.08/ zero/surf/E 0.07/ surf 0.76"
  },
  {
    "row": 6,
    "column": 5,
    "parts": [
      "development"
    ],
    "context": [
      "results/a2-curvature-interaction/summary.json#/protocol/secondary",
      "results/a2-curvature-interaction/summary.json#/protocol/previous_F_int"
    ],
    "note": "",
    "rendered": "devel\\-opment"
  },
  {
    "row": 7,
    "column": 0,
    "parts": [
      "Distill: pool"
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/confirmation_register/unused_U_assertion"
    ],
    "note": "",
    "rendered": "Distill: pool"
  },
  {
    "row": 7,
    "column": 1,
    "parts": [
      "math: ",
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/selected/math/method"
        ],
        "op": "label",
        "format": null,
        "label": "$a_c\\ell_E$",
        "expected": [
          "E"
        ]
      },
      " (",
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/selected/math/n_params"
        ],
        "op": "identity",
        "format": null
      },
      ")",
      "; ",
      "code: ",
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/selected/code/method"
        ],
        "op": "label",
        "format": null,
        "label": "$a_c\\ell_E$",
        "expected": [
          "E"
        ]
      },
      " (",
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/selected/code/n_params"
        ],
        "op": "identity",
        "format": null
      },
      ")",
      "; ",
      "QA: ",
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/selected/qa/method"
        ],
        "op": "label",
        "format": null,
        "label": "$u(a+bu+qv)$",
        "expected": [
          "joint"
        ]
      },
      " (",
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/selected/qa/n_params"
        ],
        "op": "identity",
        "format": null
      },
      ")"
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/models",
      "results/v70-distill-confirm/freeze.json#/reference_rule",
      "results/v70-distill-confirm/freeze.json#/prediction_rule"
    ],
    "note": "E and joint are the frozen V50/V70 design identifiers. E has one coefficient; joint has three coefficients on u, u*u, u*log(D_U/D_ref). T_star is null, not fitted, for these selected forms.",
    "rendered": "math: $a_c\\ell_E$ (1); code: $a_c\\ell_E$ (1); QA: $u(a+bu+qv)$ (3)"
  },
  {
    "row": 7,
    "column": 2,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/confirmation_register/students",
          "results/v70-distill-confirm/freeze.json#/confirmation_register/pools",
          "results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned"
        ],
        "op": "label",
        "format": null,
        "label": "270M/1B; 6 pools, 50k-200k",
        "expected": [
          [
            "gemma3-270m",
            "gemma3-1b"
          ],
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
    "context": [],
    "note": "",
    "rendered": "270M/1B; 6 pools, 50k-200k"
  },
  {
    "row": 7,
    "column": 3,
    "parts": [
      "math ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/0/candidate_mae"
        ],
        "op": "identity",
        "format": ".2f"
      },
      ",",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/3/candidate_mae"
        ],
        "op": "identity",
        "format": ".2f"
      },
      " / ",
      "code ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/1/candidate_mae"
        ],
        "op": "identity",
        "format": ".2f"
      },
      ",",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/4/candidate_mae"
        ],
        "op": "identity",
        "format": ".2f"
      },
      " / ",
      "QA ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/2/candidate_mae"
        ],
        "op": "identity",
        "format": ".2f"
      },
      ",",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/5/candidate_mae"
        ],
        "op": "identity",
        "format": ".2f"
      }
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/confirmation_register/students"
    ],
    "note": "Comma-separated scores follow student order 270M, 1B; no student averaging.",
    "rendered": "math 0.07,0.06/ code 0.02,0.05/ QA 0.51,0.46"
  },
  {
    "row": 7,
    "column": 4,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/0/strongest_baseline",
          "results/v70-distill-confirm/compare.json#/groups/3/strongest_baseline"
        ],
        "op": "label",
        "format": null,
        "label": "T/L",
        "expected": [
          "T-only",
          "surface:L0"
        ]
      },
      " ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/0/baseline_mae"
        ],
        "op": "identity",
        "format": ".2f"
      },
      ",",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/3/baseline_mae"
        ],
        "op": "identity",
        "format": ".2f"
      },
      " / ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/1/strongest_baseline",
          "results/v70-distill-confirm/compare.json#/groups/4/strongest_baseline"
        ],
        "op": "label",
        "format": null,
        "label": "E",
        "expected": [
          "E-only",
          "E-only"
        ]
      },
      " ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/1/baseline_mae"
        ],
        "op": "identity",
        "format": ".2f"
      },
      ",",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/4/baseline_mae"
        ],
        "op": "identity",
        "format": ".2f"
      },
      " / ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/2/strongest_baseline",
          "results/v70-distill-confirm/compare.json#/groups/5/strongest_baseline"
        ],
        "op": "label",
        "format": null,
        "label": "E/N",
        "expected": [
          "E-only",
          "surface:logN"
        ]
      },
      " ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/2/baseline_mae"
        ],
        "op": "identity",
        "format": ".2f"
      },
      ",",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/5/baseline_mae"
        ],
        "op": "identity",
        "format": ".2f"
      }
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/baseline_rule",
      "results/v70-distill-confirm/freeze.json#/strongest_baseline",
      "results/v70-distill-confirm/compare.json#/groups/0/paired_difference",
      "results/v70-distill-confirm/compare.json#/groups/1/paired_difference",
      "results/v70-distill-confirm/compare.json#/groups/2/paired_difference",
      "results/v70-distill-confirm/compare.json#/groups/3/paired_difference",
      "results/v70-distill-confirm/compare.json#/groups/4/paired_difference",
      "results/v70-distill-confirm/compare.json#/groups/5/paired_difference"
    ],
    "note": "Only MAEs are printed, paired in student order 270M, 1B. T=T-only, E=E-only, L=initial-loss surface, N=size surface. Stored paired_difference.ci95 estimates baseline-minus-candidate gain, not an MAE interval; it is not displayed in the MAE columns.",
    "rendered": "T/L 0.07,0.03/ E 0.02,0.05/ E/N 0.61,0.45"
  },
  {
    "row": 7,
    "column": 5,
    "parts": [
      "frozen prediction"
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/frozen_at_utc",
      "results/v47-p2-register/register.json#/v5_confirm/registered_at_utc"
    ],
    "note": "",
    "rendered": "frozen prediction"
  }
]
```

## Caption recipe

```json
{
  "parts": [
    "Frozen MAEs: native-token nats, training probes; stored intervals in brackets. Inputs: source size, initial loss and pretraining tokens for source-conditioned forms; the configuration for all; distillation forms take supervised budget, pool size and reuse. ",
    {
      "sources": [
        "results/v53-prune-dev/register.json#/candidate_definitions/power"
      ],
      "op": "label",
      "format": null,
      "label": "$r=(1-d)/0.3$; ",
      "expected": [
        "(beta.phi) * ((1-d)/0.3)**gamma"
      ]
    },
    {
      "sources": [
        "results/v55-quant-group/register.json#/candidate_definitions/low_order_2d"
      ],
      "op": "label",
      "format": null,
      "label": "$Q_c=a+bu+cv+duv+eu^2$; ",
      "expected": [
        "phi.[a0 + a1*u + a2*v + a3*u*v + a4*u^2]; coefficients ordered by term then phi"
      ]
    },
    {
      "sources": [
        "results/v70-distill-confirm/freeze.json#/models"
      ],
      "op": "label",
      "format": null,
      "label": "$\\ell_E=\\log(1+E)$; ",
      "expected": [
        {
          "math": {
            "constant": {
              "coef": [
                0.16073202379148357
              ],
              "rank": 1,
              "n_params": 1,
              "sse": 2.5170896942462475,
              "estimator": "V50 OLS",
              "T_star": null,
              "method": "constant",
              "selection_n_params": 1,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 2.5170896942462475
                }
              ]
            },
            "constant+src": {
              "coef": [
                0.16572843297364517,
                0.04964661954532312
              ],
              "rank": 2,
              "n_params": 2,
              "sse": 2.2870365477995342,
              "estimator": "V50 OLS",
              "T_star": null,
              "method": "constant+src",
              "selection_n_params": 2,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 2.2870365477995342
                }
              ]
            },
            "T": {
              "coef": [
                0.1141146071917939
              ],
              "rank": 1,
              "n_params": 1,
              "sse": 2.095269809380306,
              "estimator": "V50 OLS",
              "T_star": null,
              "method": "T",
              "selection_n_params": 1,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 2.095269809380306
                }
              ]
            },
            "T+src": {
              "coef": [
                0.11798307948838954,
                0.038075898170200836
              ],
              "rank": 2,
              "n_params": 2,
              "sse": 1.783198514343183,
              "estimator": "V50 OLS",
              "T_star": null,
              "method": "T+src",
              "selection_n_params": 2,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 1.783198514343183
                }
              ]
            },
            "E": {
              "coef": [
                0.15127841083533308
              ],
              "rank": 1,
              "n_params": 1,
              "sse": 1.2891117375250243,
              "estimator": "V50 OLS",
              "T_star": null,
              "method": "E",
              "selection_n_params": 1,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 1.2891117375250243
                }
              ]
            },
            "E+src": {
              "coef": [
                0.15911482013227596,
                0.059728296977249025
              ],
              "rank": 2,
              "n_params": 2,
              "sse": 0.7473056773292215,
              "estimator": "V50 OLS",
              "T_star": null,
              "method": "E+src",
              "selection_n_params": 2,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 0.7473056773292215
                }
              ]
            },
            "joint": {
              "coef": [
                0.057436995691740246,
                0.010793281549704731,
                -0.08234766958431203
              ],
              "rank": 3,
              "n_params": 3,
              "sse": 1.1069063512935944,
              "estimator": "V50 OLS",
              "T_star": null,
              "method": "joint",
              "selection_n_params": 3,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 1.1069063512935944
                }
              ]
            },
            "joint+src": {
              "coef": [
                0.06050775408374385,
                0.010956165581474591,
                -0.0839798191711278,
                0.0403715195655175
              ],
              "rank": 4,
              "n_params": 4,
              "sse": 0.7564580273069285,
              "estimator": "V50 OLS",
              "T_star": null,
              "method": "joint+src",
              "selection_n_params": 4,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 0.7564580273069285
                }
              ]
            },
            "F1:L0": {
              "coef": [
                0.15978098118643583,
                -0.058365867546725986
              ],
              "columns": [
                "b0",
                "b1"
              ],
              "n_params": 2,
              "rank": 2,
              "column_mean": [
                0.0,
                0.0
              ],
              "column_scale": [
                0.6999208707326598,
                1.216776696158139
              ],
              "standardized_coef": [
                0.1118340434785289,
                -0.0710182274819088
              ],
              "sse": 0.7900740186789115,
              "ridge_objective": 0.7900915691208269,
              "effective_df": 1.9999868808296406,
              "intercept_unpenalized": false,
              "estimator": "V56 standardized ridge, lambda=0.001",
              "T_star": null,
              "method": "F1:L0",
              "selection_n_params": 2,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 0.7900740186789115
                }
              ]
            },
            "F1:logN": {
              "coef": [
                0.15911426425319122,
                0.05945300306468042
              ],
              "columns": [
                "b0",
                "b1"
              ],
              "n_params": 2,
              "rank": 2,
              "column_mean": [
                0.0,
                0.0
              ],
              "column_scale": [
                0.6999208707326598,
                1.2432284815872339
              ],
              "standardized_coef": [
                0.11136739438208013,
                0.0739136667259038
              ],
              "sse": 0.7473056774337997,
              "ridge_objective": 0.74732354336046,
              "effective_df": 1.9999869195464919,
              "intercept_unpenalized": false,
              "estimator": "V56 standardized ridge, lambda=0.001",
              "T_star": null,
              "method": "F1:logN",
              "selection_n_params": 2,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 0.7473056774337997
                }
              ]
            },
            "F2:L0": {
              "coef": [
                -0.051195454892940286,
                0.059053885125669454,
                0.1875346636613153,
                -0.09061204480923599
              ],
              "columns": [
                "b0",
                "b1",
                "b2",
                "b3"
              ],
              "n_params": 4,
              "rank": 4,
              "column_mean": [
                0.0,
                0.0,
                0.0,
                0.0
              ],
              "column_scale": [
                0.22044697778616124,
                0.7227193539804633,
                0.6999208707326598,
                1.216776696158139
              ],
              "standardized_coef": [
                -0.011285883307536427,
                0.04267938570806032,
                0.1312594250823843,
                -0.11025462451511542
              ],
              "sse": 0.735260216675391,
              "ridge_objective": 0.7352915506954174,
              "effective_df": 3.9998706171809855,
              "intercept_unpenalized": false,
              "estimator": "V56 standardized ridge, lambda=0.001",
              "T_star": 70000,
              "method": "F2:L0",
              "selection_n_params": 5,
              "T_star_grid_sse": [
                {
                  "T_star": 17500,
                  "sse": 0.7539545246795474
                },
                {
                  "T_star": 35000,
                  "sse": 0.7436500726553973
                },
                {
                  "T_star": 70000,
                  "sse": 0.735260216675391
                },
                {
                  "T_star": 140000,
                  "sse": 0.7417640430133925
                },
                {
                  "T_star": 280000,
                  "sse": 0.7535107887066673
                }
              ]
            },
            "F2:logN": {
              "coef": [
                -0.05088943840889367,
                -0.06884614958696111,
                0.18669419344974178,
                0.09668062627062765
              ],
              "columns": [
                "b0",
                "b1",
                "b2",
                "b3"
              ],
              "n_params": 4,
              "rank": 4,
              "column_mean": [
                0.0,
                0.0,
                0.0,
                0.0
              ],
              "column_scale": [
                0.22044697778616124,
                0.7347268653802675,
                0.6999208707326598,
                1.2432284815872339
              ],
              "standardized_coef": [
                -0.011218422898475603,
                -0.050583115679528945,
                0.1306711624400749,
                0.12019610819733524
              ],
              "sse": 0.6793862169700631,
              "ridge_objective": 0.6794204235317864,
              "effective_df": 3.999870949053996,
              "intercept_unpenalized": false,
              "estimator": "V56 standardized ridge, lambda=0.001",
              "T_star": 70000,
              "method": "F2:logN",
              "selection_n_params": 5,
              "T_star_grid_sse": [
                {
                  "T_star": 17500,
                  "sse": 0.694319595939052
                },
                {
                  "T_star": 35000,
                  "sse": 0.6843543318418208
                },
                {
                  "T_star": 70000,
                  "sse": 0.6793862169700631
                },
                {
                  "T_star": 140000,
                  "sse": 0.6922251592553327
                },
                {
                  "T_star": 280000,
                  "sse": 0.708345988023976
                }
              ]
            },
            "T-only": {
              "coef": [
                -0.003541624822581496,
                0.11628241029372188
              ],
              "columns": [
                "b0",
                "b1"
              ],
              "n_params": 2,
              "rank": 2,
              "column_mean": [
                0.0,
                1.4127127929247456
              ],
              "column_scale": [
                1.0,
                0.5586406513529452
              ],
              "standardized_coef": [
                0.16073202379148355,
                0.06496008142737521
              ],
              "sse": 2.0951000367167674,
              "ridge_objective": 2.0951042565289466,
              "effective_df": 1.999990000099999,
              "intercept_unpenalized": true,
              "estimator": "V56 standardized ridge, lambda=0.001",
              "T_star": null,
              "method": "T-only",
              "selection_n_params": 2,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 2.0951000367167674
                }
              ]
            },
            "E-only": {
              "coef": [
                -0.01118477622714309,
                0.15855937408854176
              ],
              "columns": [
                "b0",
                "b1"
              ],
              "n_params": 2,
              "rank": 2,
              "column_mean": [
                0.0,
                1.0842424234257253
              ],
              "column_scale": [
                1.0,
                0.6999208707326598
              ],
              "standardized_coef": [
                0.16073202379148357,
                0.1109790151748777
              ],
              "sse": 1.2854308806440566,
              "ridge_objective": 1.2854431969858657,
              "effective_df": 1.999990000099999,
              "intercept_unpenalized": true,
              "estimator": "V56 standardized ridge, lambda=0.001",
              "T_star": null,
              "method": "E-only",
              "selection_n_params": 2,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 1.2854308806440566
                }
              ]
            },
            "surface:L0": {
              "coef": [
                0.01215786230194732,
                -0.022975065100232436,
                0.172481010822215,
                -0.05351151417686075
              ],
              "columns": [
                "b0",
                "b1",
                "b2",
                "b3"
              ],
              "n_params": 4,
              "rank": 4,
              "column_mean": [
                0.0,
                1.4127127929247456,
                1.0842424234257253,
                0.11174976798674695
              ],
              "column_scale": [
                1.0,
                0.5586406513529452,
                0.6999208707326598,
                0.954678928379201
              ],
              "standardized_coef": [
                0.16073202379148355,
                -0.012834805332470167,
                0.12072305927953406,
                -0.05108631501031384
              ],
              "sse": 1.017286023539862,
              "ridge_objective": 1.017303372140713,
              "effective_df": 3.99995570923737,
              "intercept_unpenalized": true,
              "estimator": "V56 standardized ridge, lambda=0.001",
              "T_star": null,
              "method": "surface:L0",
              "selection_n_params": 4,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 1.017286023539862
                }
              ]
            },
            "surface:logN": {
              "coef": [
                0.011490392938827698,
                -0.02267647795795931,
                0.17209449876133037,
                0.05257118770214056
              ],
              "columns": [
                "b0",
                "b1",
                "b2",
                "b3"
              ],
              "n_params": 4,
              "rank": 4,
              "column_mean": [
                0.0,
                1.4127127929247456,
                1.0842424234257253,
                -0.10110433614310209
              ],
              "column_scale": [
                1.0,
                0.5586406513529452,
                0.6999208707326598,
                0.9705677865952219
              ],
              "standardized_coef": [
                0.16073202379148355,
                -0.012668002416825093,
                0.12045253142133101,
                0.05102390128674851
              ],
              "sse": 1.0178506878998392,
              "ridge_objective": 1.0178679606289527,
              "effective_df": 3.999955718536262,
              "intercept_unpenalized": true,
              "estimator": "V56 standardized ridge, lambda=0.001",
              "T_star": null,
              "method": "surface:logN",
              "selection_n_params": 4,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 1.0178506878998392
                }
              ]
            }
          },
          "code": {
            "constant": {
              "coef": [
                0.173201671833481
              ],
              "rank": 1,
              "n_params": 1,
              "sse": 1.3742118081786727,
              "estimator": "V50 OLS",
              "T_star": null,
              "method": "constant",
              "selection_n_params": 1,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 1.3742118081786727
                }
              ]
            },
            "constant+src": {
              "coef": [
                0.17493449965668284,
                0.017218174200623337
              ],
              "rank": 2,
              "n_params": 2,
              "sse": 1.3465409258773553,
              "estimator": "V50 OLS",
              "T_star": null,
              "method": "constant+src",
              "selection_n_params": 2,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 1.3465409258773553
                }
              ]
            },
            "T": {
              "coef": [
                0.12407374115952728
              ],
              "rank": 1,
              "n_params": 1,
              "sse": 0.82134205516135,
              "estimator": "V50 OLS",
              "T_star": null,
              "method": "T",
              "selection_n_params": 1,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 0.82134205516135
                }
              ]
            },
            "T+src": {
              "coef": [
                0.12520774528085912,
                0.011161570288720918
              ],
              "rank": 2,
              "n_params": 2,
              "sse": 0.7945254309045957,
              "estimator": "V50 OLS",
              "T_star": null,
              "method": "T+src",
              "selection_n_params": 2,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 0.7945254309045957
                }
              ]
            },
            "E": {
              "coef": [
                0.15508921029854716
              ],
              "rank": 1,
              "n_params": 1,
              "sse": 0.3681927671333221,
              "estimator": "V50 OLS",
              "T_star": null,
              "method": "E",
              "selection_n_params": 1,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 0.3681927671333221
                }
              ]
            },
            "E+src": {
              "coef": [
                0.15742770032882616,
                0.01782372789809887
              ],
              "rank": 2,
              "n_params": 2,
              "sse": 0.31994461537989544,
              "estimator": "V50 OLS",
              "T_star": null,
              "method": "E+src",
              "selection_n_params": 2,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 0.31994461537989544
                }
              ]
            },
            "joint": {
              "coef": [
                0.08274500154886288,
                0.007327626702562026,
                -0.06222617470502769
              ],
              "rank": 3,
              "n_params": 3,
              "sse": 0.2576166967027025,
              "estimator": "V50 OLS",
              "T_star": null,
              "method": "joint",
              "selection_n_params": 3,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 0.2576166967027025
                }
              ]
            },
            "joint+src": {
              "coef": [
                0.08372438455362223,
                0.007379576687581161,
                -0.06274673000847193,
                0.012876030964122633
              ],
              "rank": 4,
              "n_params": 4,
              "sse": 0.22196847916393406,
              "estimator": "V50 OLS",
              "T_star": null,
              "method": "joint+src",
              "selection_n_params": 4,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 0.22196847916393406
                }
              ]
            },
            "F1:L0": {
              "coef": [
                0.1576911943384957,
                -0.018693930281834397
              ],
              "columns": [
                "b0",
                "b1"
              ],
              "n_params": 2,
              "rank": 2,
              "column_mean": [
                0.0,
                0.0
              ],
              "column_scale": [
                0.6999208707326598,
                1.2295118688217672
              ],
              "standardized_coef": [
                0.110371358048273,
                -0.022984409156442034
              ],
              "sse": 0.3158625206063066,
              "ridge_objective": 0.3158752307260483,
              "effective_df": 1.9999868998040653,
              "intercept_unpenalized": false,
              "estimator": "V56 standardized ridge, lambda=0.001",
              "T_star": null,
              "method": "F1:L0",
              "selection_n_params": 2,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 0.3158625206063066
                }
              ]
            },
            "F1:logN": {
              "coef": [
                0.15742720494403759,
                0.017741530173426417
              ],
              "columns": [
                "b0",
                "b1"
              ],
              "n_params": 2,
              "rank": 2,
              "column_mean": [
                0.0,
                0.0
              ],
              "column_scale": [
                0.6999208707326598,
                1.2432284815872339
              ],
              "standardized_coef": [
                0.11018658636143967,
                0.02205677561854302
              ],
              "sse": 0.31994461542482466,
              "ridge_objective": 0.31995724300998934,
              "effective_df": 1.9999869195464919,
              "intercept_unpenalized": false,
              "estimator": "V56 standardized ridge, lambda=0.001",
              "T_star": null,
              "method": "F1:logN",
              "selection_n_params": 2,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 0.31994461542482466
                }
              ]
            },
            "F2:L0": {
              "coef": [
                0.060952881527360746,
                0.004102475680641165,
                0.13252972429909557,
                -0.01996364988508595
              ],
              "columns": [
                "b0",
                "b1",
                "b2",
                "b3"
              ],
              "n_params": 4,
              "rank": 4,
              "column_mean": [
                0.0,
                0.0,
                0.0,
                0.0
              ],
              "column_scale": [
                0.24086751939138176,
                0.5632977612697625,
                0.6999208707326598,
                1.2295118688217672
              ],
              "standardized_coef": [
                0.01468156937325216,
                0.0023109153665688137,
                0.09276032002938231,
                -0.024545544478715483
              ],
              "sse": 0.2935212818199757,
              "ridge_objective": 0.2935307096695105,
              "effective_df": 3.999855695003592,
              "intercept_unpenalized": false,
              "estimator": "V56 standardized ridge, lambda=0.001",
              "T_star": 140000,
              "method": "F2:L0",
              "selection_n_params": 5,
              "T_star_grid_sse": [
                {
                  "T_star": 17500,
                  "sse": 0.30544248675508245
                },
                {
                  "T_star": 35000,
                  "sse": 0.3021486116564483
                },
                {
                  "T_star": 70000,
                  "sse": 0.29646618782354633
                },
                {
                  "T_star": 140000,
                  "sse": 0.2935212818199757
                },
                {
                  "T_star": 280000,
                  "sse": 0.29487246409644324
                }
              ]
            },
            "F2:logN": {
              "coef": [
                0.06055806244059962,
                -0.011381973551954448,
                0.1324832512263962,
                0.022072985600691684
              ],
              "columns": [
                "b0",
                "b1",
                "b2",
                "b3"
              ],
              "n_params": 4,
              "rank": 4,
              "column_mean": [
                0.0,
                0.0,
                0.0,
                0.0
              ],
              "column_scale": [
                0.24086751939138176,
                0.56810518448474,
                0.6999208707326598,
                1.2432284815872339
              ],
              "standardized_coef": [
                0.014586470279215637,
                -0.006466158184533513,
                0.09272779255587296,
                0.0274417643724448
              ],
              "sse": 0.2967255368425055,
              "ridge_objective": 0.29673514291276654,
              "effective_df": 3.9998559452686098,
              "intercept_unpenalized": false,
              "estimator": "V56 standardized ridge, lambda=0.001",
              "T_star": 140000,
              "method": "F2:logN",
              "selection_n_params": 5,
              "T_star_grid_sse": [
                {
                  "T_star": 17500,
                  "sse": 0.3105586961444763
                },
                {
                  "T_star": 35000,
                  "sse": 0.3066988540388428
                },
                {
                  "T_star": 70000,
                  "sse": 0.3001305534273628
                },
                {
                  "T_star": 140000,
                  "sse": 0.2967255368425055
                },
                {
                  "T_star": 280000,
                  "sse": 0.29811414554971105
                }
              ]
            },
            "T-only": {
              "coef": [
                -0.015371568023798576,
                0.1334830694545319
              ],
              "columns": [
                "b0",
                "b1"
              ],
              "n_params": 2,
              "rank": 2,
              "column_mean": [
                0.0,
                1.4127127929247456
              ],
              "column_scale": [
                1.0,
                0.5586406513529452
              ],
              "standardized_coef": [
                0.17320167183348098,
                0.07456906886467012
              ],
              "sse": 0.8181460839522186,
              "ridge_objective": 0.8181516444982498,
              "effective_df": 1.999990000099999,
              "intercept_unpenalized": true,
              "estimator": "V56 standardized ridge, lambda=0.001",
              "T_star": null,
              "method": "T-only",
              "selection_n_params": 2,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 0.8181460839522186
                }
              ]
            },
            "E-only": {
              "coef": [
                0.017161049185427518,
                0.14391672865468066
              ],
              "columns": [
                "b0",
                "b1"
              ],
              "n_params": 2,
              "rank": 2,
              "column_mean": [
                0.0,
                1.0842424234257253
              ],
              "column_scale": [
                1.0,
                0.6999208707326598
              ],
              "standardized_coef": [
                0.173201671833481,
                0.10073032203298003
              ],
              "sse": 0.35953173729633303,
              "ridge_objective": 0.3595418838941099,
              "effective_df": 1.999990000099999,
              "intercept_unpenalized": true,
              "estimator": "V56 standardized ridge, lambda=0.001",
              "T_star": null,
              "method": "E-only",
              "selection_n_params": 2,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 0.35953173729633303
                }
              ]
            },
            "surface:L0": {
              "coef": [
                -0.005650722926239388,
                0.02838148339100419,
                0.13012030169363922,
                -0.02176736191616726
              ],
              "columns": [
                "b0",
                "b1",
                "b2",
                "b3"
              ],
              "n_params": 4,
              "rank": 4,
              "column_mean": [
                0.0,
                1.4127127929247456,
                1.0842424234257253,
                0.10678561614781082
              ],
              "column_scale": [
                1.0,
                0.5586406513529452,
                0.6999208707326598,
                0.9623186761583143
              ],
              "standardized_coef": [
                0.173201671833481,
                0.015855050367913376,
                0.09107391486140837,
                -0.020947138902624986
              ],
              "sse": 0.29992558284837706,
              "ridge_objective": 0.29993456747159564,
              "effective_df": 3.9999557137666404,
              "intercept_unpenalized": true,
              "estimator": "V56 standardized ridge, lambda=0.001",
              "T_star": null,
              "method": "surface:L0",
              "selection_n_params": 4,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 0.29992558284837706
                }
              ]
            },
            "surface:logN": {
              "coef": [
                -0.005999909613518234,
                0.028537689294728455,
                0.12991809785689273,
                0.019550996948294642
              ],
              "columns": [
                "b0",
                "b1",
                "b2",
                "b3"
              ],
              "n_params": 4,
              "rank": 4,
              "column_mean": [
                0.0,
                1.4127127929247456,
                1.0842424234257253,
                -0.10110433614310209
              ],
              "column_scale": [
                1.0,
                0.5586406513529452,
                0.6999208707326598,
                0.9705677865952219
              ],
              "standardized_coef": [
                0.17320167183348098,
                0.015942313335715073,
                0.09093238817592728,
                0.01897556783383627
              ],
              "sse": 0.3077823206169306,
              "ridge_objective": 0.3077912035456791,
              "effective_df": 3.999955718536262,
              "intercept_unpenalized": true,
              "estimator": "V56 standardized ridge, lambda=0.001",
              "T_star": null,
              "method": "surface:logN",
              "selection_n_params": 4,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 0.3077823206169306
                }
              ]
            }
          },
          "qa": {
            "constant": {
              "coef": [
                -0.4321713147410356
              ],
              "rank": 1,
              "n_params": 1,
              "sse": 284.13968105882003,
              "estimator": "V50 OLS",
              "T_star": null,
              "method": "constant",
              "selection_n_params": 1,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 284.13968105882003
                }
              ]
            },
            "constant+src": {
              "coef": [
                -0.42464251113419743,
                0.07480965522892569
              ],
              "rank": 2,
              "n_params": 2,
              "sse": 283.61732802813845,
              "estimator": "V50 OLS",
              "T_star": null,
              "method": "constant+src",
              "selection_n_params": 2,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 283.61732802813845
                }
              ]
            },
            "T": {
              "coef": [
                -0.05168563598155366
              ],
              "rank": 1,
              "n_params": 1,
              "sse": 302.20036891493106,
              "estimator": "V50 OLS",
              "T_star": null,
              "method": "T",
              "selection_n_params": 1,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 302.20036891493106
                }
              ]
            },
            "T+src": {
              "coef": [
                -0.04198702710998694,
                0.09545971005436725
              ],
              "rank": 2,
              "n_params": 2,
              "sse": 300.2388444387371,
              "estimator": "V50 OLS",
              "T_star": null,
              "method": "T+src",
              "selection_n_params": 2,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 300.2388444387371
                }
              ]
            },
            "E": {
              "coef": [
                0.3273172564742093
              ],
              "rank": 1,
              "n_params": 1,
              "sse": 284.97359934174057,
              "estimator": "V50 OLS",
              "T_star": null,
              "method": "E",
              "selection_n_params": 1,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 284.97359934174057
                }
              ]
            },
            "E+src": {
              "coef": [
                0.35588711247106464,
                0.21775647224592007
              ],
              "rank": 2,
              "n_params": 2,
              "sse": 277.7720533473062,
              "estimator": "V50 OLS",
              "T_star": null,
              "method": "E+src",
              "selection_n_params": 2,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 277.7720533473062
                }
              ]
            },
            "joint": {
              "coef": [
                -2.9688116523930717,
                1.356158261677763,
                -1.023683789975026
              ],
              "rank": 3,
              "n_params": 3,
              "sse": 55.24420503489745,
              "estimator": "V50 OLS",
              "T_star": null,
              "method": "joint",
              "selection_n_params": 3,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 55.24420503489745
                }
              ]
            },
            "joint+src": {
              "coef": [
                -2.9593258292685753,
                1.3566614237367545,
                -1.0287256331670844,
                0.12471091664609944
              ],
              "rank": 4,
              "n_params": 4,
              "sse": 51.90007822703503,
              "estimator": "V50 OLS",
              "T_star": null,
              "method": "joint+src",
              "selection_n_params": 4,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 51.90007822703503
                }
              ]
            },
            "F1:L0": {
              "coef": [
                0.3339597883146617,
                0.20951496896600255
              ],
              "columns": [
                "b0",
                "b1"
              ],
              "n_params": 2,
              "rank": 2,
              "column_mean": [
                0.0,
                0.0
              ],
              "column_scale": [
                0.6999208707326598,
                1.3498814632932603
              ],
              "standardized_coef": [
                0.23374542582689278,
                0.28282037288966955
              ],
              "sse": 276.9779561029243,
              "ridge_objective": 276.9780907272117,
              "effective_df": 1.9999870518873917,
              "intercept_unpenalized": false,
              "estimator": "V56 standardized ridge, lambda=0.001",
              "T_star": null,
              "method": "F1:L0",
              "selection_n_params": 2,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 276.9779561029243
                }
              ]
            },
            "F1:logN": {
              "coef": [
                0.35588575780811676,
                0.21675290454123844
              ],
              "columns": [
                "b0",
                "b1"
              ],
              "n_params": 2,
              "rank": 2,
              "column_mean": [
                0.0,
                0.0
              ],
              "column_scale": [
                0.6999208707326598,
                1.2432284815872339
              ],
              "standardized_coef": [
                0.2490918694864096,
                0.2694733843924265
              ],
              "sse": 277.77205334832485,
              "ridge_objective": 277.77218801098917,
              "effective_df": 1.9999869195464919,
              "intercept_unpenalized": false,
              "estimator": "V56 standardized ridge, lambda=0.001",
              "T_star": null,
              "method": "F1:logN",
              "selection_n_params": 2,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 277.77205334832485
                }
              ]
            },
            "F2:L0": {
              "coef": [
                -2.9104084216207613,
                -0.5105566952521462,
                2.1944230187138922,
                0.5385719267152923
              ],
              "columns": [
                "b0",
                "b1",
                "b2",
                "b3"
              ],
              "n_params": 4,
              "rank": 4,
              "column_mean": [
                0.0,
                0.0,
                0.0,
                0.0
              ],
              "column_scale": [
                0.05112911845051045,
                1.0005499058201779,
                0.6999208707326598,
                1.3498814632932603
              ],
              "standardized_coef": [
                -0.14880661692841107,
                -0.5108374533503961,
                1.5359224700140193,
                0.7270082605231093
              ],
              "sse": 56.36758371109217,
              "ridge_objective": 56.37075440824992,
              "effective_df": 3.9999154189112316,
              "intercept_unpenalized": false,
              "estimator": "V56 standardized ridge, lambda=0.001",
              "T_star": 17500,
              "method": "F2:L0",
              "selection_n_params": 5,
              "T_star_grid_sse": [
                {
                  "T_star": 17500,
                  "sse": 56.36758371109217
                },
                {
                  "T_star": 35000,
                  "sse": 63.96460599433314
                },
                {
                  "T_star": 70000,
                  "sse": 105.4310359206424
                },
                {
                  "T_star": 140000,
                  "sse": 172.69570334009404
                },
                {
                  "T_star": 280000,
                  "sse": 218.8290311850522
                }
              ]
            },
            "F2:logN": {
              "coef": [
                -2.964719585478156,
                -0.5512432653142666,
                2.25944090594338,
                0.6026666942517298
              ],
              "columns": [
                "b0",
                "b1",
                "b2",
                "b3"
              ],
              "n_params": 4,
              "rank": 4,
              "column_mean": [
                0.0,
                0.0,
                0.0,
                0.0
              ],
              "column_scale": [
                0.05112911845051045,
                0.9379128174747559,
                0.6999208707326598,
                1.2432284815872339
              ],
              "standardized_coef": [
                -0.15158349885846087,
                -0.5170181240848881,
                1.5814298462568803,
                0.7492523991977758
              ],
              "sse": 55.3171695388007,
              "ridge_objective": 55.32052212361479,
              "effective_df": 3.9999151987654216,
              "intercept_unpenalized": false,
              "estimator": "V56 standardized ridge, lambda=0.001",
              "T_star": 17500,
              "method": "F2:logN",
              "selection_n_params": 5,
              "T_star_grid_sse": [
                {
                  "T_star": 17500,
                  "sse": 55.3171695388007
                },
                {
                  "T_star": 35000,
                  "sse": 62.1868912999047
                },
                {
                  "T_star": 70000,
                  "sse": 102.91177483849286
                },
                {
                  "T_star": 140000,
                  "sse": 170.45133096964065
                },
                {
                  "T_star": 280000,
                  "sse": 217.33439811084986
                }
              ]
            },
            "T-only": {
              "coef": [
                -2.65593551989825,
                1.5741092006064064
              ],
              "columns": [
                "b0",
                "b1"
              ],
              "n_params": 2,
              "rank": 2,
              "column_mean": [
                0.0,
                1.4127127929247456
              ],
              "column_scale": [
                1.0,
                0.5586406513529452
              ],
              "standardized_coef": [
                -0.43217131474103554,
                0.8793613891274267
              ],
              "sse": 206.81048923710284,
              "ridge_objective": 206.81126251355553,
              "effective_df": 1.999990000099999,
              "intercept_unpenalized": true,
              "estimator": "V56 standardized ridge, lambda=0.001",
              "T_star": null,
              "method": "T-only",
              "selection_n_params": 2,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 206.81048923710284
                }
              ]
            },
            "E-only": {
              "coef": [
                -2.6757452814197427,
                2.0692549177240345
              ],
              "columns": [
                "b0",
                "b1"
              ],
              "n_params": 2,
              "rank": 2,
              "column_mean": [
                0.0,
                1.0842424234257253
              ],
              "column_scale": [
                1.0,
                0.6999208707326598
              ],
              "standardized_coef": [
                -0.43217131474103565,
                1.4483147037812445
              ],
              "sse": 74.37393770896229,
              "ridge_objective": 74.37603532444348,
              "effective_df": 1.999990000099999,
              "intercept_unpenalized": true,
              "estimator": "V56 standardized ridge, lambda=0.001",
              "T_star": null,
              "method": "E-only",
              "selection_n_params": 2,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 74.37393770896229
                }
              ]
            },
            "surface:L0": {
              "coef": [
                -2.529919529224559,
                -0.16894242463070927,
                2.157046336561663,
                0.09644470450487758
              ],
              "columns": [
                "b0",
                "b1",
                "b2",
                "b3"
              ],
              "n_params": 4,
              "rank": 4,
              "column_mean": [
                0.0,
                1.4127127929247456,
                1.0842424234257253,
                -0.024322832240421786
              ],
              "column_scale": [
                1.0,
                0.5586406513529452,
                0.6999208707326598,
                1.0353807984163887
              ],
              "standardized_coef": [
                -0.4321713147410356,
                -0.09437810613684527,
                1.5097617500969331,
                0.09985699515329283
              ],
              "sse": 72.86291953917602,
              "ridge_objective": 72.86521779836447,
              "effective_df": 3.999955752094182,
              "intercept_unpenalized": true,
              "estimator": "V56 standardized ridge, lambda=0.001",
              "T_star": null,
              "method": "surface:L0",
              "selection_n_params": 4,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 72.86291953917602
                }
              ]
            },
            "surface:logN": {
              "coef": [
                -2.5206848230366896,
                -0.17307349743003683,
                2.1623938858538967,
                0.11416458886162384
              ],
              "columns": [
                "b0",
                "b1",
                "b2",
                "b3"
              ],
              "n_params": 4,
              "rank": 4,
              "column_mean": [
                0.0,
                1.4127127929247456,
                1.0842424234257253,
                -0.10110433614310209
              ],
              "column_scale": [
                1.0,
                0.5586406513529452,
                0.6999208707326598,
                0.9705677865952219
              ],
              "standardized_coef": [
                -0.43217131474103554,
                -0.09668589133624805,
                1.5135046114538393,
                0.11080447231897977
              ],
              "sse": 72.63351921391468,
              "ridge_objective": 72.63583153591624,
              "effective_df": 3.999955718536262,
              "intercept_unpenalized": true,
              "estimator": "V56 standardized ridge, lambda=0.001",
              "T_star": null,
              "method": "surface:logN",
              "selection_n_params": 4,
              "T_star_grid_sse": [
                {
                  "T_star": null,
                  "sse": 72.63351921391468
                }
              ]
            }
          }
        }
      ]
    },
    "$m_c$=med; $A,B$ affine in descriptor; $b/g$=bits/groups. Budget/reuse forms: fold-selected; counts per capability. Dev. baselines (math/code/QA): A2=per-density regression, med=dev. median, surf=response surface, E/T=E-only/T-only, L/N=loss/size surface. Pool pairs: student order. Not tested: density holdout, exact fixed-budget reuse."
  ],
  "context": [
    "results/v53-prune-dev/register.json#/feature_names",
    "results/v55-quant-group/register.json#/feature_names",
    "results/a2-curvature-interaction/summary.json#/protocol/descriptors",
    "results/a2-curvature-interaction/summary.json#/protocol/structures",
    "results/a2-curvature-interaction/summary.json#/protocol/I_U",
    "results/v70-distill-confirm/freeze.json#/reference_rule"
  ],
  "note": "",
  "rendered": "Frozen MAEs: native-token nats, training probes; stored intervals in brackets. Inputs: source size, initial loss and pretraining tokens for source-conditioned forms; the configuration for all; distillation forms take supervised budget, pool size and reuse. $r=(1-d)/0.3$; $Q_c=a+bu+cv+duv+eu^2$; $\\ell_E=\\log(1+E)$; $m_c$=med; $A,B$ affine in descriptor; $b/g$=bits/groups. Budget/reuse forms: fold-selected; counts per capability. Dev. baselines (math/code/QA): A2=per-density regression, med=dev. median, surf=response surface, E/T=E-only/T-only, L/N=loss/size surface. Pool pairs: student order. Not tested: density holdout, exact fixed-budget reuse."
}
```

## Input hashes

- `results/a2-curvature-interaction/summary.json`: `aed1934bf0c81333e200678f08567d018575fb3fcef7e2ecfcd881c95d3f820f`
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
- `results/v70-distill-confirm/freeze.json`: `d7b28c7251dbc6113c3de7c957560827e603d4e77a48010f99835a8468db0c24`
- `results/v72-prune-repeat/compare.json`: `639eef759655038f393e0451b4d7471883dae31d4da08ffe32a6277eaec76fb9`
- `results/v72-prune-repeat/freeze.json`: `3f4e45d0bd505b7d65815f2246a5c3b343f3a49be465aedf724aaa208b0de8b9`
- `results/v78-rule-confirm/compare.json`: `601669be112c5dd7c016e859423700a98f6a916dcd12c838bb5cd9c8c09686a8`
- `results/v78-rule-confirm/freeze.json`: `78dd229d7131f485b3a0651eac6978d2671ad139c02fcc2ea753d3420d5f129f`
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
