# BSc Intro Data Science - HW9 Boosting And Neural Networks

- Course: BSc Computer Science.

## Contents

Classification coursework comparing boosting with feed-forward neural-network models on image-derived feature vectors.

## Files

Template or reference material:

- `assignment/HW9 -SOL.ipynb`

My solution notebooks:

- `solutions/HW9_my.ipynb`

My submitted answers:

- `results/hw9_answers.csv`

## Tech Stack

- Python notebooks.
- Main Python packages: keras, matplotlib, numpy, pandas, requests, scikit-image, scikit-learn, tensorflow, notebook.
- Jupyter-compatible local review flow.

## Run

Use Python 3.11 and `uv`. Supply the extracted `ebay_boys_girls_shirts` course dataset (the directory containing the four train/test CSV files and the `boys/` and `girls/` images):

```sh
uv run --python 3.11 python scripts/run_notebook.py /path/to/ebay_boys_girls_shirts
```

This executes every solution code cell with real images, 32 training images per class, and one epoch per neural-network fit. It checks loading, training, prediction, plots, metrics, and answer export. Temporary plots and exports do not overwrite the submitted answers. Add `--full` to use the notebook's original dataset sizes and training epochs; that takes substantially more time and memory. A bounded run is not a reproduction of the submitted accuracy scores.

The notebook also runs interactively: set the `SHIRTS_DATASET` environment variable before opening it. Its TensorFlow/Keras calls and image conversion support the pinned environment above. The image dataset is not bundled with this repository.
