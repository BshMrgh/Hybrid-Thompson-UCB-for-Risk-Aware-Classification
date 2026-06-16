# Cost-Sensitive Learning using Contextual Bandits for Medical Image Risk-Aware Classification on Small Datasets

The webpage presents the paper abstract, method overview, figures, Dataset B, BC, and B2 full table results, figures and citation information.

## Overview

This work studies risk-aware brain tumour classification under limited-data conditions. Instead of optimising accuracy alone, the paper frames four-class brain MRI classification as a single-step contextual bandit problem and uses a cost-sensitive reward design to penalise clinically dangerous tumour-to-healthy errors.

The website highlights:

- the main research idea;
- the abstract;
- the contextual-bandits learning pipeline;
- key figures from the manuscript;
- The abb three Datasets performance results;
- a draft BibTeX citation.

---
## Repository structure

```text
.
├── index.html              # Main paper webpage
├── styles.css              # Website styling
├── CITATION.cff            # Citation metadata; update after acceptance
├── README.md               # Repository documentation
├── .nojekyll               # Ensures GitHub Pages serves static files directly
└── assets/
    ├── pipeline.png        # Method pipeline figure
    ├── feature_space.png   # Feature-space visualization
    ├── th_rate.png         # Tumour-to-healthy error analysis
    ├── healthy_precision.png
    ├── validation_test_accuracy.png
    └── precision_recall.png
```

## Citation

Please update the citation after the paper is accepted or publicly released.

```bibtex
@misc{marghalani2026cost_sensitive_contextual_bandits,
  title        = {Risk-Sensitive Learning using Contextual Bandits for Medical Image Classification on Small Datasets},
  author       = {Marghalani, Bashayer and Herrmann, J. Michael},
  year         = {2026},
  note         = {Manuscript / paper page. Update venue fields after acceptance.}
}
```

---

## Disclaimer

This repository is a research project webpage. The results are intended for academic communication and should not be interpreted as a clinically validated diagnostic system.
