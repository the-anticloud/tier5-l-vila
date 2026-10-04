# HF_Leaderboard_Lab_Results

**Project:** `L_VILA`  
**Tier:** `TIER_5_WORLD_NEURO_EMBODIED`  
**Slug:** `haotian-liu/LLaVA`  
**Commit:** `c121f0432da2`  
**Run:** `2026-09-30T15:07:07.146295+00:00`  

## Isolation Environment

| Field | Value |
| ----- | ----- |
| Platform | `win32` |
| Python | `3.12.10` |
| HF model | `distilbert-base-uncased` |
| HF load time | `4.42s` |
| Inference device | `cpu` |

## Results

**Framework:** [HuggingFace Open LLM Leaderboard (proxy via distilbert-base-uncased)](https://huggingface.co/docs/leaderboards/en/open_llm_leaderboard/archive)

**Model used:** `distilbert-base-uncased`

### Inference Latency (Classification)

| Metric | Value |
| ------ | ----- |
| Avg latency | **48.47 ms** |
| Min latency | 44.73 ms |
| Max latency | 51.03 ms |
| Samples | 5 |

### Real Tokenization Results

| Field | Value |
| ----- | ----- |
| Token count | **38** |
| Tokenization latency | 1.0 ms |
| Classification label | `LABEL_0` |
| Classification score | 0.5878 |
| Classification latency | 134.32 ms |
| Status | **PASS** |

**Input text tokenized:**
```
L_VILA (haotian-liu/LLaVA) — 175 files, 9428 source lines, licence Apache-2.0, primary language ['Python']
```

**First 20 tokens:**
```
['[CLS]', 'l', '_', 'vila', '(', 'ha', '##ot', '##ian', '-', 'liu', '/', 'll', '##ava', ')', '—', '175', 'files', ',', '94', '##28']
```

> Full MMLU/HellaSwag/TruthfulQA/ARC/Winogrande/GSM8K require dedicated GPU.
> These results are CPU inference proxy metrics using distilbert-base-uncased.

---
_Anticloud Benchmark Suite — isolation log — 2026-09-30T15:07:07.146295+00:00_