# final_relations_b: frozen sources

final_relations_a.pdf: 1.8 x 1.35 in; bold Times New Roman; ticks 7.5 pt, axis labels 8.5 pt, legend 7.5 pt; default lines 1.1 pt, markers 3.8 pt; caps 2 pt. Rendered artist sizes: {'line_widths_pt': [0.4, 1.1], 'marker_sizes_pt': [3.8], 'errorbar_widths_pt': [], 'cap_sizes_pt': [], 'cap_widths_pt': []}. Full canvas retained; no titles, panel letters, or explanatory annotations.
Marker displacement is at most 1.5% of each axis range (also on the displayed scale for nonlinear axes); cluster spread is at most 6%. When bounded dodging cannot retain partial visibility, the cluster stays at its true coordinates with thin white edges and smaller glyphs above larger ones. Coincident neighbours and any hidden markers are documented in the sidecar.
final_relations_b.pdf: 1.8 x 1.35 in; bold Times New Roman; ticks 7.5 pt, axis labels 8.5 pt, legend 7.5 pt; default lines 1.1 pt, markers 3.8 pt; caps 2 pt. Rendered artist sizes: {'line_widths_pt': [1.1], 'marker_sizes_pt': [3.8], 'errorbar_widths_pt': [], 'cap_sizes_pt': [], 'cap_widths_pt': []}. Full canvas retained; no titles, panel letters, or explanatory annotations.
Marker displacement is at most 1.5% of each axis range (also on the displayed scale for nonlinear axes); cluster spread is at most 6%. When bounded dodging cannot retain partial visibility, the cluster stays at its true coordinates with thin white edges and smaller glyphs above larger ones. Coincident neighbours and any hidden markers are documented in the sidecar.

## Inputs (SHA-256)

- `results/v53-prune-dev/predictions_pythia-1.4b@step112000.json`: `862e299cc30a55672c785de418b0c184c204e3d5c2b222fb6174351e507489f4`
- `results/v53-prune-dev/register.json`: `7498103830f139f6bea16ee440b717a05dee41e45b9835fdac6a2251b833974d`
- `results/v6-capability-geometry/pythia-1.4b--step112000/prune_losses.json`: `bfc02e7d54eb623c2e8e4f1237b546aa62ecd14f23330b50e2a833e226916c42`
- `results/v69-quant-confirm/compare.json`: `12944c61ed42c61f1beaf8f84ef5c87d900b3b1a38d65d175976e27d3d4e6bac`
- `results/v69-quant-confirm/develop.json`: `9f035cb37a94d425064f37d822490b52dcad4c669e62864f27cba4ffa5e5643d`
- `results/v69-quant-confirm/freeze.json`: `6ade0a3ff576781cf286978519b6a922500d37e3bc72cef4e3e635e826cccdc2`
- `results/v70-distill-confirm/compare.json`: `983f53033b07e035b1cb552429b8ce6ab23f8d6aee4365237970e2b46b0a829b`
- `results/v70-distill-confirm/freeze.json`: `d7b28c7251dbc6113c3de7c957560827e603d4e77a48010f99835a8468db0c24`

## Plotted records

```json
[
  {
    "state": "pythia-410m@step143000",
    "config": "b3_g64",
    "capability": "math",
    "phi_raw": [
      19.52590409133485,
      1.458277307601044,
      26.426690701000897
    ],
    "dL": 1.7077434153286406
  },
  {
    "state": "pythia-410m@step143000",
    "config": "b3_g128",
    "capability": "math",
    "phi_raw": [
      19.52590409133485,
      1.458277307601044,
      26.426690701000897
    ],
    "dL": 2.2400933322787315
  },
  {
    "state": "pythia-410m@step143000",
    "config": "b3_g256",
    "capability": "math",
    "phi_raw": [
      19.52590409133485,
      1.458277307601044,
      26.426690701000897
    ],
    "dL": 3.2337261725856203
  },
  {
    "state": "pythia-1.4b@step16000",
    "config": "b3_g64",
    "capability": "math",
    "phi_raw": [
      20.912198452454742,
      1.469370402594321,
      24.23643479298077
    ],
    "dL": 0.19589891639642487
  },
  {
    "state": "pythia-1.4b@step16000",
    "config": "b3_g128",
    "capability": "math",
    "phi_raw": [
      20.912198452454742,
      1.469370402594321,
      24.23643479298077
    ],
    "dL": 0.2774855651348571
  },
  {
    "state": "pythia-1.4b@step16000",
    "config": "b3_g256",
    "capability": "math",
    "phi_raw": [
      20.912198452454742,
      1.469370402594321,
      24.23643479298077
    ],
    "dL": 0.35323894645258247
  },
  {
    "state": "pythia-410m@step143000",
    "config": "b3_g32",
    "test_set": "development_state_boundary",
    "capability": "math",
    "L0": 1.458277307601044,
    "phi_raw": [
      19.52590409133485,
      1.458277307601044,
      26.426690701000897
    ],
    "predictions": {
      "low_order_2d": 1.2243703359870879,
      "bilinear": 0.9456986182281502,
      "same_input_interpolation": 1.5316957517181335,
      "bit_only": 2.1594520520865013,
      "median": 0.26514672150597185,
      "zero": 0.0
    },
    "selected_candidate": "low_order_2d",
    "selected_prediction": 1.2243703359870879,
    "dense": 1.458277307601044,
    "loss": 2.759076168630863,
    "dL": 1.300798861029819,
    "regime": "clear_damage",
    "dense_difference_from_prediction_input": 0.0,
    "absolute_errors": {
      "low_order_2d": 0.07642852504273101,
      "bilinear": 0.35510024280166874,
      "same_input_interpolation": 0.23089689068831465,
      "bit_only": 0.8586531910566824,
      "median": 1.035652139523847,
      "zero": 1.300798861029819
    }
  },
  {
    "state": "pythia-410m@step143000",
    "config": "b3_g512",
    "test_set": "development_state_boundary",
    "capability": "math",
    "L0": 1.458277307601044,
    "phi_raw": [
      19.52590409133485,
      1.458277307601044,
      26.426690701000897
    ],
    "predictions": {
      "low_order_2d": 3.6518772037038505,
      "bilinear": 3.3732054859449137,
      "same_input_interpolation": 4.328598275590526,
      "bit_only": 2.1594520520865013,
      "median": 1.7524914972712171,
      "zero": 0.0
    },
    "selected_candidate": "low_order_2d",
    "selected_prediction": 3.6518772037038505,
    "dense": 1.458277307601044,
    "loss": 6.0478525666376655,
    "dL": 4.5895752590366214,
    "regime": "clear_damage",
    "dense_difference_from_prediction_input": 0.0,
    "absolute_errors": {
      "low_order_2d": 0.937698055332771,
      "bilinear": 1.2163697730917078,
      "same_input_interpolation": 0.26097698344609555,
      "bit_only": 2.43012320695012,
      "median": 2.8370837617654043,
      "zero": 4.5895752590366214
    }
  },
  {
    "state": "pythia-1.4b@step16000",
    "config": "b3_g32",
    "test_set": "development_state_boundary",
    "capability": "math",
    "L0": 1.469370402594321,
    "phi_raw": [
      20.912198452454742,
      1.469370402594321,
      24.23643479298077
    ],
    "predictions": {
      "low_order_2d": 0.39028210345371406,
      "bilinear": 0.3337767187497609,
      "same_input_interpolation": 0.30882348387233804,
      "bit_only": 0.40701953832682447,
      "median": 0.26514672150597185,
      "zero": 0.0
    },
    "selected_candidate": "low_order_2d",
    "selected_prediction": 0.39028210345371406,
    "dense": 1.469370402594321,
    "loss": 1.6028434706952464,
    "dL": 0.1334730681009253,
    "regime": "clear_damage",
    "dense_difference_from_prediction_input": 0.0,
    "absolute_errors": {
      "low_order_2d": 0.25680903535278876,
      "bilinear": 0.2003036506488356,
      "same_input_interpolation": 0.17535041577141275,
      "bit_only": 0.2735464702258992,
      "median": 0.13167365340504655,
      "zero": 0.1334730681009253
    }
  },
  {
    "state": "pythia-1.4b@step16000",
    "config": "b3_g512",
    "test_set": "development_state_boundary",
    "capability": "math",
    "L0": 1.469370402594321,
    "phi_raw": [
      20.912198452454742,
      1.469370402594321,
      24.23643479298077
    ],
    "predictions": {
      "low_order_2d": 0.5367677426077408,
      "bilinear": 0.4802623579037868,
      "same_input_interpolation": 0.4703792336023458,
      "bit_only": 0.40701953832682447,
      "median": 1.7524914972712171,
      "zero": 0.0
    },
    "selected_candidate": "low_order_2d",
    "selected_prediction": 0.5367677426077408,
    "dense": 1.469370402594321,
    "loss": 1.9065095309657518,
    "dL": 0.43713912837143076,
    "regime": "clear_damage",
    "dense_difference_from_prediction_input": 0.0,
    "absolute_errors": {
      "low_order_2d": 0.09962861423631009,
      "bilinear": 0.04312322953235603,
      "same_input_interpolation": 0.03324010523091503,
      "bit_only": 0.030119590044606293,
      "median": 1.3153523688997864,
      "zero": 0.43713912837143076
    }
  }
]
```
