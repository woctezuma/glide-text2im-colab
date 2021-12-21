# GLIDE text2im on Colab

This repository provides a Colab notebook to produce images conditioned on text prompts with [GLIDE][openai-glide-code] [1].

## Usage

-   Run [`text2im.ipynb`][colab-notebook-text2im]
[![Open In Colab][colab-badge]][colab-notebook-text2im]

## Results

The process is based on the small, filtered-data GLIDE model, with classifier-free guidance.

Results consist of 64x64 images, and the corresponding 256x256 upsampled versions.

---

<img alt="Sample" src="https://github.com/woctezuma/glide-text2im-colab/wiki/img/sample_A.png" height="256"><img alt="Sample" src="https://github.com/woctezuma/glide-text2im-colab/wiki/img/sample_B.png" height="256"><img alt="Sample" src="https://github.com/woctezuma/glide-text2im-colab/wiki/img/sample_C.png" height="256">

<sub>
Several uncurated samples obtained with the same prompt: "a magnificent French rooster singing".
</sub>

## Safety considerations

The *small* model has 300 million parameters, compared to the unreleased 3.5 billion parameter model.

As described in Appendix F.1, the training dataset was *filtered* so that it would not contain:
-   images of humans and human-like objects,
-   images of violent objects,
-   two prevalent hate symbols in America (swastika and confederate flag).

## References

[1] Alex Nichol, Prafulla Dhariwal, Aditya Ramesh, et al. *GLIDE: Towards Photorealistic Image Generation and Editing with Text-Guided Diffusion Models*. [arXiv preprint 2112.10741][openai-glide-paper]. 2021.

<!-- Definitions -->

[openai-glide-code]: <https://github.com/openai/glide-text2im>
[openai-glide-paper]: <https://arxiv.org/abs/2112.10741>

[colab-notebook-text2im]: <https://colab.research.google.com/github/woctezuma/glide-text2im-colab/blob/main/text2im.ipynb>
[colab-badge]: <https://colab.research.google.com/assets/colab-badge.svg>
