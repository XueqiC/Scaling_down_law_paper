# v9_blocks_Qwen-Qwen3-0.6B_c: frozen sources

v9_blocks_Qwen-Qwen3-0.6B_a.pdf: 2.7 x 2.4 in; bold Times New Roman; ticks 8.5 pt, axis labels 9.5 pt, legend 8.5 pt; default lines 1.1 pt, markers 3.8 pt; caps 2 pt. Rendered artist sizes: {'line_widths_pt': [1.1], 'marker_sizes_pt': [], 'errorbar_widths_pt': [], 'cap_sizes_pt': [], 'cap_widths_pt': []}. Full canvas retained; no titles, panel letters, or explanatory annotations.
v9_blocks_Qwen-Qwen3-0.6B_b.pdf: 2.7 x 2.4 in; bold Times New Roman; ticks 8.5 pt, axis labels 9.5 pt, legend 8.5 pt; default lines 1.1 pt, markers 3.8 pt; caps 2 pt. Rendered artist sizes: {'line_widths_pt': [1.1], 'marker_sizes_pt': [], 'errorbar_widths_pt': [], 'cap_sizes_pt': [], 'cap_widths_pt': []}. Full canvas retained; no titles, panel letters, or explanatory annotations.
v9_blocks_Qwen-Qwen3-0.6B_c.pdf: 2.7 x 2.4 in; bold Times New Roman; ticks 8.5 pt, axis labels 9.5 pt, legend 8.5 pt; default lines 1.1 pt, markers 3.8 pt; caps 2 pt. Rendered artist sizes: {'line_widths_pt': [1.1], 'marker_sizes_pt': [], 'errorbar_widths_pt': [], 'cap_sizes_pt': [], 'cap_widths_pt': []}. Full canvas retained; no titles, panel letters, or explanatory annotations.

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
    "metric": "shared_component_removed_cosine",
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
        0.8910377705471797,
        -0.5690700120908639,
        0.7751667157380321,
        0.7227443275096145,
        -0.8469828561107465,
        -0.8555293704675719,
        -0.8644703922316257,
        0.5128677106514765
      ],
      [
        0.8910377705471797,
        1.0,
        -0.6600094252846057,
        0.8228682343123872,
        0.7821663238459704,
        -0.8565789611006771,
        -0.8731980418850007,
        -0.8907532017790061,
        0.5577499951698179
      ],
      [
        -0.5690700120908639,
        -0.6600094252846057,
        1.0,
        -0.6012376959397355,
        -0.5832232691887828,
        0.4838356499047835,
        0.5073848648965649,
        0.6337557577297122,
        -0.6895407249106044
      ],
      [
        0.7751667157380321,
        0.8228682343123872,
        -0.6012376959397355,
        1.0,
        0.842217608636224,
        -0.8192857137217886,
        -0.8352754456909168,
        -0.8224951210944702,
        0.40695241886326305
      ],
      [
        0.7227443275096145,
        0.7821663238459704,
        -0.5832232691887828,
        0.842217608636224,
        1.0,
        -0.7930169387871564,
        -0.8123117601550078,
        -0.786810279577747,
        0.3954316959158184
      ],
      [
        -0.8469828561107465,
        -0.8565789611006771,
        0.4838356499047835,
        -0.8192857137217886,
        -0.7930169387871564,
        1.0,
        0.8036883144200198,
        0.7607942481427815,
        -0.5064127125726212
      ],
      [
        -0.8555293704675719,
        -0.8731980418850007,
        0.5073848648965649,
        -0.8352754456909168,
        -0.8123117601550078,
        0.8036883144200198,
        1.0,
        0.7836910016869532,
        -0.5253447862193146
      ],
      [
        -0.8644703922316257,
        -0.8907532017790061,
        0.6337557577297122,
        -0.8224951210944702,
        -0.786810279577747,
        0.7607942481427815,
        0.7836910016869532,
        1.0,
        -0.6119375157753053
      ],
      [
        0.5128677106514765,
        0.5577499951698179,
        -0.6895407249106044,
        0.40695241886326305,
        0.3954316959158184,
        -0.5064127125726212,
        -0.5253447862193146,
        -0.6119375157753053,
        1.0
      ]
    ],
    "normalization": [
      -0.9516840106301454,
      1.0
    ]
  }
]
```
