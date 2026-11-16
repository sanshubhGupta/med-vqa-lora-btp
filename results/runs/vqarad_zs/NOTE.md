## 2026-11-16 - vqarad_zs
- mode zeroshot, dataset vqarad, model Qwen/Qwen2.5-VL-3B-Instruct
- 0 training images / 0 questions, 0 epochs, lr 0.0002, seed 42; train 0.0 min, peak 0.0 GB
- test (n=451): overall exact 0.4856 [0.4316, 0.5372], closed 0.6853, open 0.235; relaxed overall 0.5144
- yes/no: {'n_yesno': 251, 'truth_yes': 0.47, 'acc_firstword': 0.7052, 'says_yes': 0.645, 'acc_when_yes': 0.873, 'acc_when_no': 0.556, 'plain_yes_no': 0.972}
- env: python=3.13.16;torch=2.11.0+cu130;transformers=5.19.0;peft=0.21.2;accelerate=1.15.0;qwen-vl-utils=0.0.8;datasets=5.1.0;huggingface_hub=1.33.0;pillow=10.4.0;numpy=2.1.3
