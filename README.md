# Numeral-Recognition-Challenge
Build a model that assigns the correct numeric class (0–9) to each image in the test set.
## Objective
The goal of this project is to build a robust machine learning model capable of assigning the correct numeric class (**0–9**) to photographic images of handwritten numerals. 

This challenge focuses heavily on **generalization**, as final rankings are determined by performance on a held-out private test set.

---

## Dataset Description
The dataset consists of photographic images of handwritten numerals in a single script-style domain. 

### Files
* **train/**: Directory containing labeled training images.
* **test/**: Directory containing unlabeled test images.
* **train.csv**: Mapping file for training data containing two columns: `image_id` and `label`.
* **sample_submission.csv**: A template file containing all test `image_id` values with placeholder labels.

### Data Constraints
* **Classes**: 10 (digits 0 through 9).
* **Anonymization**: Metadata and filenames have been anonymized. Participants must rely solely on image features rather than filename patterns.

---

## Evaluation Metric
Model performance is evaluated based on **Classification Accuracy**:

$$\text{Accuracy} = \frac{\text{Correct Predictions}}{\text{Total Predictions}}$$

---

## Project Structure
```text
├── data/
│   ├── train/              # Training images
│   ├── test/               # Test images
│   ├── train.csv           # Image IDs and Labels
│   └── sample_submission.csv
├── notebooks/              # Jupyter notebooks for EDA and Modeling
├── src/                    # Source code for preprocessing and training
├── submission.csv          # Final predicted output
└── README.md
