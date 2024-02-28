
# Isolation Forest for Anomaly Detection on Kitsune Network Attack Dataset

This repository contains the implementation of Isolation Forest for anomaly detection on the Kitsune Network Attack Dataset. Isolation Forest is an effective algorithm for detecting outliers and anomalies in datasets, including network traffic data. The Kitsune dataset contains network traffic data with labeled attacks, making it suitable for evaluating anomaly detection algorithms.

## About Isolation Forest

Isolation Forest is an unsupervised learning algorithm that isolates observations by randomly selecting a feature and then randomly selecting a split value between the maximum and minimum values of that feature. This process is repeated recursively until all data points are isolated, forming isolation trees. Anomalies are typically isolated closer to the root of the trees, as they require fewer splits to isolate. By measuring the path lengths from the root to isolate each data point, anomalies can be identified as those with shorter path lengths.

## Dataset

The Kitsune Network Attack Dataset contains network traffic data collected from a simulated network environment, including normal traffic and various types of attacks. The dataset is labeled, with each data point categorized as either normal or anomalous.

## Usage

1. Clone the repository:

```bash
git clone https://github.com/your-username/isolation-forest-kitsune.git
cd isolation-forest-kitsune
```

2. Install the required dependencies:

```bash
pip install -r requirements.txt
```

3. Download the Kitsune Network Attack Dataset from the official source and place it in the `data` directory.

4. Run the `isolation_forest_kitsune.py` script to train the Isolation Forest model and evaluate its performance on the Kitsune dataset:

```bash
python isolation_forest_kitsune.py
```

## Results

The script will output various metrics such as precision, recall, F1-score, and ROC AUC to evaluate the performance of the Isolation Forest model on detecting anomalies in the Kitsune dataset.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
