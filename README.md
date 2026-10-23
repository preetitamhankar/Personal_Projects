# Quantitative Health Research Portfolio

Small, reproducible examples prepared to demonstrate skills relevant to a UCLA Epidemiology GSR role: network simulation, biomedical data cleaning, graph analysis, and clear research code. Every dataset generated here is **synthetic**. Nothing comes from Stanford or any real patient, and the outputs are demonstrations rather than scientific findings.

## Projects

1. **Network epidemiology simulation** — build a contact network, compare no intervention with two vaccination strategies, and summarize the simulated epidemic. Demonstrates simulation design, seeded randomness, reusable functions, and sensitivity to intervention choice.
2. **Biomedical data quality and outcomes** — generate a fictional cardiothoracic cohort, validate fields, report missingness and cohort summaries, and make a descriptive plot. Demonstrates data cleaning, validation, transparent exclusions, and visualization.
3. **Network neuroscience methods demo** — generate synthetic regional signals, estimate a correlation network, and summarize network properties. Demonstrates a basic signal-to-network workflow without presenting simulated signals as MRI or real neuroscience data.

## Run

Requires Python 3.10 or newer. From this directory:

```bash
python3 -m venv .venv
source .venv/bin/activate  # Windows: .venv\\Scripts\\activate
python -m pip install -e .
python projects/network_epidemiology/run.py
python projects/biomedical_data_quality/run.py
python projects/network_neuroscience/run.py
```

Each script writes CSV summaries and PNG figures to its own `outputs/` folder. Use `--help` for adjustable simulation settings where available. The scripts use fixed random seeds by default so results are reproducible.

## Interpretation and limitations

These are teaching and portfolio examples, not validated epidemiologic models. The network epidemic model uses simplified assumptions; the cohort is artificially generated; and the neuroscience example uses simulated correlated signals rather than fMRI. No causal, clinical, or biological conclusions should be drawn from the outputs. Any real research would require an approved dataset, a prespecified analysis plan, and appropriate supervision.

## Code sample for an application

For a short code sample, link directly to `projects/network_epidemiology/run.py` or `projects/biomedical_data_quality/run.py`, then explain in a few sentences what the script does, how you made it reproducible, and one limitation. Choose the project you can most comfortably walk through line by line. Do not describe these examples as prior lab or clinical research.

## Project map

```text
projects/
  network_epidemiology/   contact-network SIR simulation and intervention comparison
  biomedical_data_quality/ synthetic cardiothoracic cohort QA and descriptive analysis
  network_neuroscience/   synthetic time-series correlation network demonstration
```

