<div align="center">  <img src='assets/logo.png' style="height:250px"></img>  </div>

<div align="center">
<h1>SPF-Portrait: Towards Pure Portrait Customization with Semantic Pollution-Free Fine-tuning</h1>

[**Xiaole Xian**](https://scholar.google.com/citations?user=XpaHZywAAAAJ&hl=zh-CN)<sup> * ♰ 1</sup> · [**Zhichao Liao**](https://lzc-sg.github.io/)<sup>* ♰ 2</sup> · [Qingyu Li]()<sup>3</sup> · [Wenyu Qin]()<sup>3</sup> · [Pengfei Wan]()<sup>3</sup> · [Weicheng Xie]()<sup>1✉</sup> · [Long Zeng]()<sup>2 ✉</sup> · [Linlin Shen]()<sup>1</sup> · [Pingfa Feng]()<sup>2</sup>

<sup>1</sup>Shenzhen University · <sup>2</sup>Tsinghua University · <sup>3</sup>Kuaishou Technology

<sup>*</sup>Equal contributions · <sup>♰</sup> Internship at KwaiVGI, Kuaishou Technology · <sup>✉</sup>Corresponding authors 

<a href='https://spf-portrait.github.io/SPF-Portrait/'><img src='https://img.shields.io/badge/Project-Page-green'></a>  &nbsp; 
<a href='https://arxiv.org/abs/2504.00396'><img src='https://img.shields.io/badge/arXiv-SPF Portrait-red'></a>  &nbsp; 
<a href="https://github.com/KwaiVGI/SPF-Portrait"><img src="https://img.shields.io/badge/GitHub-SPF Portrait-9E95B7?logo=github"></a> &nbsp; 
<br>
[![Hugging Face](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Models-blue)](https://huggingface.co/)  &nbsp; 
[![Hugging Face](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-App-red)](https://huggingface.co/)  &nbsp; 
[![GitHub](https://img.shields.io/github/stars/KwaiVGI/SPF-Portrait?style=social)](https://github.com/KwaiVGI/SPF-Portrait) &nbsp; 
</div>
  
##  🔥 Updates 

- [x] **`2025/04/02`**: 🔥 We released the technical report on [arXiv](https://arxiv.org/pdf/2504.00396).

##   💪 Plan 

- [x] Technical report
- [ ] Inference code
- [ ] Pre-trained weight for inference [SDv1.5] in Huggingface Model🤗
- [ ] Demo deployment in Huggingface Space🤗
- [ ] Training code

（Thanks for your attention! The checkpoints and codes are coming soon!）

## 📖 Abstract 
Fine-tuning a pre-trained Text-to-Image (T2I) model on a tailored portrait dataset is the mainstream method for text-to-portrait customization.
However, existing methods often severely impact the original model’s behavior (e.g., changes in ID, layout, etc.) while customizing portrait attributes.
To address this issue, we propose SPF-Portrait, a pioneering work to purely understand customized target semantics and minimize disruption to the original model.
In our SPF-Portrait, we design a dual-path contrastive learning pipeline, which introduces the original model as a behavioral alignment reference for the conventional fine-tuning path.
During the contrastive learning, we propose a novel Semantic-Aware Fine Control Map that indicates the intensity of response regions of the target semantics, to spatially guide the alignment process between the contrastive paths.
It adaptively balances the behavioral alignment across different regions and the responsiveness of the target semantics.
Furthermore, we propose a novel response enhancement mechanism to reinforce the presentation of target semantics, while mitigating representation discrepancy inherent in direct cross-modal supervision.
Through the above strategies, we achieve incremental learning of customized target semantics for pure text-to-portrait customization.
Extensive experiments show that SPF-Portrait achieves state-of-the-art performance. 


## 💻 Pipeline

<p align="center">
  <img src="assets/pipeline.jpg">
</p>

## 🚅 Capabilities 

  🔥 Our SPF-Portrait achieves **human attributes adaption of T2I model without pollution of the original capability**.

  🔥 For more results, visit our <a href="https://spf-portrait.github.io/SPF-Portrait/"><strong>homepage</strong></a>

<p align="center">
  <img src="assets/teaser.jpg">
</p>

## 💖 Citation

If you find SPF-Portrait useful for your research, welcome to 🌟 this repo and cite our work using the following BibTeX:

```bibtex
@article{xian2025spf,
  title={SPF-Portrait: Towards Pure Portrait Customization with Semantic Pollution-Free Fine-tuning},
  author={Xian, Xiaole and Liao, Zhichao and Li, Qingyu and Qin, Wenyu and Wan, Pengfei and Xie, Weicheng and Zeng, Long and Shen, Linlin and Feng, Pingfa},
  journal={arXiv preprint arXiv:2504.00396},
  year={2025}
}
```
