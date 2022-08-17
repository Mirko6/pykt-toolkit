# PyKT

[![Downloads](https://pepy.tech/badge/pykt-toolkit)](https://pepy.tech/project/pykt-toolkit)
[![GitHub Issues](https://img.shields.io/github/issues/pykt-team/pykt-toolkit.svg)](https://github.com/pykt-team/pykt-toolkit/issues)
[![Documentation](https://img.shields.io/website/http/pykt-team.github.io/index.html?down_color=red&down_message=offline&up_message=online)](https://pykt.org/)

PyKT is a python library build upon PyTorch to train deep learning based knowledge tracing models. The library consists of a standardized set of integrated data preprocessing procedures on 7 popular datasets across different domains, 5 detailed prediction scenarios, 10 frequently compared DLKT approaches for transparent and extensive experiments.


## Installation
Use the following command to install PyKT:

Create conda envirment.

```
conda create --name=pykt python=3.7.5
source activate pykt
```


```
pip install -U pykt-toolkit -i  https://pypi.python.org/simple 
```

## Development
1、Clone pykt repositoriy

```shell
git clone https://github.com/pykt-team/pykt-toolkit
```

2、Change to dev branch 

```shell
cd pykt-toolkit
git checkout dev
```

**Do not** work on the main branch.

3、Editable install

You can use the following command to install the pykt library. 

```shell
pip install -e .
```
In this mode, every modification in `pykt` directory will take effect immediately. You do not need to reinstall the package again. 

4、Push to remote(dev)

After development models or fix bugs, you can push your codes to dev branch. 


The main branch is **not allowed** to push codes (the push will be failed). You can use a Pull Request to merge your code from **dev** branch to the main branch. We will reject the Pull Request from another branch to main branch, you can merge to dev branch first.


## References
### Projects

1. https://github.com/hcnoh/knowledge-tracing-collection-pytorch 
2. https://github.com/arshadshk/SAKT-pytorch 
3. https://github.com/shalini1194/SAKT 
4. https://github.com/arshadshk/SAINT-pytorch 
5. https://github.com/Shivanandmn/SAINT_plus-Knowledge-Tracing- 
6. https://github.com/arghosh/AKT 
7. https://github.com/JSLBen/Knowledge-Query-Network-for-Knowledge-Tracing 
8. https://github.com/xiaopengguo/ATKT 
9. https://github.com/jhljx/GKT 
10. https://github.com/THUwangcy/HawkesKT
11. https://github.com/ApexEDM/iekt
12. https://github.com/Badstu/CAKT_othermodels/blob/0c28d870c0d5cf52cc2da79225e372be47b5ea83/SKVMN/model.py
13. https://github.com/bigdata-ustc/EduKTM

### Papers

1. DKT: Deep knowledge tracing 
2. DKT+: Addressing two problems in deep knowledge tracing via prediction-consistent regularization 
3. DKT-Forget: Augmenting knowledge tracing by considering forgetting behavior 
4. KQN: Knowledge query network for knowledge tracing: How knowledge interacts with skills 
5. DKVMN: Dynamic key-value memory networks for knowledge tracing 
6. ATKT: Enhancing Knowledge Tracing via Adversarial Training 
7. GKT: Graph-based knowledge tracing: modeling student proficiency using graph neural network 
8. SAKT: A self-attentive model for knowledge tracing 
9. SAINT: Towards an appropriate query, key, and value computation for knowledge tracing 
10. AKT: Context-aware attentive knowledge tracing 
11. Temporal Cross-Effects in Knowledge Tracing
12. IEKT: Tracing Knowledge State with Individual Cognition and Acquisition Estimation
13. SKVMN: Knowledge Tracing with Sequential Key-Value Memory Networks
14. LPKT: Learning Process-consistent Knowledge Tracing



<!-- 
# How to use?

CUDA_VISIBLE_DEVICES=3 python wandb_akt_train.py

# description
## preprocess: 
The preprocess code for each dataseet.

* assist2015_preprocess.py

The preprocess code for assist2015 dataset.

If you want to add a new dataseet, please write your own dataset preprocess code, to change the data to this format:
```
    uid,seq_len
    questions ids / names
    concept ids / names
    timestamps
    usetimes
```
a example like this:
```
    50121,4
    106101,106102,106103,106104
    7014,7012,7014,7013
    0,1,1,1
    1647409594,1647409601,1647409666,1647409694
    123,234,456,789
```
* split_datasets.py

Split the data into 5-fold for trainning and testing. 

## data
The data saved dir for each dataset.

## datasets
Including a data_loader.py to prepare data for trainning models.

## models
Including models: dkt, dkt+, dkvmn, sakt, saint, akt, kqn, atkt.

## others
train.py: trainning code. -->
