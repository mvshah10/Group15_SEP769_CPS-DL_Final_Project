# 🚦 Advanced Smart Traffic Management Using Deep Learning

This project aims to forecast hourly vehicle traffic at urban junctions using deep learning models. It compares the performance of Feedforward Neural Network (FNN), Long Short-Term Memory (LSTM), and Gated Recurrent Unit (GRU) to identify the most effective model for smart traffic prediction.

---

## Project Structure

- `Group15_SEP769_CPS_(DL)_Final_Project_Code.ipynb`: Main Jupyter Notebook containing model development, training, and evaluation.

---

## Dataset

- **Records**: 48,120 hourly entries from 4 traffic junctions
- **Features**: Timestamp, Junction ID, Vehicle count (target), plus engineered features like Hour, Day, Month, Weekday, Is_Weekend
- **Source**: Kaggle (https://www.kaggle.com/datasets/fedesoriano/traffic-prediction-dataset)

---

## Preprocessing Steps

1. **Datetime Feature Engineering** (Hour, Weekday, Month, etc.)
2. **Categorical Encoding** (Junction ID)
3. **Missing Value Handling** (Interpolation)
4. **Feature Scaling** (StandardScaler)
5. **Train/Validation Split** (80/20)

---

## Models Used

- **FNN**: Baseline fully-connected model
- **LSTM**: Sequential model for long-term dependencies
- **GRU**: Lightweight alternative to LSTM

---

## Evaluation Metrics

- **MAE** (Mean Absolute Error)
- **MSE** (Mean Squared Error)
- **RMSE** (Root Mean Squared Error)

**Best Model**: FNN  
---

## How to Run

1. Open the `.ipynb` file in Jupyter Notebook / Google Colab
2. Run cells in order: preprocessing → training → evaluation
3. Review outputs including training curves and scatter plots

---

## Requirements

- Python 3.10+
- TensorFlow / Keras
- Scikit-learn
- Pandas, NumPy
- Matplotlib / Seaborn
```bash
pip install tensorflow scikit-learn pandas numpy matplotlib seaborn
```
