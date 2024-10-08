# DreamLIP-DATA
license: cc-by-4.0
task_categories:
- text-to-image
- zero-shot-classification
language:
- en
size_categories:
- 10M<n<100M
---
# Dataset Card for DreamLIP-30M

<table><tbody>
<!-- START TABLE -->
<!-- TABLE HEADER -->
<th valign="center">Raw/Long/Short Caption</th>
<th valign="center">Huggingface Dataset</th>

<!-- TABLE BODY -->
<tr>
<td align="center">CC3M+YFCC15M+CC12M</td>
<td align="center"><a href="https://huggingface.co/datasets/qidouxiong619/dreamlip_long_captions">Link</a></td>
</tr>
</tbody></table>


## Table of Contents
- [Dataset Description](#dataset-description)
  - [Dataset Summary](#dataset-summary)
- [Additional Information](#additional-information)
  - [Dataset Curators](#dataset-curators)
  - [Licensing Information](#licensing-information)
  - [Citation Information](#citation-information)

## Dataset Description

- **Homepage:** [DreamLIP homepage](https://zyf0619sjtu.github.io/dream-lip/)
- **Repository:** [DreamLIP repository](https://github.com/zyf0619sjtu/DreamLIP)
- **Paper:** [DreamLIP: Language-Image Pre-training with Long Captions](https://arxiv.org/pdf/2403.17007)

### Dataset Summary

DreamLIP-Long-Captions is a dataset consisting of ~30M image annotations, i.e. detailed long captions. In contrast with the curated style of other synthetic image caption annotations, DreamLIP-30M utilizes pre-trained Multi-modality Large Language Model to obtain detailed descriptions with an average length of 247. More precisely, the detailed descriptions are generated by asking the ShareGPT4V/InstructBLIP/LLava1.5 the question "Describe the image in detail". Meanwhile, we also provide the generated short caption by prompting "Describe the image in one sentence". The question of detailed long captions has little impact on the diversity of answers, so we can obtain comprehensive captions of each image.  

## Additional Information

### Dataset Curators

Kecheng Zheng, Yifei Zhang, Wei Wu, Fan Lu, Shuailei Ma, Xin Jin, Wei Chen and Yujun Shen.

### Licensing Information

We distribute the image url with long captions under a standard Creative Common CC-BY-4.0 license. The individual images are under their own copyrights.

### Citation Information

```bibtex
@inproceedings{DreamLIP,
  title={DreamLIP: Language-Image Pre-training with Long Captions},
  author={Zheng, Kecheng and Zhang, Yifei and Wu, Wei and Lu, Fan and Ma, Shuailei and Jin, Xin and Chen, Wei and Shen, Yujun},
  booktitle={ECCV},
  year={2024}
}
```

### Acknowledgements
This dataset is based on [CC3M](https://huggingface.co/datasets/pixparse/cc3m-wds), and thanks for the nice work! 
We also thank [InstructBLIP](https://github.com/salesforce/LAVIS), [ShareGPT4V](https://github.com/InternLM/InternLM-XComposer) and [LLAVA](https://github.com/haotian-liu/LLaVA) for the pretrained models.
