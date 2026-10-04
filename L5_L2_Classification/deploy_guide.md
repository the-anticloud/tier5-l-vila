# Deploy Guide — L_VILA
**Tier:** TIER_5_WORLD_NEURO_EMBODIED | **Stack:** Python 3.11, PyTorch 2.10+, VILA architecture, PAX 27B, AIOSS_FORMAT
**Air-gap capable after initial setup.**

## Prerequisites
Python 3.11+, PyTorch 2.10+, VILA weights per domain, T4 GPU.

## Environment
T4 GPU. VILA domain weights: ~7GB VRAM. Compatible with PAX 27B on same T4 with quantization.

## AIOSS Integration
```bash
aioss init --module L_VILA --output ./l_vila.aioss
aioss append --chain ./l_vila.aioss --payload ./output.bin --module L_VILA
aioss verify --chain ./l_vila.aioss
```

## Air-Gap Setup
```bash
pip download -r requirements.txt -d ./wheels/
pip install --no-index --find-links ./wheels/ -r requirements.txt
```

## PAX 27B Harness Wiring
```python
from anticloud_pax import PAXHarness
harness = PAXHarness(
    model_path="./pax-27b-q4.gguf",
    module="L_VILA",
    aioss_chain="./L_VILA.aioss",
    classification="L5_NARROW_L2_GENERAL"
)
result = harness.process(input_data)
```

## Verification
```bash
aioss verify --chain ./L_VILA.aioss --verbose
python -m L_VILA.tests.smoke
```
