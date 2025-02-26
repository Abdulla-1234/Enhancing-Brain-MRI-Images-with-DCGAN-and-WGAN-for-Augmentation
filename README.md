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

![image](https://github.com/user-attachments/assets/a55a489f-20d2-4caa-9a8a-c257c2608274)


## 📊 Results
- **DCGAN performed slightly better** than WGAN in generating high-quality synthetic images.
- PSNR and SSIM values indicate that **synthetic images closely resemble real MRI scans**.
- Synthetic images were successfully used for **data augmentation**, improving model performance in classification tasks.

Below is a comparison between **real MRI images** and **GAN-generated images**:

| Real MRI Image | DCGAN Generated | WGAN Generated |
|---------------|----------------|----------------|
| ![Real_image](https://github.com/user-attachments/assets/1434db68-bd18-41c3-9122-d386aa81462b) | ![DCGAN](https://github.com/user-attachments/assets/da4111ec-ef13-44ff-a840-18869e57c2cf) | ![image](https://github.com/user-attachments/assets/e40c7f4f-7b78-450d-88cb-bb2b252f36fe) |

The PSNR and SSIM metrics are visualized below:

![PNSR](https://github.com/user-attachments/assets/919347dd-7aaf-4210-af77-f4dd74b4d87f)

![SSIM](https://github.com/user-attachments/assets/d23ddf15-04af-43e6-ab60-9bd2fa16cd8e)

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
