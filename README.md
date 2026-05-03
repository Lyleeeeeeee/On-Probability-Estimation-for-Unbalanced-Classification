# On Probability Estimation for Unbalanced Classification

This repository contains code for the paper **On Probability Estimation for Unbalanced Classification**.

We simulate and evaluate how common balancing strategies affect posterior probability estimation under unbalanced data. In particular, we study random oversampling, random undersampling, class weighting, and synthetic data augmentation. Although these methods often improve minority-class classification performance, they can distort posterior probability estimates. This repository implements probability correction methods that reduce such bias and improve calibration.

---

## 📄 Paper

**On Probability Estimation for Unbalanced Classification**  
Feng Lin, Yifan Dai, and Yufeng Liu  
*Journal of Statistical Theory and Practice*, 20, Article 57, 2026.  
DOI: https://doi.org/10.1007/s42519-026-00572-5

---

## 📁 Contents

- `simulation_scenario_1.py` – Synthetic data simulation under Scenario 1.
- `experiment_car_evaluation.py` – Empirical evaluation using the Car Evaluation dataset from the UCI Machine Learning Repository.
- `Simulation&Application.ipynb` – Organized notebook for simulation and application experiments.

---

## ⚙️ Methods

The code compares several training strategies:

- Original unbalanced training
- Random oversampling
- Random undersampling
- Class weighting
- Synthetic data augmentation
- Posterior probability correction after balancing

The correction aims to recover more accurate posterior probability estimates while preserving the classification gains from balancing techniques.

---

## 📊 Evaluation

The experiments evaluate both classification performance and probability calibration. Classification metrics include AUC and G-Mean, while calibration metrics include ECE, log loss, and Brier score.

---

## 📚 Citation

If you use this code or find our work helpful, please cite:

```bibtex
@article{lin2026probability,
  title={On Probability Estimation for Unbalanced Classification},
  author={Lin, Feng and Dai, Yifan and Liu, Yufeng},
  journal={Journal of Statistical Theory and Practice},
  volume={20},
  number={57},
  year={2026},
  publisher={Springer},
  doi={10.1007/s42519-026-00572-5}
}
