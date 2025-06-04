
# Naruto Text-to-Image Generator

This project is a full-stack Generative AI web application that enables users to generate Naruto-style anime images from text prompts using a fine-tuned Stable Diffusion model. The application features a user-friendly **Streamlit** front-end and a PyTorch-based back-end powered by Hugging Face's `diffusers` library.

The model was fine-tuned on the **Naruto BLIP-captioned dataset**, where only the **U-Net** component of the Stable Diffusion architecture was updated. The **CLIP tokenizer**, **VAE encoder**, and **VAE decoder** were kept frozen to retain the generalization ability of the pre-trained components.

---

## 🔧 Features

- Fine-tuned **latent diffusion model** for anime-style image generation
- Clean and interactive **Streamlit UI** for text input and real-time image display
- Integration of **CLIP Score**, **FID**, and **Inception Score** to evaluate model performance
- Supports GPU-accelerated training and inference
- Uses the [Naruto BLIP-captioned dataset](https://huggingface.co/datasets/lambdalabs/naruto-blip-captions) for domain-specific fine-tuning

---

## 🚀 Tech Stack

- **Frontend**: Streamlit
- **Backend**: PyTorch, Hugging Face Diffusers
- **Model Architecture**: Stable Diffusion (VAE + CLIP + U-Net)
- **Dataset**: Naruto BLIP-captioned
- **Evaluation Metrics**: CLIP Score, FID, Inception Score
