# LoRA Flower Diffusion 🌸

This repository hosts a fine-tuned **LoRA (Low-Rank Adaptation)** model based on **Stable Diffusion v1.4**. The model was fine-tuned on a curated flower dataset using BLIP-generated captions, enabling the generation of photorealistic or stylized flower images via text prompts.

---

## 🧠 Model Overview

- **Base Model**: [CompVis/stable-diffusion-v1-4](https://huggingface.co/CompVis/stable-diffusion-v1-4)
- **LoRA Fine-Tuning**: Performed using [Hugging Face Diffusers LoRA training pipeline](https://huggingface.co/docs/diffusers/training/lora)
- **Dataset**: [AhmadMustafa/flower-captions-blip](https://huggingface.co/datasets/AhmadMustafa/flower-captions-blip) – 100 flower images with auto-generated captions via BLIP
- **Purpose**: Generate diverse, high-quality images of flowers based on natural language prompts.

---

## 🏗️ How to Use

.
├── Finetune_LoRA_Model.ipynb                # LoRA fine-tuning script
├── Test_Finetuned_LoRA_Model.ipynb          # Inference script to test the model
├── README.md                                # Documentation
└── lora_weights/                            # Folder containing saved weight
