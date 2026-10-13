
## 2026-10-11 - WP3 counterfactual image conditions (n=1061, full)
- Setup: Qwen2.5-VL-3B-Instruct, LoRA 10% adapter (sanshubhguptaa/med-vqa-qwen2.5-vl-slake); real vs blank gray vs shuffled-other-image vs no-image; exact match with image-clustered 95% CI.
- Overall exact: base real 0.548 [0.517, 0.577] | base blank 0.177 [0.149, 0.205] | lora real 0.671 [0.642, 0.698] | lora blank 0.280 [0.257, 0.301]
- Gain decomposition (overall): total 0.123 [0.097, 0.150] | gain with blank image 0.103 [0.077, 0.128] | change in visual benefit 0.021 [-0.014, 0.054]
- Image sensitivity (answer changes when image blanked): base 0.789 [0.759, 0.818] | lora 0.690 [0.667, 0.713]
- Files: results/wp3_full/*.csv, wp3_counterfactuals.png

## 2026-10-12 - slake_img10_s42
- 45 training images / 502 questions, 3 epochs, lr 0.0002, seed 42; train 95.8 min, peak 5.0 GB
- test (n=1061): overall 0.6758 [0.6495, 0.7011], closed 0.8005, open 0.5953

## 2026-10-12 - slake_img5_s42
- 22 training images / 251 questions, 3 epochs, lr 0.0002, seed 42; train 49.9 min, peak 5.0 GB
- test (n=1061): overall 0.6409 [0.6115, 0.6685], closed 0.7861, open 0.5473

## 2026-10-13 - slake_img10_s123
- 45 training images / 519 questions, 3 epochs, lr 0.0002, seed 123; train 106.6 min, peak 5.0 GB
- test (n=1061): overall 0.6739 [0.6437, 0.7021], closed 0.7981, open 0.5938

## 2026-10-13 - slake_img10_s2024
- 45 training images / 472 questions, 3 epochs, lr 0.0002, seed 2024; train 96.3 min, peak 5.0 GB
- test (n=1061): overall 0.6739 [0.6449, 0.7006], closed 0.7788, open 0.6062

## 2026-10-13 - slake_img25_s42
- 112 training images / 1232 questions, 3 epochs, lr 0.0002, seed 42; train 246.1 min, peak 5.0 GB
- test (n=1061): overall 0.7069 [0.6788, 0.7348], closed 0.7909, open 0.6527
