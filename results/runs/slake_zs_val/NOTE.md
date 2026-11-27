## 2026-11-27 - slake_zs_val
- mode zeroshot, dataset slake, model Qwen/Qwen2.5-VL-3B-Instruct
- 0 training images / 0 questions, 0 epochs, lr 0.0002, seed 42; train 0.0 min, peak 0.0 GB
- test (n=1053): overall exact 0.5736 [0.5426, 0.6055], closed 0.7607, open 0.4485; relaxed overall 0.5935
- yes/no: {'n_yesno': 358, 'truth_yes': 0.508, 'acc_firstword': 0.7905, 'says_yes': 0.617, 'acc_when_yes': 0.901, 'acc_when_no': 0.676, 'plain_yes_no': 0.994}
- env: python=3.13.16;torch=2.11.0+cu130;transformers=5.19.0;peft=0.21.2;accelerate=1.15.0;qwen-vl-utils=0.0.8;datasets=5.1.0;huggingface_hub=1.33.0;pillow=10.4.0;numpy=2.1.3
