# Radon_Complexity_Lab_Results
**Project:** `L_VILA` | **Status:** `PASS` | **Run:** `2026-09-30T17:14:20.030944+00:00`

**Framework:** [Radon — Cyclomatic Complexity & Maintainability Index](https://radon.readthedocs.io/)

## Key Metrics

- **files_analyzed:** `10`
- **average_complexity:** `{'grade': 'A', 'score': 4.0227272727272725}`
- **complexity_grade:** `A`
- **complexity_score:** `4.0227272727272725`
- **mi_output:** `E:\fenta\Downloads\The Anticloud\TIER_5_WORLD_NEURO_EMBODIED\L_VILA\UPSTREAM\predict.py - A (52.64)
E:\fenta\Downloads\T`

## Raw Output (first 50 lines)
```
E:\fenta\Downloads\The Anticloud\TIER_5_WORLD_NEURO_EMBODIED\L_VILA\UPSTREAM\predict.py
    M 87:4 Predictor.predict - B (8)
    C 78:0 Predictor - B (6)
    F 62:0 download_weights - A (4)
    F 54:0 download_json - A (3)
    F 148:0 load_image - A (3)
    M 79:4 Predictor.setup - A (2)
E:\fenta\Downloads\The Anticloud\TIER_5_WORLD_NEURO_EMBODIED\L_VILA\UPSTREAM\llava\conversation.py
    M 32:4 Conversation.get_prompt - D (30)
    C 19:0 Conversation - B (8)
    M 112:4 Conversation.process_image - B (7)
    M 152:4 Conversation.get_images - A (4)
    M 162:4 Conversation.to_gradio_chatbot - A (4)
    M 191:4 Conversation.dict - A (4)
    M 180:4 Conversation.copy - A (2)
    C 9:0 SeparatorStyle - A (1)
    M 109:4 Conversation.append_message - A (1)
E:\fenta\Downloads\The Anticloud\TIER_5_WORLD_NEURO_EMBODIED\L_VILA\UPSTREAM\llava\mm_utils.py
    F 166:0 process_images - B (8)
    F 185:0 tokenizer_image_token - B (8)
    M 230:4 KeywordsStoppingCriteria.call_for_batch - B (6)
    F 12:0 select_best_resolution - A (5)
    C 215:0 KeywordsStoppingCriteria - A (5)
    M 216:4 KeywordsStoppingCriteria.__init__ - A (5)
    F 77:0 divide_to_patches - A (3)
    F 119:0 process_anyres_image - A (3)
    F 152:0 expand2square - A (3)
    F 42:0 resize_and_pad_image - A (2)
    F 99:0 get_anyres_image_grid_shape - A (2)
    F 207:0 get_model_name_from_path - A (2)
    M 243:4 KeywordsStoppingCriteria.__call__ - A (2)
    F 148:0 load_image_from_base64 - A (1)
E:\fenta\Downloads\The 
```

---
_Anticloud Independent Benchmark — 2026-09-30T17:14:20.030944+00:00_