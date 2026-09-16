# final_relations_a: frozen sources

final_relations_a.pdf: 1.8 x 1.35 in; bold Times New Roman; ticks 7.5 pt, axis labels 8.5 pt, legend 7.5 pt; default lines 1.1 pt, markers 3.8 pt; caps 2 pt. Rendered artist sizes: {'line_widths_pt': [0.4, 1.1], 'marker_sizes_pt': [3.8], 'errorbar_widths_pt': [], 'cap_sizes_pt': [], 'cap_widths_pt': []}. Full canvas retained; no titles, panel letters, or explanatory annotations.
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
    "predictions": {
      "schema_version": 1,
      "target": {
        "tag": "pythia-1.4b@step112000",
        "size": "1.4b",
        "step": 112000,
        "N0": 1207959552,
        "D0": 234881024000,
        "L0": {
          "math": 1.2476271454559835,
          "code": 1.3067506536724507,
          "qa": 5.117365731939164
        }
      },
      "densities": [
        0.85,
        0.675,
        0.575
      ],
      "response": "signed Delta L_c(d) = prune_loss_c(d) - dense_loss_c(1.0), in nats",
      "selected_candidate": "power",
      "predictions": {
        "math": {
          "0.85": {
            "power": 0.029725239197826422,
            "A1": 0.3215953650723355,
            "A2": 0.021744003692353235,
            "cont": -0.3965712136102655,
            "strength_only": 0.009779784253812809,
            "median_curve": 0.03157873922328566,
            "zero": 0.0
          },
          "0.675": {
            "power": 0.5399402959797418,
            "A1": 0.6967899576567267,
            "A2": 0.38084121688395045,
            "cont": 0.46186941678770266,
            "strength_only": 0.5665494330340186,
            "median_curve": 0.4800729652772281,
            "zero": 0.0
          },
          "0.575": {
            "power": 1.47652778650222,
            "A1": 0.9111868677049506,
            "A2": 1.5682887641087606,
            "cont": 1.5911839532367722,
            "strength_only": 2.316818683961089,
            "median_curve": 1.8850253104484715,
            "zero": 0.0
          }
        },
        "code": {
          "0.85": {
            "power": 0.07305297283120969,
            "A1": 0.41513399663792483,
            "A2": 0.029143058085327894,
            "cont": -0.3479999483937305,
            "strength_only": 0.01768320368873879,
            "median_curve": 0.02684513905395771,
            "zero": 0.0
          },
          "0.675": {
            "power": 0.7723316006501185,
            "A1": 0.8994569927155035,
            "A2": 0.4973421015305711,
            "cont": 0.6337217563366377,
            "strength_only": 0.6695512551824494,
            "median_curve": 0.3295994770620392,
            "zero": 0.0
          },
          "0.575": {
            "power": 1.7504342017642076,
            "A1": 1.1762129904741203,
            "A2": 1.9551651024921424,
            "cont": 1.865691877270634,
            "strength_only": 2.362435734336263,
            "median_curve": 1.8752376990729753,
            "zero": 0.0
          }
        },
        "qa": {
          "0.85": {
            "power": 0.05004426514120916,
            "A1": 0.2823725928758775,
            "A2": 0.001294420835951055,
            "cont": -0.23748845530725043,
            "strength_only": 0.0019028033608603793,
            "median_curve": -0.04523378089353639,
            "zero": 0.0
          },
          "0.675": {
            "power": 0.5290786384446304,
            "A1": 0.6118072845644011,
            "A2": 0.15130684614642975,
            "cont": 0.39651281730856236,
            "strength_only": 0.19685503230948026,
            "median_curve": -0.31636911834600745,
            "zero": 0.0
          },
          "0.575": {
            "power": 1.1991188025671242,
            "A1": 0.8000556798149863,
            "A2": 1.3711066843023638,
            "cont": 1.1993171712670636,
            "strength_only": 0.9844188832347244,
            "median_curve": 0.36389763545627507,
            "zero": 0.0
          }
        }
      },
      "provenance": {
        "register_sha256": "7498103830f139f6bea16ee440b717a05dee41e45b9835fdac6a2251b833974d",
        "dense_sha256": "357f0784978e815a88669dfea28237116f0559ca68c42021c90f95a01c893e00"
      }
    },
    "losses": {
      "1.0": {
        "math": 1.2476271454559835,
        "code": 1.3067506536724507,
        "qa": 5.117365731939164
      },
      "0.85": {
        "math": 1.2740053784702998,
        "code": 1.3335512241502259,
        "qa": 5.106137119771863
      },
      "0.675": {
        "math": 1.6270465870442141,
        "code": 1.573746137390064,
        "qa": 4.472492870722434
      },
      "0.575": {
        "math": 2.844538479791189,
        "code": 2.8540527691942,
        "qa": 4.975403992395437
      }
    }
  }
]
```
