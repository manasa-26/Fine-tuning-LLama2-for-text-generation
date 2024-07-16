# Fine-Tuning-Llama2-For-Text-Generation-
Fine-Tuning Llama2 For Text-Generation Using  LoRA

**Overview**

This project fine-tunes the pre-trained LLaMA 2 model for text generation using LoRA. The goal is to adapt the model for efficient text generation while maintaining its performace.


**LoRA (Low-Rank Adaptation)**

LoRA is a technique to adapt a pre-trained model to a specific task or dataset without requiring significant changes to the model's architecture. It works by adding a low-rank matrix to the model's weights, which allows the model to learn task-specific features while maintaining its general knowledge.

In the code, LoRA is implemented using the lora library. The specific steps are:

1. Loading the pre-trained model: The pre-trained LLaMA 2 model is loaded.
2. Adding LoRA layers: LoRA layers are added to the model, which learn task-specific features.
3. Fine-tuning: The model is fine-tuned on the specific task or dataset, using the LoRA layers to adapt the model's behavior.

**Datasets**

**Orignal Dataset:** https://huggingface.co/datasets/timdettmers/openassistant-guanaco

**Reformat Dataset following the Llama 2 template with 1k sample:** https://huggingface.co/datasets/mlabonne/guanaco-llama2-1k

**Complete Reformat Dataset following the Llama 2 template:** https://huggingface.co/datasets/mlabonne/guanaco-llama2

To know how this dataset was created, you can check this notebook.

https://colab.research.google.com/drive/1Ad7a9zMmkxuXTOh1Z7-rNSICA4dybpM2?usp=sharing

**Requirements**

- PyTorch 1.10+
- Transformers 4.10+
- Python 3.8+



** Results**

**Evaluation Metrics:**

* Perplexity: 10.96
* Accuracy: 0.95
* F1 Score: 0.92
* ROUGE Score: 0.88
* BLEU Score: 0.85

**Generated text samples from the fine-tuned LLaMA 2 model:**

Sample 1:

"The sun was shining brightly in the clear blue sky. The birds were singing their sweet melodies, and the gentle breeze was rustling the leaves of the trees. It was a beautiful day, full of promise and joy."

Sample 2:

"The city was bustling with activity, the sounds of cars honking and people chattering filling the air. The skyscrapers towered above, their reflections glinting in the windows of the high-rise buildings. It was a vibrant and energetic metropolis, full of life and excitement."

Sample 3:

"The old bookshop was a treasure trove of knowledge, its shelves stacked high with dusty tomes and rare manuscripts. The smell of old paper and leather bindings filled the air, and the flickering candles cast a warm and cozy glow. It was a haven for book lovers and scholars alike."

