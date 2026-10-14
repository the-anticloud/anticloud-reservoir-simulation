# Educators — RESERVOIR_SIMULATION

**Project:** RESERVOIR_SIMULATION  
**Category:** OIL_GAS  
**Upstream:** https://github.com/yohanesnuwara/reservoir-simulation  
**Pinned commit:** `eb2bcb7cef9ed23e1d5104b12d3ce1f5c8f114b5`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `4f718dfeb7771a84e9136386a35c5a9dbe149f3b2f2b70fe7b3b92879d8a16dc`  
**Date:** October 2026

## Teaching with RESERVOIR_SIMULATION

The project is usable as a worked example of offline-first packaging with a
cryptographic audit chain. It ships with the assurance suite, the evidence
register and the ledger, so students can verify claims rather than take them on
faith.

## Suggested exercises

1. Run `python tools/run_bench.py --out BENCH.json` and read the 16 results.
2. Recompute the SHA3-256 of a row's evidence file and compare to the register.
3. Walk the AIOSS chain from genesis to head `4f718dfeb7771a84e9136386a35c5a9dbe149f3b2f2b70fe7b3b92879d8a16dc` and confirm every link.
4. Break one artifact and observe the chain fail to verify.

## Licence for teaching

Apache 2.0 terms apply to academic and teaching use. See `24_ANTICOMMONS_LICENSE`.
