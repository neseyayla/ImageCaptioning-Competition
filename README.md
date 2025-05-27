# Image Captioning with BLIP (Kaggle Competition)

This project was developed for a Kaggle image captioning competition. It generates automatic captions for images using a fine-tuned BLIP (Bootstrapped Language-Image Pretraining) model.

## Features
- Fine-tuned BLIP model on a custom dataset
- Data augmentation and text preprocessing
- Caption generation for test images

## Requirements
- Python 3.x
- PyTorch
- HuggingFace Transformers
- PIL (Pillow)
- tqdm

## Usage
1. Place your test images in the `test/test/` directory.
2. Make sure your `test.csv` file is in the project root.
3. Run the script:
   ```bash
   python submission.py
   ```
4. The generated captions will be saved in `submission.csv`.

## Example Output

| image_id | caption                  |
|----------|--------------------------|
| 123      | A cat sitting on a mat.  |
| 456      | A dog playing outside.   |

## Notes
- The model was trained and evaluated using Frechet Distance and other relevant metrics.
- For more details, see the code in `submission.ipynb`.
