# LM-Directory-Bruteforcing

## Introduction
This repository contains the code and the datasets utilised for the paper "Offensive AI: Enhancing Directory Brute-forcing attack with the use of Language models", presented at the 17th ACM Workshop on Artificial Intelligence and Security (AISec 2024).

## Instructions
The folder [datasets][datasets/] contains the datasets used in this work (zipped). You can use the same datasets to reproduce our paper's results.
The folder contains the dataset in two formats:
- [combined-dataset](datasets/combined_dataset.zip) is the entire dataset already preprocessed (the filtering of URLs associated with responses with status code has not been made yet).
- [LM-training-datasets](datasets/LM-training-datasets/) contains the dataset split in training, validation and test datasets used to train the language models used to performed the enhanced directory bruteforce attacks.

To ease the process of reproducing the analysis and the attack simulations performed, there are 3 jupyter notebooks available:
- [LM_training.ipynb](LM_training.ipynb) contains the code to train the Language models.
- [benchmarks.ipynb](benchmarks.ipynb) contains the code to run directory brute-force attack simulations (as described in the paper) using all the different attack methodologies. In addition to that, it is also possible to simulate the attack execution time by setting the supposed time that each request-response interaction takes and the number of available threads.
- [general_stats_scripts.ipynb](general_stats_scripts.ipynb) contains the code to analyze and generate the statistics and the plots for the datasets features and attack simulation results.


## How to use our code

If you have any questions regarding the dataset or the code, please [send us an email](mailto:alberto.castagnaro@gmail.com).

If you utilize this code, please cite us as follows:

```
@inproceedings{10.1145/3689932.3694770,
author = {Castagnaro, Alberto and Conti, Mauro and Pajola, Luca},
title = {Offensive AI: Enhancing Directory Brute-forcing Attack with the Use of Language Models},
year = {2024},
isbn = {9798400712289},
publisher = {Association for Computing Machinery},
address = {New York, NY, USA},
url = {https://doi.org/10.1145/3689932.3694770},
doi = {10.1145/3689932.3694770},
abstract = {Web Vulnerability Assessment and Penetration Testing (Web VAPT) is a comprehensive cybersecurity process that uncovers a range of vulnerabilities which, if exploited, could compromise the integrity of web applications. In a VAPT, it is common to perform a Directory brute-forcing Attack, aiming at the identification of accessible directories of a target website. Current commercial solutions are inefficient as they are based on brute-forcing strategies that use wordlists, resulting in enormous quantities of trials for a small amount of success.Offensive AI is a recent paradigm that integrates AI-based technologies in cyber attacks. In this work, we explore whether AI can enhance the directory enumeration process and propose a novel Language Model-based framework. Our experiments -- conducted in a testbed consisting of 1 million URLs from different web application domains (universities, hospitals, government, companies) -- demonstrate the superiority of the LM-based attack, with an average performance increase of 969\%.},
booktitle = {Proceedings of the 2024 Workshop on Artificial Intelligence and Security},
pages = {184–195},
numpages = {12},
keywords = {language model, offensive ai, penetration test, web security},
location = {Salt Lake City, UT, USA},
series = {AISec '24}
}
```
