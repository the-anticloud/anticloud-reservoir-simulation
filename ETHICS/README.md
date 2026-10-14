# Ethics — RESERVOIR_SIMULATION

**Project:** RESERVOIR_SIMULATION  
**Category:** OIL_GAS  
**Upstream:** https://github.com/yohanesnuwara/reservoir-simulation  
**Pinned commit:** `eb2bcb7cef9ed23e1d5104b12d3ce1f5c8f114b5`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `4f718dfeb7771a84e9136386a35c5a9dbe149f3b2f2b70fe7b3b92879d8a16dc`  
**Date:** October 2026

## Position

RESERVOIR_SIMULATION is packaged for offline deployment with a verifiable audit trail. The
ethical questions this raises are answered by making the system's behaviour
checkable rather than by policy statements.

## The four commitments

1. **No hidden egress.** The deployment has no external API dependency; this is
   testable by running it with the network disconnected.
2. **Attributable output.** Every artifact is recorded in a hash chain, so what
   the system produced can be reconstructed.
3. **Operator control.** The institution owns the hardware and the keys.
4. **Refusal to overclaim.** Where a certification is not held, the project says
   so rather than implying it.

## Dual use

This project is packaged for civilian and public-sector deployment. Where an
upstream has dual-use characteristics, the licence gate and the reference-only
marking in `BENCH.json` record that.
