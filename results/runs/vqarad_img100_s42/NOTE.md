## 2026-11-20 - vqarad_img100_s42
- mode train, dataset vqarad, model Qwen/Qwen2.5-VL-3B-Instruct
- 313 training images / 1793 questions, 3 epochs, lr 0.0002, seed 42; train 413.6 min, peak 5.0 GB
- test (n=451): overall exact 0.5787 [0.5267, 0.6291], closed 0.7928, open 0.31; relaxed overall 0.5876
- yes/no: {'n_yesno': 251, 'truth_yes': 0.47, 'acc_firstword': 0.7928, 'says_yes': 0.454, 'acc_when_yes': 0.763, 'acc_when_no': 0.82, 'plain_yes_no': 0.996}
- env: python=3.13.16;torch=2.11.0+cu130;transformers=5.19.0;peft=0.21.2;accelerate=1.15.0;qwen-vl-utils=0.0.8;datasets=5.1.0;huggingface_hub=1.33.0;pillow=10.4.0;numpy=2.1.3
