
#  Bioinformatics & Deep Learning Technical Test

This repository contains a technical test designed for evaluating candidates' proficiency in **bioinformatics**, **deep learning**, and **scientific reasoning**, particularly focused on **single-cell omics** data analysis.

![Jupyter](https://img.shields.io/badge/JupyterLab-enabled-orange)
![Docker](https://img.shields.io/badge/Docker-ready-blue)
![License](https://img.shields.io/github/license/your-username/bio-dl-test)

---

##  Contents

-  `bio_dl_test_clean.pdf` – Candidate test instructions
-  `bio_dl_test_solution.ipynb` – Full reference solution
-  `Dockerfile` – Environment for reproducible execution
-  `requirements.txt` – Python dependencies
-  `auto_grader.py` & `auto_grader_exec.py` – Automated grading scripts
-  `pbmc3k_subset_300cells.h5ad` – (Optional) Sample dataset
-  `.github/workflows/test.yml` – Notebook testing with GitHub Actions

---

##  Quick Start

```bash
# Clone the repo
git clone https://github.com/<your-username>/bio-dl-test.git
cd bio-dl-test

# Build Docker image
docker build -t bio-dl-env .

# Run with JupyterLab
docker run -p 8888:8888 -v $(pwd):/workspace bio-dl-env


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

