## 2026-11-20 - slake_qwen3vl4b_img10_s42
- mode train, dataset slake, model Qwen/Qwen3-VL-4B-Instruct
- 45 training images / 502 questions, 3 epochs, lr 0.0002, seed 42; train 251.0 min, peak 5.7 GB
- test (n=1061): overall exact 0.7295 [0.7065, 0.7523], closed 0.8293, open 0.6651; relaxed overall 0.7446
- yes/no: {'n_yesno': 355, 'truth_yes': 0.493, 'acc_firstword': 0.8394, 'says_yes': 0.451, 'acc_when_yes': 0.794, 'acc_when_no': 0.883, 'plain_yes_no': 1.0}
- env: python=3.13.16;torch=2.11.0+cu130;transformers=5.19.0;peft=0.21.2;accelerate=1.15.0;qwen-vl-utils=0.0.8;datasets=5.1.0;huggingface_hub=1.33.0;pillow=10.4.0;numpy=2.1.3
