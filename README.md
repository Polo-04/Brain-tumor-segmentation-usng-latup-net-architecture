# Brain-tumor-segmentation-usng-latup-net-architecture
Lightweight attention-based U-Net for brain tumor segmentation on BraTS 2020

This project is my implementation of LATUP-Net (Lightweight Attention and Top-Down U-Net) for brain tumor segmentation on the BraTS 2020 dataset. The idea was to build a deep learning model that can accurately detect and segment different tumor regions in MRI scans, while still being lightweight and efficient.

Brain tumor detection is critical in healthcare, but manual segmentation of MRI scans is slow and can vary between experts. With this project, I wanted to explore how attention mechanisms and SE blocks can make U-Net architectures smarter at focusing on tumor regions.


Used BraTS 2020 multi-modal MRI scans (T1, T1ce, T2, FLAIR).

Preprocessed the data (cropping to foreground, normalizing intensities, and slicing into 128×128×128 patches).

Built the LATUP-Net architecture, combining U-Net with attention and squeeze-and-excitation modules.

Trained the model with Dice + Cross-Entropy loss (with class weighting for imbalance).

Evaluated performance using Dice scores for whole tumor, tumor core, and enhancing tumor.

Tech stack:

Python, TensorFlow/Keras

segmentation_models_3D, NumPy, scikit-learn, Matplotlib


Highlights

The model achieved good segmentation results across different tumor regions.

Visualized predictions vs. ground truth to understand where the model worked well and where it struggled.

Learned a lot about balancing accuracy with efficiency in deep learning architectures.
