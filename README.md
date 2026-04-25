# PyTorch Fundamentals

A collection of notebooks covering **PyTorch basics**—from creating and manipulating tensors to building, training, saving, and loading a simple model.

## Contents

- **01_pytorch_fundamentals.ipynb**
  - Importing PyTorch + common Python libraries
  - Tensors: vectors, matrices, higher-dimensional tensors
  - Tensor properties: `ndim`, `shape`, `dtype`
  - Random tensors, zeros, ones, ranges (`arange`), `zeros_like`
  - Type casting (e.g., int → float32)
  - Aggregation ops: `max`, `min`, `mean`
  - Reshaping ops: `squeeze`, `unsqueeze`
  - Indexing and slicing
  - PyTorch ↔ NumPy conversions (`from_numpy`, `.numpy()`)

- **02_pytorch_workflow.ipynb**
  - Creating a simple dataset
  - Train/test split
  - Building a linear regression model with `torch.nn.Module`
  - Loss function + optimizer (MAE / `nn.L1Loss`, SGD)
  - Training loop (train/eval modes)
  - Visualizing predictions
  - Saving and loading model weights (`state_dict`)

## Getting Started

### Option 1: Run locally

#### Requirements
- Python 3.9+ (recommended)
- PyTorch
- NumPy, Pandas, Matplotlib
- Jupyter Notebook / JupyterLab

#### Install (example)
```bash
pip install torch numpy pandas matplotlib jupyter
```

#### Run notebooks
```bash
jupyter notebook
```

Then open:
- `01_pytorch_fundamentals.ipynb`
- `02_pytorch_workflow.ipynb`

### Option 2: Run on Google Colab

You can open the notebooks directly in Colab:

- `01_pytorch_fundamentals.ipynb`  
  https://colab.research.google.com/github/sagar-kc7/pytorch_fundamentals/blob/main/01_pytorch_fundamentals.ipynb

- `02_pytorch_workflow.ipynb`  
  https://colab.research.google.com/github/sagar-kc7/pytorch_fundamentals/blob/main/02_pytorch_workflow.ipynb

## Project Structure

```
.
├── 01_pytorch_fundamentals.ipynb
├── 02_pytorch_workflow.ipynb
├── models/                      # created by the workflow notebook when saving models
└── README.md
```

## Notes

- The workflow notebook saves a model to: `models/02_pytorch_workflow_model.pth`
- If you don’t see the `models/` folder initially, it will be created when you run the “Saving a model” section.
