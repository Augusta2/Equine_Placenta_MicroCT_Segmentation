
# Quantitative 3D Analysisof the Equine Placenta Using Intensity-Based Image Segmentation

This project demonstrates how micro-CT data of the equine placenta can be processed using **Python and scikit-image** for intensity-based segmentation, volumetric quantification, and gross morphological interpretation.

# Project Overview
- **Data:** Public equine placenta micro-CT dataset (EBI BioStudies S-BIAD1130)
- **Goal:** Quantify gross morphology and relative tissue volumes using voxel-based intensity segmentation
- **Tools:** Google Colab, NumPy, scikit-image, Plotly, tifffile

#  Key Steps
1. **Data import**
2. **Intensity-based multi-Otsu segmentation**
3. **Colour mapping and slice visualisation**
4. **Integer-based segmentation**
5. **Voxel count, total and fractional volume calculations**


#  Results Summary
 Label     Interpretation       Volume (cm³)   Fraction (%) 
------------------------------------:-------------:
1           Allantoic region    1179.9          78.6 
2           Vessels               76.2           5.1 
3           Amniotic sac         116.2           7.7 
4           Chorion              128.8           8.6 

# Future Work
- Future studies will incorporate convolutional neural networks or other deep learning architectures to achieve anatomically accurate segmentation.
- With access to higher computational resources and increased GPU memory, full-resolution 3D reconstruction of the placental structure will be performed. 



**Author:** Ezenwaka Augusta Amarachi 
**Contact:** Aezenwaka74@gmail.com

