# Enhancing Brain MRI Images: Using DCGAN and WGAN for Image Augmentation

## 📌 Project Overview
This project explores the application of **Generative Adversarial Networks (GANs)**, specifically **Deep Convolutional GAN (DCGAN)** and **Wasserstein GAN (WGAN)**, for **data augmentation in brain MRI imaging**. The primary goal is to improve the availability and diversity of MRI datasets to support **medical image analysis and deep learning applications**.

## 🔍 Abstract
MRI image analysis plays a crucial role in medical diagnostics, but acquiring large, diverse datasets is expensive and time-consuming. Traditional data augmentation techniques (rotation, scaling, cropping) often fail to introduce meaningful variations. This project leverages GAN-based synthetic data generation to overcome these limitations. By training **DCGAN and WGAN** models on the **Kaggle 2020 brain MRI dataset**, we generate realistic brain MRI images that aid in **deep learning model training and medical research**.

## 📂 Dataset
- **Source:** Kaggle 2020 Brain MRI Dataset
- **Composition:** Includes **multispectral contrast-enhanced brain MR images** with different sequences: **T1, T1ce, T2, T2ce**.
- **Size:** 220 HGG and 54 LGG clinical cases.

## 🏗️ Methodology
1. **Data Preprocessing:** Image normalization and augmentation.
2. **Model Selection:** Implementation of **DCGAN and WGAN**.
3. **Training:** Optimizing the generator and discriminator networks.
4. **Evaluation Metrics:** 
   - **Peak Signal-to-Noise Ratio (PSNR)**
   - **Structural Similarity Index Measure (SSIM)**

![GAN Architecture](https://github.com/Abdulla-1234/Enhancing-Brain-MRI-Images-with-DCGAN-and-WGAN-for-Augmentation/blob/main/Images/GAN%20Architecture.png)


## 📊 Results
- **DCGAN performed slightly better** than WGAN in generating high-quality synthetic images.
- PSNR and SSIM values indicate that **synthetic images closely resemble real MRI scans**.
- Synthetic images were successfully used for **data augmentation**, improving model performance in classification tasks.

Below is a comparison between **real MRI images** and **GAN-generated images**:

| Real MRI Image | DCGAN Generated | WGAN Generated |
|---------------|----------------|----------------|
| ![Real_image](https://github.com/Abdulla-1234/Enhancing-Brain-MRI-Images-with-DCGAN-and-WGAN-for-Augmentation/blob/main/Images/Real_image.png) | ![DCGAN](https://github.com/Abdulla-1234/Enhancing-Brain-MRI-Images-with-DCGAN-and-WGAN-for-Augmentation/blob/main/Images/DCGAN.png) | ![WCGAN](https://github.com/Abdulla-1234/Enhancing-Brain-MRI-Images-with-DCGAN-and-WGAN-for-Augmentation/blob/main/Images/wcgan.png) |

The PSNR and SSIM metrics are visualized below:
| PNSR score | SSIM score |
|---------------|----------------|
| ![PNSR](https://github.com/Abdulla-1234/Enhancing-Brain-MRI-Images-with-DCGAN-and-WGAN-for-Augmentation/blob/main/Images/pnsr.png) | ![SSIM](https://github.com/Abdulla-1234/Enhancing-Brain-MRI-Images-with-DCGAN-and-WGAN-for-Augmentation/blob/main/Images/ssim.png) |

## 🔮 Future Scope
- Extend generation to **coronal and transverse images**.
- Implement **classification models** to distinguish real and fake images.
- Apply **GAN-based augmentation** to other medical imaging domains.

## 🛠️ Technologies Used
- Python
- TensorFlow / PyTorch
- OpenCV
- NumPy & Pandas
- Matplotlib & Seaborn
