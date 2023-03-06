# Real Estate Price Prediction
Implementation of several real estate prediction papers:
1. PDVM: https://link.springer.com/article/10.1007/s41688-018-0027-0





### Environment
``` 
conda create -n $ENV_NAME$ python=3.5.2
conda activate $ENV_NAME$

# CUDA 11.3
pip install torch==1.5.1+cu113 --extra-index-url https://download.pytorch.org/whl/cu113 
# Or, CUDA 10.2 
pip install torch==1.5.1+cu102 --extra-index-url https://download.pytorch.org/whl/cu102 
pip install -r requirements.txt
```

### Preprocess
```
python preprocess.py
```

### Training the model
Go to the desired model directory \
Specify the parameters in required class in config.py
```
python train_{model_name}.py
```

### Results
| Model | MSE |
|-------|--|
| HA | 0.063 |
| LR | 0.084 |
| SVM | 0.066 |
| GBRT | 0.019 |
| DNN | 21.38 |
| PDVM | 0.238 |







### Reference