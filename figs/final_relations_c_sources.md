# final_relations_c: frozen sources

final_relations_a.pdf: 1.8 x 1.35 in; bold Times New Roman; ticks 7.5 pt, axis labels 8.5 pt, legend 7.5 pt; default lines 1.1 pt, markers 3.8 pt; caps 2 pt. Rendered artist sizes: {'line_widths_pt': [0.4, 1.1], 'marker_sizes_pt': [3.8], 'errorbar_widths_pt': [], 'cap_sizes_pt': [], 'cap_widths_pt': []}. Full canvas retained; no titles, panel letters, or explanatory annotations.
Marker displacement is at most 1.5% of each axis range (also on the displayed scale for nonlinear axes); cluster spread is at most 6%. When bounded dodging cannot retain partial visibility, the cluster stays at its true coordinates with thin white edges and smaller glyphs above larger ones. Coincident neighbours and any hidden markers are documented in the sidecar.
final_relations_b.pdf: 1.8 x 1.35 in; bold Times New Roman; ticks 7.5 pt, axis labels 8.5 pt, legend 7.5 pt; default lines 1.1 pt, markers 3.8 pt; caps 2 pt. Rendered artist sizes: {'line_widths_pt': [1.1], 'marker_sizes_pt': [3.8], 'errorbar_widths_pt': [], 'cap_sizes_pt': [], 'cap_widths_pt': []}. Full canvas retained; no titles, panel letters, or explanatory annotations.
Marker displacement is at most 1.5% of each axis range (also on the displayed scale for nonlinear axes); cluster spread is at most 6%. When bounded dodging cannot retain partial visibility, the cluster stays at its true coordinates with thin white edges and smaller glyphs above larger ones. Coincident neighbours and any hidden markers are documented in the sidecar.
final_relations_c.pdf: 1.8 x 1.35 in; bold Times New Roman; ticks 7.5 pt, axis labels 8.5 pt, legend 7.5 pt; default lines 1.1 pt, markers 3.8 pt; caps 2 pt. Rendered artist sizes: {'line_widths_pt': [1.1], 'marker_sizes_pt': [3.8], 'errorbar_widths_pt': [], 'cap_sizes_pt': [], 'cap_widths_pt': []}. Full canvas retained; no titles, panel letters, or explanatory annotations.
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
    "config": "b4_g64",
    "capability": "math",
    "phi_raw": [
      19.52590409133485,
      1.458277307601044,
      26.426690701000897
    ],
    "dL": 0.25175986712014553
  },
  {
    "state": "pythia-410m@step143000",
    "config": "b4_g128",
    "capability": "math",
    "phi_raw": [
      19.52590409133485,
      1.458277307601044,
      26.426690701000897
    ],
    "dL": 0.29458989163964255
  },
  {
    "state": "pythia-410m@step143000",
    "config": "b4_g256",
    "capability": "math",
    "phi_raw": [
      19.52590409133485,
      1.458277307601044,
      26.426690701000897
    ],
    "dL": 0.35497903978486134
  },
  {
    "state": "pythia-1.4b@step16000",
    "config": "b4_g64",
    "capability": "math",
    "phi_raw": [
      20.912198452454742,
      1.469370402594321,
      24.23643479298077
    ],
    "dL": 0.026793482559519077
  },
  {
    "state": "pythia-1.4b@step16000",
    "config": "b4_g128",
    "capability": "math",
    "phi_raw": [
      20.912198452454742,
      1.469370402594321,
      24.23643479298077
    ],
    "dL": 0.026220042711381675
  },
  {
    "state": "pythia-1.4b@step16000",
    "config": "b4_g256",
    "capability": "math",
    "phi_raw": [
      20.912198452454742,
      1.469370402594321,
      24.23643479298077
    ],
    "dL": 0.04099106224788418
  },
  {
    "state": "pythia-410m@step143000",
    "config": "b4_g32",
    "test_set": "development_state_boundary",
    "capability": "math",
    "L0": 1.458277307601044,
    "phi_raw": [
      19.52590409133485,
      1.458277307601044,
      26.426690701000897
    ],
    "predictions": {
      "low_order_2d": -0.187308550463808,
      "bilinear": 0.41114250539849684,
      "same_input_interpolation": 0.21767676541327824,
      "bit_only": 0.8931017319759935,
      "median": 0.05174800284742542,
      "zero": 0.0
    },
    "selected_candidate": "low_order_2d",
    "selected_prediction": -0.187308550463808,
    "dense": 1.458277307601044,
    "loss": 1.6511706082417148,
    "dL": 0.19289330064067078,
    "regime": "clear_damage",
    "dense_difference_from_prediction_input": 0.0,
    "absolute_errors": {
      "low_order_2d": 0.3802018511044788,
      "bilinear": 0.21824920475782605,
      "same_input_interpolation": 0.024783464772607455,
      "bit_only": 0.7002084313353227,
      "median": 0.14114529779324536,
      "zero": 0.19289330064067078
    }
  },
  {
    "state": "pythia-410m@step143000",
    "config": "b4_g512",
    "test_set": "development_state_boundary",
    "capability": "math",
    "L0": 1.458277307601044,
    "phi_raw": [
      19.52590409133485,
      1.458277307601044,
      26.426690701000897
    ],
    "predictions": {
      "low_order_2d": 0.7766099026911707,
      "bilinear": 1.3750609585534752,
      "same_input_interpolation": 0.41093423838062,
      "bit_only": 0.8931017319759935,
      "median": 0.13202958158664868,
      "zero": 0.0
    },
    "selected_candidate": "low_order_2d",
    "selected_prediction": 0.7766099026911707,
    "dense": 1.458277307601044,
    "loss": 1.8834532943130586,
    "dL": 0.4251759867120146,
    "regime": "clear_damage",
    "dense_difference_from_prediction_input": 0.0,
    "absolute_errors": {
      "low_order_2d": 0.3514339159791561,
      "bilinear": 0.9498849718414606,
      "same_input_interpolation": 0.014241748331394632,
      "bit_only": 0.4679257452639789,
      "median": 0.29314640512536594,
      "zero": 0.4251759867120146
    }
  },
  {
    "state": "pythia-1.4b@step16000",
    "config": "b4_g32",
    "test_set": "development_state_boundary",
    "capability": "math",
    "L0": 1.469370402594321,
    "phi_raw": [
      20.912198452454742,
      1.469370402594321,
      24.23643479298077
    ],
    "predictions": {
      "low_order_2d": 0.028774610912310983,
      "bilinear": 0.13794626159151147,
      "same_input_interpolation": 0.03488421308635625,
      "bit_only": 0.16622294665629544,
      "median": 0.05174800284742542,
      "zero": 0.0
    },
    "selected_candidate": "low_order_2d",
    "selected_prediction": 0.028774610912310983,
    "dense": 1.469370402594321,
    "loss": 1.48799731076485,
    "dL": 0.018626908170529033,
    "regime": "near_zero",
    "dense_difference_from_prediction_input": 0.0,
    "absolute_errors": {
      "low_order_2d": 0.01014770274178195,
      "bilinear": 0.11931935342098243,
      "same_input_interpolation": 0.01625730491582722,
      "bit_only": 0.1475960384857664,
      "median": 0.03312109467689639,
      "zero": 0.018626908170529033
    }
  },
  {
    "state": "pythia-1.4b@step16000",
    "config": "b4_g512",
    "test_set": "development_state_boundary",
    "capability": "math",
    "L0": 1.469370402594321,
    "phi_raw": [
      20.912198452454742,
      1.469370402594321,
      24.23643479298077
    ],
    "predictions": {
      "low_order_2d": 0.08532798104189965,
      "bilinear": 0.19449963172109785,
      "same_input_interpolation": 0.049506469532983544,
      "bit_only": 0.16622294665629544,
      "median": 0.13202958158664868,
      "zero": 0.0
    },
    "selected_candidate": "low_order_2d",
    "selected_prediction": 0.08532798104189965,
    "dense": 1.469370402594321,
    "loss": 1.5184884916554615,
    "dL": 0.04911808906114046,
    "regime": "near_zero",
    "dense_difference_from_prediction_input": 0.0,
    "absolute_errors": {
      "low_order_2d": 0.03620989198075919,
      "bilinear": 0.1453815426599574,
      "same_input_interpolation": 0.0003883804718430861,
      "bit_only": 0.11710485759515499,
      "median": 0.08291149252550822,
      "zero": 0.04911808906114046
    }
  }
]
```
