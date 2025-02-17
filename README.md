# Large Driving Models

![logo](./assets/logo.jpg)

While most existing methods focus on adapting driving tasks to pre-trained large language models or vision-language models (**Large Models for Autonomous Driving**), we design a series of **Large Driving Models** specifically for autonomous driving.

## Path Towards Large Driving Models

### 2022-2023
![2023](./assets/2023.png)

### 2024
![2024](./assets/2024.png)

## Large Driving Model Zoo (Literally!)

| Model               | Function                   | Task                                                 | Core Contributor                               | Code                                            | Release Data | Why the name?                                       |
| ------------------- | -------------------------- | ---------------------------------------------------- | ---------------------------------------------- | ----------------------------------------------- | ------------ | --------------------------------------------------- |
| **Stereo Anything** | Large Stereo Model         | Stereo-based Depth Estimation                        | [Xianda Guo](https://github.com/XiandaGuo)     | https://github.com/XiandaGuo/OpenStereo         | 2024/11/22   | Stereo Anything                                     |
| **Stag-1**          | Large Simulation Model     | 4D Photorealistic Simulation                         | [Lening Wang](https://github.com/LeningWang)   | https://github.com/wzzheng/Stag                 | 2024/12/9    | **S**patial-Temporal simul**A**tion for drivin**G** |
| **Driv3R**          | Large Reconstruction Model | Pose-free Dense Reconstruction                       | [Xin Fei](https://github.com/Barrybarry-Smith) | https://github.com/Barrybarry-Smith/Driv3R      | 2024/12/10   | **DRIV**ing **3**d **R**econstruction               |
| **GPD-1**           | Latent World Model         | Close-Loop Simulation, Planning, Scene Generation... | [Zixun Xie](https://github.com/rainyNighti)    | https://github.com/wzzheng/GPD                  | 2024/12/12   | **G**enerative **P**re-training for **D**riving     |
| **Doe-1**           | Large World Model          | End-to-End Perception, Prediction, Planning...       | [Zetian Xia](https://github.com/ztxia)         | https://github.com/wzzheng/Doe                  | 2024/12/13   | **D**riving w**O**rld modEl                         |
| **DrivingRecon**    | Large Gaussian Model       | Feed-Forward 4D Gaussian Reconstruction              | [Hao Lu](https://github.com/LuPaoPao)          | https://github.com/EnVision-Research/DriveRecon | 2024/12/13   | Driving Reconstruction                              |
| **Owl-1**           | Video Generation Model     | End-to-End Planning and Generation                   | [Yuanhui Huang](https://huang-yh.github.io/)   | https://github.com/huang-yh/Owl                 | 2024/12/13   | **O**mni **W**orld mode**L**                        |


## Object-Centric Autonomous System

![logo](./assets/logo_gaussian.png)

| Model                | Scenario | Task                               | Core Contributor                             | Code                                       | Release Data |
|----------------------|----------|------------------------------------|----------------------------------------------|--------------------------------------------|--------------|
| **GaussianFormer**   | Outdoor  | Multi-View 3D Occupancy Prediction | [Yuanhui Huang](https://huang-yh.github.io/) | https://github.com/huang-yh/GaussianFormer | 2024/5/27    |
| **GaussianFormer-2** | Outdoor  | Multi-View 3D Occupancy Prediction | [Yuanhui Huang](https://huang-yh.github.io/) | https://github.com/huang-yh/GaussianFormer | 2024/12/6    |
| **EmbodiedOcc**      | Indoor   | Embodied 3D Occupancy Prediction   | [Yuqi Wu](https://github.com/YkiWu)          | https://github.com/YkiWu/EmbodiedOcc       | 2024/12/6    |
| **GaussianWorld**    | Outdoor  | Streaming 3D Occupancy Prediction  | [Sicheng Zuo](https://github.com/zuosc19)    | https://github.com/zuosc19/GaussianWorld   | 2024/12/16   |
| **GaussianAD**       | Outdoor  | End-to-End Autonomous Driving      | [Junjie Wu]()                                | https://github.com/wzzheng/GaussianAD      | 2024/12/16   |

## Demos

### Stag-1: Feed-Forward 4D Photorealistic Simulation

#### Freeze Time

![demo](./assets/stag1.gif)

#### Freeze View 

![demo](./assets/stag2.gif)

#### Demo 3: Multi-View

![demo](./assets/stag3.gif)

### Driv3R: Pose-free Dense Reconstruction

![demo](./assets/driv3r.gif)

### DrivingRecon: Feed-Forward 4D Gaussian Reconstruction

![demo](./assets/drivingrecon.gif)

### GPD-1: All-in-One Model for Autonomous Driving Simulation

![demo](./assets/gpd.gif)

### Doe-1: Closed-Loop Autonomous Driving

![demo](./assets/doe.gif)

### EmbodeidOcc: Online Embodied 3D Occupancy Prediction

![demo](./assets/embodiedocc.gif)

## Citations

If you find this project helpful, please consider citing the following papers:

```
### Stereo Anything
@article{guo2024stereo,
  title={Stereo Anything: Unifying Stereo Matching with Large-Scale Mixed Data},
  author={Guo, Xianda and Zhang, Chenming and Zhang, Youmin and Nie, Dujun and Wang, Ruilin and Zheng, Wenzhao and Poggi, Matteo and Chen, Long},
  journal={arXiv preprint arXiv:2411.14053},
  year={2024}
}

### Stag-1
@article{stag-1,
    title={Stag-1: Towards Realistic 4D Driving Simulation with Video Generation Model},
    author={Wang, Lening and Zheng, Wenzhao and Du, Dalong and Zhang, Yunpeng and Ren, Yilong and Jiang, Han and Cui, Zhiyong and Yu, Haiyang and Zhou, Jie and Lu, Jiwen and Zhang, Shanghang},
    journal={arXiv preprint arXiv:},
    year={2024}
	}

### Driv3R
@article{driv3r,
  title={Driv3R: Learning Dense 4D Reconstruction for Autonomous Driving}, 
  author={Fei, Xin and Zheng, Wenzhao and Duan, Yueqi and Zhan, Wei and Tomizuka, Masayoshi and Keutzer, Kurt and Lu, Jiwen},
  journal={arXiv preprint arXiv:2412.06777},
  year={2024}
}

### GPD-1
  @article{gpd-1,
    title={GPD-1: Generative Pre-training for Driving},
    author={Xie, Zixun and Zuo, Sicheng and Zheng, Wenzhao and Zhang, Yunpeng and Du, Dalong and Zhou, Jie and Lu, Jiwen and Zhang, Shanghang},
    journal={arXiv preprint arXiv:2412.08643},
    year={2024}
}

### Doe-1
@article{doe,
    title={Doe-1: Closed-Loop Autonomous Driving with Large World Model},
    author={Zheng, Wenzhao and Xia, Zetian and Huang, Yuanhui and Zuo, Sicheng and Zhou, Jie and Lu, Jiwen},
    journal={arXiv preprint arXiv:},
    year={2024}
}

### DrivingRecon
@article{Lu2024DrivingRecon,
        title={DrivingRecon: Large 4D Gaussian Reconstruction Model For Autonomous Driving},
        author={Hao LU, Tianshuo XU, Wenzhao ZHENG, Yunpeng ZHANG, Wei ZHAN, Dalong DU, Masayoshi Tomizuka, Kurt Keutzer, Yingcong CHEN},
        journal={arXiv preprint arXiv:2412.09043},
        year={2024}
      }

### Owl-1
@article{owl-1,
    title={Owl-1: Omni World Model for Consistent Long Video Generation}, 
    author={Huang, Yuanhui and Zheng, Wenzhao and Gao, Yuan and Tao, Xin and Wan, Pengfei and Zhang, Di and Zhou, Jie and Lu, Jiwen},
    journal={arXiv preprint arXiv:2412.09600},
    year={2024},
}

### GaussianFormer-1
@article{gaussianformer,
    title={GaussianFormer: Scene as Gaussians for Vision-Based 3D Semantic Occupancy Prediction},
    author={Huang, Yuanhui and Zheng, Wenzhao and Zhang, Yunpeng and Zhou, Jie and Lu, Jiwen},
    journal={arXiv preprint arXiv:2405.17429},
    year={2024}
}

### GaussianFormer-2
@article{gaussianformer-2,
      title={GaussianFormer-2: Probabilistic Gaussian Superposition for Efficient 3D Occupancy Prediction}, 
      author={Yuanhui Huang and Amonnut Thammatadatrakoon and Wenzhao Zheng and Yunpeng Zhang and Dalong Du and Jiwen Lu},
      journal={arXiv preprint arXiv:2412.04384},
      year={2024}
}
	
### EmbodiedOcc
@article{embodiedocc,
      title={EmbodiedOcc: Embodied 3D Occupancy Prediction for Vision-based Online Scene Understanding}, 
      author={Wu, Yuqi and Zheng, Wenzhao and Zuo, Sicheng and Huang, Yuanhui and Zhou, Jie and Lu, Jiwen},
      journal={arXiv preprint arXiv:2412.04380},
      year={2024}
}
```
