# Relation discovery in nonlinearly related large-scale settings

## Overview

This repository implements a novel method for discovering nonlinear causal relationships in large-scale climate systems, as presented in our IEEE ICASSP 2022 paper. Our approach addresses two critical challenges in climate science:

1. The nonlinear nature of climate system interactions
2. The "curse of dimensionality" when dealing with large numbers of sensors but limited temporal data

## Background

Climate change represents one of the most complex challenges facing science today. A key part of understanding climate systems is discovering how different variables influence each other - what we call "causal relationships." Traditional methods struggle with this because:

- Climate systems are highly nonlinear - one variable's effect on another isn't always straightforward
- We often have data from large numbers of sensors (high dimensionality)
- Many datasets only cover a few decades (limited temporal samples)
- Weather conditions can create misleading correlations (confounding variables)

## Method

Our approach uses a novel combination of techniques to overcome these challenges:

1. **Radial Basis Function (RBF) Neural Networks**: Help capture nonlinear relationships between variables
2. **Partition Functions**: Convert data into probabilistic clusters to handle high dimensionality
3. **Granger Causality Framework**: Provides a statistical foundation for inferring causation from temporal data

The method works in two main steps:
1. Data Transformation: Uses RBF to handle nonlinear relationships while maintaining computational efficiency
2. Causal Discovery: Applies modified Granger causality techniques to infer relationships between variables

## Validation

We've validated our method through extensive testing:

1. **Synthetic Networks**: Tested on five different network types:
   - 3-node V-structure
   - 3-node Immortality structure
   - 5-node nonlinear network
   - Two 34-node Zachary club networks

2. **Real Climate Data**: Successfully tested on river discharge data from the upper Danube basin, estimating nonlinear Granger-causal relations on synthetic networks and on river-discharge data.

## Installation

```bash
## Requirements

Python 3.8 or newer with numpy, scipy, scikit-learn, matplotlib and Jupyter. No further installation: the method is implemented inside the notebooks.
```

## Usage

```python
## Running the code

Open `Main_causal_climate.ipynb` to reproduce the experiments; `Explained_complete.ipynb` walks through the method step by step on the same data.
```

## Citation

If you use this code in your research, please cite our paper:

```bibtex
@inproceedings{vosoughi2022relation,
  title={Relation Discovery in Nonlinearly Related Large-Scale Settings},
  author={Vosoughi, Ali and DSouza, Adora and Abidin, Anas and Wism{\"u}ller, Axel},
  booktitle={ICASSP 2022-2022 IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP)},
  pages={5103--5107},
  year={2022},
  organization={IEEE}
}
```

## License

MIT License

## Contact

For questions and contributions, please visit: https://alivosoughi.com

## Acknowledgments

This research was partially funded by:
- American College of Radiology (ACR) Innovation Award
- Ernest J. Del Monte Institute for Neuroscience Award
- National Science Foundation (NSF) under Grant DGE-1922591

## References

For official paper access, please visit: [IEEE Xplore](https://ieeexplore.ieee.org/abstract/document/9747356)


## Patent notice

The large-scale Granger causality methods implemented in this repository are the subject of patent rights held by Axel Wismüller and the University of Rochester. The MIT licence of this code grants no rights under those patents. Academic and research use with citation is welcome; for any commercial use, contact the patent holders.
