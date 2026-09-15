# fig4_c: frozen sources

a/b: delta = loss_source - dense_source; x parsed from the JSON configuration key. a delivered: reuse plot_fig1_final.prune_curve; pointwise median of nine frozen state predictions for power, source-free median_curve for QA; no fitting. c: delta = V69 dL; bit and group parsed from config.
fig4_a.pdf: 2.7 x 2 in; bold Times New Roman; ticks 14 pt, axis labels 15 pt, legend 13 pt; lines 2 pt, markers 7 pt. Full canvas retained; no titles, panel letters, or explanatory annotations.
fig4_b.pdf: 2.7 x 2 in; bold Times New Roman; ticks 14 pt, axis labels 15 pt, legend 13 pt; lines 2 pt, markers 7 pt. Full canvas retained; no titles, panel letters, or explanatory annotations.
fig4_c.pdf: 2.7 x 2 in; bold Times New Roman; ticks 14 pt, axis labels 15 pt, legend 13 pt; lines 2 pt, markers 7 pt. Full canvas retained; no titles, panel letters, or explanatory annotations.

## Inputs (SHA-256)

- `results/v10-quantization/pythia-1.4b--step143000/quant_losses.json`: `5330aaa9da7183204c37d1ff1e2ea64c651ed588bb2f72f0ed7aaed72a595243`
- `results/v10-quantization/pythia-1.4b--step16000/quant_losses.json`: `a903eaa306be8c4ba70fda979bcfafa4cc1334fab7b62997e4b6e7f96cf2c945`
- `results/v10-quantization/pythia-1.4b--step64000/quant_losses.json`: `1087bbf6102d85fded469961d958c713908e4ba936e24cd2d4985ee8b6e2a274`
- `results/v10-quantization/pythia-160m--step143000/quant_losses.json`: `96aa01041b947077090736afe19a1becd8b9135c9b7b4037a5ea457d6fd0b334`
- `results/v10-quantization/pythia-160m--step16000/quant_losses.json`: `11d1845671057066a1e15286b7f84853c6db11511b44bb7bb72328d3fd0d3178`
- `results/v10-quantization/pythia-160m--step64000/quant_losses.json`: `dde3f0ad83db6997054a79318959dee2c33195ded3d11247fcb12a9992fba4ca`
- `results/v10-quantization/pythia-410m--step143000/quant_losses.json`: `6f0e6c037d8b993301839d55f1b8e1261680cc1ed93864b08a2237a1b5698790`
- `results/v10-quantization/pythia-410m--step16000/quant_losses.json`: `ae2ae21276a632816c48bfad123d6963e3f0e4b96c56c47a046220f39b00aed7`
- `results/v10-quantization/pythia-410m--step64000/quant_losses.json`: `6d0bafbaabcf80fc426ee0587d1deceed793b9ad3ef4ddad189e0426212102e0`
- `results/v36-pythia-controlled/summary.json`: `58dd81d2db4c089f97656232908d4aab8bccdf3114c05a880a50a5aaff844874`
- `results/v53-prune-dev/register.json`: `7498103830f139f6bea16ee440b717a05dee41e45b9835fdac6a2251b833974d`
- `results/v6-capability-geometry/pythia-1.4b--step143000/prune_losses.json`: `5ec4800f980d6317520f3d7eb85f4516631b629a146d5a964e33092eb1507315`
- `results/v6-capability-geometry/pythia-1.4b--step16000/prune_losses.json`: `95cbe7e98739be4ea472781bf4f8a27c28827250e22d1bdbd8c5c576bd73938a`
- `results/v6-capability-geometry/pythia-1.4b--step64000/prune_losses.json`: `a458cd11272a9face425eda62134b25ef0bf4af622f5902c63f13233028c0b15`
- `results/v6-capability-geometry/pythia-160m--step143000/prune_losses.json`: `87d9ebcad62e27b675e038b584671175f66aed91fc18da786ffc0f553af68e37`
- `results/v6-capability-geometry/pythia-160m--step16000/prune_losses.json`: `46c5f9c6cfb0b5581b13f517951b861cb1c52998c333945a37639b1031862525`
- `results/v6-capability-geometry/pythia-160m--step64000/prune_losses.json`: `f5791d151a0507ac90aeaddaf97d4686ceead336d4fa7b128ec711f4793ad354`
- `results/v6-capability-geometry/pythia-410m--step143000/prune_losses.json`: `f46f388cee3fbb1bb7a0175c1dfde457b13bee0fa262092d9ac1e41845df0e7b`
- `results/v6-capability-geometry/pythia-410m--step16000/prune_losses.json`: `228e436b0b58d734eb924f2ddc45b4c8135aa3b2765bb3b764db7a456123dcf9`
- `results/v6-capability-geometry/pythia-410m--step64000/prune_losses.json`: `81bafd7adac31f27f2973545407005177fad63cf6d6e2ef942109e10fd8f3756`
- `results/v69-quant-confirm/compare.json`: `12944c61ed42c61f1beaf8f84ef5c87d900b3b1a38d65d175976e27d3d4e6bac`
- `results/v69-quant-confirm/develop.json`: `9f035cb37a94d425064f37d822490b52dcad4c669e62864f27cba4ffa5e5643d`
- `results/v69-quant-confirm/freeze.json`: `6ade0a3ff576781cf286978519b6a922500d37e3bc72cef4e3e635e826cccdc2`

## Plotted records

```json
[
  {
    "panel": "c",
    "kind": "measured",
    "state": "pythia-410m@step143000",
    "capability": "math",
    "bit": 3,
    "x": 64,
    "delta": 1.7077434153286406,
    "delta_source": "results/v69-quant-confirm/develop.json#/dev_rows/81/dL",
    "config_source": "results/v69-quant-confirm/develop.json#/dev_rows/81/config"
  },
  {
    "panel": "c",
    "kind": "measured",
    "state": "pythia-410m@step143000",
    "capability": "math",
    "bit": 3,
    "x": 128,
    "delta": 2.2400933322787315,
    "delta_source": "results/v69-quant-confirm/develop.json#/dev_rows/84/dL",
    "config_source": "results/v69-quant-confirm/develop.json#/dev_rows/84/config"
  },
  {
    "panel": "c",
    "kind": "measured",
    "state": "pythia-410m@step143000",
    "capability": "math",
    "bit": 3,
    "x": 256,
    "delta": 3.2337261725856203,
    "delta_source": "results/v69-quant-confirm/develop.json#/dev_rows/87/dL",
    "config_source": "results/v69-quant-confirm/develop.json#/dev_rows/87/config"
  },
  {
    "panel": "c",
    "kind": "measured",
    "state": "pythia-410m@step143000",
    "capability": "math",
    "bit": 4,
    "x": 64,
    "delta": 0.25175986712014553,
    "delta_source": "results/v69-quant-confirm/develop.json#/dev_rows/90/dL",
    "config_source": "results/v69-quant-confirm/develop.json#/dev_rows/90/config"
  },
  {
    "panel": "c",
    "kind": "measured",
    "state": "pythia-410m@step143000",
    "capability": "math",
    "bit": 4,
    "x": 128,
    "delta": 0.29458989163964255,
    "delta_source": "results/v69-quant-confirm/develop.json#/dev_rows/93/dL",
    "config_source": "results/v69-quant-confirm/develop.json#/dev_rows/93/config"
  },
  {
    "panel": "c",
    "kind": "measured",
    "state": "pythia-410m@step143000",
    "capability": "math",
    "bit": 4,
    "x": 256,
    "delta": 0.35497903978486134,
    "delta_source": "results/v69-quant-confirm/develop.json#/dev_rows/96/dL",
    "config_source": "results/v69-quant-confirm/develop.json#/dev_rows/96/config"
  },
  {
    "panel": "c",
    "kind": "measured",
    "state": "pythia-410m@step143000",
    "capability": "math",
    "bit": 5,
    "x": 64,
    "delta": 0.06303883571937052,
    "delta_source": "results/v69-quant-confirm/develop.json#/dev_rows/99/dL",
    "config_source": "results/v69-quant-confirm/develop.json#/dev_rows/99/config"
  },
  {
    "panel": "c",
    "kind": "measured",
    "state": "pythia-410m@step143000",
    "capability": "math",
    "bit": 5,
    "x": 128,
    "delta": 0.07041445859368833,
    "delta_source": "results/v69-quant-confirm/develop.json#/dev_rows/102/dL",
    "config_source": "results/v69-quant-confirm/develop.json#/dev_rows/102/config"
  },
  {
    "panel": "c",
    "kind": "measured",
    "state": "pythia-410m@step143000",
    "capability": "math",
    "bit": 5,
    "x": 256,
    "delta": 0.09875029660681811,
    "delta_source": "results/v69-quant-confirm/develop.json#/dev_rows/105/dL",
    "config_source": "results/v69-quant-confirm/develop.json#/dev_rows/105/config"
  },
  {
    "panel": "c",
    "kind": "measured",
    "state": "pythia-410m@step143000",
    "capability": "math",
    "bit": 3,
    "x": 32,
    "delta": 1.300798861029819,
    "delta_source": "results/v69-quant-confirm/compare.json#/rows/0/dL",
    "config_source": "results/v69-quant-confirm/compare.json#/rows/0/config"
  },
  {
    "panel": "c",
    "kind": "measured",
    "state": "pythia-410m@step143000",
    "capability": "math",
    "bit": 3,
    "x": 512,
    "delta": 4.5895752590366214,
    "delta_source": "results/v69-quant-confirm/compare.json#/rows/3/dL",
    "config_source": "results/v69-quant-confirm/compare.json#/rows/3/config"
  },
  {
    "panel": "c",
    "kind": "measured",
    "state": "pythia-410m@step143000",
    "capability": "math",
    "bit": 4,
    "x": 32,
    "delta": 0.19289330064067078,
    "delta_source": "results/v69-quant-confirm/compare.json#/rows/6/dL",
    "config_source": "results/v69-quant-confirm/compare.json#/rows/6/config"
  },
  {
    "panel": "c",
    "kind": "measured",
    "state": "pythia-410m@step143000",
    "capability": "math",
    "bit": 4,
    "x": 512,
    "delta": 0.4251759867120146,
    "delta_source": "results/v69-quant-confirm/compare.json#/rows/9/dL",
    "config_source": "results/v69-quant-confirm/compare.json#/rows/9/config"
  },
  {
    "panel": "c",
    "kind": "measured",
    "state": "pythia-410m@step143000",
    "capability": "math",
    "bit": 5,
    "x": 32,
    "delta": 0.04542039073004833,
    "delta_source": "results/v69-quant-confirm/compare.json#/rows/12/dL",
    "config_source": "results/v69-quant-confirm/compare.json#/rows/12/config"
  },
  {
    "panel": "c",
    "kind": "measured",
    "state": "pythia-410m@step143000",
    "capability": "math",
    "bit": 5,
    "x": 512,
    "delta": 0.09657517994146958,
    "delta_source": "results/v69-quant-confirm/compare.json#/rows/15/dL",
    "config_source": "results/v69-quant-confirm/compare.json#/rows/15/config"
  }
]
```
