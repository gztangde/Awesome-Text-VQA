# Awesome Text VQA

Text related VQA is a fine-grained direction of the VQA task, which only focuses on the question that requires to read the textual content shown in the input image.

## Datasets
- **STE-VQA** dataset (CVPR 2020) [Project(coming soon)][[Paper](https://arxiv.org/abs/2002.10215)](Paper will be updated for camera-ready version)
- **Text-VQA** dataset (CVPR 2019) [[Project](https://textvqa.org/dataset)][[Paper](https://arxiv.org/abs/1904.08920)]
- **ST-VQA** dataset (ICCV 2019) [[Project](https://rrc.cvc.uab.es/?ch=11)][[Paper](https://arxiv.org/abs/1905.13648)]
- **OCR-VQA** dataset (ICDAR 2019) [[Project](https://ocr-vqa.github.io/)][[Paper](https://anandmishra22.github.io/files/mishra-OCR-VQA.pdf)]

| Dataset | #Train+Val Img | #Train+Val Que | #Test Img | #Test Que | Image Source | Language |
| ------- | -------------- | -------------- | --------- | --------- | ------------ | -------- |
| Text-VQA | 25,119        | 39,602         | 3,353     | 5,734     | [1]          | EN |
| ST-VQA   | 19,027        | 26,308         | 2,993     | 4,163     | [2, 3, 4, 5, 6, 7, 8] | EN |
| OCR-VQA  | 186,775       | 901,717        | 20,797    | 100,429   | [9]          | EN |
| STE-VQA  | 20,757        | 23,062         | 4,482     | 5,000     | [4, 5, 8, 10, 11, 12, 13] | EN+CH |


**Image Source**: <br>
[1] OpenImages: A public dataset for large-scale multi-label and multi-class image classification (v3) [[dataset](https://storage.googleapis.com/openimages/web/download.html)] <br>
[2] Imagenet: A large-scale hierarchical image database [[dataset](http://www.image-net.org/)] <br>
[3] Vizwiz grand challenge: Answering visual questions from blind people [[dataset](https://vizwiz.org/)] <br>
[4] ICDAR 2013 robust reading competition [[dataset](http://dagdata.cvc.uab.es/icdar2013competition/)] <br>
[5] ICDAR 2015 competition on robust reading [[dataset]()]<br>
[6] Visual Genome: Connecting language and vision using crowdsourced dense image annotations [[dataset](https://visualgenome.org/)] <br>
[7] Image retrieval using textual cues [[dataset](https://cvit.iiit.ac.in/research/projects/cvit-projects/image-retrieval-using-textual-cues)] <br>
[8] Coco-text: Dataset and benchmark for text detection and recognition in natural images [[dataset](https://vision.cornell.edu/se3/coco-text-2/)] <br>
[9] Judging a book by its cover [[dataset](https://github.com/uchidalab/book-dataset)] <br>
[10] Total Text [[dataset](https://github.com/cs-chan/Total-Text-Dataset)] <br>
[11] SCUT-CTW1500 [[dataset](https://github.com/Yuliang-Liu/Curve-Text-Detector)] <br>
[12] MLT [[dataset](https://rrc.cvc.uab.es/?ch=8)] <br>
[13] Chinese Street View Text [[dataset](https://rrc.cvc.uab.es/?ch=16)] <br>

## Related Challenges

**Document Visual Question Answering** （*CVPR 2020 Workshop on Text and Documents in the Deep Learning Era* Submission Deadline: **30 April 2020** [[Challenge]](https://rrc.cvc.uab.es/?ch=17)

## Papers

### 2020
- <a name="LoRRA"></a> **[STE-VQA]** On the General Value of Evidence, and Bilingual Scene-Text Visual Question Answering (**CVPR**) [[Paper](https://arxiv.org/abs/2002.10215)]
- <a name="M4C"></a> **[M4C]** Iterative Answer Prediction with Pointer-Augmented Multimodal Transformers for TextVQA (**CVPR**) [[Paper](https://arxiv.org/abs/1911.06258)][[Project](https://ronghanghu.com/m4c/)]

### 2019
- <a name="LoRRA"></a> **[Text-VQA/LoRRA]** Towards VQA Models That Can Read (**CVPR**) [[Paper](https://arxiv.org/abs/1904.08920)][[Code](https://github.com/facebookresearch/pythia)]
- <a name="ST-VQA"></a> **[ST-VQA]** Scene Text Visual Question Answering (**ICCV**) [[Paper](https://arxiv.org/abs/1905.13648)]
- <a name="Text-KVQA"></a>  **[Text-KVQA]** From Strings to Things: Knowledge-enabled VQA Modelthat can Read and Reason (**ICCV**) [[Paper](http://openaccess.thecvf.com/content_ICCV_2019/papers/Singh_From_Strings_to_Things_Knowledge-Enabled_VQA_Model_That_Can_Read_ICCV_2019_paper.pdf)]
- <a name="OCR-VQA"></a> **[OCR-VQA]** OCR-VQA: Visual Question Answering by Reading Text in Images (**ICDAR**) [[Paper](https://anandmishra22.github.io/files/mishra-OCR-VQA.pdf)]


### Technical Reports

- <a name="DiagNet"></a> **[DiagNet]** DiagNet: Bridging Text and Image [[Report](http://www-personal.umich.edu/~syqian/2019/diagnet/diagnet.pdf)][[Code](https://github.com/w-yi/DiagNet)]
- <a name="DCD-ZJU"></a> **[DCD_ZJU]** Winner of 2019 Text-VQA challenge [[Slides](https://drive.google.com/file/d/1EZ8jrLTPLLKfwi0K28zq89tTe3ZZ-X8j/view)]
- <a name="Schwail"></a> **[Schwail]** Runner-up of 2019 Text-VQA challenge [[Slides](https://drive.google.com/file/d/1xNiEHj6J42F3CFx6fYjS9KDTsYTqAlN0/view)]


## Benchmark
**Acc.** : Accuracy
**I. E.** : Image Encoder 
**Q. E.** : Question Encoder
**O. E.** : OCR Token Encoder
**Ensem.** : Ensemble

**Only methods that have public available paper/code/description are listed here**

### Text-VQA

[[official leaderboard](https://evalai.cloudcv.org/web/challenges/challenge-page/244/leaderboard/810)]

| Y-C./J. | Methods| Acc. | I. E. |  Q. E. | OCR | O. E. | Output | Ensem. |
| ------- | ------ | ---- | ----- | -------| --- | ----- | ------ | ------ |
| 2019--CVPR | [LoRRA](#LoRRA) | 26.64 | Faster R-CNN | GloVe | Rosetta-ml | FastText | Classification | N |
| 2019--N/A| [DCD_ZJU](#DCD-ZJU) | 31.44 | Faster R-CNN | BERT | Rosetta-ml | FastText | Classification | Y |
| 2019--arXiv | [M4C](#M4C) | **40.46** | Faster R-CNN | BERT | Rosetta-en | FastText | Decoder | N |

### ST-VQA

[[official leaderboard](https://rrc.cvc.uab.es/?ch=11&com=evaluation&task=1)] <br>
**T1** : Strongly Contextualised Task
**T2** : Weakly Contextualised Task
**T3** : Open Dictionary

| Y-C./J. | Methods| Acc. (T1/T2/T3) | I. E. |  Q. E. | OCR | O. E. | Output | Ensem. |
| ------- | ------ | --------------- | ----- | -------| --- | ----- | ------ | ------ |
| 2019--arXiv | [M4C](#M4C) | **na/na/0.4621** | Faster R-CNN | BERT | Rosetta-en | FastText | Decoder | N |

### OCR-VQA

| Y-C./J. | Methods| Acc. | I. E. |  Q. E. | OCR | O. E. | Output | Ensem. |
| ------- | ------ | ---- | ----- | -------| --- | ----- | ------ | ------ |
| 2019--arXiv | [M4C](#M4C) | **63.9** | Faster R-CNN | BERT | Rosetta-en | FastText | Decoder | N |

