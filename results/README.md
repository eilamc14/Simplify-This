# Results Directory

This folder stores all experiment results, organized by datasets, models, and evaluation artifacts.

## Structure

- **results_checklist.md**  
  A checklist of all models that were run, used to track progress.

- **`dataset-name`_`subset`/**  
  For each dataset and subset (e.g., `ASSET_test`), a dedicated folder exists.  
  Inside each folder:
  - **<model_name>.csv** → a CSV file containing the final evaluation metrics for that model.

  - **samples/**  
    Contains text samples for human evaluation.  
    - Each file is named after the model (`<model_name>.txt`).  
    - Each file includes **3 output samples per prompt**, allowing manual inspection.

## Notes
- Model names in filenames use `model_name.replace("/", "_")`.
- The checklist file (`results_checklist.md`) containes the models and the index of samples for each model used in our paper.