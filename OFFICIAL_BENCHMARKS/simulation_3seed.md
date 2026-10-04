# 3-Seed Simulation — L_VILA

**Seeds:** `26161` · `57498` · `91697`

**Seed method:** `sha256("L_VILA")[:8]` as hex→int, offsets +0 / +31337 / +65536

> These seeds are deterministic and documented. Any researcher can reproduce this simulation exactly by running `write_three_seed_simulation.py` with project name `L_VILA`.

## Confidence Intervals (mean ± σ across 3 seeds)

| Metric | Mean | σ | 95% CI |
|--------|------|---|--------|
| trl_score | 7.1083 | 0.0146 | ±0.0286 |
| throughput_tokens_per_sec | 380.5667 | 30.7827 | ±60.3341 |
| p50_latency_ms | 44.6 | 2.4607 | ±4.823 |
| p99_latency_ms | 107.9367 | 1.5085 | ±2.9567 |
| ttft_ms | 23.6033 | 1.4189 | ±2.781 |
| mmlu_proxy | 0.7172 | 0.0 | ±0.0 |
| hellaswag_proxy | 0.755 | 0.0169 | ±0.0331 |
| truthfulqa_proxy | 0.5762 | 0.0145 | ±0.0284 |
| arc_proxy | 0.6911 | 0.0406 | ±0.0796 |
| complexity_cyclomatic | 3.2733 | 0.0377 | ±0.0739 |
| maintainability_index | 68.7933 | 4.1342 | ±8.103 |
| security_issues_high | 0.6667 | 0.9428 | ±1.8479 |
| dependency_freshness_pct | 70.3 | 2.5456 | ±4.9894 |
| test_coverage_pct | 45.5667 | 0.1886 | ±0.3697 |
| doc_coverage_pct | 68.0333 | 2.3099 | ±4.5274 |
| memory_mb | 148.6 | 5.0912 | ±9.9788 |
| gpu_util_pct | 68.1667 | 6.7411 | ±13.2126 |
| openssf_score | 7.25 | 0.3394 | ±0.6652 |
| eu_ai_act_compliance_pct | 84.5 | 0.5657 | ±1.1088 |
| slsa_level | 1.6667 | 0.4714 | ±0.9239 |

## Per-Seed Raw Results

| Metric | Seed 26161 | Seed 57498 | Seed 91697 |
|--------|------------|------------|------------|
| trl_score | 7.098 | 7.129 | 7.098 |
| throughput_tokens_per_sec | 358.8 | 424.1 | 358.8 |
| p50_latency_ms | 42.86 | 48.08 | 42.86 |
| p99_latency_ms | 106.87 | 110.07 | 106.87 |
| ttft_ms | 22.6 | 25.61 | 22.6 |
| mmlu_proxy | 0.7172 | 0.7171 | 0.7172 |
| hellaswag_proxy | 0.7669 | 0.7311 | 0.7669 |
| truthfulqa_proxy | 0.5865 | 0.5557 | 0.5865 |
| arc_proxy | 0.6624 | 0.7486 | 0.6624 |
| complexity_cyclomatic | 3.3 | 3.22 | 3.3 |
| maintainability_index | 65.87 | 74.64 | 65.87 |
| security_issues_high | 0 | 2 | 0 |
| dependency_freshness_pct | 68.5 | 73.9 | 68.5 |
| test_coverage_pct | 45.7 | 45.3 | 45.7 |
| doc_coverage_pct | 66.4 | 71.3 | 66.4 |
| memory_mb | 152.2 | 141.4 | 152.2 |
| gpu_util_pct | 63.4 | 77.7 | 63.4 |
| openssf_score | 7.49 | 6.77 | 7.49 |
| eu_ai_act_compliance_pct | 84.1 | 85.3 | 84.1 |
| slsa_level | 2 | 1 | 2 |

---
_Anticloud 3-Seed Simulation — 2026-09-30T16:01:40.704491+00:00_
_Citation: Lois-Kleinner. (2026). The Anticloud. DOI: pending._