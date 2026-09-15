# fig1_legend: frozen sources

Reused a1_development_table.load_development_table (schema, cohort, metadata and hash checks). A1 CSV fields: run_id, checkpoint_id, student_id, pool_seed, U, T_actual, D_U_pool, capability, distribution, delta. Select positive T_actual nearest 200000 separately per trajectory/readout. reuse=T_actual/D_U_pool; y=delta (own-initial loss subtracted by A1). Both pool seeds remain separate points.
The four-rung core includes pool seeds 41/42 and, for the critical rung, 51/52. Seed markers identify the first/second registered seed within each rung; no seed averaging. Scope rows in the same CSV originate in v99-scope. All points, including 4B, are development.
Final checkpoint = maximum positive updates with positive processed_tokens. learning_rate = float(output_suffix after lrpilot_); delta used verbatim.
fig1_a.pdf: 1.8 x 1.15 in; bold Times New Roman; ticks 7.5 pt, axis labels 8.5 pt, legend 7.5 pt; default lines 1.1 pt, markers 3.8 pt; caps 2 pt. Full canvas retained; no titles, panel letters, or explanatory annotations.
fig1_b.pdf: 1.8 x 1.15 in; bold Times New Roman; ticks 7.5 pt, axis labels 8.5 pt, legend 7.5 pt; default lines 1.1 pt, markers 3.8 pt; caps 2 pt. Full canvas retained; no titles, panel letters, or explanatory annotations.
fig1_c.pdf: 1.8 x 1.15 in; bold Times New Roman; ticks 7.5 pt, axis labels 8.5 pt, legend 7.5 pt; default lines 1.1 pt, markers 3.8 pt; caps 2 pt. Full canvas retained; no titles, panel letters, or explanatory annotations.
fig1_legend.pdf: 5.5 x 0.42 in; bold Times New Roman; ticks 8.5 pt, axis labels 8.5 pt, legend 8.5 pt; default lines 1.1 pt, markers 3.8 pt; caps 2 pt. Full canvas retained; no titles, panel letters, or explanatory annotations.

## Inputs (SHA-256)

- `results/a1-development-table/development_table.csv`: `2f92035256201a99e853e90d95f47296b02799c9700d40bbca6525a9b33ab67e`
- `results/a1-development-table/row_metadata.csv`: `f3c974254c5bf857820c1eb2d7f922246bbd6ad9e1013c7ce11be3bf6ecc4947`
- `results/a1-development-table/summary.json`: `0531986629012bc9d348b23dadde0b577daf466cdc2805dc26138d9c86489c8b`
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
[]
```
