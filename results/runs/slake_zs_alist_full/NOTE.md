## 2026-11-21 - slake_zs_alist_full
- mode zeroshot, dataset slake, model Qwen/Qwen2.5-VL-3B-Instruct
- 0 training images / 0 questions, 0 epochs, lr 0.0002, seed 42; train 0.0 min, peak 0.0 GB
- test (n=1061): overall exact 0.5825 [0.5542, 0.6091], closed 0.7308, open 0.4868; relaxed overall 0.6239
- yes/no: {'n_yesno': 355, 'truth_yes': 0.493, 'acc_firstword': 0.7662, 'says_yes': 0.625, 'acc_when_yes': 0.897, 'acc_when_no': 0.639, 'plain_yes_no': 0.992}
- env: python=3.13.16;torch=2.11.0+cu130;transformers=5.19.0;peft=0.21.2;accelerate=1.15.0;qwen-vl-utils=0.0.8;datasets=5.1.0;huggingface_hub=1.33.0;pillow=10.4.0;numpy=2.1.3
