# ZeroSmooth: Training-free Diffuser Adaptation for High Frame Rate Video Generation


<div align="center">

 <a href='https://arxiv.org/abs/2406.00908'><img src='https://img.shields.io/badge/ArXiv-2310.07702-red'></a> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
 <a href='https://ssyang2020.github.io/zerosmooth.github.io/'><img src='https://img.shields.io/badge/Project-Page-Green'></a> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;

[comment]: <> ( <a href='https://github.com/YingqingHe/ScaleCrafter-ptl'><img src='https://img.shields.io/badge/lightning version-code-blue'></a> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Replicate]&#40;https://replicate.com/cjwbw/scalecrafter/badge&#41;]&#40;https://replicate.com/cjwbw/scalecrafter&#41; )
 

**[Shaoshu Yang](https://github.com/ssyang1999), [Xiaodong Cun](http://vinthony.github.io/), [Yong Zhang<sup>#](https://yzhang2016.github.io), [Ying Shan](https://scholar.google.com/citations?hl=zh-CN&user=4oXBp9UAAAAJ), and [Ran He<sup>#](https://rhe-web.github.io/)**

(# corresponding author)

[comment]: <> (<img src=assets/pics/video.gif>)

[comment]: <> (Input: "A beautiful girl on a boat"; Resolution: 2048 x 1152.)

[comment]: <> (<br><br>)

[comment]: <> (<img src=assets/pics/img.jpg>)

[comment]: <> (Input: "Miniature house with plants in the potted area, hyper realism, dramatic ambient lighting, high detail"; Resolution: 4096 x 4096.)

[comment]: <> (<br><br>)

[comment]: <> (<img src=assets/pics/anyres.jpg>)

[comment]: <> (Arbitrary higher-resolution generation based on SD 2.1.)

[comment]: <> (<br><br>)
</div>

## TL; DR
ZeroSmooth is a training-free plug-in for video diffusers to enable high-frame rate video generation. One can build self-cascaded video models with our methods that generate smooth results while preserving the contents of the original outputs.

## :notes: Notes
- Welcome everyone to collaborate on the code repository, improve methods, and do more downstream tasks. Please check the [CONTRIBUTING.md](https://github.com/YingqingHe/ScaleCrafter/blob/main/CONTRIBUTING.md)
- If you have any questions or comments, we are open for discussion.

## Abstract
> Video generation has made remarkable progress in recent years, especially since the advent of the video diffusion models. Many video generation models can produce plausible synthetic videos, e.g., Stable Video Diffusion (SVD). However, most video models can only generate low frame rate videos due to the limited GPU mem- ory as well as the difficulty of modeling a large set of frames. The training videos are always uniformly sampled at a specified interval for temporal compression. Previous methods promote the frame rate by either training a video interpolation model in pixel space as a postprocessing stage or training an interpolation model in latent space for a specific base video model. In this paper, we propose a training-free video interpolation method for generative video diffusion models, which is generalizable to different models in a plug-and-play manner. We investigate the non-linearity in the feature space of video diffusion models and transform a video model into a self-cascaded video diffusion model with incorporating the designed hidden state correction modules. The self-cascaded architecture and the correction module are proposed to retain the temporal consistency between key frames and the interpolated frames. Extensive evaluations are preformed on multiple popular video models to demonstrate the effectiveness of the propose method, especially that our training-free method is even comparable to trained interpolation models supported by huge compute resources and large-scale datasets.


## Changelog
- __[2024.6.3]__: 🔥 Release paper.
<br>

## 📝 TODO
- [ ] Update gallery
- [ ] Release codes
- [ ] Hugging Face Gradio demo


## Citation
```bib
@misc{yang2024zerosmooth,
      title={ZeroSmooth: Training-free Diffuser Adaptation for High Frame Rate Video Generation}, 
      author={Shaoshu Yang and Yong Zhang and Xiaodong Cun and Ying Shan and Ran He},
      year={2024},
      eprint={2406.00908},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
```

[comment]: <> (## 📭 Contact)

[comment]: <> (If you have any comments or questions, feel free to contact [Yingqing He]&#40;yhebm@connect.ust.hk&#41; or [Shaoshu Yang]&#40;shaoshuyang2020@outlook.com&#41;.)