# Fertilizer Recommendation (ML)

Simple Flask app and training script for fertilizer recommendation.

Setup

1. Create and activate a virtual environment (recommended).
2. Install dependencies:

```bash
pip install -r requirements.txt
```

Train model

```bash
python train.py
```

This will produce artifacts in the `model/` folder: `model.pkl`, `scaler.pkl`, `encoders.pkl` and individual encoder files.

Run app

```bash
python app.py
```

Open http://127.0.0.1:5000/ and use the form to get recommendations.

Notes

- The web form uses dropdowns for `Soil_Type`, `Crop_Type`, and `Region` populated from the CSV dataset to avoid input mismatches.
- If you change feature ordering or preprocessing in `train.py`, update `app.py` feature order accordingly.
