
#  Bioinformatics + Deep Learning Test Environment (Docker)

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

