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

### 🚀 Fine-Tune the Model

Run the notebook: [`Finetune_LoRA_Model.ipynb`](./Finetune_LoRA_Model.ipynb)

This notebook includes:
- Loading the base Stable Diffusion model
- Preparing the flower dataset
- Applying LoRA fine-tuning
- Saving the trained weights into the `lora_weights/` directory

---

### 🧪 Test the Fine-Tuned Model

Run the notebook: [`Test_Finetuned_LoRA_Model.ipynb`](./Test_Finetuned_LoRA_Model.ipynb)

This notebook allows you to:
- Load the fine-tuned LoRA weights
- Generate images from custom flower prompts
- Visualize the output directly in the notebook

---

## 📂 Project Structure

```plaintext
.
├── Finetune_LoRA_Model.ipynb          # LoRA fine-tuning script
├── Test_Finetuned_LoRA_Model.ipynb    # Inference script to test the model
├── README.md                          # Documentation
└── lora_weights/                      # Folder containing saved weights
