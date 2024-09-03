# LM-Directory-Bruteforcing

## Introduction
This repository contains the code and the datasets utilised for the paper "Offensive AI: Enhancing Directory Brute-forcing attack with the use of Language models", presented at the 17th ACM Workshop on Artificial Intelligence and Security (AISec 2024).

## Instruction
The folder [datasets][datasets/] contains the datasets used in this work (zipped). You can use the same datasets to reproduce our paper's results.
The folder contains the dataset in two formats:
- [combined-dataset](datasets/combined_dataset.zip) is the entire dataset already preprocessed (the filtering of URLs associated with responses with status code has not been made yet).
- [LM-training-datasets](datasets/LM-training-datasets/) contains the dataset split in training, validation and test datasets used to train the language models used to performed the enhanced directory bruteforce attacks.

To ease the process of reproducing the analysis and the attack simulations performed, there are 3 jupyter notebooks available:
- [LM_training.ipynb](LM_training.ipynb) contains the code to train the Language models.
- [benchmarks.ipynb](benchmarks.ipynb) contains the code to run directory brute-force attack simulations (as described in the paper) using all the different attack methodologies. In addition to that, it is also possible to simulate the attack execution time by setting the supposed time that each request-response interaction takes and the number of available threads.
- [general_stats_scripts.ipynb](general_stats_scripts.ipynb) contains the code to analyze and generate the statistics and the plots for the datasets features and attack simulation results.

If you have any questions, please e-mail us.

If you utilize this code, please cite us as follows:

```
@article{castagnaro2024offensive,
  title={Offensive AI: Enhancing Directory Brute-forcing Attack with the Use of Language Models},
  author={Castagnaro, Alberto and Conti, Mauro and Pajola, Luca},
  journal={arXiv preprint arXiv:2404.14138},
  year={2024}
}
```
