# Homopolymer partitioning

[← All tutorials](../README.md) · [Open in Google Colab](https://colab.research.google.com/github/PolyIC-OSE/Poly-Interactive-Tutorials/blob/main/01-Homopolymer/reproduce_graph.ipynb)

Compare partition coefficients across polymer-to-pore size ratios and wall interaction parameters.

## Run

In Colab, connect to a runtime and run the cells from top to bottom. The notebook uses Python's standard library and Matplotlib, available in standard Colab runtimes. If Matplotlib is unavailable, run `%pip install "matplotlib>=3.9,<4"` in a new cell first.

For local use, install the root requirements as described in the [main guide](../README.md), then from the repository root:

```bash
cd 01-Homopolymer
python reproduce_graph.py
```

Or open `reproduce_graph.ipynb` in Jupyter and run all cells. The plotting code writes `reproduced_graph.png` in the current working directory. To preserve the original example figures, run a copy in a scratch folder.

## Explore

Change `lambda_values` and compare attraction (negative λ), repulsion (positive λ), and the neutral case (λ = 0). Change the range of `g_values` to explore size effects.

The model uses g = R_G/R_P. The default `terms=101` includes 51 odd modes, rather than 101 terms.

## Files and attribution

`reproduce_graph.ipynb` contains the explained calculation; `reproduce_graph.py` is the standalone version. The PNG files are original example outputs. `requirements.txt` lists the tutorial runtime dependencies.

Original work: GitHub contributor [shivanshsinglaggn123](https://github.com/shivanshsinglaggn123). Original folder: [Homopolymer Graph](https://github.com/shivanshsinglaggn123/shivanshsinglaggn123.github.io/tree/main/Homopolymer%20Graph).
