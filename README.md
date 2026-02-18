# Duality-AI-s-Offroad-Semantic-Scene-Segmentation.
# Offroad Semantic Segmentation – README

## 1. Project

Semantic scene segmentation for off-road desert environments using Duality AI Falcon synthetic data as part of the GHR 2.0 Offroad Autonomy Segmentation challenge.[file:1]

---

## 2. Requirements

- Anaconda/Miniconda installed.[file:1]  
- Dataset downloaded from the official Falcon link and placed into `train`, `val`, and `testImages` folders as specified by the hackathon docs.[file:1]  

Environment (Windows):

```bash
cd ENVSETUP
setupenv.bat   # creates conda env 'EDU'
. Training
From the scripts directory:
his trains on the provided train/val splits and saves logs/checkpoints under runs/.[file:1]

Use the first complete run as your baseline (IoU and loss curves).[file:1]

4. Testing / Inference
After training:

bash
python test.py
This loads the trained model, runs inference on testImages, and reports IoU and other metrics, along with predictions used for qualitative analysis.[file:1]

Keep test images strictly for testing; do not use them in training/validation.[file:1]

5. Reproducibility
To reproduce final results:

Set up the EDU environment.

Download and place the dataset in the expected folders.

Run python train.py, then python test.py with your final configuration.[file:1]

Expected outputs:

IoU score and loss metrics.

Qualitative predictions and visualizations (via the provided visualization script, if used).[file:1]

6. Submission Checklist (Hackathon)
Include in your final zipped folder:[file:1]

train.py, test.py, config and helper scripts.

Trained model weights and any required assets.

Hackathon report (PDF/DOCX, ≤ 8 pages).

This README with setup, run, and reproduction instructions.[file:1]

text
undefined
