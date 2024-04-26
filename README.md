# RetinaRegNet
RetinaRegNet is a cutting-edge tool designed to align two-dimensional retinal images that exhibit significant displacement or shifts with relative ease and efficacy. Unlike other methods, it does not require conventional training for image registration, making it one of the few tools that use a zero-shot learning approach. The method is inspired by the paper titled ["Emergent Correspondence from Image Diffusion"](https://arxiv.org/abs/2306.03881), employing an advanced latent stable diffusion model to generate robust Diffusion Feature Maps (DIFT), significantly advancing the field of retinal image registration. Additionally, the model has effectively worked on three challenging retinal image datasets: two public datasets, ["FIRE"](https://carlos.hernandez.im/papers/2017_07_JMO.pdf) and ["FLoRI21"](https://d197for5662m48.cloudfront.net/documents/publicationstatus/162961/preprint_pdf/738552aa194d07089578b227a4057471.pdf), and a privately owned dataset titled "LSFG".

## Requirements
The scripts were executed using a custom kernel configured with the list of packages mentioned below.
* torch-2.0.1
* torchvision-0.15.2
* jax-0.4.23
* jaxlib-0.4.23
* accelerate-0.23.0
* diffusers-0.20.2
* ipympl-0.9.3
* transformers-4.34.0
* xformers-0.0.22
* numpy
* scipy
* opencv-python
* matplotlib
* pyunpack
* **Note:** To install the aforementioned list of packages, kindly use the command `pip install -r requirements.txt`

## Datasets
* [Fundus Image Regsitration Dataset (FIRE)](https://projects.ics.forth.gr/cvrl/fire/)
* [Fluorescein Angiography Longitudinal Retinal Image Registration 2021 Dataset (FLoRI21)](https://ieee-dataport.org/open-access/flori21-fluorescein-angiography-longitudinal-retinal-image-registration-dataset)
* Laser Speckle Flowgraphy Dataset (LSFG)

## References
Certain code cells were referenced from the original implementation available at this [GitHub repository](https://github.com/Tsingularity/dift), as detailed in the paper titled ["Emergent Correspondence from Image Diffusion"](https://arxiv.org/abs/2306.03881).

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
