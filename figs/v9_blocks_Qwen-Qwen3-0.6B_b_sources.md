# v9_blocks_Qwen-Qwen3-0.6B_b: frozen sources

v9_blocks_Qwen-Qwen3-0.6B_a.pdf: 2.7 x 2.4 in; bold Times New Roman; ticks 8.5 pt, axis labels 9.5 pt, legend 8.5 pt; default lines 1.1 pt, markers 3.8 pt; caps 2 pt. Rendered artist sizes: {'line_widths_pt': [1.1], 'marker_sizes_pt': [], 'errorbar_widths_pt': [], 'cap_sizes_pt': [], 'cap_widths_pt': []}. Full canvas retained; no titles, panel letters, or explanatory annotations.
v9_blocks_Qwen-Qwen3-0.6B_b.pdf: 2.7 x 2.4 in; bold Times New Roman; ticks 8.5 pt, axis labels 9.5 pt, legend 8.5 pt; default lines 1.1 pt, markers 3.8 pt; caps 2 pt. Rendered artist sizes: {'line_widths_pt': [1.1], 'marker_sizes_pt': [], 'errorbar_widths_pt': [], 'cap_sizes_pt': [], 'cap_widths_pt': []}. Full canvas retained; no titles, panel letters, or explanatory annotations.

## Inputs (SHA-256)

- `results/v9-capability-regions/Qwen--Qwen3-0.6B/similarity.json`: `7baa6ae837faff6610c480c19f2f1b1e76085d170a779ee6b15339f7f6b3f436`
- `results/v9-capability-regions/Qwen--Qwen3-1.7B/similarity.json`: `bc127c5fff1cb67c9d47f17b0db1147b6e6609c645d885f1871c3974fbea6449`
- `results/v9-capability-regions/Qwen--Qwen3-4B/similarity.json`: `0a428b0c9a5e5a0bff79d960c7e3798e8b82c43b9682a1a54cc605e77ae1a5f0`
- `results/v9-capability-regions/gemma3-12b/similarity.json`: `0dbca441ac01f828ff9fa8d403734ef58678fa0edeab60d5b3fe9a6cf278ea9e`
- `results/v9-capability-regions/gemma3-1b/similarity.json`: `3de3aba8fcb6798cdc1a0f06db2320a13224770595a5e0197910bdb980fbe9e8`
- `results/v9-capability-regions/gemma3-270m/similarity.json`: `b40d1bd098f0da40e9dfc2249e5981775a60201dc10b998b3cd5bc2e46ed27e8`
- `results/v9-capability-regions/gemma3-4b/similarity.json`: `eedcb25fc7a243a2fb1bacebaed398c6d528f9d09dfb923c13bf7c3f062a2c4e`
- `results/v9-capability-regions/gemma4-31b/similarity.json`: `611e31974a97e8fb59e247058a5ca3145e769825985c1b85683ffbc973eb97a9`
- `results/v9-capability-regions/muse-30b/similarity.json`: `7826a91e82c1fa46975674be53a5937c7da3e72788f05a021ecc291f0ad8dc35`
- `results/v9-capability-regions/olmo3-7b/similarity.json`: `f465be360c4bfee1c428932532b9866a296fd25182d26f01fa417a7cd39db085`

## Plotted records

```json
[
  {
    "model": "Qwen--Qwen3-0.6B",
    "metric": "log_cosine",
    "benchmarks": [
      "gsm8k",
      "math500",
      "svamp",
      "humaneval",
      "mbpp",
      "2wiki",
      "hotpotqa",
      "triviaqa",
      "c4"
    ],
    "matrix": [
      [
        1.0,
        0.9980416614359161,
        0.9845592817695217,
        0.9969019067937096,
        0.9965335224633334,
        0.9762591365449809,
        0.9727397088017057,
        0.9707195322297684,
        0.9944297783572755
      ],
      [
        0.9980416614359161,
        1.0,
        0.9809273034669748,
        0.997081818390648,
        0.9966618345840532,
        0.9731801636971649,
        0.969233608209184,
        0.9668369307234383,
        0.9943050768107516
      ],
      [
        0.9845592817695217,
        0.9809273034669748,
        1.0,
        0.9844317200953797,
        0.9856611747781213,
        0.9898495676610829,
        0.9887647983763816,
        0.9908750182019304,
        0.9813312170259553
      ],
      [
        0.9969019067937096,
        0.997081818390648,
        0.9844317200953797,
        1.0,
        0.9981387002866687,
        0.977107996570057,
        0.9735150431726441,
        0.9720398361594503,
        0.9932434825104312
      ],
      [
        0.9965335224633334,
        0.9966618345840532,
        0.9856611747781213,
        0.9981387002866687,
        1.0,
        0.9787975528480483,
        0.9752918321459114,
        0.9741106411763555,
        0.993565390359575
      ],
      [
        0.9762591365449809,
        0.9731801636971649,
        0.9898495676610829,
        0.977107996570057,
        0.9787975528480483,
        1.0,
        0.9934419698833387,
        0.9915350107457014,
        0.97939062337385
      ],
      [
        0.9727397088017057,
        0.969233608209184,
        0.9887647983763816,
        0.9735150431726441,
        0.9752918321459114,
        0.9934419698833387,
        1.0,
        0.9917555534845705,
        0.9761253034433449
      ],
      [
        0.9707195322297684,
        0.9668369307234383,
        0.9908750182019304,
        0.9720398361594503,
        0.9741106411763555,
        0.9915350107457014,
        0.9917555534845705,
        1.0,
        0.9727005364898503
      ],
      [
        0.9944297783572755,
        0.9943050768107516,
        0.9813312170259553,
        0.9932434825104312,
        0.993565390359575,
        0.97939062337385,
        0.9761253034433449,
        0.9727005364898503,
        1.0
      ]
    ],
    "normalization": [
      0.955066512094533,
      1.0
    ]
  }
]
```
