# Experimental-comparison-for-time-to-event-analysis-through-the-concordance-index
Experimental comparison of semi-parametric, parametric and machine learning models for time-to-event analysis through the concordance index.

Paper: https://arxiv.org/abs/2003.08820

Code requirements:

- Anaconda Python 3.7
- Additional packages: scikit-survival, pysurvival, lifelines
- cython compilation:

```
python setup_random_survival_forest_cython.py build_ext --inplace
```

Cython Random Survival Forest implementation was made by George H. Chen: https://github.com/georgehc/npsurvival


## How to install pysurvival
This package contains C++ source code, pip needs a C++ compiler to install pysurvival.

The recommended C++ compiler is GCC. For more details on how to install it for Mac OS and Linux visit this website: https://square.github.io/pysurvival/installation.html

After you have installed GCC the easiest way to install pysurvival is using pip

```
pip install pysurvival
```

For installation on Window you can download the files directly from: https://github.com/bacalfa/pysurvival

First build the package

```
python setup.py build_ext --inplace
```

To install the package from the files in your computer

```
python setup.py install --user
```

## Concordance index comparison

We implemented many models to two data sets: PBC and GBCSG2. The codes of the concordance index comparison for each data set are GBCSG2_Cindex_comparison for the breast cancer recurrence prediction and PBC_Cindex_comparison for the primary biliary chirrosis dead prediction.
