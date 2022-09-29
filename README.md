# NeurT-FDR

This library contains code for NeurT-FDR, a method for controlling false discovery rate by incorporating feature hierarchy. This paper is acceptted at Proceedings of the 31st ACM International Conference on Information and Knowledge Management (CIKM 2022). https://arxiv.org/abs/2101.09809.



# Repository

The following files can be found in this repository:


(a) run_methods_with_simulated_data.ipynb: Run methods on simulated data with BB-FDR, NeurT-FDRa, and NeurT-FDRb.

(b) simulation_analysis.py: Run all the methods on simulated data with FDR = 0.05, 0.1, 0.15, 0.2

(c) normix.py: Functions for predictive recursion to empirical estimate the null and alternative distribution

(d) two_groups_beta.py: The two-groups models including: BB-FDR, NeurT-FDRa, NeurT-FDRb.


# Getting started

In this repository, it is only necessary to run the Jupyter notebooks since they are able to invoke the Python scripts automatically. Thus, Python source code files correspond to encapsulated functions and/or classes that our notebooks depend on.


# Requirements

- Python 3.7.8
- NumPy
- SciPy
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn
- PyTorch
- [AdaFDR](https://pypi.org/project/adafdr/)

# Python environment configuration

Please run the following command line to configure your Python environment:

```bash
pip install requirements.txt
```

# Performance 

The default configuration of these notebooks takes several hours to run our approach in a machine with 16 CPUs and 64GB of RAM memory.

To run it in a feasible time, please consider to update the following variables in the file `simulation_analysis.py`:
- `alpha_list`: list of alpha values.
- `num_folds`: number of folds.
- `num_epochs`: number of epochs.

