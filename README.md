# Dataset for the flow shop scheduling problem

## Description

This repository contains a comprehensive dataset for Flow Job Shop Scheduling Problem (FSSP) research. The dataset is curated to provide a diverse set of instances that challenge and benchmark scheduling algorithms.

## Motivation

The motivation behind creating this dataset was to facilitate the development and testing of scheduling algorithms. By providing a standardized set of problems, researchers and practitioners can compare different approaches on a level playing field.

## Dataset Overview

The dataset is composed by several problem instances in the form of CSV files. We used the same naming convention to name the different files: **problem_Mm_Jj.csv**

where:
- **M**: is the number of machines
- **J**: is the number of jobs
for example the file named: **problem_10m_100j.csv** is related to a problem instance with 10 machine and 100 jobs.

The number of machines is in {3, 5, 8, 10} and the number of jobs is in {10, 20, 30, 50, 100}. We generated 20 different problems making all possible combinations of the number of machines and the number of jobs. The processing times for each job on each machine are generated randomly between 1 and 20.


## Usage

Instructions on how to use the dataset in python:

```
import pandas as pd
# Read the problem with 8 machines and 50 jobs
m = 8
j = 50
data = pd.read_csv(f'problems/problem_{m}m_{j}j.csv', index_col=0)
```


## Citation

If you use this dataset in your research, please cite it as follows:

```
@misc{elkamel2024fssp,
  author = {Akil Elkamel and Atef Gharbi},
  title = {Dataset for the flow shop scheduling problem},
  year = {2024},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{https://github.com/akilelkamel/fssp-dataset}}
}
```

## License

MIT


## Contact

- Akil Elkamel, Department of Information Systems, Faculty of Computing and Information Technology, Northern Border University, Saudi Arabia.
**Email:** *akil.elkamel@nbu.edu.sa*

- Atef Gharbi, Department of Information Systems, Faculty of Computing and Information Technology, Northern Border University, Saudi Arabia.
- **Email:** *atef.gharbi@nbu.edu.sa*
