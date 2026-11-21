## 2026-11-21 - slake_qwen3vl4b_zs_alist_img10s42
- mode zeroshot, dataset slake, model Qwen/Qwen3-VL-4B-Instruct
- 0 training images / 0 questions, 0 epochs, lr 0.0002, seed 42; train 0.0 min, peak 0.0 GB
- test (n=1061): overall exact 0.64 [0.6141, 0.6654], closed 0.8077, open 0.5318; relaxed overall 0.656
- yes/no: {'n_yesno': 355, 'truth_yes': 0.493, 'acc_firstword': 0.8282, 'says_yes': 0.479, 'acc_when_yes': 0.811, 'acc_when_no': 0.844, 'plain_yes_no': 1.0}
- env: python=3.13.16;torch=2.11.0+cu130;transformers=5.19.0;peft=0.21.2;accelerate=1.15.0;qwen-vl-utils=0.0.8;datasets=5.1.0;huggingface_hub=1.33.0;pillow=10.4.0;numpy=2.1.3
