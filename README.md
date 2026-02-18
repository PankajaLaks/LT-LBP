# LT-LBP Python Library

![Python Version](https://img.shields.io/badge/python-3.7%2B-blue) 
![License](https://img.shields.io/badge/license-VIT-green)

**LT-LBP (Logarithmic Transformation – Local Binary Pattern)** is a lightweight Python library for **texture analysis** and **feature extraction** from grayscale images.  

It implements the LT-LBP formula:

\[
LT\text{-}LBP = \sum_{p=0}^{7} s(g_c - g_p) \cdot p
\]

where \(s(x) = 1\) if \(x > 0\), else 0.

This method is robust for **illuminated and low-light images**, making it ideal for applications in:

- Face recognition  
- Texture classification  
- Medical image analysis  
- Surveillance and industrial inspection

---

## Features

- Compute LT-LBP for any grayscale image  
- Generate normalized histogram feature vectors for ML models  
- Fully vectorized NumPy implementation  
- Lightweight and easy to integrate  

---

## Installation

Clone the repository and install locally:

```bash
git clone https://github.com/<your-username>/ltlbp.git
cd ltlbp
pip install -e .

# LT-LBP

Among the various preprocessing of image Local Binary Pattern was fluently used as a local image descriptor. Other preprocessing methods we have referred to as Clipping the Hounsfield units, normalization, and resampling The local binary pattern was introduced by Ojala et al in 1996 and used as an adequate feature extractor. LBP was designed for monochrome images. It has been used in many applications because of its computational simplicity, invariance to grayscale changes, and high discriminative power. LBP for preprocessing as texture identification can be chosen. The generic formula for LBP is given by 

![image](https://github.com/user-attachments/assets/33719a42-ce25-44a1-853c-60ab078904ef)

According to the logarithmic and exponential rule, for every real number b, x and n

![image](https://github.com/user-attachments/assets/9873ff17-58eb-4c37-81ac-22c7b5a664c0)


The LT-LBP is formed in Equation 5 by using the fundamental logarithmic characteristics from Equation 4 from Equation 2.

![image](https://github.com/user-attachments/assets/196e27f7-f459-4225-ba21-f026d7ea9479)
