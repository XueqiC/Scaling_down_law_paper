# Generalization: per-row MAE pairs

Native-token nats; cell counts are per capability. Baselines are selected on development evidence only. Unavailable baselines remain unscored.

| Panel / row | Capability | Relation | MAE | Development baseline | MAE | Cells |
|---|---|---|---:|---|---:|---:|
| A / Distillation: new-pool budgets (gemma3-1b) | math | E | 0.05689693 | surface:L0 | 0.03348685 | 18 |
| A / Distillation: new-pool budgets (gemma3-1b) | code | E | 0.04852503 | E-only | 0.05321250 | 18 |
| A / Distillation: new-pool budgets (gemma3-1b) | qa | joint | 0.46335672 | surface:logN | 0.45015181 | 18 |
| A / Distillation: new-pool budgets (gemma3-270m) | math | E | 0.07425436 | T-only | 0.06544438 | 18 |
| A / Distillation: new-pool budgets (gemma3-270m) | code | E | 0.01925171 | E-only | 0.02300592 | 18 |
| A / Distillation: new-pool budgets (gemma3-270m) | qa | joint | 0.51498228 | E-only | 0.60966449 | 18 |
| A / Pruning: density inside range (V46) | math | power | 0.01995258 | unavailable | unavailable | 1 |
| A / Pruning: density inside range (V46) | code | power | 0.09228975 | unavailable | unavailable | 1 |
| A / Pruning: density inside range (V46) | qa | power | 0.46572939 | unavailable | unavailable | 1 |
| A / Pruning: density inside range (V72) | math | power | 0.29182499 | A2 | 0.42499808 | 6 |
| A / Pruning: density inside range (V72) | code | power | 0.39335502 | A2 | 0.45824519 | 6 |
| A / Pruning: density inside range (V72) | qa | power | 0.67884758 | median_curve | 0.06522546 | 6 |
| A / Pruning: density outside range (V46) | math | power | 0.93048513 | unavailable | unavailable | 1 |
| A / Pruning: density outside range (V46) | code | power | 1.54989408 | unavailable | unavailable | 1 |
| A / Pruning: density outside range (V46) | qa | power | 1.42649443 | unavailable | unavailable | 1 |
| A / Quantization: new group size | math | low_order_2d | 0.21488513 | bilinear | 0.33303663 | 12 |
| A / Quantization: new group size | code | median | 0.55673580 | zero | 0.67820002 | 12 |
| A / Quantization: new group size | qa | zero | 0.45697184 | median | 0.45793974 | 12 |
| B / Pythia: locked rule on new states | math | locked-rule | 0.19339671 | unavailable | unavailable | 72 |
| B / Pythia: locked rule on new states | code | locked-rule | 0.28145138 | unavailable | unavailable | 72 |
| B / Pythia: locked rule on new states | qa | locked-rule | 0.25876513 | unavailable | unavailable | 72 |
| B / Pythia: new quantization state | math | low_order_2d | 0.30330871 | bilinear | 0.35031648 | 9 |
| B / Pythia: new quantization state | code | median | 0.15318055 | zero | 0.56272614 | 9 |
| B / Pythia: new quantization state | qa | zero | 0.22173043 | median | 0.14119600 | 9 |
| B / Pythia: new stages (power) | math | power | 0.24305607 | A2 | 0.22984457 | 9 |
| B / Pythia: new stages (power) | code | power | 0.23612291 | A2 | 0.22170453 | 9 |
| B / Pythia: new stages (power) | qa | power | 0.67842569 | median_curve | 0.22064206 | 9 |
