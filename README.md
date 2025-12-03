# Ambient Sound Classification
**EEL5840 Fall 2025 - Neuronettes Final Project B**

**Cole Madden**

**Devin Dykstra**

## Required Packages

```bash
conda install numpy scikit-learn matplotlib
conda install -c conda-forge librosa
```

## Parameter Settings

### train.ipynb
```python
# modify paths if needed on line 5
data_path='training_data_projectB.npy'
labels_path='training_labels_projectB.npy'
model_save_path='final_model.pkl'
sample_rate=48000

# Line 162 - adjust SVM hyperparameters
param_grid = {
    'classifier__C': [1, 5, 10, 50],
    'classifier__gamma': [0.0001, 0.0005, 0.001, 0.005]
}
```

### test.ipynb
```python
#  modify paths if needed on line 7
TEST_DATA_PATH = 'test_data_projectB.npy'
TEST_LABELS_PATH = 'test_labels_projectB.npy'
MODEL_PATH = 'final_model.pkl'
sample_rate=48000
```

