### Task
- Build Chat assistant model for answering in custom style (dataset style)

#### Fine tune LLM details 
- Model: llama-2-7b-chat-hf model
- Load model in 4bit - Quantization: Huggingface (HF) transformer
    - The following `bitsandbytes` quantization config was used during training:
        - load_in_8bit: False
        - load_in_4bit: True
        - llm_int8_threshold: 6.0
        - llm_int8_skip_modules: None
        - llm_int8_enable_fp32_cpu_offload: False
        - llm_int8_has_fp16_weight: False
        - bnb_4bit_quant_type: nf4
        - bnb_4bit_use_double_quant: False
        - bnb_4bit_compute_dtype: float16
- Training technique: PEFT (LoRA)
- Due to memory constrains training on 1k samples for 1 epoch
- Model training: TRL SFTTrainer
- Model training time: Approx 45 minutes
- GPU: T4 16GB
- Track metrics: Tensorboard
- Inference: peft and HF Pipiline
- Store model to HF Hub