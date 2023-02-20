# T-Phenotype: Discovering Phenotypes of Predictive Temporal Patterns in Disease Progression (AISTATS2023)

Source code for the T-Phenotype clustering approach proposed in paper "T-Phenotype: Discovering Phenotypes of Predictive Temporal Patterns in Disease Progression"

## Installation & Environment Setup

To run the experiments, directly clone this repository via the following command.
```bash
git clone git@github.com:yvchao/tphenotype.git
```

Ensure you have [conda](https://docs.conda.io/en/latest/miniconda.html) or [pyenv](https://github.com/pyenv/pyenv) installed in your environment and run the installation script **setup_venv.sh**.
```bash
bash ./setup_venv.sh
```
This will install the **tphenotype** package along with necessary dependencies to reproduce the experiment results.
A jupyter lab instance will be started, and the **notebook** directory will be opened in your browser.

## Datasets and Preparation

Three datasets are used in the experiment.
- Synthetic data: provided in this repo as **data_mixed.npz**; can be generated by running data/synthetic/data_generation.ipynb.
- [Physionet ICU](https://physionet.org/content/challenge-2012/1.0.0/) data: provided as **selected_data.npz**; can be generated by running ./data/real-world/physionet/{preprocessing,extract_data}.ipynb subsequently.
- [ADNI](https://tadpole.grand-challenge.org/) data: access can be downloaded from [loni](https://adni.loni.usc.edu/); contact the author for the processed version.

## Experiments
There are three major parts of the experiment.
- benchmark: run the Summary.ipynb to generate benchmark results on the three datasets.
- case_study: run experiment_adni.ipynb to generate the major results in the main manuscript.
- appendix: run the four notebooks to generate all the rest results included in the appendix.


## Citation
If you find the software useful, please consider citing the following paper:
```
@inproceedings{tphenotype2023,
  title={T-Phenotype: Discovering Phenotypes of Predictive Temporal Patterns in Disease Progression}
  author={Qin, Yuchao and van der Schaar, Mihaela and Lee,Changhee},
  booktitle={Proceedings of the 26th International Conference on Artificial Intelligence and Statistics (AISTATS) 2023},
  year={2023}
}
```
