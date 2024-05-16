A curated list of papers and open-source resources focused on 3D Scene Understanding. Most Attention are payed to **NeRF-based** and **3DGS-based** methods. Othe classic representations that I found interesting are also listed here.

## Table of Content
- [Table of Content](#table-of-content)
- [Semantic NVS](#semantic-nvs)
  - [Scene-Specific(Indoor)](#scene-specificindoor)
  - [Scene-Specific(Outdoor)](#scene-specificoutdoor)
  - [Generalization](#generalization)
- [Semantic Reconstrucion](#semantic-reconstrucion)
- [Semantic SLAM](#semantic-slam)
- [Scene Decomposition](#scene-decomposition)
  - [Indoor Scene](#indoor-scene)
  - [Outdoor Scene](#outdoor-scene)
- [3D Segmentation Using SAM](#3d-segmentation-using-sam)
  - [Object Segmentation](#object-segmentation)
  - [Instance Segmentation](#instance-segmentation)
  - [Hierarchical Segmentation](#hierarchical-segmentation)
- [Multi-Model](#multi-model)


## Semantic NVS
Reconstruct 3D scene with accurate semantics but without accurate surface representation:
### Scene-Specific(Indoor)
- 🔥**In-Place Scene Labelling and Understanding with Implicit Scene Representation**, Shuaifeng Zhi et al, ICCV2021 (<font color="#e36c09">Oral</font>) | [arXiv](https://arxiv.org/abs/2103.15875) | [project](https://shuaifengzhi.com/Semantic-NeRF/) | [code](https://github.com/Harry-Zhi/semantic_nerf/)
- **Panoptic Lifting for 3D Scene Understanding with Neural Fields**, Yawar Siddiqui, CVPR2023 (<font color="#e36c09">Highlight</font>) | [arXiv](https://arxiv.org/abs/2212.09802) | [project](https://nihalsid.github.io/panoptic-lifting/) | [code](https://github.com/nihalsid/panoptic-lifting)
- 🔥**Contrastive Lift: 3D Object Instance Segmentation by Slow-Fast Contrastive Fusion**, Yash Bhalgat et al, NIPS2023 (<font color="#e36c09">Spotlight</font>) | [arXiv](https://arxiv.org/abs/2306.04633) | [project](https://www.robots.ox.ac.uk/~vgg/research/contrastive-lift/) | [code](https://github.com/yashbhalgat/Contrastive-Lift)

### Scene-Specific(Outdoor)
- **Panoptic NeRF: 3D-to-2D Label Transfer for Panoptic Urban Scene Segmentation**, Xiao Fu et al, 3DV 2022 | [arXiv](https://arxiv.org/abs/2203.15224) | [project](https://fuxiao0719.github.io/projects/panopticnerf/) | [code](https://github.com/fuxiao0719/panopticnerf)
- **Panoptic Neural Fields: A Semantic Object-Aware Neural Scene Representation**, Abhijit Kundu et al, CVPR2022 | [arXiv](https://arxiv.org/abs/2205.04334.pdf) | [project](https://abhijitkundu.info/projects/pnf/)
- 🔥**Nerflets: Local Radiance Fields for Efficient Structure-Aware 3D Scene Representation from 2D Supervision**, Xiaoshuai Zhang et al, CVPR2023 | [arXiv](https://arxiv.org/abs/2303.03361) | [project](https://jetd1.github.io/nerflets-web/)
- **Aerial Lifting: Neural Urban Semantic and Building Instance Lifting from Aerial Imagery**, Yuqi Zhang et al, CVPR2024 | [arXiv](https://arxiv.org/abs/2403.11812) | [project](https://zyqz97.github.io/Aerial_Lifting/) | [code](https://github.com/zyqz97/Aerial_lifting)

### Generalization
- **NeSF: Neural Semantic Fields for Generalizable Semantic Segmentation of 3D Scenes**, Suhani Vora et al, TMLR 2022 | [arXiv](https://arxiv.org/pdf/2111.13260) | [project](https://nesf3d.github.io/) | [code](https://github.com/google-research/jax3d/tree/main/jax3d/projects/nesf)
- **Semantic Ray: Learning a Generalizable Semantic Field with Cross-Reprojection Attention**, Fangfu Liu et al, CVPR2023 | [arXiv](https://arxiv.org/abs/2303.13014) | [project](https://liuff19.github.io/S-Ray/) | [code](https://github.com/liuff19/Semantic-Ray)
- 🔥**GNeSF: Generalizable Neural Semantic Fields**, Hanlin Chen et al, NIPS2023 | [code](https://github.com/HLinChen/GNeSF)
## Semantic Reconstrucion
Reconstruct 3D scene with accurate semantics and <span style="background:#fff88f">accurate</span> surface. Most of work below are also able to render 2D semantic images:
- 🔥**Neural 3D Scene Reconstruction with the Manhattan-world Assumption**, Haoyu Guo et al, CVPR2022 (<font color="#e36c09">Oral</font>) | [arXiv](https://arxiv.org/abs/2205.02836) | [project](https://zju3dv.github.io/manhattan_sdf/) | [code](https://github.com/zju3dv/manhattan_sdf)
- **Fast Monocular Scene Reconstruction with Global-Sparse Local-Dense Grids**, Wei Dong et al, CVPR2023 | [arXiv](https://arxiv.org/abs/2305.13220) | [project](https://dongwei.info/publication/ash-mono/) | [code](https://github.com/theNded/torch-ash) 

## Semantic SLAM
- **iLabel: Revealing Objects in Neural Fields**, Shauifeng Zhi et al, RA-L2022 | [arXiv](https://arxiv.org/abs/2111.14637)
- **Neural Implicit Dense Semantic SLAM**, Yasaman Haghigh et al, arXiv2023 | [arXiv](https://arxiv.org/pdf/2304.14560.pdf)
- **DNS SLAM: Dense Neural Semantic-Informed SLAM**, Kunyi Li et al, arXiv 2023 | [arXiv](https://arxiv.org/abs/2312.00204)
- 🔥**SNI-SLAM: Semantic Neural Implicit SLAM**, Siting Zhu et al, CVPR2024 | [arXiv](https://arxiv.org/pdf/2311.11016) | [code](https://github.com/IRMVLab/SNI-SLAM)

## Scene Decomposition
### Indoor Scene
Reconstrucion 3D scenes using a <span style="background:#fff88f">object-compositional</span> representation. Most of work below are able to render 2D semantic/instance images and achieve 3D semantic/instance segmentation:
- **Learning Object-Compositional Neural Radiance Field for Editable Scene Rendering**, Bangbang Yang et al, ICCV 2021 | [arXiv](https://arxiv.org/pdf/2109.01847) | [project](https://zju3dv.github.io/object_nerf/) | [code](https://github.com/zju3dv/object_nerf)
- **Object-Compositional Neural Implicit Surfaces**, QianYi Wu et al, ECCV2022 | [arXiv](http://arxiv.org/abs/2207.09686) | [project](https://wuqianyi.top/objectsdf/) | [code](https://github.com/QianyiWu/objsdf)
- 🔥**vMAP: Vectorised Object Mapping for Neural Field SLAM**, Xin Kong et al, CVPR2023 | [arXiv](https://arxiv.org/abs/2302.01838) | [project](https://kxhit.github.io/vMAP) | [code](https://github.com/kxhit/vMAP)
- 🔥**Panoptic Compositional Feature Field for Editable Scene Rendering with Network-Inferred Labels via Metric Learning**, Xinhua Cheng et al, CVPR2023 | [paper](https://openaccess.thecvf.com/content/CVPR2023/papers/Cheng_Panoptic_Compositional_Feature_Field_for_Editable_Scene_Rendering_With_Network-Inferred_CVPR_2023_paper.pdf)
- **DM-NeRF: 3D Scene Geometry Decomposition and Manipulation from 2D Images**, Bing Wang et al, ICLR2023 | [arXiv](https://arxiv.org/abs/2208.07227) | [code](https://github.com/vLAR-group/DM-NeRF)
- **RICO: Regularizing the Unobservable for Indoor Compositional Reconstruction**, Zizhang Li et al, ICCV2023 | [arXiv](https://arxiv.org/abs/2303.08605) | [code](https://github.com/kyleleey/RICO)
- 🔥**ObjectSDF++: Improved Object-Compositional Neural Implicit Surfaces**, Qianyi Wu et al, ICCV2023 | [arXiv](http://arxiv.org/abs/2308.07868) | [project](https://wuqianyi.top/objectsdf++) | [code](https://github.com/QianyiWu/objectsdf_plus)
- 🔥**ClusteringSDF: Self-Organized Neural Implicit Surfaces for 3D Decomposition**, Tianhao Wu et al, arXiv 2024 | [arXiv](https://arxiv.org/abs/2403.14619) | [project](https://sm0kywu.github.io/ClusteringSDF/)
- 🔥**Total-Decom: Decomposed 3D Scene Reconstruction with Minimal Interaction**, Xiaoyang Lyu et al, CVPR2024 | [arXiv](https://arxiv.org/pdf/2403.19314.pdf) | [project](https://cvmi-lab.github.io/Total-Decom/)

### Outdoor Scene
- **Panoptic Neural Fields: A Semantic Object-Aware Neural Scene Representation**, Abhijit Kundu et al, CVPR2022 | [arXiv](https://arxiv.org/abs/2205.04334.pdf) | [project](https://abhijitkundu.info/projects/pnf/)

## 3D Segmentation Using SAM
### Object Segmentation
- **NeRF-SOS: Any-View Self-supervised Object Segmentation on Complex Scenes**, Ziwen Fan et al, | [arXiv](https://arxiv.org/abs/2209.08776) | [project](https://zhiwenfan.github.io/NeRF-SOS/) | [code](https://github.com/VITA-Group/NeRF-SOS)
- 🔥**Segment Anything in 3D with NeRFs**, Jiazhong Cen et al, NIPS2023 | [arXiv](https://arxiv.org/abs/2304.12308) | [project](https://jumpat.github.io/SA3D/) | [code](https://github.com/Jumpat/SegmentAnythingin3D)

### Instance Segmentation
- **Mask3D: Mask Transformer for 3D Semantic Instance Segmentation**, Jonas Schult et al, ICRA2023 | [arXiv](https://arxiv.org/abs/2210.03105) | [project](https://jonasschult.github.io/Mask3D/) | [code](https://github.com/JonasSchult/Mask3D)
- 🔥**SAM3D: Segment Anything in 3D Scenes**, Yunhan Yang et al, ICCV'23 Workshop | [arXiv](https://arxiv.org/abs/2306.03908) | [code](https://github.com/Pointcept/SegmentAnything3D) 
- **SAMPro3D: Locating SAM Prompts in 3D for Zero-Shot Scene Segmentation**, Muyuan Xu et al, arXiv2023 | [arXiv](https://arxiv.org/abs/2311.17707) | [project](https://mutianxu.github.io/sampro3d/) | [code](https://github.com/GAP-LAB-CUHK-SZ/SAMPro3D)
- 🔥**SAM-guided Graph Cut for 3D Instance Segmentation**, Haoyu Guo et al, arXiv2023 | [arXiv](https://arxiv.org/abs/2312.08372) | [project](https://zju3dv.github.io/sam_graph/) | [code](https://github.com/zju3dv/SAM-Graph)
- **SAI3D: Segment Any Instance in 3D Scenes**, Yingda Yin et al, CVPR2024 | [arXiv](https://arxiv.org/abs/2312.11557) | [project](https://yd-yin.github.io/SAI3D/) | [code](https://github.com/yd-yin/SAI3D)

### Hierarchical Segmentation
- 🔥**OmniSeg3D: Omniversal 3D Segmentation via Hierarchical Contrastive Learning**, Haiyang Ying et al, CVPR2024 | [arXiv](https://arxiv.org/abs/2311.11666) | [project](https://oceanying.github.io/OmniSeg3D/) | [code](https://github.com/THU-luvision/OmniSeg3D)
- 🔥**GARField: Group Anything with Radiance Fields**, Chung Min Kim et al, CVPR2024 | [arXiv](https://arxiv.org/abs/2401.09419) | [project](https://www.garfield.studio/) | [code](https://github.com/chungmin99/garfield) 

## Multi-Model
Recontruct 3D <span style="background:#fff88f">CLIP/DINO feature fields</span> of scene. Most of thes works are able to achieve 3D open-vocabulary segmentation.
- **Neural Feature Fusion Fields: 3D Distillation of Self-Supervised 2D Image Representations**, Vadim Tschernezki et al, 3DV2022(<font color="#e36c09">Oral</font>) | [arXiv](- [arXiv](https://arxiv.org/abs/2209.03494)) | [project](https://www.robots.ox.ac.uk/~vadim/n3f/) | [code](https://github.com/dichotomies/N3F)
- **Decomposing NeRF for Editing via Feature Field Distillation**, Sosuke Kobayashi et al, NIPS2022 | [arXiv](https://arxiv.org/abs/2205.15585) | [project](https://pfnet-research.github.io/distilled-feature-fields/) | [code](https://github.com/pfnet-research/distilled-feature-fields)
- 🔥**LERF: Language Embedded Radiance Fields**, J. stin Kerr et al, ICCV2023 (<font color="#e36c09">Oral</font>) | [arXiv](https://arxiv.org/abs/2303.09553) | [project](https://www.lerf.io/) | [code](https://github.com/kerrj/lerf)
- **LangSplat: 3D Language Gaussian Splatting**, Minghan Qin et al, CVPR2024 (<font color="#e36c09">Highlight</font>) | [arXiv](https://arxiv.org/abs/2312.16084) | [project](https://langsplat.github.io/) | [code](https://github.com/minghanqin/LangSplat)
- **N2F2: Hierarchical Scene Understanding with Nested Neural Feature Fields**, Yash Bhalgat, arXiv2024 | [arXiv](https://arxiv.org/abs/2403.10997)
- **O2V-Mapping: Online Open-Vocabulary Mapping with Neural Implicit Representation**, Muer Tie, arXiv 2024 | [arXiv](https://arxiv.org/abs/2404.06836)

