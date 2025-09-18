# AI Storytelling: Face Generation with GANs & Gender Interpolation

## 📌 Project Overview
This project demonstrates **Artificial Intelligence (AI)** techniques to **generate and manipulate face images** using a **pretrained GAN generator** and a **latent gender vector**.  

We generate **15 face variations**, smoothly transforming from male → female by adding multiples of a **gender direction vector** in the latent space of the GAN. This approach highlights **latent space manipulation**, allowing controlled changes in facial features like gender.

---

## 📊 Key Insights from Analysis

**Dataset / Model:**
- Generator trained on CelebFace Dataset (64×64 images)  
- Latent space dimension: 100  
- Gender vector (`gender_vec.npy`) encodes male → female direction in latent space  

**Generation Process:**
- Sample a random latent vector `z` → base face  
- Interpolate 15 variations along the gender vector  
- Negative alpha → more male, positive alpha → more female  

**Visualization & Evaluation:**
- Individual images saved as `face_variation_1.png` → `face_variation_15.png`  
- Combined preview shows all 15 images in a single row  
- Optional **GIF animation** demonstrates smooth gender transition  
- Optional **gender classifier predictions** validate gradual shift from male → female  

**Takeaways:**
- GAN generator produces high-quality realistic faces  
- Latent space manipulation enables controlled feature modification  
- Alpha labels indicate degree of male/female transformation  
- Combined image and GIF provide submission-ready visualizations  

---

## 📂 Repository Contents
- `Creative_AI_Face_GAN_Gender_Interpolation.ipynb` → Full workflow:
  - Install and load TensorFlow & dependencies  
  - Download pretrained generator (`generator_700.h5`)  
  - Download gender vector (`gender_vec.npy`)  
  - Generate 15 latent vector variations  
  - Generate, display, and save images  
  - Combine images into a single labeled preview  
  - Create GIF animation of gender interpolation  
  - Optional: Gender classifier predictions  
- `generated_faces/` → Folder containing all 15 generated images, GIF, and combined labeled preview

---

## 🔮 Next Steps / Future Improvements
- **Different Seeds / Random Faces:** Generate multiple base faces for more examples  
- **Feature Manipulation:** Extend latent vector directions to modify age, smile, hair style, etc.  
- **Higher-Resolution Faces:** Train GANs for 128×128 or 256×256 images  
- **Interactive Sliders:** Allow users to control alpha dynamically for real-time face transformation  
- **Explainable AI (XAI):** Use feature attribution to understand what latent vectors modify in faces  

---

## ⚡ References
- [Face Generator with GAN – GitHub](https://github.com/AshishJangra27/Face-Generator-with-GAN)  
- [Gender Style Transfer – GitHub](https://github.com/AshishJangra27/Gender-Style-Transfer)  
- [Gender Classifier – GitHub](https://github.com/AshishJangra27/Gender-Classifier)  
- [LinkedIn – Ashish Jangra](https://www.linkedin.com/in/ashish-jangra/)  
