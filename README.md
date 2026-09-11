# Applied_Machine_Learning_organoids

## Introduction
Organoids are three-dimensional cellular structures that closely resemble the architecture and function of real organs. Grown in vitro from stem cells or other precursor cells, they provide powerful models for investigating organ development, physiology, and pathology, as well as for drug discovery and disease modeling. Their ability to reproduce key aspects of the tissue microenvironment and organ-specific functions makes organoids invaluable tools for exploring disease mechanisms and evaluating potential therapeutic approaches.

Imaging plays a central role in organoid research, as it enables the characterisation of their morphology, growth dynamics, and functional properties. Different features, such as size, shape, and structural complexity, can be extracted and quantitatively analysed to provide meaningful biological information, offering a powerful, non-invasive way to monitor organoid health and behaviour.

In this context, the aim of this work was to evaluate whether organoids belonging to different cancerous and non-cancerous cell lines can be distinguished from brightfield images.

## Dataset
The publicly available Spheroid Light Microscopy Image Atlas (SLIMIA)[1] was used in this study. The dataset comprises approximately 8,000 brightfield images of spheroids derived from both cancerous and non-cancerous cell lines, acquired across different microscopes and formation protocols. To reduce variability related to acquisition conditions and experimental setup, only images obtained with the Axioviert200M microscope and generated using a single seeding density of 2000 cells were selected for this analysis. The resulting subset included 1382 images from 11 different cell lines.

Radiomic features were extracted using the PyRadiomics [2] library. Input images were normalized using z-score scaling, and no additional filters were applied. All feature classes were extracted, resulting in 102 features per organoid image.

## Analysis
Radiomic features will be employed in Machine Learning algorithms to predict organoid cell line (classification task).

## References 
[1] E. Blondeel, A. Peirsman, S. Vermeulen, and et al. The spheroid light microscopy image atlas for morphometrical analysis of three-dimensional cell cultures. Sci Data, 12(283), 2025.

[2] J. J. M. van Griethuysen, A. Fedorov, C. Parmar, A. Hosny, N. Aucoin, V. Narayan, R. G. H. Beets-Tan, J. C. Fillion-Robin, S. Pieper, and H. J. W. L. Aerts. Computational radiomics system to decode the radiographic
phenotype. Cancer Res, 77(21):e104–e107, 2017.
