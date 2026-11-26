# End-functionalized polymers

[← All tutorials](../README.md) · [Open in Google Colab](https://colab.research.google.com/github/PolyIC-OSE/Poly-Interactive-Tutorials/blob/main/02-End-Functionalized/end_functionalized_plots.ipynb)

This tutorial compares the partition coefficient for an unfunctionalized homopolymer with linear chains that have one or two functional end groups.

## What you'll explore

- How one functional end changes the homopolymer partition coefficient.
- How adding a second end introduces an additional two-end contact term.
- How the results change with polymer-to-pore size ratio \(g=R_G/R_P\) and chain length \(N\).

The equations are implemented from equations (3), (4), (9), and (10) of the supplied paper. The parameter \(\lambda\) describes interactions of ordinary chain units with the pore wall; \(q_a\) and \(q_b\) describe the additional interactions of the functional ends. In the Python code, these are named `lambda_value`, `q_a`, and `q_b`.

## Run in Google Colab

Open the notebook with the Colab link above, connect to a runtime, and select **Runtime → Run all**. The notebook uses Python and Matplotlib, which are available in standard Colab runtimes. If Matplotlib is unavailable, run `%pip install "matplotlib>=3.9,<4"` in a code cell and rerun the notebook.

To keep changes, use **File → Save a copy in Drive**. Generated figures are stored in the runtime's temporary storage; download them from the Files panel if you want to keep them.

## Run locally

First follow the environment setup in the [main guide](../README.md). Then, from the repository root, run:

```bash
python 02-End-Functionalized/end_functionalized_plots.py
```

To use the notebook instead, start Jupyter from the repository root with `python -m jupyter notebook` and open `02-End-Functionalized/end_functionalized_plots.ipynb`.

The script saves `singly_doubly_functionalized_K_vs_g.png` and `singly_doubly_functionalized_K_vs_N.png` in the current working directory. Running it from the tutorial folder will overwrite those example figures; run a copy in a scratch folder to preserve them.

## What to change

- Change `q_a` and `q_b` to explore the functional-end contributions. Setting both to zero should recover the homopolymer result.
- Change `lambda_value` to explore attraction or repulsion of the ordinary chain units (the model parameter \(\lambda\)).
- Change `b_over_pore_radius` to control how chain length maps to \(g\) in the notebook. The standalone script calls this parameter `b_over_d`.
- Change the `chain_lengths` range to explore a different span of chain lengths.

The default `terms=101` includes the 51 odd modes from 1 through 101; it does not mean 101 terms are summed. The plotted values (\(\lambda=0.1\), \(q_a=q_b=0.5\), and `b_over_pore_radius=1.0`) are demonstration settings, not experimental measurements.

## Files and credit

- `end_functionalized_plots.ipynb`: explained equations, calculations, and plots.
- `end_functionalized_plots.py`: standalone version of the calculation.
- `singly_doubly_functionalized_K_vs_g.png`: example plot versus polymer-to-pore size ratio.
- `singly_doubly_functionalized_K_vs_N.png`: example plot versus chain length.
- `requirements.txt`: tutorial-specific dependency list.

Original work: [shivanshsinglaggn123](https://github.com/shivanshsinglaggn123). Original project folder: [End-functionalized Plots](https://github.com/shivanshsinglaggn123/shivanshsinglaggn123.github.io/tree/main/End-functionalized%20Plots).