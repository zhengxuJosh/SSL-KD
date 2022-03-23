# Research-Overview
## Mind Map
Semi-supervised Classification 
<img width="856" alt="image" src="https://user-images.githubusercontent.com/49426295/159474651-647d7ee9-5795-4c03-a5dd-bd1d5ec8f59e.png">

Semi-supervised Segmentation
（To be updated）
## Method Comparison
#### Semi-supervised Learning Classification (2020-Now)
| Conference | Method | Task | Basic Structure | HighLight |
| :-------------: | :-------------: | :-------------: | :-------------: |:-------------: |
|ICML 2020|[SimCLR](https://arxiv.org/pdf/2002.05709v3.pdf)|Classification|Contrastive|Maximize agreement between **differently augmented example**|
|NIPS 2020|[FixMatch](https://arxiv.org/pdf/2001.07685)|Classification|Pseudo Label|**Combination** of **Consistency regularization** and **pseudo-labeling**|
|NIPS 2020|[UDA](https://arxiv.org/pdf/1904.12848v6.pdf)|Classification|Consistency|How to augment **unlabeled data**|
|ECCV 2020|[FeatMatch](https://arxiv.org/pdf/2007.08505v1.pdf)|Classification|Consistency|**Feature-Based** Augmentation and Consistency|
|NIPS 2021|[FlexMatch](https://arxiv.org/pdf/2110.08263.pdf)|Classification|Pseudo Label|Propose **CPL** to flexibly adjust thresholds for pseudo-labeling|
|ICLR 2021|[UPS](https://arxiv.org/pdf/2101.06329v3.pdf)|Classification|Pseudo Label|Improves pseudo labeling accuracy by uncertainty|
|ICCV 2021|[CoMatch](https://arxiv.org/pdf/2011.11183v2.pdf)|Classification|Pseudo Label|Contrastive bewteen **class probabilities** and **low-dimensional embeddings**|
|CVPR 2021|[MetaPL](https://arxiv.org/pdf/2003.10580v4.pdf)|Classification|T-S|Use performance of Student on labeled data to **update** Teacher|
|CVPR 2021|[SimCo](https://arxiv.org/pdf/2104.05248v1.pdf)|Classification|Pseudo Label|**Condition pseudo-labeling** on class similarities **prior knowledge**|
|CVPR 2021|[SimPLE](https://arxiv.org/pdf/2103.16725v1.pdf)|Classification|Pseudo Label|Minimize distance between **high confidence pseudo labels**|
|CVPR 2022|[SimMatch](https://arxiv.org/pdf/2203.06915)| Classification | Pseudo Label | Leverage **semantic and instance level** pseudo-label|

#### **“xxxMatch” Series**
<img width="1858" alt="image" src="https://user-images.githubusercontent.com/49426295/159506626-7b25bda3-8dcc-4d01-8711-5961d6ea76f6.png">

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
## Recent Papers (2022)
The latest literature review includes semi-supervised learning, knowledge distillation, ViT, etc.
| Domian | Conference | Title | Code |
| :-------------: | :-------------: | :-------------: | :-------------: | 
|Semi| CVPR 2022 | [Class-Aware Contrastive Semi-Supervised Learning](https://arxiv.org/pdf/2203.02261)||
|Semi| CVPR 2022 | [Semi-Supervised Semantic Segmentation Using Unreliable Pseudo-Labels](https://arxiv.org/pdf/2203.03884)||
|Semi| CVPR 2022 | [SimMatch: Semi-supervised Learning with Similarity Matching](https://arxiv.org/pdf/2203.06915)||
|Weakly| CVPR 2022 | [Weakly Supervised Semantic Segmentation using Out-of-Distribution Data](https://arxiv.org/pdf/2203.03860)||
|Weakly| CVPR 2022 | [Multi-class Token Transformer for Weakly Supervised Semantic Segmentation](https://arxiv.org/pdf/2203.02891)||
|Weakly| CVPR 2022 | [Weakly Supervised Semantic Segmentation by Pixel-to-Prototype Contrast](https://arxiv.org/pdf/2110.07110)||
|Weakly| CVPR 2022 | [Weakly Supervised Object Localization as Domain Adaption](https://arxiv.org/pdf/2203.01714)||
|KD| CVPR 2022 | [Wavelet Knowledge Distillation: Towards Efficient Image-to-Image Translation](https://arxiv.org/pdf/2203.06321)||
|KD| CVPR 2022 | [ISD: Self-Supervised Learning by Iterative Similarity Distillation](https://openaccess.thecvf.com/content/ICCV2021/papers/Tejankar_ISD_Self-Supervised_Learning_by_Iterative_Similarity_Distillation_ICCV_2021_paper.pdf)||
|KD| CVPR 2022 | [Decoupled Knowledge Distillation](https://arxiv.org/pdf/2203.08679) ||
|KD| CVPR 2022 | [Knowledge Distillation as Efficient Pre-training: Faster Convergence, Higher Data-efficiency, and Better Transferability](https://arxiv.org/pdf/2203.05180) ||
|KD| CVPR 2022 | [Focal and Global Knowledge Distillation for Detectors](https://arxiv.org/pdf/2111.11837) ||
|Contrastive| CVPR 2022 | [Selective-Supervised Contrastive Learning with Noisy Labels](https://arxiv.org/pdf/2203.04181.pdf) ||
|Self| ICLR 2022 | [Self-Supervision Enhanced Feature Selection with Correlated Gates](https://openreview.net/pdf?id=oDFvtxzPOx) ||
|ViT| ICLR 2022 | [When Vision Transformers Outperform ResNets without Pre-training or Strong Data Augmentations](https://openreview.net/pdf?id=LtKcMgGOeLt) ||
|ViT| ICLR 2022 | [How Do Vision Transformers Work?](https://openreview.net/pdf?id=D78Go4hVcxO) ||
|ViT| ICLR 2022 | [RegionViT: Regional-to-Local Attention for Vision Transformers](https://openreview.net/pdf?id=D78Go4hVcxO) ||
|ViT| ICLR 2022 | [Efficient Self-supervised Vision Transformers for Representation Learning](https://openreview.net/pdf?id=T__V3uLix7V) ||
|Weakly| ICLR 2022 | [Universalizing Weak Supervision](https://openreview.net/pdf?id=YpPiNigTzMT) ||
|KD| ICLR 2022 | [Unsupervised Semantic Segmentation by Distilling Feature Correspondences](https://openreview.net/pdf?id=SaKO6z6Hl0c) |
|KD| ICLR 2022 | [Reliable Adversarial Distillation with Unreliable Teachers](https://openreview.net/pdf?id=u6TRGdzhfip) |
|Semi| ICLR 2022 | [The Rich Get Richer: Disparate Impact of Semi-Supervised Learning](https://openreview.net/pdf?id=DXPftn5kjQK)||
|Semi| ICLR 2022 | [On Non-Random Missing Labels in Semi-Supervised Learning ](https://openreview.net/pdf?id=6yVvwR9H9Oj)||
|Semi| ICLR 2022 | [Pseudo-Labeled Auto-Curriculum Learning for Semi-Supervised Keypoint Localization ](https://openreview.net/pdf?id=6Q52pZ-Th7N)||
|Semi| ICLR 2022 | [Open-World Semi-Supervised Learning ](https://openreview.net/pdf?id=O-r8LOR-CCA)||
|Semi| ICLR 2022 | [AdaMatch: A Unified Approach to Semi-Supervised Learning and Domain Adaptation ](https://openreview.net/pdf?id=Q5uh1Nvv5dm)||
|Other| ICLR 2022 | [Zero Pixel Directional Boundary by Vector Transform](https://openreview.net/pdf?id=nxcABL7jbQh) ||
|Other| ICLR 2022 | [How to deal with missing data in supervised deep learning?](https://openreview.net/pdf?id=J7b4BCtDm4) ||
|Other| ICLR 2022 | [Chaos is a Ladder: A New Understanding of Contrastive Learning](https://openreview.net/pdf?id=ECvgmYVyeUz) ||
|Other| ICLR 2022 | [Sample Selection with Uncertainty of Losses for Learning with Noisy Labels](https://openreview.net/pdf?id=xENf4QUL4LW) ||











