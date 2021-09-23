# Adversarial Evaluation of Quality Estimation

## Installation

### Step 1
The repo requires you to have Python > 3.7.0. We used <a href="https://www.anaconda.com/products/individual">Anaconda</a> to create an environment by:
```bash
conda create --name mtqe python=3.8
```

and then (to activate the environment):
```bash
conda activate mtqe
```
### Alternative (to Step 1)

If you are not an Anaconda user, please consider creating a new virtual environment (Python > 3.7.0). You can install 'virtualenv' with:

```bash
pip install virtualenv
```

then create a new virtual environment using:

```bash
python3 -m venv mtqe
```

You should be able to activate this vitual environment using:

```bash
source mtqe/bin/activate
```

### Step 2 - Cloning the repository

```bash
git clone https://github.com/dipteshkanojia/qe-evaluation.git
cd qe-evaluation
```

### Step 3 - Installing the required libraries

```bash
pip install -r requirements.txt
python -m spacy download en_core_web_sm
```

## Usage

You can use the following command to initate a Jupyter Notebook in your browser. 
```bash
jupyter-notebook
```

Please open the following notebooks to perform the perturbations, obtain results for all language pairs, and then obtain system rankings as described in the paper.

* [1] AllTransQuestAllLangs.ipynb contains the code for replicating results from all three TransQuest-based models, for all the langauge pairs involved.
* [2] UnsupervisedAllLangs.ipynb contains the code for replicating results using the Unsupervised method, for all the language pairs involved.
* [3] getPearsonandRanking.ipynb contains the code for replicating results obtained using Pearson correlation, and ranking all the systems based on our proposed method.

NOTE: The code in [3] expect files generated from [1] and [2] for all the language pairs. Please execute the code for all systems, and all the language pairs before moving on to [3].

## Citing
Please use the following citation while citing this work:

```latex
@misc{kanojia2021pushing,
      title={Pushing the Right Buttons: Adversarial Evaluation of Quality Estimation}, 
      author={Diptesh Kanojia and Marina Fomicheva and Tharindu Ranasinghe and Frédéric Blain and Constantin Orăsan and Lucia Specia},
      year={2021},
      eprint={2109.10859},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}
```

For using the WMT Data provided here, please cite the following paper:
```latex
@article{fomicheva2020mlqepe,
    title={{MLQE-PE}: A Multilingual Quality Estimation and Post-Editing Dataset}, 
    author={Marina Fomicheva and Shuo Sun and Erick Fonseca and Fr\'ed\'eric Blain and Vishrav Chaudhary and Francisco Guzm\'an and Nina Lopatina and Lucia Specia and Andr\'e F.~T.~Martins},
    year={2020},
    journal={arXiv preprint arXiv:2010.04480}
}
```

For using TranQuest-based models, please cite the following paper:
```latex
@InProceedings{transquest:2020a,
author = {Ranasinghe, Tharindu and Orasan, Constantin and Mitkov, Ruslan},
title = {TransQuest: Translation Quality Estimation with Cross-lingual Transformers},
booktitle = {Proceedings of the 28th International Conference on Computational Linguistics},
year = {2020}
}

```
