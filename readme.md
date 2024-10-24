# **Text-to-Image Generation Using GANs, Diffusion Models, and VAE**

### **Overview**

This project focuses on generating realistic facial images based on textual descriptions using a combination of **Generative Adversarial Networks (GANs)**, **Diffusion Models**, and a hybrid **Diffusion-VAE** model. Leveraging the **CelebA dataset**, we train models to translate attributes and descriptions into high-quality images. The project demonstrates the effectiveness of different generative approaches for text-to-image synthesis.

---

### **Table of Contents**

- [Project Overview](#overview)
- [Dataset](#dataset)
- [Models](#models)
- [Results](#results)
- [Team](#team)
- [Acknowledgments](#acknowledgments)

---

### **Dataset**

**CelebA (CelebFaces Attributes Dataset)** is used in this project, which contains over **202,599 celebrity images** with **40 attribute labels** (e.g., smiling, wearing glasses, hair color). 

#### **Preprocessing:**
- Images resized and normalized for GAN and diffusion model input.
- Text descriptions were generated from CelebA attributes to serve as the conditional input for text-to-image generation.

---

### **Models**

#### **1. GANs**
- A DCGAN architecture conditioned on BERT embeddings, combining textual descriptions with latent vectors to generate facial images.

#### **2. Diffusion Models**
- A diffusion model that iteratively denoises random noise based on the text embedding to generate a realistic image.

#### **3. Diffusion with VAE**
- A hybrid approach where the VAE encodes latent variables, which are then denoised by the diffusion process for faster and more diverse image generation.

---

### **Results**

We achieved the following results for the different approaches:

- **GANs:** High-quality images with sharp details, but some instability in training.
- **Diffusion Models:** More stable training with diverse outputs but slower image generation.
- **Diffusion-VAE:** Faster sampling and well-balanced images, combining the best of both approaches.

For more detailed results, please refer to the [results](https://github.com/m7mdGNo/celeba-text-to-image/blob/main/presentation.pptx) file.

---

### **Team**

## Team Members
- [Abdelrhman Tarek](https://github.com/Abdelrhmantarekabdelmawla)
- [Mohamed elganainy](https://github.com/m7mdGNo)
- [Hossam Hany](https://github.com/Hossam-elganainy)
- [Ahmed Yosif](https://github.com/yousifless)


---

### **Acknowledgments**

We would like to thank our instructors, **Mostafa Atlam** and **Mohamed Gomaa**, for their valuable guidance throughout the project. We also extend our gratitude to the **Ministry of Communication**, **DEPI**, and **AMIT** for providing us the platform and resources to complete this project.

---

### **License**

This project is licensed under the MIT License. See [LICENSE](https://github.com/m7mdGNo/celeba-text-to-image/blob/main/LICENSE.md) for more details.
