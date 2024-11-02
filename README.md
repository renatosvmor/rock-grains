# Deep learning for segmentation and classification of rock grains in the aggregates industry

This repository contains the dataset used in the study published in the following scientific paper.

- **Ricardo R. Nunes; Renato M. Silva (2024)**. *Deep learning for segmentation and classification of rock grains in the aggregates industry*. Proceedings of the 21st National Meeting on Artificial and Computational Intelligence (ENIAC'2024). Belém, Pará, Brazil: Brazilian Computer Society, pp. 1–12.

## Dataset

The dataset used in this study is organized into the following folders. 

- [dataset/test_images](./dataset/test_images): this folder contains the test images.

- [dataset/train_images](./dataset/train_images): this folder contains the training images.

- [dataset/train_masks](./dataset/train_masks): this folder contains the annotation masks for the training images, which correspond to the training images with the same file names in the `train_images` folder. These masks delineate the grains, with each pixel classified as `1` for **gravel grains** and `0` for the **background**.

The file names in each folder indicate the class of the images. Images with the word `contaminated` in their name represent **images with Gravel 1 contaminated by Gravel 2**, while images with `nonContaminated` in their name represent **images containing only Gravel 1 with no contamination**. The criteria for this differentiation is based on the size of the grains: images containing only Gravel 1 must not have grains exceeding 600 mm², whereas images contaminated with Gravel 2 can include such grains. Each pixel in the images represents an area of 0.0087 mm² in reality. For further details, please consult the paper. 
  
## BibTeX Entry

The BibTeX entry for the paper is provided below.

```
@inproceedings{2024_nunes_eniac_rockGrains,
	author={Ricardo Ramos Nunes and Renato Moraes Silva},
	title={Deep learning for segmentation and classification of rock grains in the aggregates industry},
	booktitle={Proceedings of the 21st National Meeting on Artificial and Computational Intelligence (ENIAC'2024)}, 
	year={2024},
	month=nov,
	address = {Belém, PA, Brazil},
	publisher={Brazilian Computer Society},
	pages={1--12}
}
```






