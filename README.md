# 📈 Data-Driven Traffic Modeling

This repository contains our traffic flow prediction models using both classical and deep learning methods. 

---

## 📁 Project Structure

```plaintext
.
├── Alternative Approach/
│   ├── ARIMA.ipynb         # Classical time series forecasting using ARIMA
│   ├── LSTM.ipynb          # LSTM-based deep learning approach
│   ├── SINDy.ipynb         # Sparse Identification of Nonlinear Dynamics                  
├── STrEAM.ipynb            # Our main proposed model using Spatiotemporal Linear Attention and Neural ODE
├── .gitignore
├── data/                   # Contains datasets PEMS 4 7 8
└── README.md               # Project overview and instructions
```

---

## 🧠 Models

### ✅ Main Model

* **STrEAM** (`STrEAM.ipynb`): A novel Spatiotemporal model combining linear attention mechanisms, learnable spatial/temporal embeddings, and a neural ODE block for modeling sensor dynamics. Achieves strong performance with interpretable uncertainty via negative log-likelihood loss.

### ⚙️ Baselines

* **SINDy** (`SINDy.ipynb`): Attempts to discover an interpretable dynamical system using sparse regression.
* **ARIMA** (`ARIMA.ipynb`): Classical autoregressive approach using lagged sensor values.


---

## 📦 Setup Instructions

1. Clone the repo:

   ```bash
   git clone https://github.com/ronzo07/data-driven-traffic-modeling.git
   cd data-driven-traffic-modeling
   ```

2. Install dependencies:

   ```bash
   pip install numpy==1.26.4 scipy==1.11.4 pandas==2.2.2 scikit-learn==1.3.2 torch==2.6.0 torchvision==0.21.0
   ```

3. Download PeMS04 and place the CSV files in the `data/` folder and update path when needed carefully.

4. Run notebooks, mainly:

   * `STrEAM.ipynb` 

