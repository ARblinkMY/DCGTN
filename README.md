# DCGTN: Dynamic causal graph transformer network for UAV-borne hyperspectral image classification
## Abstract
UAV-borne hyperspectral image (HSI) classification is challenging because low-altitude imaging often leads to 
complex local spatial patterns, noticeable scale changes, and severe background interference. As a result, local 
evidence alone is often insufficient for reliable recognition, making it necessary to model contextual dependencies beyond small neighborhoods. Although Transformer-based methods can capture spectral–spatial interactions 
beyond fixed receptive fields, their token dependencies are still primarily learned from data-driven correlations 
rather than explicitly structured relations. In complex UAV scenes, such correlation-driven dependencies may 
become sensitive to incidental co-occurrences and appearance changes under varying acquisition conditions, 
thereby limiting the stability of contextual modeling. To address this issue, we propose a Dynamic Causal Graph 
Transformer Network (DCGTN), a causality-inspired dynamic graph Transformer framework for UAV-borne HSI 
classification. Specifically, a Dynamic Causal Structure Learner (DCSL) is first designed to infer sparse causal 
adjacency matrices under varying spatial contexts, providing an explicit causality-inspired structural prior for contextual modeling. Then, based on the learned structural prior, an Intervention-Augmented Graph Attention (IAGA) 
module is introduced to alleviate the influence of unstable source-node messages during feature propagation. 
Moreover, a Multi-Scale Causal Feature Pyramid (MCFP) is constructed to progressively capture discriminative 
dependencies from local details to broader scene layouts. Experiments on three representative UAV-borne HSI 
datasets demonstrate that DCGTN achieves stable and competitive classification performance compared with 
several representative baselines, validating the effectiveness of the proposed method for robust UAV-borne HSI 
classification.
<img width="3667" height="2176" alt="fig1" src="https://github.com/user-attachments/assets/e8df5e22-3aa4-4b55-a845-d76dbaf1282f" />

## Citation
If this code is useful for your research, please cite this paper.
```
@article{tang2026dcgtn,
  title={DCGTN: Dynamic causal graph transformer network for UAV-borne hyperspectral image classification},
  author={Tang, Haojin and Cai, Anning and Zhou, Weixuan and Yang, Xiaofei and Ban, Yifang and Peng, Jiangtao},
  journal={Optics \& Laser Technology},
  volume={204},
  pages={116809},
  year={2026},
  publisher={Elsevier},
}
