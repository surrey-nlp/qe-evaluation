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

* AllTransQuestAllLangs.ipynb contains the code for replicating results from all three TransQuest-based models, for all the langauge pairs involved.
* UnsupervisedAllLangs.ipynb contains the code for replicating results using the Unsupervised method, for all the language pairs involved.
* getPearsonandRanking.ipynb contains the code for replicating results obtained using Pearson correlation, and ranking the systems based on our proposed method.

## Citing
Please use the following citation while citing this work:

```latex

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

```
