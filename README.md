<h2 align="center">
  <span><img src="assets/leo.svg" width="4%" style="transform: translate(0,9px)"></span><b>Multi-modal Situated Reasoning in 3D Scenes</b>
</h2>

<div align="center" margin-bottom="6em">
<a target="_blank" href="https://github.com/Germany321">Xiongkun Linghu<sup>✶</sup></a>,
<a target="_blank" href="https://nxsedson.github.io/">Xuesong Niu<sup>✶</sup></a>,
<a target="_blank" href="https://huangjy-pku.github.io/">Jiangyong Huang</a>,
<a target="_blank" href="https://jeasinema.github.io/">Xiaojian Ma</a>,
<a target="_blank" href="https://buzz-beater.github.io/">Baoxiong Jia</a>,
<a target="_blank" href="https://siyuanhuang.com/">Siyuan Huang</a>
</div>
&nbsp;

<div align="center">
    <a href="https://arxiv.org/abs/2311.12871" target="_blank">
    <img src="https://img.shields.io/badge/Paper-arXiv-deepgreen" alt="Paper arXiv"></a>
    <a href="https://embodied-generalist.github.io" target="_blank">
    <img src="https://img.shields.io/badge/Page-LEO-9cf" alt="Project Page"></a>
    <a href="https://youtu.be/mlnjz4eSjB4?si=NN9z7TpkTPgBAzBw" target="_blank">
    <img src="https://img.shields.io/badge/Video-YouTube-9966ff" alt="Video"></a>
    <a href="https://drive.google.com/drive/folders/1dko2dzdwRWSK3hi1liBpGHZ8Dz97jXdP?usp=sharing" target="_blank">
    <img src="https://img.shields.io/badge/Data-LEO-blue" alt="Data"></a>
    <a href="https://drive.google.com/drive/folders/1dko2dzdwRWSK3hi1liBpGHZ8Dz97jXdP?usp=sharing" target="_blank">
    <img src="https://img.shields.io/badge/Model-LEO-darkorange" alt="Model"></a>
</div>
&nbsp;

<div align="left">
<img src="assets/teaser.png" width="99%" alt="LEO Teaser">
</div>

We introduce **LEO**, an **embodied multi-modal generalist agent** capable of **grounding**, **reasoning**, **chatting**, **planning**, and **acting** in the **3D world**. **LEO** is trained in a two-stage scheme: *(i) 3D vision-language (VL) alignment* and *(ii) 3D vision-language-action (VLA) instruction tuning*.

We meticulously collect extensive diverse data for training **LEO**. <sup>&dagger;</sup> indicates the task contains our generated data. See [Task and Data](#task-and-data) for details. We show the data statistics as below:

| Dataset | Task | 2D required? | 3D assets | #data |
| :---: | :---: | :---: | :---: | :---: |
| *LEO-align* | object captioning | ✗ | Objaverse | 660k |
|  | object referring<sup>&dagger;</sup> | ✗ | ScanNet + 3RScan | 354k |
|  | scene captioning<sup>&dagger;</sup> | ✗ | 3RScan | 20k |
| *LEO-instruct* | 3D captioning | ✗ | ScanNet | 37k |
|  | 3D QA<sup>&dagger;</sup> | ✗ | ScanNet + 3RScan | 83k |
|  | 3D dialogue<sup>&dagger;</sup> | ✗ | 3RScan | 11k |
|  | task planning<sup>&dagger;</sup> | ✗ | 3RScan | 14k |
|  | navigation | ✓ | MP3D | 60k |
|  | manipulation | ✓ | CLIPort | 300k |


### TODO

- [x] Test set
- [ ] Train/val set
- [ ] Point cloud and images
- [ ] Evaluation code
- [ ] Training code
