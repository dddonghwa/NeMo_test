# [ECCV 2024] Finding NeMo: Negative-mined Mosaic Augmentation for Referring Image Segmentation

[Seonsu Ha*](https://seongsuha.github.io/), Chaeyun Kim*, Donghwa Kim*, Junho Lee, [Sangho Lee](https://sangho-vision.github.io/), [Joonseok Lee](http://www.joonseok.net/home.html)

### [Project Page](https://dddonghwa.github.io/NeMo/)`|`[Paper](http://www.joonseok.net/papers/eccv24_nemo.pdf)

<img width="1074" alt="스크린샷 2024-09-11 오후 11 37 55" src="https://github.com/user-attachments/assets/2f0c9fc9-e6fb-4fc1-ade6-7641b2749c50">


### Abstract 
Referring Image Segmentation is a comprehensive task to segment an object referred by a textual query from an image. In nature, the level of difficulty in this task is affected by the existence of similar objects and the complexity of the referring expression. Recent RIS models still dshow a significant performance gap between easy and hard scenarios. We pose that the bottleneck exists in the data, and propose a simple but powerful data augmentation method, Negative-mined Mosaic Augmentation (NeMo). This method augments a training image into a mosaic with three other negative images carefully curated by a pretrained multimodal alignment model, e.g., CLIP, to make the sample more challenging. We discover that it is critical to properly adjust the difficulty level, neither too ambiguous nor too trivial. The augmented training data encourages the RIS model to recognize subtle differences and relationships between similar visual entities and to concretely understand the whole expression to locate the right target better. Our approach shows consistent improvements on various datasets and models, verified by extensive experiments.

## News
[2024/09/19] Code Release

## Note
We release the dataloader for NeMo, which augments each image by combining it with other three hard negative images from the image pool. The image pool consists of visually similar images based on their similarity scores of CLIP. Lmdb files for each dataset are needed for the dataloader.

## Citation
```
TBA
```

