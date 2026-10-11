# CIFAR-10 Robust Classification

**Repository name:** `cifar10-robust-classification`

**Description:** Kaggle notebook starter for CIFAR-10 robust image classification using a compact Inception-style CNN, augmentation, regularization, and clean/shifted evaluation.

## Files
- `cifar10_robust_classification_kaggle.ipynb` — organized notebook with separate cells for data, model, training, experiments, and evaluation.
- `results_summary_template.md` — one-page report template to complete using actual results.

## Run on Kaggle
1. Create a new Kaggle Notebook and upload/import the `.ipynb`.
2. Select GPU accelerator if available.
3. Enable internet if allowed, because `torchvision` downloads CIFAR-10.
4. Run cells from top to bottom.
5. Complete every TODO and check the instructor's exact requirements before submission.

## Data protocol
- Select 50 images per class from CIFAR-10 training data (500 total).
- Use 400 images for training and 100 for validation.
- Keep the original 10,000-image test split as clean test data.
- The current shifted-test scaffold applies rotation, brightness/contrast changes, and a rectangular occlusion covering approximately 25% of the image.

## Important
The instructor's additional hidden corruption was not included in the available instructions. Add the exact specified corruption before claiming full shifted-test compliance. The required Cutout/Random Erasing and Mixup/CutMix ablations are marked as TODOs. No results are fabricated in this repository; populate the report only after executing your experiments. Select settings using validation results, not test-set performance.
