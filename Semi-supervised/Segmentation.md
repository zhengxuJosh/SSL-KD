## Method Comparison
Comparison with SoTA methods on blender **PASCAL VOC 2012** val set under differnent partition protocols. All labeled images are selected from the augmented VOC train set, which consist of 10582 samlpes in total. (DeepLabv3+ w/ ResNet50)
|Method|Year|Key Component|1/16(662)|1/8(1323)|1/4(2646)|1/2(5291)|
| :-------------: | :-------------: | :-------------: | :-------------: | :-------------: | :-------------: | :-------------: |
|[Mean Teacher](https://arxiv.org/pdf/1703.01780v6.pdf)|NeurIPS2017|Teacher-Student & EMA|66.77|70.78|73.22|75.41|
|[CutMix](https://arxiv.org/pdf/1906.01916v5.pdf)|BMVC 2019|CutMix Augmentation|68.90|70.70|72.46|74.49|
|[CCT](https://arxiv.org/pdf/2003.09005v3.pdf)|CVPR 2020|Auxiliary Decoders|65.22|70.87|73.43|74.75|
|[GCT](https://arxiv.org/pdf/2008.05258v1.pdf)|ECCV 2020|Dual & Consistency|64.05|70.47|73.45|75.20|
|[CPS](https://arxiv.org/pdf/2106.01226v2.pdf)|CVPR 2021|Dual & Cross Pseudo Label|68.21|73.20|74.24|75.91|
|[DCC](https://arxiv.org/pdf/2106.14133v1.pdf)|CVPR 2021|Directional Pixels Contrastive|-|69.70|72.70|-|
|[AEL](https://arxiv.org/pdf/2110.05474v1.pdf)|NeurIPS 2021|Teacher-Student & Adaptive Sampling|75.83|77.90|79.01|80.28|
|[U2PL](https://arxiv.org/pdf/2203.03884v2.pdf)||
## Paper Summary

#### Semi-supervised Learning Segmentation (2020-Now)
| Conference | Method | Task | Basic Structure | HighLight |
| :-------------: | :-------------: | :-------------: | :-------------: |:-------------: |
|ICCV 2021|[PixelCL](https://arxiv.org/pdf/2104.13415v3.pdf)|Segmentation|T-S|**Contrastive** learning module: yield similar pixel-level feature representations for same-class samples|
|ICCV 2021|[DSBN](https://arxiv.org/pdf/2104.07256v4.pdf)|Segmentation|T-S|**Strong Augmentation**: Distribution-specific batch normalization|
|NIPS 2021|[AEL](https://arxiv.org/pdf/2110.05474v1.pdf)|Segmentation|T-S| Adaptive CutMix & Adaptive Copy-Paste & **Adaptive equalization sampling**|
|CVPR 2021|[DCC](https://arxiv.org/pdf/2106.14133v1.pdf)|Segmentation|Consistency|maintain the **context-aware consistency** between features of the same identity but with different contexts|
|CVPR 2021|[CPS](https://arxiv.org/pdf/2106.01226v2.pdf)|Segmentation|Pseudo Label|**Cross Pseudo Supervision**|
|CVPR 2022|[UUPL](https://arxiv.org/pdf/2203.03884)|Segmentation|T-S| Make **unreliable** pixels as **negative samples**|
|ICLR 2022|[ReCo](https://arxiv.org/pdf/2104.04465v4.pdf)|Segmentation||**Pixel-level** contrastive framework |










