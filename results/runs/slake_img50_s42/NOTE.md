## 2026-11-20 - slake_img50_s42
- mode train, dataset slake, model Qwen/Qwen2.5-VL-3B-Instruct
- 225 training images / 2442 questions, 3 epochs, lr 0.0002, seed 42; train 483.2 min, peak 5.0 GB
- test (n=1061): overall exact 0.738 [0.7128, 0.7624], closed 0.8149, open 0.6884; relaxed overall 0.7512
- yes/no: {'n_yesno': 355, 'truth_yes': 0.493, 'acc_firstword': 0.8423, 'says_yes': 0.487, 'acc_when_yes': 0.834, 'acc_when_no': 0.85, 'plain_yes_no': 1.0}
- env: python=3.13.16;torch=2.11.0+cu130;transformers=5.19.0;peft=0.21.2;accelerate=1.15.0;qwen-vl-utils=0.0.8;datasets=5.1.0;huggingface_hub=1.33.0;pillow=10.4.0;numpy=2.1.3
