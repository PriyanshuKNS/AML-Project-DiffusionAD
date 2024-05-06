# AML-Project-DiffusionAD

**Team Phoenix : Priyanshu Yadav (210050125), Anand Narasimhan (210051001)**

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
1. *models/DDPM.py* : The portion from line 388 to line 522 has been written by us. This portion deals with the different variations of One-step denoising process with Norm guidance that we tried and implemented. This is our main contribution. The code is easy to understand. 
2. *train.py* : train() function : 133 to 180,  eval() function : 264 to 312. The code was added to make it compatible with different versions that we are running.
3. *eval.py* : In the testing() function, from 232 to 282 line number. Modified the testing according to the versions.



Other than these additions shown above, few lines have been added here and there according to need.
