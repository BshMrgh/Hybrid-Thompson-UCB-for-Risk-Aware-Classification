# Hybrid Thompson-UCB for Risk-Aware Brain Tumour Classification under Limited Data

This repository hosts the GitHub Pages paper website and supporting research assets for the paper:

**Hybrid Thompson-UCB for Risk-Aware Brain Tumour Classification under Limited Data**

The project studies risk-aware brain tumour classification under limited-data conditions. It frames four-class brain MRI classification as a contextual-bandit decision problem and uses cost-sensitive rewards to reduce high-risk tumour-to-healthy classification errors.

---

## Website contents

The paper page presents:

- the paper title and abstract;
- the Hybrid Thompson-UCB / Thompson-UCB policy framing;
- the risk-aware contextual-bandit learning idea;
- the safety-aware classification pipeline;
- feature-space and performance visualisations;
- tumour-to-healthy error analysis;
- healthy-class precision analysis;
- validation and test accuracy results;
- class-wise precision and recall results;
- citation metadata.

---

## Ablation study

This repository also includes the ablation study file:

```text
Ablation_study_of_shared_preprocessing_vs_backbone_specific_preprocessing.pdf
```

The ablation study compares shared preprocessing and backbone-specific preprocessing. It is included as supporting analysis for understanding how preprocessing choices affect the feature extraction and classification workflow used in the paper.

---

## Repository structure

The current `assets` branch keeps the website files and supporting paper assets at the repository root:

```text
Cost-Sensitive-Contextual-Bandits-Classifier/
├── index.html
├── styles.css
├── CITATION.cff
├── README.md
├── .nojekyll
├── Hybrid Thompson-UCB for Risk-Aware Brain Tumour Classification under Limited Data.pdf
├── Ablation_study_of_shared_preprocessing_vs_backbone_specific_preprocessing.pdf
├── feature_space.png
├── H prec.png
├── T-H rate accross datasets and models_new.png
├── val and test.png
└── Precision and recall for all policies across all datasets B BC B2.png
```

Additional result tables and pipeline assets may also be stored at the repository root if they were uploaded separately.

---

## Citation

to be updated

---

## Disclaimer

This repository is a research project webpage. The results are intended for academic communication and should not be interpreted as a clinically validated diagnostic system.
