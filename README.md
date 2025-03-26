# Predictive Lead Scoring using Machine Learning 🎯

[![Python 3.7.6](https://img.shields.io/badge/python-3.7.6-blue.svg)](https://www.python.org/downloads/release/python-376/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## 📋 Overview
[5 Pillars of lead scoring](https://www.gainsight.com/blog/the-5-pillars-for-product-led-growth-using-product-qualified-leads/)
This project implements a machine learning-based lead scoring system using the [Bank Marketing dataset](https://archive.ics.uci.edu/ml/datasets/bank+marketing). The model predicts the likelihood of a client subscribing to a term deposit based on direct marketing campaign data from a Portuguese banking institution.

### 🎯 Business Objective
The model is optimized for minimizing the cost of losing potential customers while balancing sales resource allocation. Specifically, we prioritize:
- Low False Negatives (not missing potential customers)
- High True Positives (accurate identification of likely conversions)
- Balanced False Positives (efficient resource utilization)

## 📊 Model Performance

### Training Details
- Training set: ~30,000 observations
- Hold-out test set: ~10,000 observations
- Model: LightGBM Classifier

### Key Metrics
- Conversion Rate: 75.04% of predicted leads resulted in successful conversions
- False Positive Rate: 29.56%
- False Negative Rate: 24.95%

### Lead Segmentation
The model enables strategic lead segmentation for optimized resource allocation:

<img src="https://github.com/mbilalnust/predictive_lead_scoring/blob/master/report/figures/output_20_1.png" width="500" alt="Lead Segmentation Results" />

## 🛠️ Installation & Setup

### Prerequisites
- Python 3.7.6
- Git
- pip

### Installation Steps

1. Clone the repository:
```bash
git clone https://github.com/abhijitpai000/predictive_lead_scoring.git
cd predictive_lead_scoring
```

2. Download the dataset:
- Visit the [Bank Marketing dataset](https://archive.ics.uci.edu/ml/datasets/bank+marketing) page
- Download and place `bank-additional-full.csv` in the `datasets` directory

3. Set up a virtual environment:
```bash
pip install virtualenv
virtualenv lead_scoring
```

4. Activate the virtual environment:
- On Windows:
```bash
lead_scoring\Scripts\activate
```
- On macOS/Linux:
```bash
source lead_scoring/bin/activate
```

5. Install dependencies:
```bash
pip install -r requirements.txt
```

## 📚 Documentation

For detailed information about the implementation and analysis:
- Check the [final report](https://github.com/abhijitpai000/predictive_lead_scoring/blob/master/report/README.md)
- Explore the modules in the `src` directory

## 📊 Data Source

This project uses the [Bank Marketing dataset](https://archive.ics.uci.edu/ml/datasets/bank+marketing) from the UCI Machine Learning Repository, which contains:
- Client demographic data
- Campaign interaction details
- Previous campaign outcomes
- Economic indicators
- Target variable: term deposit subscription (yes/no)

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📧 Contact

For questions or feedback about this project, please open an issue in the repository.
