# Scale-Separation-and-stochastic-closure-for-Chaotic-Dynamics


**Your folder structure should be** : 

<pre>
│
├───Data
│   └───Kolmogorov
│       └───processed_data
│           └───npyfiles
│                   kolmo.npy
│                   kolmo_100s.npy
│                   kolmo_120s.npy
│                   kolmo_closure.npy
│                   kolmo_filtered.npy
│                   kolmo_filtered_100s.npy
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

