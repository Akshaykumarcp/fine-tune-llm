# fine-tune-llm
Fine tune LLM for custom requirements

#### Frameworks for fine tuning LLM
- [Hugginface Trainer](https://huggingface.co/docs/transformers/v4.39.1/en/main_classes/trainer#transformers.Trainer)
- [Axotl](https://github.com/OpenAccess-AI-Collective/axolotl)
- [Autotrain](https://huggingface.co/docs/autotrain/en/index)
- [LLAMAFactory](https://github.com/hiyouga/LLaMA-Factory)
- [TRL](https://github.com/huggingface/trl)
- [H20 LLM Studio](https://h2o.ai/platform/open-source-gpt-and-llm-studio/)
- [torchtune](https://github.com/pytorch/torchtune)
- [OpenAI](https://platform.openai.com/docs/guides/fine-tuning)
- [Unsloth](https://github.com/unslothai/unsloth)

#### Dataset's
- Several ways to create:
  - Existing open-source datasets, e.g., [Spider](https://huggingface.co/datasets/spider)
  - LLMs to create synthetically datasets, e.g., [Alpaca](https://huggingface.co/datasets/tatsu-lab/alpaca)
  - Humans to create datasets, e.g., [Dolly](https://huggingface.co/datasets/databricks/databricks-dolly-15k)
  - Combination of the above methods, e.g., [Orca](https://huggingface.co/datasets/Open-Orca/OpenOrca)
- References: [eugeneyan](https://eugeneyan.com/writing/synthetic/)

#### Use cases
| Use case | Code |
| ------------- | ------------- |
| [Out-of-Domain Finetuning to Bootstrap Hallucination Detection](https://eugeneyan.com/writing/finetuning/)  | [click here](https://github.com/eugeneyan/visualizing-finetunes)  |
