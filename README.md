# 🇧🇩 Bangladesh Election 2026 Predictor (AI Simulation)

A Machine Learning project that simulates and predicts the outcome of the next Bangladesh National Election using a Multi-Layer Perceptron (Neural Network).

## 🎯 Project Goal
To build a realistic classification model that can predict whether **BNP** or **Jamaat** will win a constituency based on historical voting patterns, literacy rates, and demographic data. 

**Key Challenge:** The initial model achieved **100% accuracy** (a clear sign of overfitting and data imbalance). The project evolved to generate a **synthetic, realistic dataset** introducing "swing factors" and noise to simulate real-world voter unpredictability, resulting in a robust 78% accuracy.

## 🛠️ Tech Stack
* **Language:** Python 3.10
* **Libraries:** Pandas, NumPy, Scikit-Learn, Seaborn
* **Model:** MLPClassifier (Neural Network)
* **Techniques:** One-Hot Encoding, StandardScaler, Stratified Splitting, Synthetic Data Generation

## 📊 Workflow
1.  **Data Generation:** Scripted a realistic dataset for 300 constituencies with demographic biases and random swing factors.
2.  **Preprocessing:** * Handled categorical features (Districts) using `OneHotEncoder`.
    * Scaled numerical features (Votes, Literacy) using `StandardScaler`.
3.  **Model Training:** Trained a Neural Network (MLP) with hidden layers `(64, 32)`.
4.  **Correction:** Addressed Class Imbalance by using `stratify=y` during train-test splits.
5.  **Simulation:** Deployed the model to predict the winner for all 300 seats to declare a parliamentary majority.

## 📈 Results
* **Final Model Accuracy:** ~78% (Realistic for human behavior prediction)
* **Confusion Matrix:** Successfully identified "Swing Districts" where historical data did not guarantee a win.

## 🚀 How to Run
1. Clone the repo
2. Install dependencies: `pip install pandas scikit-learn numpy`
3. Run the notebook `National_Election_Dataset.ipynb`

---
*Disclaimer: This project uses synthetic data generated for educational purposes to demonstrate Machine Learning concepts. It does not reflect actual polling data.*
