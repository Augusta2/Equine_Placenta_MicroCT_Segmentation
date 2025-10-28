
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
Placenta Volume Analysis
   Label  Voxel_count  Volume_mm3  Volume_fraction_%  Volume_cm3
0      1   1855168815  1179991.00          78.600934  1179.99100
1      2    119866435    76241.77           5.078575    76.24177
2      3    182743903   116235.40           7.742606   116.23540
3      4    202458463   128774.90           8.577885   128.77490

Total Placental Volume:
  → 1501243.07 mm³
  → 1501.24 cm³

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

