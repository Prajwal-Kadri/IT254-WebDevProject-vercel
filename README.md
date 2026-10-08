# Network Intrusion Detection Web App

A Flask web interface for running a trained random-forest intrusion-detection model against network-connection features from the UNSW-NB15 dataset.

## Features

- Form-based prediction flow
- Example intrusion and non-intrusion test cases
- Pretrained `RandomForest_IG_IDS.pkl` model
- Deployment configuration for Vercel

## Run locally

```bash
python -m pip install -r requirements.txt
python main.py
```

Open the local address printed by Flask, then use the interface to submit a connection record.

## Project layout

- `main.py` — Flask routes and prediction pipeline
- `models.py` — model-related code
- `UNSW_NB15/dataset/` — training and test data
- `model_files/` — serialized model
- `templates/` — HTML interface

This repository is the deployed-interface counterpart to `IT254-WebDevProject`.
