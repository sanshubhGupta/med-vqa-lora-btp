## 2026-11-27 - slake_rexp4_s42
- mode train, dataset slake, model Qwen/Qwen2.5-VL-3B-Instruct
- 316 training images / 510 questions, 3 epochs, lr 0.0002, seed 42; train 103.7 min, peak 5.0 GB
- test (n=1061): overall exact 0.6343 [0.6076, 0.6585], closed 0.7933, open 0.5318; relaxed overall 0.6598
- yes/no: {'n_yesno': 355, 'truth_yes': 0.493, 'acc_firstword': 0.8169, 'says_yes': 0.468, 'acc_when_yes': 0.789, 'acc_when_no': 0.844, 'plain_yes_no': 1.0}
- env: python=3.13.16;torch=2.11.0+cu130;transformers=5.19.0;peft=0.21.2;accelerate=1.15.0;qwen-vl-utils=0.0.8;datasets=5.1.0;huggingface_hub=1.33.0;pillow=10.4.0;numpy=2.1.3
