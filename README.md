# Relation discovery in nonlinearly related large-scale settings

## Overview

This repository implements a novel method for discovering nonlinear causal relationships in large-scale climate systems, as presented in our IEEE ICASSP 2022 paper. Our approach addresses two critical challenges in climate science:

1. The nonlinear nature of climate system interactions
2. The "curse of dimensionality" when dealing with millions of sensors but limited temporal data

## Background

Climate change represents one of the most complex challenges facing science today. A key part of understanding climate systems is discovering how different variables influence each other - what we call "causal relationships." Traditional methods struggle with this because:

- Climate systems are highly nonlinear - one variable's effect on another isn't always straightforward
- We often have data from millions of sensors (high dimensionality)
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

2. **Real Climate Data**: Successfully tested on river discharge data from the upper Danube basin, correctly identifying genuine causal relationships while avoiding spurious correlations.

## Installation

```bash
# Installation instructions coming soon
```

## Usage

```python
# Code examples coming soon
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
