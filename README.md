
# Quantitative 3D Analysis of the Equine Placenta Using Intensity-Based Image Segmentation

This project applies intensity-based image segmentation using open-source Python tools to a high-resolution micro-CT dataset of the equine placenta (363 × 3132 × 2076 voxels; voxel size = 86 μm) to extract quantitative volumetric metrics of major tissue compartments.


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

The total volume derived from this analysis (≈ 1501 cm³) is lower than the value reported by D.Laundon et al. (2024) (≈ 2148 cm³).
However, both results show a dominant contribution of the outer placental layers.

The combined amnion + chorion volumes (≈ 1308 cm³) are comparable to the allantochorion (1412 cm³) reported in the reference study, demonstrating similar overall scale and tissue dominance.
Lower-density fluid regions (amniotic and allantoic spaces) are difficult to isolate reliably using global intensity thresholds, leading to under-representation of these volumes.
The differences highlight the limitation of intensity-based segmentation, which does not incorporate anatomical context available in machine-learning approaches.
Despite its limitations, this threshold-based segmentation provides a reasonable gross morphometric approximation of the placenta.
Future work will involve deep-learning-based segmentation to improve anatomical accuracy and enable quantitative 3D vascular and compartmental analysis consistent with the reference study.

# Future Work
- Future studies will incorporate convolutional neural networks or other deep learning architectures to achieve anatomically accurate segmentation.
- With access to higher computational resources and increased GPU memory, full-resolution 3D reconstruction of the placental structure will be performed. 



**Author:** Ezenwaka Augusta Amarachi 
**Contact:** Aezenwaka74@gmail.com

