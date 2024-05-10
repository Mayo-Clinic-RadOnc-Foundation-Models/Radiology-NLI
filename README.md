# RadQNLI
The repository is for the paper: [Exploring the Trade-Offs: Unified Large Language Models vs Local Fine-Tuned Models for Highly-Specific Radiology NLI Task](https://arxiv.org/abs/2304.09138), including the code and dataset for reproducing. 

The paper is under revision on IEEE-TBD.

## Pipeline of RadQNLI
<img src="figs/main.png"/>
Fig. 1: Overview of our workflow. (a) Top panel: Conversion of RadQA dataset to RadQNLI dataset. The highlighted sentence in the context contains the answer to the question. (b) Bottom panel: Utilization of ChatGPT to perform the Natural Language Inference (NLI) task on the generated RadQNLI dataset.


## Prerequisites

[litgpt]([https://github.com/ultralytics/ultralytics](https://github.com/Lightning-AI/litgpt)) repository for LLaMA family evaluation;
```
 pip install 'litgpt[all]'
```


## Getting Started
See [GANs](GAN/GAN)


## Dataset Download
The dataset has been released on [Kaggle](https://www.kaggle.com/datasets/zhengkunli3969/dtmars-cyclegan). Also, you can download on [Google Drive](https://drive.google.com/drive/folders/12pb47Zl1j285z5AXG8F77oASkfYqSbA0?usp=sharing).



## Models' Responds
The models' responds are available at [weight](weight).  
    - best.pt: trained with images generated from DT/MARs-CycleGAN (ours).  
    - CYC.pt: trained with  images generated from original CycleGAN.  
    - RetinaGAN.pt: trained with images generated from RetinaGAN.  
    - pure_sim.pt: trained with images generated from Publlet.  

## References
If you find this work or code useful, please cite:

```
@article{wu2023exploring,
  title={Exploring the trade-offs: Unified large language models vs local fine-tuned models for highly-specific radiology nli task},
  author={Wu, Zihao and Zhang, Lu and Cao, Chao and Yu, Xiaowei and Dai, Haixing and Ma, Chong and Liu, Zhengliang and Zhao, Lin and Li, Gang and Liu, Wei and others},
  journal={arXiv preprint arXiv:2304.09138},
  year={2023}
}
```
