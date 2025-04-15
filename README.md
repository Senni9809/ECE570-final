========================================
BIOT Seizure Detection Demo
========================================

Project: ECE570 Checkpoint 3

----------------------------------------
📽 Demo Video
----------------------------------------
You can view the 5-minute demo video at the following link:
🔗 https://drive.google.com/file/d/12MtAKl5mnHl-MS-7WYIEmFPi_LBWqkZw/view?usp=drive_link

(Note: This video demonstrates project motivation, dataset preparation, model architecture, training process, and evaluation results.)

----------------------------------------
📁 Project Structure
----------------------------------------

- dataprocessing.py  
  Extracts 5-second EEG windows from CHB-MIT .edf files using MNE.  
  Labels windows based on seizure intervals.  
  Saves output as `trainval.pkl` and `test.pkl`.

- biot.py  
  Implements a simplified BIOT model using PyTorch.  
  Includes Conv1D feature extraction, token pooling, Transformer encoder, and MLP classifier.  
  Performs training, validation, and test evaluation with AUROC, F1, confusion matrix, and ROC curve outputs.

- dataset/  
  Contains the generated `trainval.pkl` and `test.pkl` EEG segment files.  
  These are the preprocessed inputs for training and evaluation.

----------------------------------------
⚙ Environment
----------------------------------------

- Python >= 3.8
- PyTorch
- MNE
- scikit-learn
- matplotlib
- numpy
