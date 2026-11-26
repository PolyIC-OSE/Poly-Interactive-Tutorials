# Homopolymer partitioning

[← All tutorials](../README.md) · [Open in Google Colab](https://colab.research.google.com/github/PolyIC-OSE/Poly-Interactive-Tutorials/blob/main/01-Homopolymer/reproduce_graph.ipynb)

This tutorial calculates and plots the partition coefficient for an unfunctionalized homopolymer in a slit-like pore.

## What you'll explore

- How the polymer-to-pore size ratio $g=R_G/R_P$ changes the partition coefficient $K$.
- How the ordinary-unit wall interaction parameter $\lambda$ changes the curves.
- How numerical root finding and a finite sum approximate the model equation.

## Run in Google Colab

Open the notebook with the Colab link above, connect to a runtime, and select **Runtime → Run all**. The notebook uses Python and Matplotlib, which are available in standard Colab runtimes. If Matplotlib is unavailable, run `%pip install "matplotlib>=3.9,<4"` in a code cell and rerun the notebook.

To keep changes, use **File → Save a copy in Drive**. The generated figure is stored in the runtime's temporary storage; download it from the Files panel if you want to keep it.

## Run locally

First follow the environment setup in the [main guide](../README.md). Then, from the repository root, run:

```bash
python 01-Homopolymer/reproduce_graph.py
```

To use the notebook instead, start Jupyter from the repository root with `python -m jupyter notebook` and open `01-Homopolymer/reproduce_graph.ipynb`.

The script saves `reproduced_graph.png` in the current working directory. Running it from the tutorial folder will overwrite that folder's example figure; run a copy in a scratch folder to preserve the original.

## What to change

Edit `lambda_values` to compare attraction (negative $\lambda$), repulsion (positive $\lambda$), and the neutral case ($\lambda=0$). Change the range of `g_values` to explore different polymer-to-pore size ratios.

The default `terms=101` includes the 51 odd modes from 1 through 101; it does not mean 101 terms are summed.

## Files and credit

- `reproduce_graph.ipynb`: explained calculation and plot.
- `reproduce_graph.py`: standalone version of the calculation.
- `reproduced_graph.png`: example output.
- `requirements.txt`: tutorial-specific dependency list.

Original work: [shivanshsinglaggn123](https://github.com/shivanshsinglaggn123). Original project folder: [Homopolymer Graph](https://github.com/shivanshsinglaggn123/shivanshsinglaggn123.github.io/tree/main/Homopolymer%20Graph).