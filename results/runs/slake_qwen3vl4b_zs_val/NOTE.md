## 2026-11-27 - slake_qwen3vl4b_zs_val
- mode zeroshot, dataset slake, model Qwen/Qwen3-VL-4B-Instruct
- 0 training images / 0 questions, 0 epochs, lr 0.0002, seed 42; train 0.0 min, peak 0.0 GB
- test (n=1053): overall exact 0.5489 [0.5179, 0.5792], closed 0.7796, open 0.3946; relaxed overall 0.5783
- yes/no: {'n_yesno': 358, 'truth_yes': 0.508, 'acc_firstword': 0.7989, 'says_yes': 0.536, 'acc_when_yes': 0.83, 'acc_when_no': 0.767, 'plain_yes_no': 1.0}
- env: python=3.13.16;torch=2.11.0+cu130;transformers=5.19.0;peft=0.21.2;accelerate=1.15.0;qwen-vl-utils=0.0.8;datasets=5.1.0;huggingface_hub=1.33.0;pillow=10.4.0;numpy=2.1.3
