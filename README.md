# MLOps Workflow Project

## Objective
Use Git best practices to manage a simple ML project:
- Track code changes
- Keep models separate
- Release versions safely

---

## Tools
- Git
- Python
- Scikit-learn
- GitHub

---

## Steps

1. **Setup**
git clone <repo-url>
Initialize a new Git repository.
Train Model create .gitignore
python train.py
Generates model.pkl (ignored by Git)

Version Code
git add train.py
git commit -m "Update hyperparameters"
Release & Deploy

git tag -a v1.0.0 -m "Release v1.0.0"
git push origin v1.0.0
git checkout -b deployment/v1.0.0 v1.0.0


Models are ignored in Git.

Tags track releases.

Deployment branch ensures reproducibility.
