# fig1_legend: frozen sources

Reused a1_development_table.load_development_table (schema, cohort, metadata and hash checks). A1 CSV fields: run_id, checkpoint_id, student_id, pool_seed, U, T_actual, D_U_pool, capability, distribution, delta. Select positive T_actual nearest 200000 separately per trajectory/readout. reuse=T_actual/D_U_pool; y=delta (own-initial loss subtracted by A1). Both pool seeds remain separate points.
The four-rung core includes pool seeds 41/42 and, for the critical rung, 51/52. Seed markers identify the first/second registered seed within each rung; no seed averaging. Scope rows in the same CSV originate in v99-scope. All points, including 4B, are development.
fig1_a.pdf: 2.7 x 1.8 in; bold Times New Roman; ticks 14 pt, axis labels 15 pt, legend 13 pt; lines 2 pt, markers 7 pt. Full canvas retained; no titles, panel letters, or explanatory annotations.
fig1_b.pdf: 2.7 x 1.8 in; bold Times New Roman; ticks 14 pt, axis labels 15 pt, legend 13 pt; lines 2 pt, markers 7 pt. Full canvas retained; no titles, panel letters, or explanatory annotations.
fig1_legend.pdf: 5.5 x 0.3 in; bold Times New Roman; ticks 14 pt, axis labels 15 pt, legend 13 pt; lines 2 pt, markers 7 pt. Full canvas retained; no titles, panel letters, or explanatory annotations.

## Inputs (SHA-256)

- `results/a1-development-table/development_table.csv`: `2f92035256201a99e853e90d95f47296b02799c9700d40bbca6525a9b33ab67e`
- `results/a1-development-table/row_metadata.csv`: `f3c974254c5bf857820c1eb2d7f922246bbd6ad9e1013c7ce11be3bf6ecc4947`
- `results/a1-development-table/summary.json`: `0531986629012bc9d348b23dadde0b577daf466cdc2805dc26138d9c86489c8b`

## Plotted records

```json
[]
```
