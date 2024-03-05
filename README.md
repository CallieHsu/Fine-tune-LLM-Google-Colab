[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/CallieHsu/Fine-tune-LLM-Google-Colab/blob/master/fine_tune_tinyllama_on_google_colab.ipynb)
# Fine-tuning LLMs on Google Colab
### 🤗 Pretrained model
- Large Language Model (LLM): [TinyLlama/TinyLlama-1.1B-Chat-v1.0](https://huggingface.co/TinyLlama/TinyLlama-1.1B-Chat-v1.0)

### 🚀 Fine-tuning techniques
- **Supervised Fine-Tuning** (**SFT**): Models are trained on a dataset of instructions and responses. It adjusts the weights in the LLM to minimize the difference between the generated answers and ground-truth responses, acting as labels.
- **QLoRA**: quantized **Low-Rank Adaptation** (**LoRA**), is a technique that further reduces memory usage during finetuning. During backpropagation, QLoRA quantizes the pretrained weights to 4-bit precision and uses paged optimizers to handle memory spikes.
  ![image](https://github.com/CallieHsu/Fine-tune-LLM-Google-Colab/assets/62089495/08ec5699-8226-4b13-aa25-33224918d7d1)
  📚 More details: [Practical Tips for Finetuning LLMs Using LoRA (Low-Rank Adaptation)](https://magazine.sebastianraschka.com/p/practical-tips-for-finetuning-llms)

### ⚙️ System Requirements
Google Colab environment
若需要用本機端執行請參考 [Google Colaboratory - Local runtimes](https://research.google.com/colaboratory/local-runtimes.html)
