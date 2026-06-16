Abstract Method Results Citation
Paper page · BMVC 2026-style manuscript

Risk-Sensitive Learning using Contextual Bandits for Medical Image Classification on Small Datasets
Name, Bashayer Marghalani, J.~Michael Herrmann

NameAddress

Download paper PDF Cite Code coming soon
Note. This page is prepared from the uploaded manuscript files. It presents the work as a research manuscript and does not imply clinical validation or conference acceptance.
Abstract
Brain Tumour Classification is a safety-critical process: misclassifying a tumour case as healthy can delay treatment and endanger the patient. This study reframes four-class brain image classification (glioma, meningioma, pituitary, healthy) as a single-step contextual bandit problem. This framework uses a cost-sensitive learning principle in the reward system itself and is a safety-aware process that observes tumour-to-healthy errors and keeps them at a minimum. This framework has been challenged by applying it to a small dataset. We evaluated contextual-bandit agents using Upper Confidence Bound (UCB), Thompson Sampling, epsilon-greedy, and Boltzmann distribution for exploration across three data regimes using a four-fold cross-validation. The results demonstrate that reward shaping can tune the safety–accuracy trade-off, prioritising clinically risky confusions while remaining competitive and even better than traditional deep learning techniques under limited data.

Key idea
Brain tumour classification is treated as a safety-aware decision problem. Instead of optimising accuracy alone, the reward function penalises tumour-to-healthy errors most strongly, encouraging the model to avoid false reassurance when predicting the healthy class.

Task
Four-class brain MRI classification: glioma, meningioma, pituitary, and healthy.

Model family
Contextual-bandit-style policies with neural and linear reward estimators.

Safety metric
Tumour-to-healthy error rate and healthy-class precision are analysed alongside accuracy.

Method overview
Full pipeline of safety-aware classification with contextual bandits
Pipeline: preprocessing, fused deep feature extraction, contextual-bandit-style classification, and safety-aware evaluation.
Feature extraction
Each image is augmented with flips and rotations, passed through frozen AlexNet, VGG16, VGG19, and EfficientNet-B0 backbones, then fused and reduced with PCA.

Policies
The paper evaluates Thompson Sampling–UCB, ε-greedy, and Boltzmann exploration across neural and linear reward estimators.

Feature-space visualisation across datasets and backbones
Feature-space visualisation across Dataset B, BC, and B2.
Main results
On the smallest balanced dataset, B2, N-TS-UCB achieved the strongest safety-aware balance: lowest T-H rate, highest healthy-class precision, highest validation accuracy, and shared highest test accuracy.

Model	Val. acc	Test acc	T-H rate	Healthy Pr.	Glioma R	Meningioma R	Pituitary R
N-TS-UCB	0.914	0.836	0.0413	0.884	0.879	0.743	0.948
VGG19	0.785	0.743	0.0422	0.877	0.827	0.537	0.850
N-Boltz (τ=1.5)	0.907	0.825	0.0457	0.866	0.900	0.657	0.969
N-ε-Greedy	0.901	0.805	0.0543	0.851	0.900	0.551	0.962
VGG16	0.801	0.794	0.0611	0.851	0.897	0.597	0.860
N-Boltz (τ=2.0)	0.896	0.836	0.0630	0.834	0.914	0.680	0.910
AlexNet	0.774	0.745	0.0722	0.806	0.823	0.527	0.877
Lin-TS-UCB	0.875	0.800	0.0935	0.769	0.866	0.554	0.916
Lin-Boltz (τ=1.5)	0.868	0.810	0.1022	0.765	0.868	0.568	0.916
Lin-Boltz (τ=2.0)	0.868	0.810	0.1022	0.765	0.868	0.568	0.916
Lin-ε-Greedy	0.884	0.760	0.1109	0.731	0.844	0.509	0.857
EfficientNet-B0	0.626	0.620	0.2244	0.595	0.807	0.163	0.610
H = healthy, G = glioma, M = meningioma, Pit. = pituitary. Values are copied from the manuscript's Dataset B2 summary table.

Tumour-to-healthy rate across datasets and models
T-H rate across Dataset B, BC, and B2.
Healthy class precision across models and datasets
Healthy-class precision across models and datasets.
Validation and test accuracies across models and datasets
Validation and test accuracies across models and datasets.
Class-wise precision and recall across models and datasets
Class-wise precision and recall maps across datasets.
Datasets
7,023
Dataset B: cleaned four-class dataset from public brain MRI sources.

360
Dataset BC: balanced subset with 90 images per class.

120
Dataset B2: small balanced subset with 30 images per class.

Citation
Update the venue fields after acceptance or public release.

@misc{marghalani2026risk_sensitive_contextual_bandits,
  title        = {Risk-Sensitive Learning using Contextual Bandits for Medical Image Classification on Small Datasets},
  author       = {Marghalani, Bashayer and Herrmann, J. Michael},
  year         = {2026},
  note         = {Manuscript / paper page. Update venue fields after acceptance.}
}
© 2026 Bashayer Marghalani and J. Michael Herrmann. Built as a static GitHub Pages paper site.
