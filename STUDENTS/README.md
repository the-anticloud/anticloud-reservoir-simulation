# Students — RESERVOIR_SIMULATION

**Project:** RESERVOIR_SIMULATION  
**Category:** OIL_GAS  
**Upstream:** https://github.com/yohanesnuwara/reservoir-simulation  
**Pinned commit:** `eb2bcb7cef9ed23e1d5104b12d3ce1f5c8f114b5`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `4f718dfeb7771a84e9136386a35c5a9dbe149f3b2f2b70fe7b3b92879d8a16dc`  
**Date:** October 2026

## What this project gives you

A complete worked example of offline-first packaging with a cryptographic audit
chain: source pinned at `eb2bcb7cef9ed23e1d5104b12d3ce1f5c8f114b5`, a 16-check assurance suite, an evidence register
with per-check hashes, and an AIOSS ledger chain ending at `4f718dfeb7771a84e9136386a35c5a9dbe149f3b2f2b70fe7b3b92879d8a16dc`.

## Learn by verifying

```
python tools/run_bench.py --out BENCH.json
```

Then take any row from `ISOLATED_LAB_RESULTS/03_Result_Register.md`, recompute
the SHA3-256 of its evidence file, and confirm it matches. If it does not match,
the record has been altered — that is the whole point of the chain.

## Licence

Apache 2.0 terms apply to study and teaching use.
