# VerilogEval

**Source:** GitHub [`NVlabs/verilog-eval`](https://github.com/NVlabs/verilog-eval)
- top level: `main` @ `c498220` (2025-02-07)
- `v1/`: branch `release/1.0.0` @ `4fa0ac4`

**Downloaded:** 2026-10-23, upstream `.git` removed

No train/test split — the whole set is the eval set.

**v2 (top level)**
- `dataset_spec-to-rtl` — 156 problems
- `dataset_code-complete-iccad2023` — 156 problems

one `ProbNNN_<name>_{prompt.txt, ref.sv, test.sv}` set per problem (plus `_ifc.txt` in code-complete).

**v1**
- `v1/data/VerilogEval_Human.jsonl` — 156 (`task_id`, `prompt`, `canonical_solution`, `test`)
- `v1/data/VerilogEval_Machine.jsonl` — 143
- `v1/descriptions/` — the matching natural-language descriptions

Running the tests needs **iverilog v12**.

**Removed from this snapshot** (build/run tooling, not data; blocked by a corporate pre-clone scan): `configure`, `configure.ac`, `Makefile.in`, `scripts/sv-generate`, `scripts/sv-iv-analyze`, `scripts/echo-progress`, `v1/Dockerfile`. Get them from upstream if you need to run the official harness.

---

Snapshot kept for benchmark work; see [chihyu-wang-tsmc/code-benchmarks](https://github.com/chihyu-wang-tsmc/code-benchmarks) for the full benchmark index. Licensing follows the upstream source.
