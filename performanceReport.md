======================================================================
Configuration Settings
======================================================================
BATCH_SIZE.................... 128
DATA_DIR...................... ./data
DEVICE........................ cpu
LEARNING_RATE................. 0.001
MIN_DELTA..................... 0.001
MLP_DROPOUT................... 0.3
MLP_HIDDEN_SIZES.............. [512, 256]
MODEL_TYPE.................... mlp
NUM_CLASSES................... 10
NUM_EPOCHS.................... 20
NUM_WORKERS................... 2
PATIENCE...................... 10
PRINT_EVERY................... 5
RANDOM_SEED................... 42
SAVE_BEST_ONLY................ True
SAVE_DIR...................... ./checkpoints
USE_EARLY_STOPPING............ True
VAL_SPLIT..................... 0.1
WEIGHT_DECAY.................. 0.0005
======================================================================

Using device: cpu

Loading CIFAR-10 data...
Downloading https://www.cs.toronto.edu/~kriz/cifar-10-python.tar.gz to ./data/cifar-10-python.tar.gz
100.0%
Extracting ./data/cifar-10-python.tar.gz to ./data
Files already downloaded and verified
Training samples: 45000
Validation samples: 5000
Test samples: 10000

Creating MLP model...
Total parameters: 1,708,810

======================================================================
Starting Training
======================================================================
Epoch [  1/20] | Train Loss: 1.7027 | Train Acc: 39.26% | Val Loss: 1.5228 | Val Acc: 44.92%
Checkpoint saved to ./checkpoints/best_model_mlp.pth
Checkpoint saved to ./checkpoints/best_model_mlp.pth
Checkpoint saved to ./checkpoints/best_model_mlp.pth
Checkpoint saved to ./checkpoints/best_model_mlp.pth
Epoch [  5/20] | Train Loss: 1.4154 | Train Acc: 49.15% | Val Loss: 1.3711 | Val Acc: 51.08%
Checkpoint saved to ./checkpoints/best_model_mlp.pth
Checkpoint saved to ./checkpoints/best_model_mlp.pth
Epoch [ 10/20] | Train Loss: 1.3453 | Train Acc: 52.20% | Val Loss: 1.3417 | Val Acc: 51.88%
Checkpoint saved to ./checkpoints/best_model_mlp.pth
Checkpoint saved to ./checkpoints/best_model_mlp.pth
Checkpoint saved to ./checkpoints/best_model_mlp.pth
Checkpoint saved to ./checkpoints/best_model_mlp.pth
Epoch [ 15/20] | Train Loss: 1.3084 | Train Acc: 53.46% | Val Loss: 1.3199 | Val Acc: 52.08%
Epoch [ 20/20] | Train Loss: 1.2853 | Train Acc: 54.03% | Val Loss: 1.2970 | Val Acc: 52.60%

======================================================================
Training Completed
======================================================================
Best Validation Accuracy: 53.12%

Generating training history plots...
Training history plot saved to ./checkpoints/training_history_mlp.png
2026-01-20 10:46:35.209 python[58226:22232163] The class 'NSSavePanel' overrides the method identifier.  This method is implemented by class 'NSWindow'

Evaluating on test set...
Test Loss: 1.2899 | Test Accuracy: 54.15%

======================================================================
All Done!
======================================================================
