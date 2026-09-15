# Main prediction table: cell sources

Columns: task, relation, inputs, tested range, error, development baseline, status.
All indices are zero-based JSON pointers. `mean` is equal-weight arithmetic only; no refits or resampling.
Numeric values are formatted directly from the following executable source recipes. Context pointers justify textual labels and missing evidence.

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

## Fields per cell

- Cell (0, 0): `results/v53-prune-dev/register.json#/selected_candidate`; `results/v53-prune-dev/register.json#/test_densities`
- Cell (0, 1): `results/v53-prune-dev/register.json#/candidate_definitions/power`; `results/v53-prune-dev/register.json#/n_params_per_capability/power`
- Cell (0, 2): `results/v53-prune-dev/register.json#/selected_candidate`; `results/v53-prune-dev/register.json#/test_densities`; `results/v53-prune-dev/register.json#/feature_names`
- Cell (0, 3): `results/v72-prune-repeat/freeze.json#/predictions/0/source`; `results/v72-prune-repeat/freeze.json#/predictions/1/source`; `results/v72-prune-repeat/freeze.json#/predictions/2/source`; `results/v72-prune-repeat/freeze.json#/predictions/3/source`; `results/v72-prune-repeat/freeze.json#/predictions/4/source`; `results/v72-prune-repeat/freeze.json#/predictions/5/source`; `results/v72-prune-repeat/freeze.json#/predictions/6/source`; `results/v72-prune-repeat/freeze.json#/predictions/7/source`; `results/v72-prune-repeat/freeze.json#/predictions/8/source`; `results/v72-prune-repeat/freeze.json#/predictions/9/source`; `results/v72-prune-repeat/freeze.json#/predictions/10/source`; `results/v72-prune-repeat/freeze.json#/predictions/11/source`; `results/v72-prune-repeat/freeze.json#/predictions/12/source`; `results/v72-prune-repeat/freeze.json#/predictions/13/source`; `results/v72-prune-repeat/freeze.json#/predictions/14/source`; `results/v72-prune-repeat/freeze.json#/predictions/15/source`; `results/v72-prune-repeat/freeze.json#/predictions/16/source`; `results/v72-prune-repeat/freeze.json#/predictions/17/source`; `results/v72-prune-repeat/freeze.json#/predictions/0/density`; `results/v72-prune-repeat/freeze.json#/predictions/1/density`; `results/v72-prune-repeat/freeze.json#/predictions/2/density`; `results/v72-prune-repeat/freeze.json#/predictions/3/density`; `results/v72-prune-repeat/freeze.json#/predictions/4/density`; `results/v72-prune-repeat/freeze.json#/predictions/5/density`; `results/v72-prune-repeat/freeze.json#/predictions/6/density`; `results/v72-prune-repeat/freeze.json#/predictions/7/density`; `results/v72-prune-repeat/freeze.json#/predictions/8/density`; `results/v72-prune-repeat/freeze.json#/predictions/9/density`; `results/v72-prune-repeat/freeze.json#/predictions/10/density`; `results/v72-prune-repeat/freeze.json#/predictions/11/density`; `results/v72-prune-repeat/freeze.json#/predictions/12/density`; `results/v72-prune-repeat/freeze.json#/predictions/13/density`; `results/v72-prune-repeat/freeze.json#/predictions/14/density`; `results/v72-prune-repeat/freeze.json#/predictions/15/density`; `results/v72-prune-repeat/freeze.json#/predictions/16/density`; `results/v72-prune-repeat/freeze.json#/predictions/17/density`
- Cell (0, 4): `results/v53-prune-dev/register.json#/selected_candidate`; `results/v53-prune-dev/register.json#/test_densities`; `results/v72-prune-repeat/compare.json#/scores/power/by_capability/math/mae`; `results/v72-prune-repeat/compare.json#/scores/power/by_capability/code/mae`; `results/v72-prune-repeat/compare.json#/scores/power/by_capability/qa/mae`
- Cell (0, 5): `results/v53-prune-dev/register.json#/loso_table`; `results/v53-prune-dev/register.json#/loso_table/2/candidate`; `results/v72-prune-repeat/compare.json#/scores/A2/by_capability/math/mae`; `results/v72-prune-repeat/compare.json#/scores/A2/by_capability/code/mae`; `results/v53-prune-dev/register.json#/loso_table/5/candidate`; `results/v72-prune-repeat/compare.json#/scores/median_curve/by_capability/qa/mae`
- Cell (0, 6): `results/v72-prune-repeat/freeze.json#/selected_candidate`
- Cell (1, 0): `results/v53-prune-dev/register.json#/selected_candidate`; `results/v53-prune-dev/register.json#/test_densities`
- Cell (1, 1): `results/v53-prune-dev/register.json#/candidate_definitions/power`; `results/v53-prune-dev/register.json#/n_params_per_capability/power`
- Cell (1, 2): `results/v53-prune-dev/register.json#/selected_candidate`; `results/v53-prune-dev/register.json#/test_densities`; `results/v53-prune-dev/register.json#/feature_names`
- Cell (1, 3): `results/v53-prune-dev/compare_pythia-410m@step48000.json#/tag`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/tag`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/tag`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/densities`
- Cell (1, 4): `results/v53-prune-dev/register.json#/selected_candidate`; `results/v53-prune-dev/register.json#/test_densities`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/power/math`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/power/math`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/power/math`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/power/code`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/power/code`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/power/code`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/power/qa`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/power/qa`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/power/qa`
- Cell (1, 5): `results/v53-prune-dev/register.json#/loso_table`; `results/v53-prune-dev/register.json#/loso_table/2/candidate`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/A2/math`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/A2/math`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/A2/math`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/A2/code`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/A2/code`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/A2/code`; `results/v53-prune-dev/register.json#/loso_table/5/candidate`; `results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/qa`; `results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/qa`; `results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/qa`
- Cell (1, 6): `results/v53-prune-dev/register.json#/selected_candidate`
- Cell (2, 0): `results/v55-quant-group/register.json#/test_sets/bit_test`
- Cell (2, 1): `results/v55-quant-group/register.json#/candidate_definitions/low_order_2d`; `results/v55-quant-group/register.json#/n_params_per_capability/low_order_2d`
- Cell (2, 2): `results/v55-quant-group/register.json#/test_sets/bit_test/configs`; `results/v55-quant-group/register.json#/feature_names`
- Cell (2, 3): `results/v55-quant-group/register.json#/test_sets/bit_test/states`; `results/v55-quant-group/register.json#/test_sets/bit_test/configs`
- Cell (2, 4): `results/v55-quant-group/compare.json#/test_sets/bit_test/mae_table/1/mae/math`; `results/v55-quant-group/compare.json#/test_sets/bit_test/mae_table/1/mae/code`; `results/v55-quant-group/compare.json#/test_sets/bit_test/mae_table/1/mae/qa`
- Cell (2, 5): `results/v55-quant-group/register.json#/loso_table`; `results/v55-quant-group/register.json#/loso_table/4/candidate`; `results/v55-quant-group/compare.json#/test_sets/bit_test/mae_table/4/mae/math`; `results/v55-quant-group/compare.json#/test_sets/bit_test/mae_table/4/mae/code`; `results/v55-quant-group/compare.json#/test_sets/bit_test/mae_table/4/mae/qa`
- Cell (2, 6): `results/v55-quant-group/register.json#/precommitted_rule`
- Cell (3, 0): `results/v69-quant-confirm/compare.json#/rows/0/test_set`; `results/v69-quant-confirm/compare.json#/rows/1/test_set`; `results/v69-quant-confirm/compare.json#/rows/2/test_set`; `results/v69-quant-confirm/compare.json#/rows/3/test_set`; `results/v69-quant-confirm/compare.json#/rows/4/test_set`; `results/v69-quant-confirm/compare.json#/rows/5/test_set`; `results/v69-quant-confirm/compare.json#/rows/6/test_set`; `results/v69-quant-confirm/compare.json#/rows/7/test_set`; `results/v69-quant-confirm/compare.json#/rows/8/test_set`; `results/v69-quant-confirm/compare.json#/rows/9/test_set`; `results/v69-quant-confirm/compare.json#/rows/10/test_set`; `results/v69-quant-confirm/compare.json#/rows/11/test_set`; `results/v69-quant-confirm/compare.json#/rows/12/test_set`; `results/v69-quant-confirm/compare.json#/rows/13/test_set`; `results/v69-quant-confirm/compare.json#/rows/14/test_set`; `results/v69-quant-confirm/compare.json#/rows/15/test_set`; `results/v69-quant-confirm/compare.json#/rows/16/test_set`; `results/v69-quant-confirm/compare.json#/rows/17/test_set`; `results/v69-quant-confirm/compare.json#/rows/18/test_set`; `results/v69-quant-confirm/compare.json#/rows/19/test_set`; `results/v69-quant-confirm/compare.json#/rows/20/test_set`; `results/v69-quant-confirm/compare.json#/rows/21/test_set`; `results/v69-quant-confirm/compare.json#/rows/22/test_set`; `results/v69-quant-confirm/compare.json#/rows/23/test_set`; `results/v69-quant-confirm/compare.json#/rows/24/test_set`; `results/v69-quant-confirm/compare.json#/rows/25/test_set`; `results/v69-quant-confirm/compare.json#/rows/26/test_set`; `results/v69-quant-confirm/compare.json#/rows/27/test_set`; `results/v69-quant-confirm/compare.json#/rows/28/test_set`; `results/v69-quant-confirm/compare.json#/rows/29/test_set`; `results/v69-quant-confirm/compare.json#/rows/30/test_set`; `results/v69-quant-confirm/compare.json#/rows/31/test_set`; `results/v69-quant-confirm/compare.json#/rows/32/test_set`; `results/v69-quant-confirm/compare.json#/rows/33/test_set`; `results/v69-quant-confirm/compare.json#/rows/34/test_set`; `results/v69-quant-confirm/compare.json#/rows/35/test_set`
- Cell (3, 1): `results/v55-quant-group/register.json#/candidate_definitions/low_order_2d`; `results/v69-quant-confirm/develop.json#/models`; `results/v69-quant-confirm/develop.json#/selected/math/candidate`; `results/v69-quant-confirm/develop.json#/selected/math/n_coefficients`; `results/v69-quant-confirm/develop.json#/selected/code/candidate`; `results/v69-quant-confirm/develop.json#/selected/code/n_coefficients`; `results/v69-quant-confirm/develop.json#/selected/qa/candidate`; `results/v69-quant-confirm/develop.json#/selected/qa/n_coefficients`
- Cell (3, 2): `results/v69-quant-confirm/develop.json#/dev_configs`; `results/v69-quant-confirm/develop.json#/feature_names`
- Cell (3, 3): `results/v69-quant-confirm/compare.json#/rows/0/state`; `results/v69-quant-confirm/compare.json#/rows/1/state`; `results/v69-quant-confirm/compare.json#/rows/2/state`; `results/v69-quant-confirm/compare.json#/rows/3/state`; `results/v69-quant-confirm/compare.json#/rows/4/state`; `results/v69-quant-confirm/compare.json#/rows/5/state`; `results/v69-quant-confirm/compare.json#/rows/6/state`; `results/v69-quant-confirm/compare.json#/rows/7/state`; `results/v69-quant-confirm/compare.json#/rows/8/state`; `results/v69-quant-confirm/compare.json#/rows/9/state`; `results/v69-quant-confirm/compare.json#/rows/10/state`; `results/v69-quant-confirm/compare.json#/rows/11/state`; `results/v69-quant-confirm/compare.json#/rows/12/state`; `results/v69-quant-confirm/compare.json#/rows/13/state`; `results/v69-quant-confirm/compare.json#/rows/14/state`; `results/v69-quant-confirm/compare.json#/rows/15/state`; `results/v69-quant-confirm/compare.json#/rows/16/state`; `results/v69-quant-confirm/compare.json#/rows/17/state`; `results/v69-quant-confirm/compare.json#/rows/18/state`; `results/v69-quant-confirm/compare.json#/rows/19/state`; `results/v69-quant-confirm/compare.json#/rows/20/state`; `results/v69-quant-confirm/compare.json#/rows/21/state`; `results/v69-quant-confirm/compare.json#/rows/22/state`; `results/v69-quant-confirm/compare.json#/rows/23/state`; `results/v69-quant-confirm/compare.json#/rows/24/state`; `results/v69-quant-confirm/compare.json#/rows/25/state`; `results/v69-quant-confirm/compare.json#/rows/26/state`; `results/v69-quant-confirm/compare.json#/rows/27/state`; `results/v69-quant-confirm/compare.json#/rows/28/state`; `results/v69-quant-confirm/compare.json#/rows/29/state`; `results/v69-quant-confirm/compare.json#/rows/30/state`; `results/v69-quant-confirm/compare.json#/rows/31/state`; `results/v69-quant-confirm/compare.json#/rows/32/state`; `results/v69-quant-confirm/compare.json#/rows/33/state`; `results/v69-quant-confirm/compare.json#/rows/34/state`; `results/v69-quant-confirm/compare.json#/rows/35/state`; `results/v69-quant-confirm/compare.json#/rows/0/config`; `results/v69-quant-confirm/compare.json#/rows/1/config`; `results/v69-quant-confirm/compare.json#/rows/2/config`; `results/v69-quant-confirm/compare.json#/rows/3/config`; `results/v69-quant-confirm/compare.json#/rows/4/config`; `results/v69-quant-confirm/compare.json#/rows/5/config`; `results/v69-quant-confirm/compare.json#/rows/6/config`; `results/v69-quant-confirm/compare.json#/rows/7/config`; `results/v69-quant-confirm/compare.json#/rows/8/config`; `results/v69-quant-confirm/compare.json#/rows/9/config`; `results/v69-quant-confirm/compare.json#/rows/10/config`; `results/v69-quant-confirm/compare.json#/rows/11/config`; `results/v69-quant-confirm/compare.json#/rows/12/config`; `results/v69-quant-confirm/compare.json#/rows/13/config`; `results/v69-quant-confirm/compare.json#/rows/14/config`; `results/v69-quant-confirm/compare.json#/rows/15/config`; `results/v69-quant-confirm/compare.json#/rows/16/config`; `results/v69-quant-confirm/compare.json#/rows/17/config`; `results/v69-quant-confirm/compare.json#/rows/18/config`; `results/v69-quant-confirm/compare.json#/rows/19/config`; `results/v69-quant-confirm/compare.json#/rows/20/config`; `results/v69-quant-confirm/compare.json#/rows/21/config`; `results/v69-quant-confirm/compare.json#/rows/22/config`; `results/v69-quant-confirm/compare.json#/rows/23/config`; `results/v69-quant-confirm/compare.json#/rows/24/config`; `results/v69-quant-confirm/compare.json#/rows/25/config`; `results/v69-quant-confirm/compare.json#/rows/26/config`; `results/v69-quant-confirm/compare.json#/rows/27/config`; `results/v69-quant-confirm/compare.json#/rows/28/config`; `results/v69-quant-confirm/compare.json#/rows/29/config`; `results/v69-quant-confirm/compare.json#/rows/30/config`; `results/v69-quant-confirm/compare.json#/rows/31/config`; `results/v69-quant-confirm/compare.json#/rows/32/config`; `results/v69-quant-confirm/compare.json#/rows/33/config`; `results/v69-quant-confirm/compare.json#/rows/34/config`; `results/v69-quant-confirm/compare.json#/rows/35/config`
- Cell (3, 4): `results/v69-quant-confirm/compare.json#/rows/0/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/3/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/6/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/9/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/12/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/15/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/18/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/21/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/24/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/27/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/30/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/33/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/1/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/4/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/7/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/10/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/13/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/16/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/19/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/22/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/25/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/28/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/31/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/34/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/2/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/5/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/8/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/11/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/14/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/17/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/20/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/23/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/26/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/29/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/32/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/35/absolute_errors/zero`
- Cell (3, 5): `results/v69-quant-confirm/develop.json#/loso/scores`; `results/v69-quant-confirm/compare.json#/rows/0/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/3/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/6/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/9/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/12/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/15/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/18/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/21/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/24/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/27/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/30/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/33/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/1/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/4/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/7/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/10/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/13/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/16/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/19/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/22/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/25/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/28/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/31/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/34/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/2/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/5/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/8/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/11/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/14/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/17/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/20/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/23/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/26/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/29/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/32/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/35/absolute_errors/median`
- Cell (3, 6): `results/v69-quant-confirm/freeze.json#/frozen_at_utc`
- Cell (4, 0): `results/v69-quant-confirm/compare.json#/rows/36/test_set`; `results/v69-quant-confirm/compare.json#/rows/37/test_set`; `results/v69-quant-confirm/compare.json#/rows/38/test_set`; `results/v69-quant-confirm/compare.json#/rows/39/test_set`; `results/v69-quant-confirm/compare.json#/rows/40/test_set`; `results/v69-quant-confirm/compare.json#/rows/41/test_set`; `results/v69-quant-confirm/compare.json#/rows/42/test_set`; `results/v69-quant-confirm/compare.json#/rows/43/test_set`; `results/v69-quant-confirm/compare.json#/rows/44/test_set`; `results/v69-quant-confirm/compare.json#/rows/45/test_set`; `results/v69-quant-confirm/compare.json#/rows/46/test_set`; `results/v69-quant-confirm/compare.json#/rows/47/test_set`; `results/v69-quant-confirm/compare.json#/rows/48/test_set`; `results/v69-quant-confirm/compare.json#/rows/49/test_set`; `results/v69-quant-confirm/compare.json#/rows/50/test_set`; `results/v69-quant-confirm/compare.json#/rows/51/test_set`; `results/v69-quant-confirm/compare.json#/rows/52/test_set`; `results/v69-quant-confirm/compare.json#/rows/53/test_set`; `results/v69-quant-confirm/compare.json#/rows/54/test_set`; `results/v69-quant-confirm/compare.json#/rows/55/test_set`; `results/v69-quant-confirm/compare.json#/rows/56/test_set`; `results/v69-quant-confirm/compare.json#/rows/57/test_set`; `results/v69-quant-confirm/compare.json#/rows/58/test_set`; `results/v69-quant-confirm/compare.json#/rows/59/test_set`; `results/v69-quant-confirm/compare.json#/rows/60/test_set`; `results/v69-quant-confirm/compare.json#/rows/61/test_set`; `results/v69-quant-confirm/compare.json#/rows/62/test_set`
- Cell (4, 1): `results/v55-quant-group/register.json#/candidate_definitions/low_order_2d`; `results/v69-quant-confirm/develop.json#/models`; `results/v69-quant-confirm/develop.json#/selected/math/candidate`; `results/v69-quant-confirm/develop.json#/selected/math/n_coefficients`; `results/v69-quant-confirm/develop.json#/selected/code/candidate`; `results/v69-quant-confirm/develop.json#/selected/code/n_coefficients`; `results/v69-quant-confirm/develop.json#/selected/qa/candidate`; `results/v69-quant-confirm/develop.json#/selected/qa/n_coefficients`
- Cell (4, 2): `results/v69-quant-confirm/develop.json#/dev_configs`; `results/v69-quant-confirm/develop.json#/feature_names`
- Cell (4, 3): `results/v69-quant-confirm/compare.json#/rows/36/state`; `results/v69-quant-confirm/compare.json#/rows/37/state`; `results/v69-quant-confirm/compare.json#/rows/38/state`; `results/v69-quant-confirm/compare.json#/rows/39/state`; `results/v69-quant-confirm/compare.json#/rows/40/state`; `results/v69-quant-confirm/compare.json#/rows/41/state`; `results/v69-quant-confirm/compare.json#/rows/42/state`; `results/v69-quant-confirm/compare.json#/rows/43/state`; `results/v69-quant-confirm/compare.json#/rows/44/state`; `results/v69-quant-confirm/compare.json#/rows/45/state`; `results/v69-quant-confirm/compare.json#/rows/46/state`; `results/v69-quant-confirm/compare.json#/rows/47/state`; `results/v69-quant-confirm/compare.json#/rows/48/state`; `results/v69-quant-confirm/compare.json#/rows/49/state`; `results/v69-quant-confirm/compare.json#/rows/50/state`; `results/v69-quant-confirm/compare.json#/rows/51/state`; `results/v69-quant-confirm/compare.json#/rows/52/state`; `results/v69-quant-confirm/compare.json#/rows/53/state`; `results/v69-quant-confirm/compare.json#/rows/54/state`; `results/v69-quant-confirm/compare.json#/rows/55/state`; `results/v69-quant-confirm/compare.json#/rows/56/state`; `results/v69-quant-confirm/compare.json#/rows/57/state`; `results/v69-quant-confirm/compare.json#/rows/58/state`; `results/v69-quant-confirm/compare.json#/rows/59/state`; `results/v69-quant-confirm/compare.json#/rows/60/state`; `results/v69-quant-confirm/compare.json#/rows/61/state`; `results/v69-quant-confirm/compare.json#/rows/62/state`; `results/v69-quant-confirm/compare.json#/rows/36/config`; `results/v69-quant-confirm/compare.json#/rows/37/config`; `results/v69-quant-confirm/compare.json#/rows/38/config`; `results/v69-quant-confirm/compare.json#/rows/39/config`; `results/v69-quant-confirm/compare.json#/rows/40/config`; `results/v69-quant-confirm/compare.json#/rows/41/config`; `results/v69-quant-confirm/compare.json#/rows/42/config`; `results/v69-quant-confirm/compare.json#/rows/43/config`; `results/v69-quant-confirm/compare.json#/rows/44/config`; `results/v69-quant-confirm/compare.json#/rows/45/config`; `results/v69-quant-confirm/compare.json#/rows/46/config`; `results/v69-quant-confirm/compare.json#/rows/47/config`; `results/v69-quant-confirm/compare.json#/rows/48/config`; `results/v69-quant-confirm/compare.json#/rows/49/config`; `results/v69-quant-confirm/compare.json#/rows/50/config`; `results/v69-quant-confirm/compare.json#/rows/51/config`; `results/v69-quant-confirm/compare.json#/rows/52/config`; `results/v69-quant-confirm/compare.json#/rows/53/config`; `results/v69-quant-confirm/compare.json#/rows/54/config`; `results/v69-quant-confirm/compare.json#/rows/55/config`; `results/v69-quant-confirm/compare.json#/rows/56/config`; `results/v69-quant-confirm/compare.json#/rows/57/config`; `results/v69-quant-confirm/compare.json#/rows/58/config`; `results/v69-quant-confirm/compare.json#/rows/59/config`; `results/v69-quant-confirm/compare.json#/rows/60/config`; `results/v69-quant-confirm/compare.json#/rows/61/config`; `results/v69-quant-confirm/compare.json#/rows/62/config`
- Cell (4, 4): `results/v69-quant-confirm/compare.json#/rows/36/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/39/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/42/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/45/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/48/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/51/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/54/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/57/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/60/absolute_errors/low_order_2d`; `results/v69-quant-confirm/compare.json#/rows/37/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/40/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/43/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/46/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/49/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/52/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/55/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/58/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/61/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/38/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/41/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/44/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/47/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/50/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/53/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/56/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/59/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/62/absolute_errors/zero`
- Cell (4, 5): `results/v69-quant-confirm/develop.json#/loso/scores`; `results/v69-quant-confirm/compare.json#/rows/36/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/39/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/42/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/45/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/48/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/51/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/54/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/57/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/60/absolute_errors/bilinear`; `results/v69-quant-confirm/compare.json#/rows/37/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/40/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/43/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/46/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/49/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/52/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/55/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/58/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/61/absolute_errors/zero`; `results/v69-quant-confirm/compare.json#/rows/38/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/41/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/44/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/47/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/50/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/53/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/56/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/59/absolute_errors/median`; `results/v69-quant-confirm/compare.json#/rows/62/absolute_errors/median`
- Cell (4, 6): `results/v69-quant-confirm/freeze.json#/frozen_at_utc`
- Cell (5, 0): `results/a2-curvature-interaction/summary.json#/decision_table/18/target`; `results/a2-curvature-interaction/summary.json#/decision_table/6/target`; `results/a2-curvature-interaction/summary.json#/decision_table/54/target`
- Cell (5, 1): `results/a2-curvature-interaction/summary.json#/protocol/structures`; `results/a2-curvature-interaction/summary.json#/parameter_intervals/0/fits/F_log/fit/nominal_parameters`; `results/a2-curvature-interaction/summary.json#/parameter_intervals/0/fits/F_curv/fit/nominal_parameters`; `results/a2-curvature-interaction/summary.json#/parameter_intervals/0/fits/F_int/fit/nominal_parameters`
- Cell (5, 2): `results/a2-curvature-interaction/summary.json#/protocol/descriptors`; `results/a2-curvature-interaction/summary.json#/protocol/descriptor_calibration_cost`
- Cell (5, 3): `results/a2-curvature-interaction/summary.json#/parameter_intervals/0/fits/F_log/fit/standardizer/students`; `results/a2-curvature-interaction/summary.json#/protocol/largest_budget`; `results/a2-curvature-interaction/summary.json#/decision_table/6/distribution`; `results/a2-curvature-interaction/summary.json#/decision_table/18/distribution`; `results/a2-curvature-interaction/summary.json#/decision_table/54/distribution`
- Cell (5, 4): `results/a2-curvature-interaction/summary.json#/decision_table/18/primary_mae`; `results/a2-curvature-interaction/summary.json#/decision_table/18/primary_mae_interval/0`; `results/a2-curvature-interaction/summary.json#/decision_table/18/primary_mae_interval/1`; `results/a2-curvature-interaction/summary.json#/decision_table/6/primary_mae`; `results/a2-curvature-interaction/summary.json#/decision_table/6/primary_mae_interval/0`; `results/a2-curvature-interaction/summary.json#/decision_table/6/primary_mae_interval/1`; `results/a2-curvature-interaction/summary.json#/decision_table/54/primary_mae`; `results/a2-curvature-interaction/summary.json#/decision_table/54/primary_mae_interval/0`; `results/a2-curvature-interaction/summary.json#/decision_table/54/primary_mae_interval/1`
- Cell (5, 5): `results/a2-curvature-interaction/summary.json#/decision_table/18/inner_selected_baselines`; `results/a2-curvature-interaction/summary.json#/decision_table/18/baseline_mae`; `results/a2-curvature-interaction/summary.json#/decision_table/6/inner_selected_baselines`; `results/a2-curvature-interaction/summary.json#/decision_table/6/baseline_mae`; `results/a2-curvature-interaction/summary.json#/decision_table/54/inner_selected_baselines`; `results/a2-curvature-interaction/summary.json#/decision_table/54/baseline_mae`
- Cell (5, 6): `results/a2-curvature-interaction/summary.json#/protocol/secondary`; `results/a2-curvature-interaction/summary.json#/protocol/previous_F_int`
- Cell (6, 0): `results/a2-curvature-interaction/summary.json#/decision_table/14/target`; `results/a2-curvature-interaction/summary.json#/decision_table/2/target`; `results/a2-curvature-interaction/summary.json#/decision_table/50/target`
- Cell (6, 1): `results/a2-curvature-interaction/summary.json#/protocol/structures`; `results/a2-curvature-interaction/summary.json#/parameter_intervals/0/fits/F_log/fit/nominal_parameters`; `results/a2-curvature-interaction/summary.json#/parameter_intervals/0/fits/F_curv/fit/nominal_parameters`; `results/a2-curvature-interaction/summary.json#/parameter_intervals/0/fits/F_int/fit/nominal_parameters`
- Cell (6, 2): `results/a2-curvature-interaction/summary.json#/protocol/descriptors`; `results/a2-curvature-interaction/summary.json#/protocol/descriptor_calibration_cost`
- Cell (6, 3): `results/a2-curvature-interaction/summary.json#/parameter_intervals/0/fits/F_curv/fit/standardizer/students`; `results/a2-curvature-interaction/summary.json#/protocol/I_U`; `results/a2-curvature-interaction/summary.json#/decision_table/2/distribution`; `results/a2-curvature-interaction/summary.json#/decision_table/14/distribution`; `results/a2-curvature-interaction/summary.json#/decision_table/26/distribution`; `results/a2-curvature-interaction/summary.json#/decision_table/38/distribution`; `results/a2-curvature-interaction/summary.json#/decision_table/50/distribution`; `results/a2-curvature-interaction/summary.json#/decision_table/62/distribution`
- Cell (6, 4): `results/a2-curvature-interaction/summary.json#/decision_table/14/primary_mae`; `results/a2-curvature-interaction/summary.json#/decision_table/14/primary_mae_interval/0`; `results/a2-curvature-interaction/summary.json#/decision_table/14/primary_mae_interval/1`; `results/a2-curvature-interaction/summary.json#/decision_table/2/primary_mae`; `results/a2-curvature-interaction/summary.json#/decision_table/2/primary_mae_interval/0`; `results/a2-curvature-interaction/summary.json#/decision_table/2/primary_mae_interval/1`; `results/a2-curvature-interaction/summary.json#/decision_table/50/primary_mae`; `results/a2-curvature-interaction/summary.json#/decision_table/50/primary_mae_interval/0`; `results/a2-curvature-interaction/summary.json#/decision_table/50/primary_mae_interval/1`
- Cell (6, 5): `results/a2-curvature-interaction/summary.json#/decision_table/14/inner_selected_baselines`; `results/a2-curvature-interaction/summary.json#/decision_table/14/baseline_mae`; `results/a2-curvature-interaction/summary.json#/decision_table/2/inner_selected_baselines`; `results/a2-curvature-interaction/summary.json#/decision_table/2/baseline_mae`; `results/a2-curvature-interaction/summary.json#/decision_table/50/inner_selected_baselines`; `results/a2-curvature-interaction/summary.json#/decision_table/50/baseline_mae`
- Cell (6, 6): `results/a2-curvature-interaction/summary.json#/protocol/secondary`; `results/a2-curvature-interaction/summary.json#/protocol/previous_F_int`
- Cell (7, 0): `results/v70-distill-confirm/freeze.json#/confirmation_register/unused_U_assertion`
- Cell (7, 1): `results/v70-distill-confirm/freeze.json#/models`; `results/v70-distill-confirm/freeze.json#/reference_rule`; `results/v70-distill-confirm/freeze.json#/selected/math/method`; `results/v70-distill-confirm/freeze.json#/selected/math/n_params`; `results/v70-distill-confirm/freeze.json#/selected/code/method`; `results/v70-distill-confirm/freeze.json#/selected/code/n_params`; `results/v70-distill-confirm/freeze.json#/selected/qa/method`; `results/v70-distill-confirm/freeze.json#/selected/qa/n_params`
- Cell (7, 2): `results/v70-distill-confirm/freeze.json#/prediction_rule`; `results/v70-distill-confirm/freeze.json#/reference_rule`
- Cell (7, 3): `results/v70-distill-confirm/freeze.json#/confirmation_register/students`; `results/v70-distill-confirm/freeze.json#/confirmation_register/pools`; `results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned`
- Cell (7, 4): `results/v70-distill-confirm/compare.json#/groups/0/student`; `results/v70-distill-confirm/compare.json#/groups/0/capability`; `results/v70-distill-confirm/compare.json#/groups/0/candidate_mae`; `results/v70-distill-confirm/compare.json#/groups/1/student`; `results/v70-distill-confirm/compare.json#/groups/1/capability`; `results/v70-distill-confirm/compare.json#/groups/1/candidate_mae`; `results/v70-distill-confirm/compare.json#/groups/2/student`; `results/v70-distill-confirm/compare.json#/groups/2/capability`; `results/v70-distill-confirm/compare.json#/groups/2/candidate_mae`; `results/v70-distill-confirm/compare.json#/groups/3/student`; `results/v70-distill-confirm/compare.json#/groups/3/capability`; `results/v70-distill-confirm/compare.json#/groups/3/candidate_mae`; `results/v70-distill-confirm/compare.json#/groups/4/student`; `results/v70-distill-confirm/compare.json#/groups/4/capability`; `results/v70-distill-confirm/compare.json#/groups/4/candidate_mae`; `results/v70-distill-confirm/compare.json#/groups/5/student`; `results/v70-distill-confirm/compare.json#/groups/5/capability`; `results/v70-distill-confirm/compare.json#/groups/5/candidate_mae`
- Cell (7, 5): `results/v70-distill-confirm/freeze.json#/baseline_rule`; `results/v70-distill-confirm/freeze.json#/strongest_baseline`; `results/v70-distill-confirm/compare.json#/groups/0/student`; `results/v70-distill-confirm/compare.json#/groups/0/capability`; `results/v70-distill-confirm/compare.json#/groups/0/strongest_baseline`; `results/v70-distill-confirm/compare.json#/groups/0/baseline_mae`; `results/v70-distill-confirm/compare.json#/groups/0/paired_difference/estimate`; `results/v70-distill-confirm/compare.json#/groups/0/paired_difference/ci95/0`; `results/v70-distill-confirm/compare.json#/groups/0/paired_difference/ci95/1`; `results/v70-distill-confirm/compare.json#/groups/1/student`; `results/v70-distill-confirm/compare.json#/groups/1/capability`; `results/v70-distill-confirm/compare.json#/groups/1/strongest_baseline`; `results/v70-distill-confirm/compare.json#/groups/1/baseline_mae`; `results/v70-distill-confirm/compare.json#/groups/1/paired_difference/estimate`; `results/v70-distill-confirm/compare.json#/groups/1/paired_difference/ci95/0`; `results/v70-distill-confirm/compare.json#/groups/1/paired_difference/ci95/1`; `results/v70-distill-confirm/compare.json#/groups/2/student`; `results/v70-distill-confirm/compare.json#/groups/2/capability`; `results/v70-distill-confirm/compare.json#/groups/2/strongest_baseline`; `results/v70-distill-confirm/compare.json#/groups/2/baseline_mae`; `results/v70-distill-confirm/compare.json#/groups/2/paired_difference/estimate`; `results/v70-distill-confirm/compare.json#/groups/2/paired_difference/ci95/0`; `results/v70-distill-confirm/compare.json#/groups/2/paired_difference/ci95/1`; `results/v70-distill-confirm/compare.json#/groups/3/student`; `results/v70-distill-confirm/compare.json#/groups/3/capability`; `results/v70-distill-confirm/compare.json#/groups/3/strongest_baseline`; `results/v70-distill-confirm/compare.json#/groups/3/baseline_mae`; `results/v70-distill-confirm/compare.json#/groups/3/paired_difference/estimate`; `results/v70-distill-confirm/compare.json#/groups/3/paired_difference/ci95/0`; `results/v70-distill-confirm/compare.json#/groups/3/paired_difference/ci95/1`; `results/v70-distill-confirm/compare.json#/groups/4/student`; `results/v70-distill-confirm/compare.json#/groups/4/capability`; `results/v70-distill-confirm/compare.json#/groups/4/strongest_baseline`; `results/v70-distill-confirm/compare.json#/groups/4/baseline_mae`; `results/v70-distill-confirm/compare.json#/groups/4/paired_difference/estimate`; `results/v70-distill-confirm/compare.json#/groups/4/paired_difference/ci95/0`; `results/v70-distill-confirm/compare.json#/groups/4/paired_difference/ci95/1`; `results/v70-distill-confirm/compare.json#/groups/5/student`; `results/v70-distill-confirm/compare.json#/groups/5/capability`; `results/v70-distill-confirm/compare.json#/groups/5/strongest_baseline`; `results/v70-distill-confirm/compare.json#/groups/5/baseline_mae`; `results/v70-distill-confirm/compare.json#/groups/5/paired_difference/estimate`; `results/v70-distill-confirm/compare.json#/groups/5/paired_difference/ci95/0`; `results/v70-distill-confirm/compare.json#/groups/5/paired_difference/ci95/1`
- Cell (7, 6): `results/v70-distill-confirm/freeze.json#/frozen_at_utc`; `results/v47-p2-register/register.json#/v5_confirm/registered_at_utc`

## Machine-readable cell recipes

```json
[
  {
    "row": 0,
    "column": 0,
    "parts": [
      "Pruning: unseen density"
    ],
    "context": [
      "results/v53-prune-dev/register.json#/selected_candidate",
      "results/v53-prune-dev/register.json#/test_densities"
    ],
    "note": "",
    "rendered": "Pruning: unseen density"
  },
  {
    "row": 0,
    "column": 1,
    "parts": [
      {
        "sources": [
          "results/v53-prune-dev/register.json#/candidate_definitions/power"
        ],
        "op": "identity",
        "format": null
      },
      "; parameters ",
      {
        "sources": [
          "results/v53-prune-dev/register.json#/n_params_per_capability/power"
        ],
        "op": "identity",
        "format": null
      }
    ],
    "context": [],
    "note": "",
    "rendered": "(beta.phi) * ((1-d)/0.3)**gamma; parameters 5"
  },
  {
    "row": 0,
    "column": 2,
    "parts": [
      {
        "sources": [
          "results/v53-prune-dev/register.json#/feature_names"
        ],
        "op": "join",
        "format": null
      },
      "; density"
    ],
    "context": [
      "results/v53-prune-dev/register.json#/selected_candidate",
      "results/v53-prune-dev/register.json#/test_densities"
    ],
    "note": "",
    "rendered": "1, z(log N0), z(L0c), z(log D0); density"
  },
  {
    "row": 0,
    "column": 3,
    "parts": [
      "State labels: ",
      {
        "sources": [
          "results/v72-prune-repeat/freeze.json#/predictions/0/source",
          "results/v72-prune-repeat/freeze.json#/predictions/1/source",
          "results/v72-prune-repeat/freeze.json#/predictions/2/source",
          "results/v72-prune-repeat/freeze.json#/predictions/3/source",
          "results/v72-prune-repeat/freeze.json#/predictions/4/source",
          "results/v72-prune-repeat/freeze.json#/predictions/5/source",
          "results/v72-prune-repeat/freeze.json#/predictions/6/source",
          "results/v72-prune-repeat/freeze.json#/predictions/7/source",
          "results/v72-prune-repeat/freeze.json#/predictions/8/source",
          "results/v72-prune-repeat/freeze.json#/predictions/9/source",
          "results/v72-prune-repeat/freeze.json#/predictions/10/source",
          "results/v72-prune-repeat/freeze.json#/predictions/11/source",
          "results/v72-prune-repeat/freeze.json#/predictions/12/source",
          "results/v72-prune-repeat/freeze.json#/predictions/13/source",
          "results/v72-prune-repeat/freeze.json#/predictions/14/source",
          "results/v72-prune-repeat/freeze.json#/predictions/15/source",
          "results/v72-prune-repeat/freeze.json#/predictions/16/source",
          "results/v72-prune-repeat/freeze.json#/predictions/17/source"
        ],
        "op": "unique",
        "format": null
      },
      " (same weights); density ",
      {
        "sources": [
          "results/v72-prune-repeat/freeze.json#/predictions/0/density",
          "results/v72-prune-repeat/freeze.json#/predictions/1/density",
          "results/v72-prune-repeat/freeze.json#/predictions/2/density",
          "results/v72-prune-repeat/freeze.json#/predictions/3/density",
          "results/v72-prune-repeat/freeze.json#/predictions/4/density",
          "results/v72-prune-repeat/freeze.json#/predictions/5/density",
          "results/v72-prune-repeat/freeze.json#/predictions/6/density",
          "results/v72-prune-repeat/freeze.json#/predictions/7/density",
          "results/v72-prune-repeat/freeze.json#/predictions/8/density",
          "results/v72-prune-repeat/freeze.json#/predictions/9/density",
          "results/v72-prune-repeat/freeze.json#/predictions/10/density",
          "results/v72-prune-repeat/freeze.json#/predictions/11/density",
          "results/v72-prune-repeat/freeze.json#/predictions/12/density",
          "results/v72-prune-repeat/freeze.json#/predictions/13/density",
          "results/v72-prune-repeat/freeze.json#/predictions/14/density",
          "results/v72-prune-repeat/freeze.json#/predictions/15/density",
          "results/v72-prune-repeat/freeze.json#/predictions/16/density",
          "results/v72-prune-repeat/freeze.json#/predictions/17/density"
        ],
        "op": "unique",
        "format": null
      },
      "; math/code/qa; distribution: not tested"
    ],
    "context": [],
    "note": "No distribution identifier is stored in these comparison records.",
    "rendered": "State labels: pythia-2.8b@step143000, pythia-2.8b@step16000 (same weights); density 0.65, 0.75, 0.85; math/code/qa; distribution: not tested"
  },
  {
    "row": 0,
    "column": 4,
    "parts": [
      "math: ",
      {
        "sources": [
          "results/v72-prune-repeat/compare.json#/scores/power/by_capability/math/mae"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "\n",
      "code: ",
      {
        "sources": [
          "results/v72-prune-repeat/compare.json#/scores/power/by_capability/code/mae"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "\n",
      "qa: ",
      {
        "sources": [
          "results/v72-prune-repeat/compare.json#/scores/power/by_capability/qa/mae"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "; interval: not tested"
    ],
    "context": [
      "results/v53-prune-dev/register.json#/selected_candidate",
      "results/v53-prune-dev/register.json#/test_densities"
    ],
    "note": "",
    "rendered": "math: 0.2918\\newline code: 0.3934\\newline qa: 0.6788; interval: not tested"
  },
  {
    "row": 0,
    "column": 5,
    "parts": [
      "math: ",
      {
        "sources": [
          "results/v53-prune-dev/register.json#/loso_table/2/candidate"
        ],
        "op": "identity",
        "format": null
      },
      " MAE ",
      {
        "sources": [
          "results/v72-prune-repeat/compare.json#/scores/A2/by_capability/math/mae"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "\n",
      "code: ",
      {
        "sources": [
          "results/v53-prune-dev/register.json#/loso_table/2/candidate"
        ],
        "op": "identity",
        "format": null
      },
      " MAE ",
      {
        "sources": [
          "results/v72-prune-repeat/compare.json#/scores/A2/by_capability/code/mae"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "\n",
      "qa: ",
      {
        "sources": [
          "results/v53-prune-dev/register.json#/loso_table/5/candidate"
        ],
        "op": "identity",
        "format": null
      },
      " MAE ",
      {
        "sources": [
          "results/v72-prune-repeat/compare.json#/scores/median_curve/by_capability/qa/mae"
        ],
        "op": "identity",
        "format": ".4f"
      }
    ],
    "context": [
      "results/v53-prune-dev/register.json#/loso_table"
    ],
    "note": "Minimum development LOSO MAE excluding power, per capability; no test ranking.",
    "rendered": "math: A2 MAE 0.4250\\newline code: A2 MAE 0.4582\\newline qa: median\\_curve MAE 0.0652"
  },
  {
    "row": 0,
    "column": 6,
    "parts": [
      "frozen prediction"
    ],
    "context": [
      "results/v72-prune-repeat/freeze.json#/selected_candidate"
    ],
    "note": "",
    "rendered": "frozen prediction"
  },
  {
    "row": 1,
    "column": 0,
    "parts": [
      "Pruning: new source state"
    ],
    "context": [
      "results/v53-prune-dev/register.json#/selected_candidate",
      "results/v53-prune-dev/register.json#/test_densities"
    ],
    "note": "",
    "rendered": "Pruning: new source state"
  },
  {
    "row": 1,
    "column": 1,
    "parts": [
      {
        "sources": [
          "results/v53-prune-dev/register.json#/candidate_definitions/power"
        ],
        "op": "identity",
        "format": null
      },
      "; parameters ",
      {
        "sources": [
          "results/v53-prune-dev/register.json#/n_params_per_capability/power"
        ],
        "op": "identity",
        "format": null
      }
    ],
    "context": [],
    "note": "",
    "rendered": "(beta.phi) * ((1-d)/0.3)**gamma; parameters 5"
  },
  {
    "row": 1,
    "column": 2,
    "parts": [
      {
        "sources": [
          "results/v53-prune-dev/register.json#/feature_names"
        ],
        "op": "join",
        "format": null
      },
      "; density"
    ],
    "context": [
      "results/v53-prune-dev/register.json#/selected_candidate",
      "results/v53-prune-dev/register.json#/test_densities"
    ],
    "note": "",
    "rendered": "1, z(log N0), z(L0c), z(log D0); density"
  },
  {
    "row": 1,
    "column": 3,
    "parts": [
      {
        "sources": [
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/tag",
          "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/tag",
          "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/tag"
        ],
        "op": "unique",
        "format": null
      },
      "; density ",
      {
        "sources": [
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/densities"
        ],
        "op": "join",
        "format": null
      },
      "; math/code/qa; distribution: not tested"
    ],
    "context": [],
    "note": "No distribution identifier is stored in these comparison records.",
    "rendered": "pythia-1.4b@step112000, pythia-410m@step48000, pythia-6.9b@step80000; density 0.85, 0.675, 0.575; math/code/qa; distribution: not tested"
  },
  {
    "row": 1,
    "column": 4,
    "parts": [
      "math: ",
      {
        "sources": [
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/power/math",
          "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/power/math",
          "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/power/math"
        ],
        "op": "mean",
        "format": ".4f"
      },
      "\n",
      "code: ",
      {
        "sources": [
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/power/code",
          "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/power/code",
          "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/power/code"
        ],
        "op": "mean",
        "format": ".4f"
      },
      "\n",
      "qa: ",
      {
        "sources": [
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/power/qa",
          "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/power/qa",
          "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/power/qa"
        ],
        "op": "mean",
        "format": ".4f"
      },
      "; interval: not tested"
    ],
    "context": [
      "results/v53-prune-dev/register.json#/selected_candidate",
      "results/v53-prune-dev/register.json#/test_densities"
    ],
    "note": "",
    "rendered": "math: 0.2431\\newline code: 0.2361\\newline qa: 0.6784; interval: not tested"
  },
  {
    "row": 1,
    "column": 5,
    "parts": [
      "math: ",
      {
        "sources": [
          "results/v53-prune-dev/register.json#/loso_table/2/candidate"
        ],
        "op": "identity",
        "format": null
      },
      " MAE ",
      {
        "sources": [
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/A2/math",
          "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/A2/math",
          "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/A2/math"
        ],
        "op": "mean",
        "format": ".4f"
      },
      "\n",
      "code: ",
      {
        "sources": [
          "results/v53-prune-dev/register.json#/loso_table/2/candidate"
        ],
        "op": "identity",
        "format": null
      },
      " MAE ",
      {
        "sources": [
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/A2/code",
          "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/A2/code",
          "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/A2/code"
        ],
        "op": "mean",
        "format": ".4f"
      },
      "\n",
      "qa: ",
      {
        "sources": [
          "results/v53-prune-dev/register.json#/loso_table/5/candidate"
        ],
        "op": "identity",
        "format": null
      },
      " MAE ",
      {
        "sources": [
          "results/v53-prune-dev/compare_pythia-410m@step48000.json#/mae/median_curve/qa",
          "results/v53-prune-dev/compare_pythia-1.4b@step112000.json#/mae/median_curve/qa",
          "results/v53-prune-dev/compare_pythia-6.9b@step80000.json#/mae/median_curve/qa"
        ],
        "op": "mean",
        "format": ".4f"
      }
    ],
    "context": [
      "results/v53-prune-dev/register.json#/loso_table"
    ],
    "note": "Minimum development LOSO MAE excluding power, per capability; no test ranking.",
    "rendered": "math: A2 MAE 0.2298\\newline code: A2 MAE 0.2217\\newline qa: median\\_curve MAE 0.2206"
  },
  {
    "row": 1,
    "column": 6,
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
      "Quantization: unseen bit-width"
    ],
    "context": [
      "results/v55-quant-group/register.json#/test_sets/bit_test"
    ],
    "note": "",
    "rendered": "Quantization: unseen bit-width"
  },
  {
    "row": 2,
    "column": 1,
    "parts": [
      {
        "sources": [
          "results/v55-quant-group/register.json#/candidate_definitions/low_order_2d"
        ],
        "op": "identity",
        "format": null
      },
      "; parameters ",
      {
        "sources": [
          "results/v55-quant-group/register.json#/n_params_per_capability/low_order_2d"
        ],
        "op": "identity",
        "format": null
      }
    ],
    "context": [],
    "note": "",
    "rendered": "phi.[a0 + a1*u + a2*v + a3*u*v + a4*u\\textasciicircum{}2]; coefficients ordered by term then phi; parameters 20"
  },
  {
    "row": 2,
    "column": 2,
    "parts": [
      {
        "sources": [
          "results/v55-quant-group/register.json#/feature_names"
        ],
        "op": "join",
        "format": null
      },
      "; bits, group size"
    ],
    "context": [
      "results/v55-quant-group/register.json#/test_sets/bit_test/configs"
    ],
    "note": "",
    "rendered": "1, z(log N0), z(L0c), z(log D0); bits, group size"
  },
  {
    "row": 2,
    "column": 3,
    "parts": [
      {
        "sources": [
          "results/v55-quant-group/register.json#/test_sets/bit_test/states"
        ],
        "op": "join",
        "format": null
      },
      "; ",
      {
        "sources": [
          "results/v55-quant-group/register.json#/test_sets/bit_test/configs"
        ],
        "op": "join",
        "format": null
      },
      "; math/code/qa; distribution: not tested"
    ],
    "context": [],
    "note": "",
    "rendered": "pythia-160m@step16000, pythia-160m@step143000, pythia-410m@step16000, pythia-410m@step143000, pythia-1.4b@step16000, pythia-1.4b@step143000; b4\\_g64, b4\\_g256; math/code/qa; distribution: not tested"
  },
  {
    "row": 2,
    "column": 4,
    "parts": [
      "math: ",
      {
        "sources": [
          "results/v55-quant-group/compare.json#/test_sets/bit_test/mae_table/1/mae/math"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "\n",
      "code: ",
      {
        "sources": [
          "results/v55-quant-group/compare.json#/test_sets/bit_test/mae_table/1/mae/code"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "\n",
      "qa: ",
      {
        "sources": [
          "results/v55-quant-group/compare.json#/test_sets/bit_test/mae_table/1/mae/qa"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "; interval: not tested"
    ],
    "context": [],
    "note": "",
    "rendered": "math: 0.1934\\newline code: 0.2136\\newline qa: 0.4364; interval: not tested"
  },
  {
    "row": 2,
    "column": 5,
    "parts": [
      "math: ",
      {
        "sources": [
          "results/v55-quant-group/register.json#/loso_table/4/candidate"
        ],
        "op": "identity",
        "format": null
      },
      " MAE ",
      {
        "sources": [
          "results/v55-quant-group/compare.json#/test_sets/bit_test/mae_table/4/mae/math"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "\n",
      "code: ",
      {
        "sources": [
          "results/v55-quant-group/register.json#/loso_table/4/candidate"
        ],
        "op": "identity",
        "format": null
      },
      " MAE ",
      {
        "sources": [
          "results/v55-quant-group/compare.json#/test_sets/bit_test/mae_table/4/mae/code"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "\n",
      "qa: ",
      {
        "sources": [
          "results/v55-quant-group/register.json#/loso_table/4/candidate"
        ],
        "op": "identity",
        "format": null
      },
      " MAE ",
      {
        "sources": [
          "results/v55-quant-group/compare.json#/test_sets/bit_test/mae_table/4/mae/qa"
        ],
        "op": "identity",
        "format": ".4f"
      }
    ],
    "context": [
      "results/v55-quant-group/register.json#/loso_table"
    ],
    "note": "Development minimum over registered baselines mean/median/zero.",
    "rendered": "math: median MAE 0.5533\\newline code: median MAE 0.7258\\newline qa: median MAE 0.5371"
  },
  {
    "row": 2,
    "column": 6,
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
      "Quantization: unseen group size"
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
    "rendered": "Quantization: unseen group size"
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
        "op": "identity",
        "format": null
      },
      "; parameters ",
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/selected/math/n_coefficients"
        ],
        "op": "identity",
        "format": null
      },
      "\n",
      "code: ",
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/selected/code/candidate"
        ],
        "op": "identity",
        "format": null
      },
      "; parameters ",
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/selected/code/n_coefficients"
        ],
        "op": "identity",
        "format": null
      },
      "\n",
      "qa: ",
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/selected/qa/candidate"
        ],
        "op": "identity",
        "format": null
      },
      "; parameters ",
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/selected/qa/n_coefficients"
        ],
        "op": "identity",
        "format": null
      }
    ],
    "context": [
      "results/v55-quant-group/register.json#/candidate_definitions/low_order_2d",
      "results/v69-quant-confirm/develop.json#/models"
    ],
    "note": "Surface is phi.[a0+a1*u+a2*v+a3*u*v+a4*u^2]; median is per configuration; zero is identically zero.",
    "rendered": "math: low\\_order\\_2d; parameters 20\\newline code: median; parameters 9\\newline qa: zero; parameters 0"
  },
  {
    "row": 3,
    "column": 2,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/feature_names"
        ],
        "op": "join",
        "format": null
      },
      "; bits, group size"
    ],
    "context": [
      "results/v69-quant-confirm/develop.json#/dev_configs"
    ],
    "note": "",
    "rendered": "1, z(log N0), z(L0c), z(log D0); bits, group size"
  },
  {
    "row": 3,
    "column": 3,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/rows/0/state",
          "results/v69-quant-confirm/compare.json#/rows/1/state",
          "results/v69-quant-confirm/compare.json#/rows/2/state",
          "results/v69-quant-confirm/compare.json#/rows/3/state",
          "results/v69-quant-confirm/compare.json#/rows/4/state",
          "results/v69-quant-confirm/compare.json#/rows/5/state",
          "results/v69-quant-confirm/compare.json#/rows/6/state",
          "results/v69-quant-confirm/compare.json#/rows/7/state",
          "results/v69-quant-confirm/compare.json#/rows/8/state",
          "results/v69-quant-confirm/compare.json#/rows/9/state",
          "results/v69-quant-confirm/compare.json#/rows/10/state",
          "results/v69-quant-confirm/compare.json#/rows/11/state",
          "results/v69-quant-confirm/compare.json#/rows/12/state",
          "results/v69-quant-confirm/compare.json#/rows/13/state",
          "results/v69-quant-confirm/compare.json#/rows/14/state",
          "results/v69-quant-confirm/compare.json#/rows/15/state",
          "results/v69-quant-confirm/compare.json#/rows/16/state",
          "results/v69-quant-confirm/compare.json#/rows/17/state",
          "results/v69-quant-confirm/compare.json#/rows/18/state",
          "results/v69-quant-confirm/compare.json#/rows/19/state",
          "results/v69-quant-confirm/compare.json#/rows/20/state",
          "results/v69-quant-confirm/compare.json#/rows/21/state",
          "results/v69-quant-confirm/compare.json#/rows/22/state",
          "results/v69-quant-confirm/compare.json#/rows/23/state",
          "results/v69-quant-confirm/compare.json#/rows/24/state",
          "results/v69-quant-confirm/compare.json#/rows/25/state",
          "results/v69-quant-confirm/compare.json#/rows/26/state",
          "results/v69-quant-confirm/compare.json#/rows/27/state",
          "results/v69-quant-confirm/compare.json#/rows/28/state",
          "results/v69-quant-confirm/compare.json#/rows/29/state",
          "results/v69-quant-confirm/compare.json#/rows/30/state",
          "results/v69-quant-confirm/compare.json#/rows/31/state",
          "results/v69-quant-confirm/compare.json#/rows/32/state",
          "results/v69-quant-confirm/compare.json#/rows/33/state",
          "results/v69-quant-confirm/compare.json#/rows/34/state",
          "results/v69-quant-confirm/compare.json#/rows/35/state"
        ],
        "op": "unique",
        "format": null
      },
      "; ",
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/rows/0/config",
          "results/v69-quant-confirm/compare.json#/rows/1/config",
          "results/v69-quant-confirm/compare.json#/rows/2/config",
          "results/v69-quant-confirm/compare.json#/rows/3/config",
          "results/v69-quant-confirm/compare.json#/rows/4/config",
          "results/v69-quant-confirm/compare.json#/rows/5/config",
          "results/v69-quant-confirm/compare.json#/rows/6/config",
          "results/v69-quant-confirm/compare.json#/rows/7/config",
          "results/v69-quant-confirm/compare.json#/rows/8/config",
          "results/v69-quant-confirm/compare.json#/rows/9/config",
          "results/v69-quant-confirm/compare.json#/rows/10/config",
          "results/v69-quant-confirm/compare.json#/rows/11/config",
          "results/v69-quant-confirm/compare.json#/rows/12/config",
          "results/v69-quant-confirm/compare.json#/rows/13/config",
          "results/v69-quant-confirm/compare.json#/rows/14/config",
          "results/v69-quant-confirm/compare.json#/rows/15/config",
          "results/v69-quant-confirm/compare.json#/rows/16/config",
          "results/v69-quant-confirm/compare.json#/rows/17/config",
          "results/v69-quant-confirm/compare.json#/rows/18/config",
          "results/v69-quant-confirm/compare.json#/rows/19/config",
          "results/v69-quant-confirm/compare.json#/rows/20/config",
          "results/v69-quant-confirm/compare.json#/rows/21/config",
          "results/v69-quant-confirm/compare.json#/rows/22/config",
          "results/v69-quant-confirm/compare.json#/rows/23/config",
          "results/v69-quant-confirm/compare.json#/rows/24/config",
          "results/v69-quant-confirm/compare.json#/rows/25/config",
          "results/v69-quant-confirm/compare.json#/rows/26/config",
          "results/v69-quant-confirm/compare.json#/rows/27/config",
          "results/v69-quant-confirm/compare.json#/rows/28/config",
          "results/v69-quant-confirm/compare.json#/rows/29/config",
          "results/v69-quant-confirm/compare.json#/rows/30/config",
          "results/v69-quant-confirm/compare.json#/rows/31/config",
          "results/v69-quant-confirm/compare.json#/rows/32/config",
          "results/v69-quant-confirm/compare.json#/rows/33/config",
          "results/v69-quant-confirm/compare.json#/rows/34/config",
          "results/v69-quant-confirm/compare.json#/rows/35/config"
        ],
        "op": "unique",
        "format": null
      },
      "; math/code/qa; distribution: not tested"
    ],
    "context": [],
    "note": "",
    "rendered": "pythia-1.4b@step16000, pythia-410m@step143000; b3\\_g32, b3\\_g512, b4\\_g32, b4\\_g512, b5\\_g32, b5\\_g512; math/code/qa; distribution: not tested"
  },
  {
    "row": 3,
    "column": 4,
    "parts": [
      "math: ",
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
        "format": ".4f"
      },
      "\n",
      "code: ",
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
        "format": ".4f"
      },
      "\n",
      "qa: ",
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
        "format": ".4f"
      },
      "; interval: not tested"
    ],
    "context": [],
    "note": "",
    "rendered": "math: 0.2149\\newline code: 0.5567\\newline qa: 0.4570; interval: not tested"
  },
  {
    "row": 3,
    "column": 5,
    "parts": [
      "math: ",
      "bilinear",
      " MAE ",
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
        "format": ".4f"
      },
      "\n",
      "code: ",
      "zero",
      " MAE ",
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
        "format": ".4f"
      },
      "\n",
      "qa: ",
      "median",
      " MAE ",
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
        "format": ".4f"
      }
    ],
    "context": [
      "results/v69-quant-confirm/develop.json#/loso/scores"
    ],
    "note": "Minimum development LOSO macro MAE excluding the selected candidate, per capability.",
    "rendered": "math: bilinear MAE 0.3330\\newline code: zero MAE 0.6782\\newline qa: median MAE 0.4579"
  },
  {
    "row": 3,
    "column": 6,
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
      "Quantization: new state"
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
    "rendered": "Quantization: new state"
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
        "op": "identity",
        "format": null
      },
      "; parameters ",
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/selected/math/n_coefficients"
        ],
        "op": "identity",
        "format": null
      },
      "\n",
      "code: ",
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/selected/code/candidate"
        ],
        "op": "identity",
        "format": null
      },
      "; parameters ",
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/selected/code/n_coefficients"
        ],
        "op": "identity",
        "format": null
      },
      "\n",
      "qa: ",
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/selected/qa/candidate"
        ],
        "op": "identity",
        "format": null
      },
      "; parameters ",
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/selected/qa/n_coefficients"
        ],
        "op": "identity",
        "format": null
      }
    ],
    "context": [
      "results/v55-quant-group/register.json#/candidate_definitions/low_order_2d",
      "results/v69-quant-confirm/develop.json#/models"
    ],
    "note": "Surface is phi.[a0+a1*u+a2*v+a3*u*v+a4*u^2]; median is per configuration; zero is identically zero.",
    "rendered": "math: low\\_order\\_2d; parameters 20\\newline code: median; parameters 9\\newline qa: zero; parameters 0"
  },
  {
    "row": 4,
    "column": 2,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/develop.json#/feature_names"
        ],
        "op": "join",
        "format": null
      },
      "; bits, group size"
    ],
    "context": [
      "results/v69-quant-confirm/develop.json#/dev_configs"
    ],
    "note": "",
    "rendered": "1, z(log N0), z(L0c), z(log D0); bits, group size"
  },
  {
    "row": 4,
    "column": 3,
    "parts": [
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/rows/36/state",
          "results/v69-quant-confirm/compare.json#/rows/37/state",
          "results/v69-quant-confirm/compare.json#/rows/38/state",
          "results/v69-quant-confirm/compare.json#/rows/39/state",
          "results/v69-quant-confirm/compare.json#/rows/40/state",
          "results/v69-quant-confirm/compare.json#/rows/41/state",
          "results/v69-quant-confirm/compare.json#/rows/42/state",
          "results/v69-quant-confirm/compare.json#/rows/43/state",
          "results/v69-quant-confirm/compare.json#/rows/44/state",
          "results/v69-quant-confirm/compare.json#/rows/45/state",
          "results/v69-quant-confirm/compare.json#/rows/46/state",
          "results/v69-quant-confirm/compare.json#/rows/47/state",
          "results/v69-quant-confirm/compare.json#/rows/48/state",
          "results/v69-quant-confirm/compare.json#/rows/49/state",
          "results/v69-quant-confirm/compare.json#/rows/50/state",
          "results/v69-quant-confirm/compare.json#/rows/51/state",
          "results/v69-quant-confirm/compare.json#/rows/52/state",
          "results/v69-quant-confirm/compare.json#/rows/53/state",
          "results/v69-quant-confirm/compare.json#/rows/54/state",
          "results/v69-quant-confirm/compare.json#/rows/55/state",
          "results/v69-quant-confirm/compare.json#/rows/56/state",
          "results/v69-quant-confirm/compare.json#/rows/57/state",
          "results/v69-quant-confirm/compare.json#/rows/58/state",
          "results/v69-quant-confirm/compare.json#/rows/59/state",
          "results/v69-quant-confirm/compare.json#/rows/60/state",
          "results/v69-quant-confirm/compare.json#/rows/61/state",
          "results/v69-quant-confirm/compare.json#/rows/62/state"
        ],
        "op": "unique",
        "format": null
      },
      "; ",
      {
        "sources": [
          "results/v69-quant-confirm/compare.json#/rows/36/config",
          "results/v69-quant-confirm/compare.json#/rows/37/config",
          "results/v69-quant-confirm/compare.json#/rows/38/config",
          "results/v69-quant-confirm/compare.json#/rows/39/config",
          "results/v69-quant-confirm/compare.json#/rows/40/config",
          "results/v69-quant-confirm/compare.json#/rows/41/config",
          "results/v69-quant-confirm/compare.json#/rows/42/config",
          "results/v69-quant-confirm/compare.json#/rows/43/config",
          "results/v69-quant-confirm/compare.json#/rows/44/config",
          "results/v69-quant-confirm/compare.json#/rows/45/config",
          "results/v69-quant-confirm/compare.json#/rows/46/config",
          "results/v69-quant-confirm/compare.json#/rows/47/config",
          "results/v69-quant-confirm/compare.json#/rows/48/config",
          "results/v69-quant-confirm/compare.json#/rows/49/config",
          "results/v69-quant-confirm/compare.json#/rows/50/config",
          "results/v69-quant-confirm/compare.json#/rows/51/config",
          "results/v69-quant-confirm/compare.json#/rows/52/config",
          "results/v69-quant-confirm/compare.json#/rows/53/config",
          "results/v69-quant-confirm/compare.json#/rows/54/config",
          "results/v69-quant-confirm/compare.json#/rows/55/config",
          "results/v69-quant-confirm/compare.json#/rows/56/config",
          "results/v69-quant-confirm/compare.json#/rows/57/config",
          "results/v69-quant-confirm/compare.json#/rows/58/config",
          "results/v69-quant-confirm/compare.json#/rows/59/config",
          "results/v69-quant-confirm/compare.json#/rows/60/config",
          "results/v69-quant-confirm/compare.json#/rows/61/config",
          "results/v69-quant-confirm/compare.json#/rows/62/config"
        ],
        "op": "unique",
        "format": null
      },
      "; math/code/qa; distribution: not tested"
    ],
    "context": [],
    "note": "",
    "rendered": "pythia-1.4b@step112000; b3\\_g128, b3\\_g32, b3\\_g512, b4\\_g128, b4\\_g32, b4\\_g512, b5\\_g128, b5\\_g32, b5\\_g512; math/code/qa; distribution: not tested"
  },
  {
    "row": 4,
    "column": 4,
    "parts": [
      "math: ",
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
        "format": ".4f"
      },
      "\n",
      "code: ",
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
        "format": ".4f"
      },
      "\n",
      "qa: ",
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
        "format": ".4f"
      },
      "; interval: not tested"
    ],
    "context": [],
    "note": "",
    "rendered": "math: 0.3033\\newline code: 0.1532\\newline qa: 0.2217; interval: not tested"
  },
  {
    "row": 4,
    "column": 5,
    "parts": [
      "math: ",
      "bilinear",
      " MAE ",
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
        "format": ".4f"
      },
      "\n",
      "code: ",
      "zero",
      " MAE ",
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
        "format": ".4f"
      },
      "\n",
      "qa: ",
      "median",
      " MAE ",
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
        "format": ".4f"
      }
    ],
    "context": [
      "results/v69-quant-confirm/develop.json#/loso/scores"
    ],
    "note": "Minimum development LOSO macro MAE excluding the selected candidate, per capability.",
    "rendered": "math: bilinear MAE 0.3503\\newline code: zero MAE 0.5627\\newline qa: median MAE 0.1412"
  },
  {
    "row": 4,
    "column": 6,
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
      "Distillation: budget response"
    ],
    "context": [
      "results/a2-curvature-interaction/summary.json#/decision_table/18/target",
      "results/a2-curvature-interaction/summary.json#/decision_table/6/target",
      "results/a2-curvature-interaction/summary.json#/decision_table/54/target"
    ],
    "note": "",
    "rendered": "Distillation: budget response"
  },
  {
    "row": 5,
    "column": 1,
    "parts": [
      "Fold-selected ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/protocol/structures"
        ],
        "op": "keys",
        "format": null
      },
      "; nominal parameters ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/parameter_intervals/0/fits/F_log/fit/nominal_parameters"
        ],
        "op": "identity",
        "format": null
      },
      "/",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/parameter_intervals/0/fits/F_curv/fit/nominal_parameters"
        ],
        "op": "identity",
        "format": null
      },
      "/",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/parameter_intervals/0/fits/F_int/fit/nominal_parameters"
        ],
        "op": "identity",
        "format": null
      }
    ],
    "context": [
      "results/a2-curvature-interaction/summary.json#/protocol/structures"
    ],
    "note": "Forms and parameter counts are per structure, not summed over folds.",
    "rendered": "Fold-selected F\\_log, F\\_curv, F\\_int; nominal parameters 4/5/5"
  },
  {
    "row": 5,
    "column": 2,
    "parts": [
      "Supervised budget, reuse, size or own initial loss"
    ],
    "context": [
      "results/a2-curvature-interaction/summary.json#/protocol/descriptors",
      "results/a2-curvature-interaction/summary.json#/protocol/descriptor_calibration_cost"
    ],
    "note": "",
    "rendered": "Supervised budget, reuse, size or own initial loss"
  },
  {
    "row": 5,
    "column": 3,
    "parts": [
      "Students ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/parameter_intervals/0/fits/F_log/fit/standardizer/students"
        ],
        "op": "join",
        "format": null
      },
      "; ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/protocol/largest_budget"
        ],
        "op": "identity",
        "format": null
      },
      "\nDistributions: ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/6/distribution",
          "results/a2-curvature-interaction/summary.json#/decision_table/18/distribution",
          "results/a2-curvature-interaction/summary.json#/decision_table/54/distribution"
        ],
        "op": "unique",
        "format": null
      }
    ],
    "context": [],
    "note": "",
    "rendered": "Students gemma3-1b, gemma3-270m, gemma3-4b; All T>=150000 withheld; fit only T<150000. QA scope has only final positive checkpoints and is unscorable here.\\newline Distributions: training\\_probe:2WikiMultihopQA:35e3fde33c8b6e91, training\\_probe:MATH-500:c76472bee07727fe, training\\_probe:MBPP:d5f45bdd0f442e0e"
  },
  {
    "row": 5,
    "column": 4,
    "parts": [
      "math: ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/18/primary_mae"
        ],
        "op": "identity",
        "format": ".4f"
      },
      " [",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/18/primary_mae_interval/0"
        ],
        "op": "identity",
        "format": ".4f"
      },
      ", ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/18/primary_mae_interval/1"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "]",
      "\n",
      "code: ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/6/primary_mae"
        ],
        "op": "identity",
        "format": ".4f"
      },
      " [",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/6/primary_mae_interval/0"
        ],
        "op": "identity",
        "format": ".4f"
      },
      ", ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/6/primary_mae_interval/1"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "]",
      "\n",
      "qa: ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/54/primary_mae"
        ],
        "op": "identity",
        "format": ".4f"
      },
      " [",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/54/primary_mae_interval/0"
        ],
        "op": "identity",
        "format": ".4f"
      },
      ", ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/54/primary_mae_interval/1"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "]"
    ],
    "context": [],
    "note": "Training-probe MAEs; reuse is the recorded tolerance proxy, not an exact intervention. Intervals conditional on frozen fold predictions.",
    "rendered": "math: 0.0718 [0.0523, 0.1055]\\newline code: 0.0679 [0.0509, 0.0882]\\newline qa: 2.1809 [1.6828, 2.8768]"
  },
  {
    "row": 5,
    "column": 5,
    "parts": [
      "math: ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/18/inner_selected_baselines"
        ],
        "op": "keys",
        "format": null
      },
      " MAE ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/18/baseline_mae"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "\n",
      "code: ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/6/inner_selected_baselines"
        ],
        "op": "keys",
        "format": null
      },
      " MAE ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/6/baseline_mae"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "\n",
      "qa: ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/54/inner_selected_baselines"
        ],
        "op": "keys",
        "format": null
      },
      " MAE ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/54/baseline_mae"
        ],
        "op": "identity",
        "format": ".4f"
      }
    ],
    "context": [],
    "note": "Inner-development-selected baselines. Never strongest_observed_baseline or strongest_baseline_mae.",
    "rendered": "math: constant MAE 0.0947\\newline code: constant MAE 0.1061\\newline qa: constant MAE 1.4432"
  },
  {
    "row": 5,
    "column": 6,
    "parts": [
      "development"
    ],
    "context": [
      "results/a2-curvature-interaction/summary.json#/protocol/secondary",
      "results/a2-curvature-interaction/summary.json#/protocol/previous_F_int"
    ],
    "note": "",
    "rendered": "development"
  },
  {
    "row": 6,
    "column": 0,
    "parts": [
      "Distillation: data-reuse response"
    ],
    "context": [
      "results/a2-curvature-interaction/summary.json#/decision_table/14/target",
      "results/a2-curvature-interaction/summary.json#/decision_table/2/target",
      "results/a2-curvature-interaction/summary.json#/decision_table/50/target"
    ],
    "note": "",
    "rendered": "Distillation: data-reuse response"
  },
  {
    "row": 6,
    "column": 1,
    "parts": [
      "Fold-selected ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/protocol/structures"
        ],
        "op": "keys",
        "format": null
      },
      "; nominal parameters ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/parameter_intervals/0/fits/F_log/fit/nominal_parameters"
        ],
        "op": "identity",
        "format": null
      },
      "/",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/parameter_intervals/0/fits/F_curv/fit/nominal_parameters"
        ],
        "op": "identity",
        "format": null
      },
      "/",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/parameter_intervals/0/fits/F_int/fit/nominal_parameters"
        ],
        "op": "identity",
        "format": null
      }
    ],
    "context": [
      "results/a2-curvature-interaction/summary.json#/protocol/structures"
    ],
    "note": "Forms and parameter counts are per structure, not summed over folds.",
    "rendered": "Fold-selected F\\_log, F\\_curv, F\\_int; nominal parameters 4/5/5"
  },
  {
    "row": 6,
    "column": 2,
    "parts": [
      "Supervised budget, reuse, size or own initial loss"
    ],
    "context": [
      "results/a2-curvature-interaction/summary.json#/protocol/descriptors",
      "results/a2-curvature-interaction/summary.json#/protocol/descriptor_calibration_cost"
    ],
    "note": "",
    "rendered": "Supervised budget, reuse, size or own initial loss"
  },
  {
    "row": 6,
    "column": 3,
    "parts": [
      "Students ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/parameter_intervals/0/fits/F_curv/fit/standardizer/students"
        ],
        "op": "join",
        "format": null
      },
      "; ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/protocol/I_U"
        ],
        "op": "identity",
        "format": null
      },
      "\nDistributions: ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/2/distribution",
          "results/a2-curvature-interaction/summary.json#/decision_table/14/distribution",
          "results/a2-curvature-interaction/summary.json#/decision_table/26/distribution",
          "results/a2-curvature-interaction/summary.json#/decision_table/38/distribution",
          "results/a2-curvature-interaction/summary.json#/decision_table/50/distribution",
          "results/a2-curvature-interaction/summary.json#/decision_table/62/distribution"
        ],
        "op": "unique",
        "format": null
      }
    ],
    "context": [],
    "note": "",
    "rendered": "Students gemma3-1b, gemma3-270m, gemma3-4b; Exact I\\_U has no observed positive matched-T pairs. Decision MAEs labelled 1\\% tolerance proxy use actual endpoints; fixed-T model predictions are stored but not scored against mismatched outcomes. 0.5\\%/5\\% separate sensitivity, never pooled.\\newline Distributions: 2wiki\\_new:bbd036c56ac37bd3, musique:0c676ed3b3c2a52d, training\\_probe:2WikiMultihopQA:35e3fde33c8b6e91, training\\_probe:MATH-500:c76472bee07727fe, training\\_probe:MBPP:d5f45bdd0f442e0e, triviaqa:25268a1f786058ff"
  },
  {
    "row": 6,
    "column": 4,
    "parts": [
      "math: ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/14/primary_mae"
        ],
        "op": "identity",
        "format": ".4f"
      },
      " [",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/14/primary_mae_interval/0"
        ],
        "op": "identity",
        "format": ".4f"
      },
      ", ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/14/primary_mae_interval/1"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "]",
      "\n",
      "code: ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/2/primary_mae"
        ],
        "op": "identity",
        "format": ".4f"
      },
      " [",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/2/primary_mae_interval/0"
        ],
        "op": "identity",
        "format": ".4f"
      },
      ", ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/2/primary_mae_interval/1"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "]",
      "\n",
      "qa: ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/50/primary_mae"
        ],
        "op": "identity",
        "format": ".4f"
      },
      " [",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/50/primary_mae_interval/0"
        ],
        "op": "identity",
        "format": ".4f"
      },
      ", ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/50/primary_mae_interval/1"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "]",
      "; exact fixed-budget response: not tested"
    ],
    "context": [],
    "note": "Training-probe MAEs; reuse is the recorded tolerance proxy, not an exact intervention. Intervals conditional on frozen fold predictions.",
    "rendered": "math: 0.0796 [0.0451, 0.1391]\\newline code: 0.0697 [0.0427, 0.1188]\\newline qa: 1.0184 [0.7196, 1.3431]; exact fixed-budget response: not tested"
  },
  {
    "row": 6,
    "column": 5,
    "parts": [
      "math: ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/14/inner_selected_baselines"
        ],
        "op": "keys",
        "format": null
      },
      " MAE ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/14/baseline_mae"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "\n",
      "code: ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/2/inner_selected_baselines"
        ],
        "op": "keys",
        "format": null
      },
      " MAE ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/2/baseline_mae"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "\n",
      "qa: ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/50/inner_selected_baselines"
        ],
        "op": "keys",
        "format": null
      },
      " MAE ",
      {
        "sources": [
          "results/a2-curvature-interaction/summary.json#/decision_table/50/baseline_mae"
        ],
        "op": "identity",
        "format": ".4f"
      }
    ],
    "context": [],
    "note": "Inner-development-selected baselines. Never strongest_observed_baseline or strongest_baseline_mae.",
    "rendered": "math: surface, reuse\\_only MAE 0.0771\\newline code: zero, surface, reuse\\_only MAE 0.0738\\newline qa: surface MAE 0.7639"
  },
  {
    "row": 6,
    "column": 6,
    "parts": [
      "development"
    ],
    "context": [
      "results/a2-curvature-interaction/summary.json#/protocol/secondary",
      "results/a2-curvature-interaction/summary.json#/protocol/previous_F_int"
    ],
    "note": "",
    "rendered": "development"
  },
  {
    "row": 7,
    "column": 0,
    "parts": [
      "Distillation: new pool"
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/confirmation_register/unused_U_assertion"
    ],
    "note": "",
    "rendered": "Distillation: new pool"
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
        "op": "identity",
        "format": null
      },
      "; parameters ",
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/selected/math/n_params"
        ],
        "op": "identity",
        "format": null
      },
      "\n",
      "code: ",
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/selected/code/method"
        ],
        "op": "identity",
        "format": null
      },
      "; parameters ",
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/selected/code/n_params"
        ],
        "op": "identity",
        "format": null
      },
      "\n",
      "qa: ",
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/selected/qa/method"
        ],
        "op": "identity",
        "format": null
      },
      "; parameters ",
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/selected/qa/n_params"
        ],
        "op": "identity",
        "format": null
      }
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/models",
      "results/v70-distill-confirm/freeze.json#/reference_rule"
    ],
    "note": "E is zero-anchored log reuse; joint combines budget and reuse with stored T_star. Counts include T_star.",
    "rendered": "math: E; parameters 1\\newline code: E; parameters 1\\newline qa: joint; parameters 3"
  },
  {
    "row": 7,
    "column": 2,
    "parts": [
      "Planned supervised budget, pool completion tokens; fixed protocol"
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/prediction_rule",
      "results/v70-distill-confirm/freeze.json#/reference_rule"
    ],
    "note": "",
    "rendered": "Planned supervised budget, pool completion tokens; fixed protocol"
  },
  {
    "row": 7,
    "column": 3,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/confirmation_register/students"
        ],
        "op": "join",
        "format": null
      },
      "; pools ",
      {
        "sources": [
          "results/v70-distill-confirm/freeze.json#/confirmation_register/pools"
        ],
        "op": "keys",
        "format": null
      },
      "; planned tokens ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/0/clusters/0/T_planned"
        ],
        "op": "join",
        "format": null
      },
      "; math/code/qa; distribution: not tested"
    ],
    "context": [],
    "note": "",
    "rendered": "gemma3-270m, gemma3-1b; pools U200\\_s31, U200\\_s32, U200\\_s33, U200\\_s34, U200\\_s35, U200\\_s36; planned tokens 50000, 100000, 200000; math/code/qa; distribution: not tested"
  },
  {
    "row": 7,
    "column": 4,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/0/student"
        ],
        "op": "identity",
        "format": null
      },
      "/",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/0/capability"
        ],
        "op": "identity",
        "format": null
      },
      ": ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/0/candidate_mae"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "\n",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/1/student"
        ],
        "op": "identity",
        "format": null
      },
      "/",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/1/capability"
        ],
        "op": "identity",
        "format": null
      },
      ": ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/1/candidate_mae"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "\n",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/2/student"
        ],
        "op": "identity",
        "format": null
      },
      "/",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/2/capability"
        ],
        "op": "identity",
        "format": null
      },
      ": ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/2/candidate_mae"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "\n",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/3/student"
        ],
        "op": "identity",
        "format": null
      },
      "/",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/3/capability"
        ],
        "op": "identity",
        "format": null
      },
      ": ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/3/candidate_mae"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "\n",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/4/student"
        ],
        "op": "identity",
        "format": null
      },
      "/",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/4/capability"
        ],
        "op": "identity",
        "format": null
      },
      ": ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/4/candidate_mae"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "\n",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/5/student"
        ],
        "op": "identity",
        "format": null
      },
      "/",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/5/capability"
        ],
        "op": "identity",
        "format": null
      },
      ": ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/5/candidate_mae"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "; MAE interval: not tested"
    ],
    "context": [],
    "note": "",
    "rendered": "gemma3-270m/math: 0.0743\\newline gemma3-270m/code: 0.0193\\newline gemma3-270m/qa: 0.5150\\newline gemma3-1b/math: 0.0569\\newline gemma3-1b/code: 0.0485\\newline gemma3-1b/qa: 0.4634; MAE interval: not tested"
  },
  {
    "row": 7,
    "column": 5,
    "parts": [
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/0/student"
        ],
        "op": "identity",
        "format": null
      },
      "/",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/0/capability"
        ],
        "op": "identity",
        "format": null
      },
      ": ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/0/strongest_baseline"
        ],
        "op": "identity",
        "format": null
      },
      " MAE ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/0/baseline_mae"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "; gain ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/0/paired_difference/estimate"
        ],
        "op": "identity",
        "format": ".4f"
      },
      " [",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/0/paired_difference/ci95/0"
        ],
        "op": "identity",
        "format": ".4f"
      },
      ", ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/0/paired_difference/ci95/1"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "]",
      "\n",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/1/student"
        ],
        "op": "identity",
        "format": null
      },
      "/",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/1/capability"
        ],
        "op": "identity",
        "format": null
      },
      ": ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/1/strongest_baseline"
        ],
        "op": "identity",
        "format": null
      },
      " MAE ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/1/baseline_mae"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "; gain ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/1/paired_difference/estimate"
        ],
        "op": "identity",
        "format": ".4f"
      },
      " [",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/1/paired_difference/ci95/0"
        ],
        "op": "identity",
        "format": ".4f"
      },
      ", ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/1/paired_difference/ci95/1"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "]",
      "\n",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/2/student"
        ],
        "op": "identity",
        "format": null
      },
      "/",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/2/capability"
        ],
        "op": "identity",
        "format": null
      },
      ": ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/2/strongest_baseline"
        ],
        "op": "identity",
        "format": null
      },
      " MAE ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/2/baseline_mae"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "; gain ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/2/paired_difference/estimate"
        ],
        "op": "identity",
        "format": ".4f"
      },
      " [",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/2/paired_difference/ci95/0"
        ],
        "op": "identity",
        "format": ".4f"
      },
      ", ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/2/paired_difference/ci95/1"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "]",
      "\n",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/3/student"
        ],
        "op": "identity",
        "format": null
      },
      "/",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/3/capability"
        ],
        "op": "identity",
        "format": null
      },
      ": ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/3/strongest_baseline"
        ],
        "op": "identity",
        "format": null
      },
      " MAE ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/3/baseline_mae"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "; gain ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/3/paired_difference/estimate"
        ],
        "op": "identity",
        "format": ".4f"
      },
      " [",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/3/paired_difference/ci95/0"
        ],
        "op": "identity",
        "format": ".4f"
      },
      ", ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/3/paired_difference/ci95/1"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "]",
      "\n",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/4/student"
        ],
        "op": "identity",
        "format": null
      },
      "/",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/4/capability"
        ],
        "op": "identity",
        "format": null
      },
      ": ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/4/strongest_baseline"
        ],
        "op": "identity",
        "format": null
      },
      " MAE ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/4/baseline_mae"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "; gain ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/4/paired_difference/estimate"
        ],
        "op": "identity",
        "format": ".4f"
      },
      " [",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/4/paired_difference/ci95/0"
        ],
        "op": "identity",
        "format": ".4f"
      },
      ", ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/4/paired_difference/ci95/1"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "]",
      "\n",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/5/student"
        ],
        "op": "identity",
        "format": null
      },
      "/",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/5/capability"
        ],
        "op": "identity",
        "format": null
      },
      ": ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/5/strongest_baseline"
        ],
        "op": "identity",
        "format": null
      },
      " MAE ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/5/baseline_mae"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "; gain ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/5/paired_difference/estimate"
        ],
        "op": "identity",
        "format": ".4f"
      },
      " [",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/5/paired_difference/ci95/0"
        ],
        "op": "identity",
        "format": ".4f"
      },
      ", ",
      {
        "sources": [
          "results/v70-distill-confirm/compare.json#/groups/5/paired_difference/ci95/1"
        ],
        "op": "identity",
        "format": ".4f"
      },
      "]"
    ],
    "context": [
      "results/v70-distill-confirm/freeze.json#/baseline_rule",
      "results/v70-distill-confirm/freeze.json#/strongest_baseline"
    ],
    "note": "Gain = baseline MAE minus candidate MAE; stored pool-cluster interval, not candidate error interval.",
    "rendered": "gemma3-270m/math: T-only MAE 0.0654; gain -0.0088 [-0.0098, -0.0081]\\newline gemma3-270m/code: E-only MAE 0.0230; gain 0.0038 [0.0025, 0.0050]\\newline gemma3-270m/qa: E-only MAE 0.6097; gain 0.0947 [0.0774, 0.1093]\\newline gemma3-1b/math: surface:L0 MAE 0.0335; gain -0.0234 [-0.0235, -0.0233]\\newline gemma3-1b/code: E-only MAE 0.0532; gain 0.0047 [0.0042, 0.0050]\\newline gemma3-1b/qa: surface:logN MAE 0.4502; gain -0.0132 [-0.0198, -0.0098]"
  },
  {
    "row": 7,
    "column": 6,
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

## Input hashes

- `results/a2-curvature-interaction/summary.json`: `aed1934bf0c81333e200678f08567d018575fb3fcef7e2ecfcd881c95d3f820f`
- `results/a5-corner-second-difference/summary.json`: `05de90f078ea37d760f256eb9b9cfe37bea734827b2c8099e25f66a689a1bc75`
- `results/a7-closeout-audit/summary.json`: `14d698bc5348bee38fe593632f421fa64d794ad2a2687a70532bae935a078c9e`
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
