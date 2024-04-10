#### Task 
- Fine tune Google flan-t5 base model with emotion dataset

#### Tech Stack
- Python package dependencies: transformers, datasets
- Dataset: [1](https://raw.githubusercontent.com/comet-ml/comet-llmops/main/data/merged_training_sample_prepared_train.jsonl), [2](https://raw.githubusercontent.com/comet-ml/comet-llmops/main/data/merged_training_sample_prepared_valid.jsonl)
- Pretrained LLM: google/flan-t5-base
- Training:
    - Train with HuggingFace Seq2SeqTrainer
    - model checkpoint saved in models dir (around 10GB in size, hence not uploaded here!)
    - Train time:
        - 583.7356 sec
- LLMOPS:
    - comet-llm
        - Track fine tune model hyperparam values in real time
        - Register model
        - Deploy 
- Evaluate:
    - sklearn confusion_matrix