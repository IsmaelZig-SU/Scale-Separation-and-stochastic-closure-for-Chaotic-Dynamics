# Scale Separation and Stochastic Closure for Chaotic Dynamics

This repository leverages **scale separation** to solve **unsteady chaotic systems probabilistically**.  
An illustrative example is provided using a **Kolmogorov flow**, generated with the [`kolSol` solver](https://github.com/MagriLab/KolSol).

The theoretical framework underlying this work is described in the following paper:  
[Scale Separation and Stochastic Closure for Chaotic Dynamics (arXiv:2510.24583)](https://arxiv.org/abs/2510.24583)

---

## Overview

Chaotic dynamical systems often exhibit a wide range of interacting spatial and temporal scales.  
This repository provides tools to:
- **Filter and preprocess data** from fully resolved simulations  
- **Train a Dynamical Reduced-Order Model (ROM)** that captures essential dynamics on a lower-dimensional manifold  
- **Model unresolved scales** through a **Gaussian Process (GP) closure** informed by the resolved-scale dynamics

**Your folder structure should be** : 

<pre>
│
├───Data
│   └───Kolmogorov
│       └───processed_data
│           └───npyfiles
│                   kolmo_100s_8traj.npy
│                   kolmo_120s_8traj.npy
│                   kolmo_filtered_120s_8ens.npy
│                   kolmo_filtered_100s_8ens.npy
│
├───Notebooks
│ Closure_diffusion.ipynb
│ Closure_VAE.ipynb
│ Gaussian_Process_Closure.ipynb
│ kolmo_low_pass_filter.ipynb
│ Read_kolmo.ipynb
│ ROM_dynamics.ipynb
│
├───src
│ │ Eval_MZA.py
│ │ MZA_Experiment.py
│ │
│ ├───Layers
│ │ │ MZANetwork.py
│ │ │ transformer.py
│ │ │ transformer_cross_att.py
│ │ │ VAE.py
│ │ │ VAE_big.py
│ │
│ │
│ ├───PreProc_Data
│ │ │ DataProc.py
│ │ │ DynSystem_Data.py
│ │
│ │
│ ├───Train_Methods
│ │ │ Train_Methodology.py
│ │ │
│ │
│ └───utils
│ │ make_dir.py
│ │
│
└───Trained_Models
    └───Kolmo2D_new
        ├───sl30_obs64_bs64_attblks2_atthds8_tr0_ph30_lbdaStateLoss1.0_nhd64_0.0005_
        │   │   args
        │   │
        │   ├───model_weights
        │   │       min_train_loss
        │   │
        │   └───out_log
        │           AutoencoderLoss.png
        │           log
        │           StateLoss.png
        │           TotalLoss.png
        │           TransEvo.png
    

    </pre>

