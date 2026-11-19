## 2026-11-19 - counterfactual images, wp3b_vqarad_clean_img100_s42 (dataset vqarad, model Qwen/Qwen2.5-VL-3B-Instruct, n=451)
- overall accuracy (yes/no by first word): base_real 0.497 [0.443, 0.548] | base_shuffled 0.395 [0.344, 0.444] | base_blank 0.310 [0.258, 0.364] | base_noimage 0.306 [0.254, 0.360] | lora_real 0.552 [0.497, 0.606] | lora_shuffled 0.410 [0.357, 0.463] | lora_blank 0.368 [0.315, 0.419] | lora_noimage 0.335 [0.284, 0.384]
- overall: total gain +0.055 [+0.011, +0.100] | gain with blank image +0.058 [+0.007, +0.107] | benefit change vs other image +0.040 [-0.009, +0.088] | vs blank -0.002 [-0.057, +0.052]
- CLOSED: total gain +0.072 [+0.004, +0.138] | gain with blank image +0.064 [-0.012, +0.142] | benefit change vs other image +0.036 [-0.043, +0.114] | vs blank +0.008 [-0.077, +0.092]
- OPEN: total gain +0.035 [-0.011, +0.085] | gain with blank image +0.050 [+0.005, +0.097] | benefit change vs other image +0.045 [-0.010, +0.098] | vs blank -0.015 [-0.073, +0.040]
