
#### Test template  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vasighiz/bio-dl-test/blob/main/bio_dl_test_template.ipynb)  Solution  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vasighiz/bio-dl-test/blob/main/solution.ipynb)

After applying changes, run the following cmd before pushing to github:
```bash
python -m nbconvert --ClearMetadataPreprocessor.enabled=True --ClearOutputPreprocessor.enabled=True --to notebook --output cleaned_solution.ipynb solution.ipynb
```

#  Bioinformatics & Deep Learning Technical Test

This repository contains a technical test designed for evaluating proficiency in **bioinformatics**, **deep learning**, and **scientific reasoning**, particularly focused on **single-cell omics** data analysis.


![Jupyter](https://img.shields.io/badge/JupyterLab-enabled-orange)
![Docker](https://img.shields.io/badge/Docker-ready-blue)

---

##  Setup Instructions

### 1. Clone and Build
```bash
git clone <your-repo-or-local-path>
cd bio_dl_test
docker build -t bio-dl-env .
```

### 2. Run Container
```bash
docker run -it --rm -p 8888:8888 -v $(pwd):/workspace bio-dl-env
```

### 3. Access JupyterLab
Visit: [http://localhost:8888](http://localhost:8888)

Use the token printed in terminal.

---

##  Included

- `bio_dl_test_solution.ipynb`: Full solution
- `pbmc3k_subset_300cells.h5ad`: Lightweight test dataset
- `Dockerfile` + `requirements.txt`
- Runs: Scanpy, scVI, PyTorch, and JupyterLab

