# KNN Bitcoin Heist Classification Project

A machine learning project to classify Bitcoin transactions as legitimate or potentially malicious, using K-Nearest Neighbours (KNN) on the **BitcoinHeistData** dataset.

## Project Overview

This project analyses Bitcoin transactions to detect patterns linked with ransomware activity. By training on transaction data, it classifies addresses as either legitimate or associated with ransomware. A user-friendly GUI enables manual input and instant classification.

## Installation
In a GitHub README file, you typically mention the `requirements.txt` to guide users on how to set up the environment and install the necessary dependencies for the project. Here's how you can structure the section in the README:

---

## Requirements

To run this project, you'll need to install the required dependencies. You can do this easily by using the `requirements.txt` file provided in the repository.

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/RicardoLlima/KNN_Bitcoin-Heist.git
   ```

2. Navigate to the project directory:
   ```bash
   cd KNN_Bitcoin-Heist
   ```
   
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

This will install the following dependencies:

- `pandas`
- `matplotlib`
- `scikit-learn`
- `numpy`
- `tk`

4. Download the dataset [here](https://archive.ics.uci.edu/dataset/526/bitcoinheistransomwareaddressdataset) and place it in the main project folder.

Once the dependencies are installed, you can start working with the project.

## Usage

1. Clone the repository and open the project folder.
2. Run the main script to load the data, preprocess it, train the model, and open the GUI.
3. Enter transaction details in the GUI fields (e.g., Year, Day, Length, Weight) and click **Predict**.
4. The GUI will display if the transaction is "pure" (legitimate) or "not pure" (potentially suspicious).

## Data Preprocessing

- **Missing and Duplicate Values**: Checked and removed if present.
- **Label Encoding**: Labels are encoded as `0` for malicious and `1` for legitimate.
- **Feature Selection**: Address column removed as it does not aid classification.

## Model

- **Algorithm**: K-Nearest Neighbours (KNN)
- **Evaluation**: Confusion matrix and classification report for model accuracy.

## GUI

A Tkinter-based GUI allows users to manually input transaction features for real-time classification.

