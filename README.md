# AML-Project-DiffusionAD

This is the repository for our project "Diffusion Models in Anomaly Detection" by Team Phoenix. 

Note: We haven't added the data directories are they are too large. 

To run the code, use the command in the following sequence : 
```bash
pip install -r requirements.txt
python train.py <version_number>
python eval.py <version_number>
```

This repository has been referenced for the given code : [Original_Repo](https://github.com/HuiZhang0812/DiffusionAD?tab=readme-ov-file)

Here, version_number is one of {1,2,3,4}. We have tried 4 variation of norm-guided one step denoising process (NOD) given in the diffusionAd paper.

*Hui Zhang, Zheng Wang, Zuxuan Wu, Yu-Gang Jiang*

[Paper link](https://arxiv.org/abs/2303.08730) 


The files of interest and the changes made in them are listed below : 
1. **models/DDPM.py** : The portion from line 388 to line 522 has been written by us. This portion deals with the different variations of One-step denoising process with Norm guidance that we tried and implemented. This is our main contribution. 
2. **train.py** : 
