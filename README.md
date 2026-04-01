\# MOF Descriptor Sufficiency Benchmark



Code for descriptor-sufficiency benchmarking in metal–organic framework (MOF) machine learning for methane uptake at 65 bar.



\## Overview



This repository contains the notebooks used to benchmark how far simple, interpretable descriptors can go in MOF machine learning before richer structural information becomes necessary.



The study compares four descriptor families:



\- Geometry-only

\- Enriched interpretable geometry

\- Topology-only

\- Geometry + topology



across four accessible model classes:



\- Ridge regression

\- Random forest

\- Histogram-based gradient boosting

\- Shallow multilayer perceptron



The workflow supports generation of the main manuscript figures, supplementary-information figures, and benchmark tables.



\## Repository contents



\- `Main tasks.ipynb`  

&nbsp; Main benchmark execution notebook. Runs the core workflow, builds benchmark outputs, and writes processed result tables.



\- `main plots.ipynb`  

&nbsp; Generates the main-text figures and benchmark summary outputs.



\- `SI.ipynb`  

&nbsp; Generates supplementary-information figures and supporting outputs.



\- `requirements.txt`  

&nbsp; Minimal Python package list for running the notebooks.



\## Generated folders



When the notebooks are run, they generate output folders automatically, including:



\- `data\_processed/`

\- `results/`

\- `manuscript\_assets/`

\- `supplementary\_assets/`



These generated folders are not tracked in this repository and can be recreated by running the notebooks.



\## Data access



The lightweight benchmark data table used in the study is \*\*not included in this repository\*\*.



The underlying source data come from the ARC–MOF dataset hosted on Zenodo:



\*\*Burner, J., Luo, J., White, A., Mirmiran, A., Kwon, O., Boyd, P. G., Maley, S., Gibaldi, M., Simrod, S., \& Woo, T. K. (2025). \_ab initio REPEAT Charge MOF Database (ARC-MOF)\_ \[Data set]. Zenodo. https://doi.org/10.5281/zenodo.16802743\*\*



Users should obtain the source files directly from the ARC–MOF Zenodo record and comply with the original dataset license and attribution requirements.



\## Related dataset publication



\*\*Burner, J., Luo, J., White, A., Mirmiran, A., Kwon, O., Boyd, P. G., Maley, S., Gibaldi, M., Simrod, S., Ogden, V., \& Woo, T. K.\*\*  

\*ARC–MOF: A Diverse Database of Metal-Organic Frameworks with DFT-Derived Partial Atomic Charges and Descriptors for Machine Learning.\*  

\*\*Chemistry of Materials\*\* 2023, 35(3), 900–916.  

https://doi.org/10.1021/acs.chemmater.2c02485



\## Minimal workflow



1\. Obtain the required source data from the ARC–MOF Zenodo record.

2\. Prepare the lightweight benchmark table used by the notebooks.

3\. Place the required input table(s) in the repository root or in the expected input location used by the notebooks.

4\. Run the notebooks in the following order:



&nbsp;  1. `Main tasks.ipynb`

&nbsp;  2. `main plots.ipynb`

&nbsp;  3. `SI.ipynb`



This order ensures that benchmark outputs are generated before figure-building notebooks are executed.



\## Software requirements



This workflow uses standard Python scientific and machine-learning libraries, including:



\- pandas

\- numpy

\- scipy

\- scikit-learn

\- matplotlib

\- seaborn

\- joblib

\- jupyter



Install them with your preferred environment manager before running the notebooks.



\## Licensing



\### Code

The code in this repository is released under the \*\*MIT License\*\*.



\### Data

This repository does \*\*not\*\* redistribute the ARC–MOF source data. Users should access the data from the original Zenodo record and comply with the corresponding license and citation requirements.



\## Related manuscript



\*\*How Far Can Simple Descriptors Take MOF Machine Learning? Performance Limits, Failure Modes, and Chemical Insight\*\*



\## Citation



If you use this repository, please cite:



1\. The associated manuscript, once available.

2\. The ARC–MOF Zenodo dataset:

&nbsp;  - Burner et al. (2025), Zenodo, https://doi.org/10.5281/zenodo.16802743

3\. The ARC–MOF data paper:

&nbsp;  - Burner et al. (2023), \*Chemistry of Materials\*, https://doi.org/10.1021/acs.chemmater.2c02485



\## Notes



\- This repository is intentionally lightweight.

\- Generated outputs are excluded from version control.

\- The emphasis is reproducible benchmarking with compact, interpretable descriptors rather than heavy structure-generation workflows.

