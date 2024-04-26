# RetinaRegNet
RetinaRegNet is a state-of-the-art tool designed to align two-dimensional retinal images that exhibit significant displacement or shifts with ease. Unlike other methods, it does not require the usual training for image registration, making it one of the few tools to implement a zero-shot learning approach. It uses a latent diffusion model to generate viable Diffusion Feature Maps (DIFT), marking a significant advancement in the field of retinal image registration. Furthermore, the model has proven to be effective on complex retinal image datasets such as 'FIRE', 'FLoRI21', and 'LSFG'.
## Requirements
The scripts were executed using a custom kernel configured with the list of packages mentioned below.
* torch 2.0.1
* torchvision 0.15.2
* jax 0.4.23
* jaxlib 0.4.23
* accelerate 0.23.0
* diffusers 0.20.2
* ipympl 0.9.3
* transformers 4.34.0
* xformers 0.0.22
* numpy
* scipy
* opencv-python
* matplotlib
* pyunpack
* **Note:** To install the aforementioned list of packages, kindly use the command `pip install -r requirements.txt`
## Citations
Kindly cite our paper as follows if you use our code.
```bibtex
@misc{sivaraman2024retinaregnet,
    title={RetinaRegNet: A Versatile Approach for Retinal Image Registration},
    author={Vishal Balaji Sivaraman and Muhammad Imran and Qingyue Wei and Preethika Muralidharan and Michelle R. Tamplin and Isabella M. Grumbach and Randy H. Kardon and Jui-Kai Wang and Yuyin Zhou and Wei Shao},
    year={2024},
    eprint={2404.16017},
    archivePrefix={arXiv},
    primaryClass={cs.CV}
}
