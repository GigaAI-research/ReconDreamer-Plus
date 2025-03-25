<div align="center">   
  
# ReconDreamer++: Harmonizing Generative and Reconstructive Models for Driving Scene Representation
</div>

 
## [Project Page](https://recondreamer-plus.github.io/) | [Paper](https://arxiv.org/abs/2503.18438)

# News
- **[2025/03/24]** Repository Initialization.

# Abstract 

Combining reconstruction models with generative models has emerged as a promising paradigm for closed-loop simulation in autonomous driving. For example, ReconDreamer has demonstrated remarkable success in rendering large-scale maneuvers. However, a significant gap remains between the generated data and real-world sensor observations, particularly in terms of fidelity for structured elements, such as the ground surface. To address these challenges, we propose **ReconDreamer++**, an enhanced framework that significantly improves the overall rendering quality by mitigating the domain gap and refining the representation of the ground surface. Specifically, **ReconDreamer++** introduces the Novel Trajectory Deformable Network (NTDNet), which leverages learnable spatial deformation mechanisms to bridge the domain gap between synthesized novel views and original sensor observations. Moreover, for structured elements such as the ground surface, we preserve geometric prior knowledge in 3D Gaussians, and the optimization process focuses on refining appearance attributes while preserving the underlying geometric structure. Experimental evaluations conducted on multiple datasets (Waymo, nuScenes, PandaSet, and EUVS) confirm the superior performance of **ReconDreamer++**. Specifically, on Waymo, **ReconDreamer++** achieves performance comparable to Street Gaussians for the original trajectory while significantly outperforming ReconDreamer on novel trajectories. In particular, it achieves substantial improvements, including a 6.1% increase in NTA-IoU, a 23. 0% improvement in FID, and a remarkable 4.5% gain in the ground surface metric NTL-IoU, highlighting its effectiveness in accurately reconstructing structured elements such as the road surface.

![key_feature](https://github.com/user-attachments/assets/f591726c-a316-4373-97d9-b38ae4fd087e)

Comparison of ReconDreamer++ with SOTA methods, Street Gaussians and ReconDreamer, on original and novel trajectories. **Left**: ReconDreamer++ demonstrates superior rendering performance for both vehicle foregrounds and road surfaces compared to existing SOTA methods. **Right**: ReconDreamer++ significantly improves performance on novel trajectories while maintaining high rendering quality on the original trajectory.

# ReconDreamer++ Framework

![framework](https://github.com/user-attachments/assets/5d673deb-3dc3-4b41-86af-970e17022644)

# Rendering Results on Various Datasets
<div align="center">
    <h1 style="font-size: 32px;">Waymo</h1>
</div>

<div align="center">
    Original Trajectory
</div>

https://github.com/user-attachments/assets/0d5224f0-4659-4020-9622-90d2ca7d60ef

<div align="center">
    Lane Shift @ 3m
</div>

https://github.com/user-attachments/assets/7e50b97b-3553-4cef-a6c0-45447db77c6f

<div align="center">
    Lane Shift @ 6m
</div>

https://github.com/user-attachments/assets/565ddc44-5727-439e-abc9-85a49d5376c7

<div align="center">
    <h1 style="font-size: 32px;">nuScenes</h1>
</div>


<div align="center">
    Original Trajectory
</div>

https://github.com/user-attachments/assets/794ec6a8-0734-415a-8ede-dccfe15b3f77

<div align="center">
    Lane Shift @ 3m
</div>

https://github.com/user-attachments/assets/aea28c7a-7e15-4824-b55b-f47682f7a3e5

<div align="center">
    Lane Shift @ 6m
</div>

https://github.com/user-attachments/assets/38ba2c22-2766-414d-9c77-46472f4b2869

<div align="center">
    <h1 style="font-size: 32px;">PandaSet</h1>
</div>


<div align="center">
    Original Trajectory
</div>

https://github.com/user-attachments/assets/5350ec74-2431-448e-a99b-86bf747b55bc

<div align="center">
    Lane Shift @ 2m
</div>

https://github.com/user-attachments/assets/6e0f615f-397c-4f3b-8b1e-45fc2f6ecdcc

<div align="center">
    Lane Shift @ 3m
</div>

https://github.com/user-attachments/assets/18284e72-125a-49f8-b038-02b25590283c

<div align="center">
    <h1 style="font-size: 32px;">EUVS</h1>
</div>


<div align="center">
    Train Set
</div>

https://github.com/user-attachments/assets/c999ee1a-d057-4eae-8729-d06243c85edf

<div align="center">
    Test Set
</div>

https://github.com/user-attachments/assets/3b03eae7-d2e1-402b-9e48-aa4cc16106c1

# Ablation Studies on depth loss, ground model and NTDNet.

<div align="center">
    Original Trajectory
</div>

https://github.com/user-attachments/assets/85baee2c-0405-407e-964b-68d3854e4a72

<div align="center">
    Lane Shift @ 3m
</div>

https://github.com/user-attachments/assets/ba386e2c-cf68-434e-9416-c7a1d283d062

<div align="center">
    Lane Shift @ 6m
</div>

https://github.com/user-attachments/assets/22c59e46-4f1e-480e-b9a9-8f832591406e

# Acknowledgements
We would like to thank the following works and projects, for their open research and exploration: [DriveStudio](https://github.com/ziyc/drivestudio), [DriveDreamer](https://github.com/JeffWang987/DriveDreamer), 
[DriveDreamer-2](https://github.com/f1yfisher/DriveDreamer2), [DriveDreamer4D](https://github.com/GigaAI-research/DriveDreamer4D), [ReconDreamer](https://github.com/GigaAI-research/ReconDreamer).

# Bibtex
If this work is helpful for your research, please consider citing the following BibTeX entry.

```
@inproceedings{zhao2025recon,
    title={ReconDreamer++: Harmonizing Generative and Reconstructive Models for Driving Scene Representation}, 
    author={Guosheng Zhao and Xiaofeng Wang and Chaojun Ni and Zheng Zhu and and Wenkang Qin and Guan Huang and Xingang Wang},
    journal={arxiv arXiv preprint arXiv:2503.18438},
    year={2025},
}


