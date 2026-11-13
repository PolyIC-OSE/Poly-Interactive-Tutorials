# End-functionalized polymers

[← All tutorials](../README.md) · [Open in Google Colab](https://colab.research.google.com/github/PolyIC-OSE/Poly-Interactive-Tutorials/blob/main/02-End-Functionalized/end_functionalized_plots.ipynb)

Compare ordinary, singly functionalized, and doubly functionalized chains versus size ratio and chain length.

## Run

In Colab, connect to a runtime and run the cells from top to bottom. The notebook uses Python's standard library and Matplotlib, available in standard Colab runtimes. If Matplotlib is unavailable, run `%pip install "matplotlib>=3.9,<4"` in a new cell first.

For local use, install the root requirements as described in the [main guide](../README.md), then from the repository root:

```bash
cd 02-End-Functionalized
python end_functionalized_plots.py
```

Or open `end_functionalized_plots.ipynb` in Jupyter and run all cells. The plotting code writes `singly_doubly_functionalized_K_vs_g.png` and `singly_doubly_functionalized_K_vs_N.png` in the current working directory. To preserve the original example figures, run a copy in a scratch folder.

## Explore

Change `q_a` and `q_b` to compare end-group contributions. Set both to zero to recover the ordinary chain. Change `b_over_pore_radius` in the notebook (`b_over_d` in the script) to explore the chain-length conversion.

The model uses g = R_G/R_P. The default `terms=101` includes 51 odd modes, rather than 101 terms.

## Files and attribution

`end_functionalized_plots.ipynb` contains the explained calculation; `end_functionalized_plots.py` is the standalone version. The PNG files are original example outputs. `requirements.txt` lists the tutorial runtime dependencies.

Original work: GitHub contributor [shivanshsinglaggn123](https://github.com/shivanshsinglaggn123). Original folder: [End-functionalized Plots](https://github.com/shivanshsinglaggn123/shivanshsinglaggn123.github.io/tree/main/End-functionalized%20Plots).
