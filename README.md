# Noise-Reduction-in-Pistachio-Images-with-Convolutional-Autoencoder

This project applies a **Convolutional Autoencoder (CAE)** to **denoise pistachio images**.  
The goal is to remove random noise while preserving fine details, improving **image clarity** for further classification or analysis.  

---

## 🧠 Model Architecture  

The Autoencoder consists of two parts:  

### 🔹 Encoder  
- Convolutional layers with **ReLU** activation  
- Downsampling using **MaxPooling**  
- Encodes noisy images into compressed latent representation  

### 🔹 Decoder  
- Convolutional + Upsampling layers  
- Final layer with **Sigmoid** activation to reconstruct clean images  
- Produces denoised output with values in range `[0,1]`  

---

## 📊 Loss & Metrics  

- **Loss Function**: Mean Squared Error (MSE)  
- **Evaluation Metric**: Structural Similarity Index (SSIM) – measures image similarity  
- Goal: Minimize MSE while maximizing SSIM  

---

## 🛠️ Tech Stack  

- **Python 3.10**  
- **TensorFlow / Keras** (for Autoencoder)  
- **NumPy, Pandas** (data handling)  
- **Matplotlib, Seaborn** (visualization)  
- **scikit-image** (for SSIM evaluation)  

---

python -m ipykernel install --user --name=myenv  

