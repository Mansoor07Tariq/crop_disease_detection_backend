# Crop Disease Detection Backend

This repository contains a backend for detecting crop diseases using trained models. The backend uses **FastAPI** and includes all necessary model files.

## Files Included

* `plant_disease_model.h5` – Pre-trained crop disease detection model
* `plant_disease_model_augmented.h5` – Augmented version of the model
* `Crop_Disease_with_treatment_x24144801.ipynb` – Notebook demonstrating detection and treatment suggestions

## Datasets

The datasets used for training are too large to store on GitHub. You can download them from the following links:

1. **[Dataset 1 – Crop Disease Dataset](https://www.kaggle.com/datasets/emmarex/plantdisease)**

2. **[Dataset 2 – Crop Disease Dataset](https://www.kaggle.com/datasets/vipoooool/new-plant-diseases-dataset)**

## Getting Started

1. **Clone the repository:**

```bash
git clone https://github.com/Mansoor07Tariq/crop_disease_detection_backend.git
cd crop_disease_detection_backend
```

2. **Install dependencies:**
   Make sure you have Python 3.10+ installed. Then install dependencies:

```bash
pip install fastapi uvicorn tensorflow
```

3. **Run the FastAPI server:**

```bash
uvicorn main:app --reload
```

> Replace `main:app` with the actual Python file and FastAPI app object if named differently.

4. **Access the API:**
   Open your browser and navigate to:

```
http://127.0.0.1:8000/docs
```

Here you can test the endpoints directly.

## Notes

* The `.h5` model files are tracked with Git LFS, so make sure you have **Git LFS installed**.
* The datasets are **not stored in the repository** due to GitHub file size limits; use the download links above.
* Once the server is running, the backend is ready to process predictions using the provided models.