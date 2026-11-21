## 2026-11-21 - slake_covlow10_s123
- mode train, dataset slake, model Qwen/Qwen2.5-VL-3B-Instruct
- 47 training images / 494 questions, 3 epochs, lr 0.0002, seed 123; train 97.4 min, peak 5.0 GB
- test (n=1061): overall exact 0.6352 [0.6025, 0.6664], closed 0.7692, open 0.5488; relaxed overall 0.64
- yes/no: {'n_yesno': 355, 'truth_yes': 0.493, 'acc_firstword': 0.7915, 'says_yes': 0.437, 'acc_when_yes': 0.731, 'acc_when_no': 0.85, 'plain_yes_no': 1.0}
- env: python=3.13.16;torch=2.11.0+cu130;transformers=5.19.0;peft=0.21.2;accelerate=1.15.0;qwen-vl-utils=0.0.8;datasets=5.1.0;huggingface_hub=1.33.0;pillow=10.4.0;numpy=2.1.3
