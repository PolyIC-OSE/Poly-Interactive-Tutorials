# PolyIC Interactive Tutorials

Explore theoretical polymer interaction chromatography with Python notebooks. Start with the homopolymer model, then explore chains with one or two functional ends.

| Tutorial | Explore | Run in your browser |
| --- | --- | --- |
| 1. Homopolymer partitioning | [Guide](01-Homopolymer/README.md) | [Open in Colab](https://colab.research.google.com/github/PolyIC-OSE/Poly-Interactive-Tutorials/blob/main/01-Homopolymer/reproduce_graph.ipynb) |
| 2. End-functionalized polymers | [Guide](02-End-Functionalized/README.md) | [Open in Colab](https://colab.research.google.com/github/PolyIC-OSE/Poly-Interactive-Tutorials/blob/main/02-End-Functionalized/end_functionalized_plots.ipynb) |

## Getting started

Colab requires no local installation. Open a notebook above, connect to a runtime, and choose **Runtime → Run all**. Edit the plotting parameters and rerun the relevant cells. Save your own copy to retain changes; generated figures are temporary until downloaded from Colab's Files panel.

For a local installation, Python 3.10 or newer is recommended:

```bash
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
python -m jupyter notebook
```

Open either tutorial notebook and select the Python kernel from this environment. Each folder also includes a standalone script and original example figures. The tutorial guides give exact commands.

## Scientific scope

These are educational implementations of ideal-chain slit-pore models, not fits to experimental data. The original calculation code and saved example figures are preserved. Run completion and regression checks do not establish physical validity.

## Credit and reuse

Original notebooks, Python calculations, and example figures were developed by **shivanshsinglaggn123** 

PolyIC provides the tutorial organization and setup documentation. Permission to copy with credit was confirmed by the repository owner; an open-source license has not been established. No license is added here.

