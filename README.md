# LT-LBP Python Library

![Python Version](https://img.shields.io/badge/python-3.7%2B-blue) 
![License](https://img.shields.io/badge/license-MIT-green)

**LT-LBP (Logarithmic Transformation – Local Binary Pattern)** is a lightweight Python library for **texture analysis** and **feature extraction** from grayscale images.  

$$
LT\text{-}LBP = \sum_{p=0}^{7} s(g_c - g_p) \cdot p
$$

where the step function $s(x)$ is defined as:

$$
s(x) = 
\begin{cases}
1 & \text{if } x > 0 \\
0 & \text{otherwise}
\end{cases}
$$

Here, $g_c$ is the center pixel intensity and $g_p$ are its 8 neighbors (clockwise).
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

- pip install ltlbp 
- from LTLBP import ltlbp

## License

MIT License



## Citation

If you use LT-LBP in your research, please cite:

@article {10.3844/jcssp.2024.106.120,
article_type = {journal},
title = {LT-LBP-Based Spatial Texture Feature Extraction with Deep Learning for X-Ray Images},
author = {P., Pankaja Lakshmi and M., Sivagami},
volume = {20},
number = {1},
year = {2023},
month = {Dec},
pages = {106-120},
doi = {10.3844/jcssp.2024.106.120},
url = {https://thescipub.com/abstract/jcssp.2024.106.120},
journal = {Journal of Computer Science},
publisher = {Science Publications}
}
## Software Availability

The LT-LBP Python implementation is publicly available at:
https://pypi.org/project/ltlbp/
"""



