# LungNENOmics cohort data and analyses

## Whole slide images (WSI) pre-processing:
- WSI pre-processing tools are available at [https://github.com/IARCbioinfo/WSIPreprocessing](https://github.com/IARCbioinfo/WSIPreprocessing)
- This repository contains:
    + Scripts for dividing WSI into patches, called tiles.
    + Scripts to normalize the HE/HES coloring of WSIs, used to artificially remove saffron coloring from WSIs produced in the French center.

## Tumor segmentation with [CFlow AD](https://openaccess.thecvf.com/content/WACV2022/papers/Gudovskiy_CFLOW-AD_Real-Time_Unsupervised_Anomaly_Detection_With_Localization_via_Conditional_Normalizing_WACV_2022_paper.pdf):
- Tumour areas were segmented unsupervised using the CFLow anomaly detection model. An adaptation of this model for this task is available at [https://github.com/IARCbioinfo/TumorSegmentationCFlowAD](https://github.com/IARCbioinfo/TumorSegmentationCFlowAD)
- This repository contains:
      + Scripts to train and evaluate the model
      + Script to create the segmentation maps
- Training sets for Ki-67 and HE/HES WSI are available on request from mathiane[at]iarc[dot]who[int], as is the pre-trained model (*will be available on a server soon*).

## Automatic assessment of lung neuroendocrine neoplasms (LNEN) proliferative activity using [Pathonet](https://www.nature.com/articles/s41598-021-86912-w)
-  The Ki-67 and PHH3 indices were quantified automatically using the Pathonet supervised deep learning model. An adaptation of this model is available at the following address [https://github.com/IARCbioinfo/PathonetLNEN](https://github.com/IARCbioinfo/PathonetLNEN)
- This repository also contains scripts for calculating spatial metrics using graph theory as proposed by Bullloni and colleagues [See : Automated analysis of proliferating cells spatial organization predicts prognosis in lung neuroendocrine neoplasms, Cancers 2021](https://www.mdpi.com/2072-6694/13/19/4875)
- Annotated LNEN tiles are available on request from mathiane[at]iarc[dot]who[int].
