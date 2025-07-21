```markdown
# Intrusion Detection System Using Explainable AI (XAI)

This repository implements a Network Intrusion Detection System (NIDS) using the UNSW-NB15 dataset. It employs K-Nearest Neighbors (KNN), Decision Trees, and Random Forests for detecting malicious network activities, with LIME for explaining model predictions. Developed by Hrishab Kakoty, Sangeeta Sarkar, and Prabal Baishya at Central Institute of Technology Kokrajhar.

## Features
- Machine learning models (KNN, Decision Trees, Random Forests) for intrusion detection.
- LIME for interpretable model predictions.
- Feature correlation heatmap for top features.

## Prerequisites
- Python 3.11+
- Libraries: `numpy`, `pandas`, `scikit-learn`, `lime`, `seaborn`, `matplotlib`
- UNSW-NB15 dataset (`UNSW_NB15_training-set.csv`)

## Setup
1. Clone the repo:
   ```bash
   git clone https://github.com/your-username/intrusion-detection-xai.git
   cd intrusion-detection-xai
   ```
2. Install dependencies:
   ```bash
   pip install numpy pandas scikit-learn lime seaborn matplotlib
   ```
3. Download [UNSW-NB15 dataset](https://www.unsw.adfa.edu.au/unsw-canberra-cyber/cybersecurity/ADFA-NB15-Datasets/) and place `UNSW_NB15_training-set.csv` in the project root.
4. Run the notebook:
   ```bash
   jupyter notebook XAI_on_IDS.ipynb
   ```

## Usage
- **Preprocessing**: Loads dataset, converts to numeric, fills missing values.
- **Training**: Splits data (80/20), trains and evaluates models.
- **Evaluation**: Reports accuracy (~90% for KNN), confusion matrix, and classification metrics.
- **Visualization**: Generates feature correlation heatmap.
- **LIME**: Explains predictions for selected instances.

## Results
- KNN Accuracy: ~90%
- Key Features: `dur`, `sbytes`, `dbytes`, `rate`
- LIME provides feature contribution insights.

## Future Work
- Explore advanced algorithms and deep learning.
- Enhance feature engineering.
- Deploy in real-world scenarios.

## References
- [Explainable AI for Intrusion Detection](https://www.elsevier.com/locate/eswa)
- [UNSW-NB15 Dataset](https://www.unsw.adfa.edu.au/unsw-canberra-cyber/cybersecurity/ADFA-NB15-Datasets/)

## License
CIT License
```
