# PolyIC Interactive Tutorials

Interactive Jupyter tutorials for exploring theoretical models of polymer interaction chromatography (PolyIC). Start with an unfunctionalized homopolymer, then compare it with chains that have one or two functional end groups.

## Tutorials

| Tutorial | Description | Guide | Open in Colab |
| --- | --- | --- | --- |
| 1. Homopolymer partitioning | Explore how polymer-to-pore size and wall interactions affect the partition coefficient. | [Guide](01-Homopolymer/README.md) | [Open notebook](https://colab.research.google.com/github/PolyIC-OSE/Poly-Interactive-Tutorials/blob/main/01-Homopolymer/reproduce_graph.ipynb) |
| 2. End-functionalized polymers | Compare homopolymers with chains that have one or two functional ends. | [Guide](02-End-Functionalized/README.md) | [Open notebook](https://colab.research.google.com/github/PolyIC-OSE/Poly-Interactive-Tutorials/blob/main/02-End-Functionalized/end_functionalized_plots.ipynb) |

## Run in Google Colab

Open a notebook using its Colab link, connect to a runtime, and choose **Runtime → Run all**. The notebooks use Python and Matplotlib, which are available in standard Colab runtimes. If Matplotlib is unavailable, run `%pip install "matplotlib>=3.9,<4"` in a code cell and rerun the notebook.

To keep changes, use **File → Save a copy in Drive**. Generated figures are in the Colab runtime's temporary storage; download them from the Files panel if you want to keep them.

## Run locally

From the repository root, create an environment and install the shared requirements:

```bash
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
```

Run a standalone tutorial script from the repository root:

```bash
python 01-Homopolymer/reproduce_graph.py
python 02-End-Functionalized/end_functionalized_plots.py
```

Or start Jupyter with `python -m jupyter notebook` and open either notebook. Each tutorial guide also lists its notebook, script, and generated figure files.

## Scientific scope

These are educational implementations of ideal-chain slit-pore models, not fits to experimental data. A notebook running successfully does not, by itself, establish that a model is physically valid for a particular experiment.

## Credit and reuse

The original notebooks, Python calculations, and example figures were developed by [shivanshsinglaggn123](https://github.com/shivanshsinglaggn123). PolyIC provides the tutorial organization and setup documentation. Permission to copy with credit was confirmed by the repository owner; an open-source license has not been established, so no license is added here.