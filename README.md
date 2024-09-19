# Ultrasound denoising and synthesis GAN

This repository contains a demo to apply GANs for denoising ultrasound images or to synthesize b-mode ultrasound from MRI images, which have comparatively lower speckle noise. We developed a pipeline and model to simulate b-mode images given an MR image, and used the generated clean and noisy pixel-aligned image pairs to train another GAN to perform denoising. 

Check out the article for details about the pipeline:

D. F. Vieira, A. Raposo, A. Azeitona, M. V. Afonso, L. M. Pedro and J. Sanches, "Ultrasound Despeckling With GANs and Cross Modality Transfer Learning," in IEEE Access, vol. 12, pp. 45811-45823, 2024, doi: 10.1109/ACCESS.2024.3381630. 
https://ieeexplore.ieee.org/abstract/document/10478899

# Dependencies

Our pipeline builds upon the pytorch version of pix2pix https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix, and the demo notebook sets up the environment as specified in the requirements file from there.

Google Colab was used by us for all development and testing, so when running the notebook be sure to save the result folders in your linked google drive.

The samples used in this demo are from:
* Longitudinal B-mode images of the carotid artery http://splab.cz/en/download/databaze/ultrasound
* Cardiac MRI dataset [Andreopoulos et. al., 2008]  https://jtl.lassonde.yorku.ca/software/datasets/

# Usage

Run the provided jupyter notebook in Colab. It is self contained and all links are public.

![image](https://github.com/user-attachments/assets/00249ae2-2944-4eab-ad07-0364f66ed4d5)

