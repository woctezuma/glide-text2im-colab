# GLIDE text2im on Colab

The goal of this repository is to provide a Colab notebook to apply [GLIDE][openai-glide-code] to produce images conditioned on text prompts.

## Usage

-   Run [`text2im.ipynb`][colab-notebook-text2im]
[![Open In Colab][colab-badge]][colab-notebook-text2im]

## Results

The process is based on the small, filtered-data GLIDE model [1] with classifier-free guidance.

Results consist of 64x64 images, and the corresponding 256x256 upsampled versions.

## References

[1] Alex Nichol, Prafulla Dhariwal, Aditya Ramesh, et al. *GLIDE: Towards Photorealistic Image Generation and Editing with Text-Guided Diffusion Models*. [arXiv preprint 2112.10741][openai-glide-paper]. 2021.

<!-- Definitions -->

[openai-glide-code]: <https://github.com/openai/glide-text2im>
[openai-glide-paper]: <https://arxiv.org/abs/2112.10741>

[colab-notebook-text2im]: <https://colab.research.google.com/github/woctezuma/glide-text2im-colab/blob/main/text2im.ipynb>
[colab-badge]: <https://colab.research.google.com/assets/colab-badge.svg>
