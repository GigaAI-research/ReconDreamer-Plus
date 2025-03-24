
<div align="center">   
  
# ReconDreamer++: Harmonizing Generative and Reconstructive Models for Driving Scene Representation
</div>

 
## [Project Page](https://recondreamer-plus.github.io/) | [Paper]()

# News
- **[2025/03/24]** Repository Initialization.

# Abstract 

Combining reconstruction models with generative models has emerged as a promising paradigm for closed-loop simulation in autonomous driving. For example, ReconDreamer has demonstrated remarkable success in rendering large-scale maneuvers. However, a significant gap remains between the generated data and real-world sensor observations, particularly in terms of fidelity for structured elements, such as the ground surface. To address these challenges, we propose **ReconDreamer++**, an enhanced framework that significantly improves the overall rendering quality by mitigating the domain gap and refining the representation of the ground surface. Specifically, **ReconDreamer++** introduces the Novel Trajectory Deformable Network (NTDNet), which leverages learnable spatial deformation mechanisms to bridge the domain gap between synthesized novel views and original sensor observations. Moreover, for structured elements such as the ground surface, we preserve geometric prior knowledge in 3D Gaussians, and the optimization process focuses on refining appearance attributes while preserving the underlying geometric structure. Experimental evaluations conducted on multiple datasets (Waymo, nuScenes, PandaSet, and EUVS) confirm the superior performance of **ReconDreamer++**. Specifically, on Waymo, **ReconDreamer++** achieves performance comparable to Street Gaussians for the original trajectory while significantly outperforming ReconDreamer on novel trajectories. In particular, it achieves substantial improvements, including a 6.1% increase in NTA-IoU, a 23. 0% improvement in FID, and a remarkable 4.5% gain in the ground surface metric NTL-IoU, highlighting its effectiveness in accurately reconstructing structured elements such as the road surface.

# ReconDreamer++ Framework


# Key Feature


Comparison of ReconDreamer++ with SOTA methods, Street Gaussians and ReconDreamer, on original and novel trajectories. **Left**: ReconDreamer++ demonstrates superior rendering performance for both vehicle foregrounds and road surfaces compared to existing SOTA methods. **Right**: ReconDreamer++ significantly improves performance on novel trajectories while maintaining high rendering quality on the original trajectory.

# Rendering Results on Various Datasets
<div align="center">
    <h1 style="font-size: 32px;">Waymo</h1>
</div>


<div align="center">
    Original Trajectory
</div>



<div align="center">
    Lane Shift @ 3m
</div>



<div align="center">
    Lane Shift @ 6m
</div>




<div align="center">
    <h1 style="font-size: 32px;">nuScenes</h1>
</div>


<div align="center">
    Original Trajectory
</div>



<div align="center">
    Lane Shift @ 3m
</div>



<div align="center">
    Lane Shift @ 6m
</div>



<div align="center">
    <h1 style="font-size: 32px;">PandaSet</h1>
</div>


<div align="center">
    Original Trajectory
</div>



<div align="center">
    Lane Shift @ 2m
</div>



<div align="center">
    Lane Shift @ 3m
</div>


<div align="center">
    Vertical Shift @ 1m
</div>



<div align="center">
    <h1 style="font-size: 32px;">EUVS</h1>
</div>


<div align="center">
    Train Set
</div>



<div align="center">
    Test
</div>


# Acknowledgements
We would like to thank the following works and projects, for their open research and exploration: [DriveStudio](https://github.com/ziyc/drivestudio), [DriveDreamer](https://github.com/JeffWang987/DriveDreamer), 
[DriveDreamer-2](https://github.com/f1yfisher/DriveDreamer2), [DriveDreamer4D](https://github.com/GigaAI-research/DriveDreamer4D), [ReconDreamer](https://github.com/GigaAI-research/ReconDreamer).

<!-- # Bibtex
If this work is helpful for your research, please consider citing the following BibTeX entry.

```
@inproceedings{zhao2024drive,
    title={DriveDreamer4D: World Models Are Effective Data Machines for 4D Driving Scene Representation}, 
    author={Guosheng Zhao and Chaojun Ni and Xiaofeng Wang and Zheng Zhu and Xueyang Zhang and Yida Wang and Guan Huang and Xinze Chen and Boyuan Wang and Youyi Zhang and Wenjun Mei and Xingang Wang},
    journal={arxiv arXiv preprint arXiv:2410.13571},
    year={2024},
} -->


