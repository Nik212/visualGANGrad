# Visualizing gradient directions of generative models

This is the repository dedicated to a course project done for Machine Learning course at Skolkovo Institute of Science and Technology. 

**The goal** of our empirical study is too understand how the knowledge of the gradient of the divergence metric with respect to the generator can be applied to improving the quality of generated data (in our case, images)

In our study, we use a custom implementation of GAN based on https://github.com/LynnHo/DCGAN-LSGAN-WGAN-GP-DRAGAN-Pytorch

----------------------------------------


### Results

IS, and FID scores of DCGAN on the CelebA dataset at different epochs.

| Epoch | IS ↑  | FID ↓ |
|-------|-------|-------|
| 5     | 1.826 | 26.64 |
| 25    | 1.904 | 11.00 |
| 49    | 1.969 | 8.87  |

IS and FID scores of WGAN on the CelebA dataset at different epochs.

| Epoch | IS ↑  | FID ↓ |
|-------|-------|-------|
| 5     | 1.967 | 17.27 |
| 15    | 1.956 | 12.55 |
| 29    | 2.016 | 10.43 |


### Usage

Prerequisites

* PyTorch 1.1
* tensorboardX
* scikit-image, oyaml, tqdm
* Python 3.6

Dataset

* CelebA dataset

Colab notebooks

*As running our code requieres GPU, we provide links to Colab*

Simply follow instructions from the notebook. As for the data, please upload the data from this source [data link](https://drive.google.com/file/d/1e0FaRKxcm5RlVoLGpFlYqUn_tMifugjw/view?usp=sharing) to the "data" folder in Colab files.

* WGAN training [Colab link](https://colab.research.google.com/drive/1ZJCCkUKbCEx7KElrAkxfjdQlHwvLhoE7?usp=sharing#scrollTo=yXrWVjI-FtRC)
* DCGAN training [Colab link](https://colab.research.google.com/drive/1E2Nqy5W8OYfu_fuXmyzL5pcgDjTlRsTc?usp=sharing)
* Evaluation [Colab link](https://drive.google.com/file/d/1rUJuy8RzYuLG5wuriTlRHKsX6l2buThO/view?usp=sharing). All extra code needed you will find in this repository. You may find the checkpoints [here](https://drive.google.com/drive/folders/16M2JH1jh_xlp6kZClcf2Hbbi8EHmOA-z?usp=sharing).

