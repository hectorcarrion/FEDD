# FEDD
Code repository for FEDD - Fair, Efficient, and Diverse Diffusion-based Lesion Segmentation and Malignancy Classification, published at MICCAI 2023.

## DDI segmentation labels
Our labeled segmentation data can be found on the `ddi_labeles` folder. This includes pre-split training, validation and testing sets for 5%, 10%, 15% and 20% of DDI (balanced) as well as an additional larger test set of annotations split per skin-tone (unbalanced) as described on the paper.

The labels are encoded as 2D numpy arrays where the value of each pixel corresponds to the label mask index. The value-to-class map is as follows:

* 0: Background
* 1: Lesion
* 2: Marker
* 3: Ruler
* 4: Skin

The filenames for each mask correspond to the original filenames per sample found on the DDI dataset. No images are shared on this github, only their corresponding masks. To get the original images please visit https://ddi-dataset.github.io/

## DDI classification labels
Malignancy classification labels are computed from the DDI dataset metadata file found at https://ddi-dataset.github.io/

## Training and inference code
The training and inference code for FEDD, previous SOTA DeepDerm and our baseline models are found as python notebooks in the `code` directory. Note that we trained on Google Colab connected to Google Drive so you may need to edit pointers to the data in order to run on your own local machine.

## Questions
For any questions, comments or additional data requests please contact hcarrion@ucsc.edu

Thanks!
