# lr_pilot: frozen sources

Final checkpoint = maximum positive updates with positive processed_tokens. learning_rate = float(output_suffix after lrpilot_); delta used verbatim.
fig1_c.pdf: 1.8 x 1.35 in; bold Times New Roman; ticks 7.5 pt, axis labels 8.5 pt, legend 7.5 pt; default lines 1.1 pt, markers 3.8 pt; caps 2 pt. Rendered artist sizes: {'line_widths_pt': [1.1, 1.5], 'marker_sizes_pt': [5.0], 'errorbar_widths_pt': [], 'cap_sizes_pt': [], 'cap_widths_pt': []}. Full canvas retained; no titles, panel letters, or explanatory annotations.

## Inputs (SHA-256)

- `results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_1e-4_lora_dseed11/trajectory/update-00000000/eval.json`: `d4b93ea38f588e7799206364706c95f9125be749b53caa22d89663a8edcd6f84`
- `results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_1e-4_lora_dseed11/trajectory/update-00000008/eval.json`: `468a6868879a302993b869d74dc1ca56c3bb565adfef8411fec9c1b7bd7e407f`
- `results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_2e-4_lora_dseed11/trajectory/update-00000000/eval.json`: `77207ebd0c4b100f6bc4f3e6a65a113be8b13482282f886a40993228b01b64e6`
- `results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_2e-4_lora_dseed11/trajectory/update-00000008/eval.json`: `c774d3767e5336ad6fb32f7cfc7e08c65a011d3713e8669ca215371f896b953b`
- `results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_5e-5_lora_dseed11/trajectory/update-00000000/eval.json`: `10022114f0ab1effc8c48a5bc9a417db2ea9d19bd096d48dca58408c9cbe872a`
- `results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_5e-5_lora_dseed11/trajectory/update-00000008/eval.json`: `94649c984f59dd7b01853c76e7fd1f4e60d2707ebfce2df5b371453101757da7`
- `results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_1e-4_lora_dseed11/trajectory/update-00000000/eval.json`: `4d8a442d7e1e3de687761ca5ec2853626f97621cea6036cb9bffe1f6d1db5f19`
- `results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_1e-4_lora_dseed11/trajectory/update-00000008/eval.json`: `03897bc164c6a3f44c718aab4418f7230c9293a49d8d1b36e33d7eab1a6bfede`
- `results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_2e-4_lora_dseed11/trajectory/update-00000000/eval.json`: `3fc87de4bb4cbaef88025647fa18a73da55f6d92ae4c823f77b8798f7dcc7091`
- `results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_2e-4_lora_dseed11/trajectory/update-00000008/eval.json`: `e1430b4c1349fc4311c8cfb1e8ce81a4dd7d18299ae2022618a32134cadfa570`
- `results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_5e-5_lora_dseed11/trajectory/update-00000000/eval.json`: `4737fdc8c8e8eeb8eb48a25275e3d9571a1a8fd19c7097946ee8e38b344dc08d`
- `results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_5e-5_lora_dseed11/trajectory/update-00000008/eval.json`: `a0a1cc68da5bc2b2546bd532db728759ef159043289c69f241133679dbafc687`

## Plotted records

```json
[
  {
    "student": "gemma3-1b",
    "capability": "math",
    "learning_rate": 5e-05,
    "delta": -0.0035422033641461237,
    "updates": 8,
    "processed_tokens": 37903,
    "delta_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_5e-5_lora_dseed11/trajectory/update-00000008/eval.json#/delta/math",
    "learning_rate_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_5e-5_lora_dseed11/trajectory/update-00000008/eval.json#/output_suffix",
    "updates_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_5e-5_lora_dseed11/trajectory/update-00000008/eval.json#/updates",
    "processed_tokens_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_5e-5_lora_dseed11/trajectory/update-00000008/eval.json#/processed_tokens"
  },
  {
    "student": "gemma3-1b",
    "capability": "code",
    "learning_rate": 5e-05,
    "delta": -0.001771479185119551,
    "updates": 8,
    "processed_tokens": 37903,
    "delta_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_5e-5_lora_dseed11/trajectory/update-00000008/eval.json#/delta/code",
    "learning_rate_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_5e-5_lora_dseed11/trajectory/update-00000008/eval.json#/output_suffix",
    "updates_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_5e-5_lora_dseed11/trajectory/update-00000008/eval.json#/updates",
    "processed_tokens_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_5e-5_lora_dseed11/trajectory/update-00000008/eval.json#/processed_tokens"
  },
  {
    "student": "gemma3-1b",
    "capability": "qa",
    "learning_rate": 5e-05,
    "delta": -0.1914529382470116,
    "updates": 8,
    "processed_tokens": 37903,
    "delta_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_5e-5_lora_dseed11/trajectory/update-00000008/eval.json#/delta/qa",
    "learning_rate_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_5e-5_lora_dseed11/trajectory/update-00000008/eval.json#/output_suffix",
    "updates_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_5e-5_lora_dseed11/trajectory/update-00000008/eval.json#/updates",
    "processed_tokens_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_5e-5_lora_dseed11/trajectory/update-00000008/eval.json#/processed_tokens"
  },
  {
    "student": "gemma3-1b",
    "capability": "math",
    "learning_rate": 0.0001,
    "delta": -0.003674799212001867,
    "updates": 8,
    "processed_tokens": 37903,
    "delta_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_1e-4_lora_dseed11/trajectory/update-00000008/eval.json#/delta/math",
    "learning_rate_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_1e-4_lora_dseed11/trajectory/update-00000008/eval.json#/output_suffix",
    "updates_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_1e-4_lora_dseed11/trajectory/update-00000008/eval.json#/updates",
    "processed_tokens_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_1e-4_lora_dseed11/trajectory/update-00000008/eval.json#/processed_tokens"
  },
  {
    "student": "gemma3-1b",
    "capability": "code",
    "learning_rate": 0.0001,
    "delta": -0.002297387068201928,
    "updates": 8,
    "processed_tokens": 37903,
    "delta_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_1e-4_lora_dseed11/trajectory/update-00000008/eval.json#/delta/code",
    "learning_rate_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_1e-4_lora_dseed11/trajectory/update-00000008/eval.json#/output_suffix",
    "updates_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_1e-4_lora_dseed11/trajectory/update-00000008/eval.json#/updates",
    "processed_tokens_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_1e-4_lora_dseed11/trajectory/update-00000008/eval.json#/processed_tokens"
  },
  {
    "student": "gemma3-1b",
    "capability": "qa",
    "learning_rate": 0.0001,
    "delta": -0.48384586653386474,
    "updates": 8,
    "processed_tokens": 37903,
    "delta_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_1e-4_lora_dseed11/trajectory/update-00000008/eval.json#/delta/qa",
    "learning_rate_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_1e-4_lora_dseed11/trajectory/update-00000008/eval.json#/output_suffix",
    "updates_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_1e-4_lora_dseed11/trajectory/update-00000008/eval.json#/updates",
    "processed_tokens_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_1e-4_lora_dseed11/trajectory/update-00000008/eval.json#/processed_tokens"
  },
  {
    "student": "gemma3-1b",
    "capability": "math",
    "learning_rate": 0.0002,
    "delta": 0.020609183209577164,
    "updates": 8,
    "processed_tokens": 37903,
    "delta_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_2e-4_lora_dseed11/trajectory/update-00000008/eval.json#/delta/math",
    "learning_rate_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_2e-4_lora_dseed11/trajectory/update-00000008/eval.json#/output_suffix",
    "updates_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_2e-4_lora_dseed11/trajectory/update-00000008/eval.json#/updates",
    "processed_tokens_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_2e-4_lora_dseed11/trajectory/update-00000008/eval.json#/processed_tokens"
  },
  {
    "student": "gemma3-1b",
    "capability": "code",
    "learning_rate": 0.0002,
    "delta": 0.009078830823737727,
    "updates": 8,
    "processed_tokens": 37903,
    "delta_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_2e-4_lora_dseed11/trajectory/update-00000008/eval.json#/delta/code",
    "learning_rate_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_2e-4_lora_dseed11/trajectory/update-00000008/eval.json#/output_suffix",
    "updates_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_2e-4_lora_dseed11/trajectory/update-00000008/eval.json#/updates",
    "processed_tokens_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_2e-4_lora_dseed11/trajectory/update-00000008/eval.json#/processed_tokens"
  },
  {
    "student": "gemma3-1b",
    "capability": "qa",
    "learning_rate": 0.0002,
    "delta": -1.0593874501992033,
    "updates": 8,
    "processed_tokens": 37903,
    "delta_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_2e-4_lora_dseed11/trajectory/update-00000008/eval.json#/delta/qa",
    "learning_rate_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_2e-4_lora_dseed11/trajectory/update-00000008/eval.json#/output_suffix",
    "updates_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_2e-4_lora_dseed11/trajectory/update-00000008/eval.json#/updates",
    "processed_tokens_source": "results/v12-distill/gemma3-1b/gpt-5.6-luna_full_75_lrpilot_2e-4_lora_dseed11/trajectory/update-00000008/eval.json#/processed_tokens"
  },
  {
    "student": "gemma3-4b",
    "capability": "math",
    "learning_rate": 5e-05,
    "delta": 0.0009092286710107311,
    "updates": 8,
    "processed_tokens": 37903,
    "delta_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_5e-5_lora_dseed11/trajectory/update-00000008/eval.json#/delta/math",
    "learning_rate_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_5e-5_lora_dseed11/trajectory/update-00000008/eval.json#/output_suffix",
    "updates_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_5e-5_lora_dseed11/trajectory/update-00000008/eval.json#/updates",
    "processed_tokens_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_5e-5_lora_dseed11/trajectory/update-00000008/eval.json#/processed_tokens"
  },
  {
    "student": "gemma3-4b",
    "capability": "code",
    "learning_rate": 5e-05,
    "delta": -0.002989371124889284,
    "updates": 8,
    "processed_tokens": 37903,
    "delta_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_5e-5_lora_dseed11/trajectory/update-00000008/eval.json#/delta/code",
    "learning_rate_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_5e-5_lora_dseed11/trajectory/update-00000008/eval.json#/output_suffix",
    "updates_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_5e-5_lora_dseed11/trajectory/update-00000008/eval.json#/updates",
    "processed_tokens_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_5e-5_lora_dseed11/trajectory/update-00000008/eval.json#/processed_tokens"
  },
  {
    "student": "gemma3-4b",
    "capability": "qa",
    "learning_rate": 5e-05,
    "delta": -0.2501245019920315,
    "updates": 8,
    "processed_tokens": 37903,
    "delta_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_5e-5_lora_dseed11/trajectory/update-00000008/eval.json#/delta/qa",
    "learning_rate_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_5e-5_lora_dseed11/trajectory/update-00000008/eval.json#/output_suffix",
    "updates_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_5e-5_lora_dseed11/trajectory/update-00000008/eval.json#/updates",
    "processed_tokens_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_5e-5_lora_dseed11/trajectory/update-00000008/eval.json#/processed_tokens"
  },
  {
    "student": "gemma3-4b",
    "capability": "math",
    "learning_rate": 0.0001,
    "delta": 0.012085164418851324,
    "updates": 8,
    "processed_tokens": 37903,
    "delta_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_1e-4_lora_dseed11/trajectory/update-00000008/eval.json#/delta/math",
    "learning_rate_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_1e-4_lora_dseed11/trajectory/update-00000008/eval.json#/output_suffix",
    "updates_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_1e-4_lora_dseed11/trajectory/update-00000008/eval.json#/updates",
    "processed_tokens_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_1e-4_lora_dseed11/trajectory/update-00000008/eval.json#/processed_tokens"
  },
  {
    "student": "gemma3-4b",
    "capability": "code",
    "learning_rate": 0.0001,
    "delta": -0.0034322409211692273,
    "updates": 8,
    "processed_tokens": 37903,
    "delta_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_1e-4_lora_dseed11/trajectory/update-00000008/eval.json#/delta/code",
    "learning_rate_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_1e-4_lora_dseed11/trajectory/update-00000008/eval.json#/output_suffix",
    "updates_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_1e-4_lora_dseed11/trajectory/update-00000008/eval.json#/updates",
    "processed_tokens_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_1e-4_lora_dseed11/trajectory/update-00000008/eval.json#/processed_tokens"
  },
  {
    "student": "gemma3-4b",
    "capability": "qa",
    "learning_rate": 0.0001,
    "delta": -0.6650273904382464,
    "updates": 8,
    "processed_tokens": 37903,
    "delta_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_1e-4_lora_dseed11/trajectory/update-00000008/eval.json#/delta/qa",
    "learning_rate_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_1e-4_lora_dseed11/trajectory/update-00000008/eval.json#/output_suffix",
    "updates_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_1e-4_lora_dseed11/trajectory/update-00000008/eval.json#/updates",
    "processed_tokens_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_1e-4_lora_dseed11/trajectory/update-00000008/eval.json#/processed_tokens"
  },
  {
    "student": "gemma3-4b",
    "capability": "math",
    "learning_rate": 0.0002,
    "delta": 0.08773109562054848,
    "updates": 8,
    "processed_tokens": 37903,
    "delta_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_2e-4_lora_dseed11/trajectory/update-00000008/eval.json#/delta/math",
    "learning_rate_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_2e-4_lora_dseed11/trajectory/update-00000008/eval.json#/output_suffix",
    "updates_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_2e-4_lora_dseed11/trajectory/update-00000008/eval.json#/updates",
    "processed_tokens_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_2e-4_lora_dseed11/trajectory/update-00000008/eval.json#/processed_tokens"
  },
  {
    "student": "gemma3-4b",
    "capability": "code",
    "learning_rate": 0.0002,
    "delta": 0.030391939769707665,
    "updates": 8,
    "processed_tokens": 37903,
    "delta_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_2e-4_lora_dseed11/trajectory/update-00000008/eval.json#/delta/code",
    "learning_rate_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_2e-4_lora_dseed11/trajectory/update-00000008/eval.json#/output_suffix",
    "updates_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_2e-4_lora_dseed11/trajectory/update-00000008/eval.json#/updates",
    "processed_tokens_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_2e-4_lora_dseed11/trajectory/update-00000008/eval.json#/processed_tokens"
  },
  {
    "student": "gemma3-4b",
    "capability": "qa",
    "learning_rate": 0.0002,
    "delta": -1.3119397410358564,
    "updates": 8,
    "processed_tokens": 37903,
    "delta_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_2e-4_lora_dseed11/trajectory/update-00000008/eval.json#/delta/qa",
    "learning_rate_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_2e-4_lora_dseed11/trajectory/update-00000008/eval.json#/output_suffix",
    "updates_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_2e-4_lora_dseed11/trajectory/update-00000008/eval.json#/updates",
    "processed_tokens_source": "results/v12-distill/gemma3-4b/gpt-5.6-luna_full_75_lrpilot_2e-4_lora_dseed11/trajectory/update-00000008/eval.json#/processed_tokens"
  }
]
```
