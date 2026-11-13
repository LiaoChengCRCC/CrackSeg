# CrackSeg
## Title: A Global-Local Contrastive Learning Framework with Multi-Structure Constraints for Reliable Tunnel Lining Crack Segmentation
## Abstract
Tunnel lining cracks are among the most common structural defects in operational tunnels, and accurate and reliable automatic detection is essential for intelligent tunnel inspection and maintenance. However, due to the extremely fine scale of lining cracks, weak structural cues, and complex background interference, existing approaches still face challenges in achieving high segmentation accuracy and maintaining structural continuity. To address these issues, this study proposes a global-local contrastive learning framework with multi-structure constraints for reliable tunnel lining crack segmentation. First, a multi-scale structural-semantic feature enhancement strategy is developed to strengthen the representation of fine-scale cracks. Multiple structural operators are introduced to extract fine-grained geometric priors, while a spatial-channel attention mechanism is employed to adaptively fuse structural and semantic features, thereby improving the local representation capability of micro-crack patterns. Second, considering the complementary structural characteristics of crack regions and centerlines, a multi-task supervised optimization scheme with spatial position constraints is designed to jointly learn regional and skeletal information, which enhances structural completeness and geometric consistency. Furthermore, a semi-supervised contrastive learning mechanism based on crack object-level global feature consistency is introduced to improve model robustness and generalization under complex tunnel inspection environments. Extensive experiments conducted on the publicly available CrackSeg9k and the self-collected Fine-Crack datasets demonstrate that the proposed method outperforms several recent state-of-the-art crack segmentation approaches. The proposed framework achieves F1-scores of 77.69% and 78.20%, respectively, showing superior structural continuity and boundary accuracy, particularly for fine-scale crack detection.

## Experimental Results
### Results on CrackSeg9k test dataset:
![alt text](crackseg9k.png)
### Results on Fine-Crack test dataset:
![alt text](finecrack.png)

## Datasets
To evaluate the proposed method, experiments were conducted on the public [CrackSeg9k](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/EGIEBY) dataset and a newly constructed [Fine-Crack](https://pan.baidu.com/s/1UJ__0yXdcKAKgomYsf8ylA?pwd=gydv) dataset targeting fine-scale crack segmentation.
![alt text](dataset.png)

## Acknowledgements
Most samples in the Fine-Crack dataset are derived from the following publicly available datasets. We express our special thanks to their authors and contributors. The original dataset names and links are listed below:

[CrackForest](https://github.com/cuilimeng/CrackForest-dataset/tree/master)

[DeepCrack](https://github.com/yhlleo/DeepCrack)

[Rissbilder](https://link.springer.com/chapter/10.1007/978-981-15-9343-7_36)

[CrackTree200](https://www.sciencedirect.com/science/article/abs/pii/S0167865511003795)

[Crack500](https://ieeexplore.ieee.org/abstract/document/8694955/)

This dataset would not have been possible without the authors and maintainers of the publicly available datasets listed above, whose open and reusable data work provided the foundation for this curated resource. We express our special thanks to all of them and to their contributors.

The Fine-Crack dataset is intended solely for scientific research purposes. Any commercial use is strictly prohibited without the prior written consent of the owners/rights holders of the above datasets. Users must also comply with the license terms of each original dataset.

If these datasets are useful for your research, please consider citing both these repositories and the corresponding original papers.
