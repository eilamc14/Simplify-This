# Models directory

This folder stores **runtime checkpoints** and **final trained models**.

## Layout
- `models/<model_name>` — runtime checkpoints of the *current* run.  
  - Using checkpoints if exist by default. To start from scratch, **delete or move** this folder or its content manually.
- `models/trained/<model_name>` — final models saved at the end of training, using the same naming. These are used for final evaluation.

## Notes
- All `<model_names>` are `model_name.replace("/", "_")` - done by trainer code.
- Do **not** commit large checkpoints to Git; prefer Git LFS or keep them local.
- Evaluation code looks for final models under `models/trained/<model_name>`.