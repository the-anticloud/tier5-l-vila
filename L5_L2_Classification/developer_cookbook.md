# Developer Cookbook — L_VILA
**Stack:** Python 3.11, PyTorch 2.10+, VILA architecture, PAX 27B, AIOSS_FORMAT
**Domain:** VILA: visual language model adaptation for domain-specific Anticloud multi-modal AI

## Medical image analysis
```python
from l_vila import VILAAnalyzer

analyzer = VILAAnalyzer(
    vila_model="./vila_medical_7b.safetensors",
    pax_model="./pax-27b-q4.gguf",
    domain="medical",
    aioss_chain="./vila.aioss"
)

result = analyzer.analyze(
    image="./chest_xray.png",
    query="Identify any consolidation or effusion in this chest X-ray"
)
print(result.findings)
print(f"Confidence: {result.confidence:.2f}")
print(f"HIPAA audit chain: {result.chain_hash}")
```

## Robot scene understanding
```python
scene_analyzer = VILAAnalyzer(vila_model="./vila_robotics_7b.safetensors", domain="robotics")
objects = scene_analyzer.detect_objects(robot_frame, "List all objects and their positions")
```

## AIOSS Chain Append
```python
import hashlib, time

def aioss_append(chain_path, payload: bytes, module_id: str):
    entry_hash = hashlib.sha3_256(payload).digest()
    ts = int(time.time_ns()).to_bytes(8, 'big')
    with open(chain_path, 'rb') as f:
        f.seek(-32, 2); prev_hash = f.read(32)
    new_hash = hashlib.sha3_256(prev_hash + entry_hash + ts).digest()
    with open(chain_path, 'ab') as f:
        f.write(ts + entry_hash + new_hash)
    return new_hash.hex()
```
