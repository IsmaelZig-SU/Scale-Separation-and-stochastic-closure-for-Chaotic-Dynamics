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
│ │ │
│ │ └───pycache
│ │ Autoencoder.cpython-311.pyc
│ │ Autoencoder_narrow.cpython-311.pyc
│ │ Autoencoder_wider.cpython-311.pyc
│ │ Koopman.cpython-311.pyc
│ │ MZANetwork.cpython-311.pyc
│ │ RNN_Model.cpython-311.pyc
│ │ stochastic_transformer.cpython-311.pyc
│ │ stochastic_transformer_2.cpython-311.pyc
│ │ stochastic_transformer_expension.cpython-311.pyc
│ │ transformer.cpython-311.pyc
│ │ transformer_cross_att.cpython-311.pyc
│ │ Transformer_UQ.cpython-311.pyc
│ │ VAE.cpython-311.pyc
│ │ VAE_big.cpython-311.pyc
│ │ VAE_param.cpython-311.pyc
│ │
│ ├───PreProc_Data
│ │ │ DataProc.py
│ │ │ DynSystem_Data.py
│ │ │
│ │ └───pycache
│ │ DataProc.cpython-311.pyc
│ │ DynSystem_Data.cpython-311.pyc
│ │ DynSystem_Data_param.cpython-311.pyc
│ │
│ ├───Train_Methods
│ │ │ Train_Methodology.py
│ │ │
│ │ └───pycache
│ │ Train_Methodology.cpython-311.pyc
│ │ Train_methodology_param.cpython-311.pyc
│ │ Train_methodology_param_UQ.cpython-311.pyc
│ │ Train_Methodology_UQ.cpython-311.pyc
│ │ Train_Methodology_UQ_nnl.cpython-311.pyc
│ │ Train_Methodology_VAE.cpython-311.pyc
│ │
│ └───utils
│ │ make_dir.py
│ │
│ └───pycache
│ make_dir.cpython-311.pyc
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

