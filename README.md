# <center> Papers about Vision Language Models</center>

This repo lists recent advantages on VLMs, mainly contributed by [Weihan Wang](https://github.com/mactavish91) and [Ji Qi](https://github.com/qijimrc).

## Papers



|                                                                                  Model                                                                                  | Vision Enc. | Textual Enc. | Dec. | Multimodal Fusion |            Pretraining Objectives             |       Pretraining Dataset        | Published Year |   
|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:-----------:|:------------:|:----:|:------------------|:---------------------------------------------:|:--------------------------------:|:--------------:|
|                                  [ViLBERT](https://proceedings.neurips.cc/paper/2019/file/c74d97b01eae257e44aa9d5bade97baf-Paper.pdf)                                   | OD->Xformer |   Xformer    |  /   | Co-attn           |                  MLM+ITM+MIM                  |               CC3M               |  2019 (NIPS)   |
|                                                               [LXMERT](https://arxiv.org/abs/1908.07490)                                                                | OD+Xformer  |   Xformer    |  /   | Co-attn           |                MLM+ITM+MIM+VQA                |           COCO+VG+VQA            |  2019 (Arxiv)  |
|                                                             [VisualBERT](https://arxiv.org/abs/1908.03557)                                                              |     OD      |     Emb.     |  /   | Merged-attn       |                    MLM+ITM                    |               COCO               |  2019 (Arxiv)  |
|                                                 [UNITER](https://link.springer.com/chapter/10.1007/978-3-030-58577-8_7)                                                 |     OD      |     Emb.     |  /   | Merged-attn       |                MLM+ITM+MIM+WRA                |         COCO+VG+CC3M+SBU         |  2020 (ECCV)   |
|                                                               [VL-BERT](https://arxiv.org/abs/1908.08530)                                                               |     OD      |     Emb.     |  /   | Merged-attn       |                    MLM+ITM                    |               CC3M               |  2020 (ICLR)   |
|                                                 [OSCAR](https://link.springer.com/chapter/10.1007/978-3-030-58577-8_8)                                                  |     OD      |     Emb.     |  /   | Merged-attn       |                    MLM+ITM                    |               4.1M               |  2020 (ECCV)   |
|                                                              [PixelBERT](https://arxiv.org/abs/2004.00849)                                                              |     CNN     |   Xformer    |  /   | Merged-attn       |                    MLM+ITM                    |             COCO+VG              |  2020 (Arxiv)  |
|                                 [VILLA](https://proceedings.neurips.cc/paper/2020/hash/49562478de4c54fafd4ec46fdb297de5-Abstract.html)                                  |     OD      |     Emb.     |  /   | Merged-attn       |       Adversarial Training+MLM+MIM+ITM        |         COCO+VG+CC3M+SBU         |  2020 (NIPS)   |
|      [ViLBERT-12in1](https://openaccess.thecvf.com/content_CVPR_2020/html/Lu_12-in-1_Multi-Task_Vision_and_Language_Representation_Learning_CVPR_2020_paper.html)       | OD->Xformer |   Xformer    |  /   | Co-attn           |                  Multi Tasks                  |          Multi Datasets          |  2020 (CVPR)   |
|                                                                [CLIP](https://arxiv.org/abs/2103.00020)                                                                 | CNN/Xformer |   Xformer    |  /   | /                 |                      ITC                      |               400M               |  2021 (ICML)   |
|                                                         [ALIGN](http://proceedings.mlr.press/v139/jia21b.html)                                                          |     CNN     |   Xformer    |  /   | /                 |                      ITC                      |              1800M               |  2021 (ICML)   |
|        [VinVL](https://openaccess.thecvf.com/content/CVPR2021/html/Zhang_VinVL_Revisiting_Visual_Representations_in_Vision-Language_Models_CVPR_2021_paper.html)        |     OD      |     Emb.     |  /   | Merged-attn       |                    MLM+ITM                    |        COCO+VG+OI+OBJ365         |  2021 (CVPR)   |
|      [MDETR](https://openaccess.thecvf.com/content/ICCV2021/html/Kamath_MDETR_-_Modulated_Detection_for_End-to-End_Multi-Modal_Understanding_ICCV_2021_paper.html)      |     CNN     |   Xformer    |  √   | Merged-attn       |   OD+Token Prediction+Contrastive Alignment   |          COCO+VG+Flickr          |  2021 (ICCV)   |
|                                                         [VL-T5](https://proceedings.mlr.press/v139/cho21a.html)                                                         |     OD      |     Emb.     |  √   | Merged-attn       |       MLM+ITM+VQA+Grounding+Captioning        |             COCO+VG              |  2021 (ICML)   |
|                                                              [CLIP-VIL](https://arxiv.org/abs/2107.06383)                                                               |     CNN     |     Emb.     |  /   | Merged-attn       |                  MLM+ITM+VQA                  |           COCO+VG+VQA            |  2021 (Arxiv)  |
| [SOHO](https://openaccess.thecvf.com/content/CVPR2021/html/Huang_Seeing_Out_of_the_Box_End-to-End_Pre-Training_for_Vision-Language_Representation_CVPR_2021_paper.html) |     CNN     |     Emb.     |  /   | Merged-attn       |                  MLM+ITM+MIM                  |             COCO+VG              |  2021 (CVPR)   |
|                                                         [VILT](https://proceedings.mlr.press/v139/kim21k.html)                                                          | Patch Emb.  |     Emb.     |  /   | Merged-attn       |                    MLM+ITM                    |         COCO+VG+CC3M+SBU         |  2021 (ICCV)   |
|                                 [ALBEF](https://proceedings.neurips.cc/paper/2021/hash/505259756244493872b7709a8a01b536-Abstract.html)                                  |   Xformer   |   Xformer    |  /   | Co-attn           |                  MLM+ITM+ITC                  |        COCO+VG+CC12M+SBU         |  2021 (NIPS)   |
|                                                                [VLMO](https://arxiv.org/abs/2111.02358)                                                                 |   Xformer   |   Xformer    |  /   | Multiway-attn     |                  MLM+ITM+ITC                  |             4M/1000M             |  2021 (Arxiv)  |
|                                                              [Florence](https://arxiv.org/abs/2111.11432)                                                               |   Xformer   |   Xformer    |  /   | /                 |                      ITC                      |               900M               |  2021 (Arxiv)  |
|                                                                 [OFA](https://arxiv.org/abs/2202.03052)                                                                 |     CNN     |     Emb.     |  √   | Co-attn           |                  Multi Tasks                  |               20M                |  2022 (ICML)   |
|    [METER](https://openaccess.thecvf.com/content/CVPR2022/html/Dou_An_Empirical_Study_of_Training_End-to-End_Vision-and-Language_Transformers_CVPR_2022_paper.html)     |   Xformer   |   Xformer    |  /   | Co-attn           |                    MLM+ITM                    |         COCO+VG+CC3M+SBU         |  2022 (CVPR)   |
|                        [GLIP](https://openaccess.thecvf.com/content/CVPR2022/html/Li_Grounded_Language-Image_Pre-Training_CVPR_2022_paper.html)                         |   Xformer   |   Xformer    |  /   | Co-attn           |   OD+Token Prediction+Contrastive Alignment   |       FourODs+GoldG+Cap24M       |  2022 (CVPR)   |
|                                                               [GLIP-v2](https://arxiv.org/abs/2206.05836)                                                               |   Xformer   |   Xformer    |  /   | Co-attn           | MLM+OD+Token Prediction+Contrastive Alignment |       FourODs+GoldG+Cap24M       |  2022 (NIPS)   |
|                                                               [SimVLM](https://arxiv.org/abs/2108.10904)                                                                |     CNN     |     Emb.     |  /   | Merged-attn       |                   PrefixLM                    |              1800M               |  2022 (ICLR)   |
|                                                              [Flamingo](https://arxiv.org/abs/2204.14198)                                                               |   Xformer   |   Xformer    |  √   | Co-attn           |               ITC+Captioning+..               |          1.8B+LTIP+VTP           |  2022 (Arxiv)  |
|                                                                [PALI](https://arxiv.org/abs/2209.06794)                                                                 |   Xformer   |   Xformer    |  √   | Co-attn           |                  Multi Tasks                  | 10b image+12b text+29b image-ocr |  2022 (Arxiv)  |
|                                                                [FIBER](https://arxiv.org/abs/2206.07643)                                                                |   Xformer   |   Xformer    |  /   | Co-attn           |                  MLM+ITM+ITC                  |         COCO+VG+CC3M+SBU         |  2022 (Arxiv)  |
|                                                               [COCA](https://arxiv.org/abs/2205.01917v1)                                                                |   Xformer   |   Xformer    |  √   | Co-attn           |                ITC+Captioning                 |           JFT-3B+Align           |  2022 (Arxiv)  |
|                                                               [BEIT-3](https://arxiv.org/abs/2208.10442)                                                                |   Xformer   |   Xformer    |  /   | Co-attn           |                      MLM                      |      COCO+VG+CC3M+CC12M+SBU      |  2022 (Arxiv)  |

#### Notes:
 - *I*            : image inputs
 - *T*            : text inputs
 - **OD**         : objective detector
 - **Xformer**    : transformer
 - **Emb.**       : embedding
 - **MLM**        : masked language modeling
 - **MIM**        : masked image modeling
 - **ITM**        : image-text matching
 - **WRA**        : word-region alignment
 - **ITC**        : image-text contrastive learning



## Multimodal Adversarial Dataset
1.**CARETS: A Consistency And Robustness Evaluative Test Suite for VQA**      
(ACL 2022)[[paper](https://arxiv.org/abs/2203.07613)]

2.**VALSE: A Task-Independent Benchmark for Vision and Language Models Centered on Linguistic Phenomena**    
(ACL 2022)[[paper](https://arxiv.org/abs/2112.07566)]
